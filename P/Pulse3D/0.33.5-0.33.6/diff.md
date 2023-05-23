# Comparing `tmp/Pulse3D-0.33.5.tar.gz` & `tmp/Pulse3D-0.33.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.5.tar", last modified: Wed May 17 19:31:07 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.6.tar", last modified: Tue May 23 20:06:15 2023, max compression
```

## Comparing `Pulse3D-0.33.5.tar` & `Pulse3D-0.33.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-17 19:30:05.000000 Pulse3D-0.33.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-17 19:31:07.000000 Pulse3D-0.33.5/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 19:31:07.000000 Pulse3D-0.33.5/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:30:53.000000 Pulse3D-0.33.5/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/nb_peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.644726 Pulse3D-0.33.6/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.644726 Pulse3D-0.33.6/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.648726 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-23 20:05:00.000000 Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.644726 Pulse3D-0.33.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 20:06:15.000000 Pulse3D-0.33.6/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 20:06:15.000000 Pulse3D-0.33.6/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:05:57.000000 Pulse3D-0.33.6/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.648726 Pulse3D-0.33.6/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-23 20:05:28.000000 Pulse3D-0.33.6/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:15.652726 Pulse3D-0.33.6/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-23 20:04:54.000000 Pulse3D-0.33.6/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.5/LICENSE` & `Pulse3D-0.33.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/PKG-INFO` & `Pulse3D-0.33.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.5
+Version: 0.33.6
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.5/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.6/mantarray-magnet-finding/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 """Setup configuration."""
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name="mantarray_magnet_finding",
-    version="0.5.2",
+    version="0.5.1",
     description="Magnet Finding",
     url="https://github.com/CuriBio/mantarray-magnet-finding",
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
         "nptyping==1.4.4",
         "numpy==1.23.4",  # Tanner (12/3/21): pinned for numba compatibility
         "scipy==1.9.3",
-        "numba==0.57.0",
+        "numba==0.56.4",
         "stdlib_utils>=0.4.4",
         "labware-domain-models>=0.3.1",
         "h5py>=3.7.0",
         "immutabledict>=2.2.1",
     ],
     zip_safe=False,
     include_package_data=True,
@@ -31,14 +31,13 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

### Comparing `Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/setup.py` & `Pulse3D-0.33.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.5",
+    version="0.33.6",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.5/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.6/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.5
+Version: 0.33.6
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.5/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.6/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.6/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.6/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.6/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/constants.py` & `Pulse3D-0.33.6/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.6/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/exceptions.py` & `Pulse3D-0.33.6/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.6/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/metrics.py` & `Pulse3D-0.33.6/src/pulse3D/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,31 +389,29 @@
         is_contraction: bool = True,
         baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
         **kwargs: Dict[str, Any],
     ):
         super().__init__(rounded=rounded, **kwargs)
 
         self.baseline_widths = baseline_widths_to_use
-
-        self.velocity_start = self.baseline_widths[0]
-        self.velocity_end = self.baseline_widths[1]
-
         self.is_contraction = is_contraction
+        # always need the 10 for relaxation and 90 for contraction to compare against input baseline width
+        self.twitch_widths = set(self.baseline_widths) | {10, 90}
 
     def fit(
         self,
         peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
         filtered_data: NDArray[(2, Any), int],
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
         **kwargs: Dict[str, Any],
     ) -> Series:
         _, coordinates = TwitchWidth.calculate_twitch_widths(
             filtered_data=filtered_data,
             twitch_indices=twitch_indices,
-            twitch_width_percents=self.baseline_widths,
+            twitch_width_percents=tuple(self.twitch_widths),
             rounded=self.rounded,
         )
 
         velocities = self.calculate_twitch_velocity(
             coordinate_df=coordinates, is_contraction=self.is_contraction
         )
 
@@ -435,21 +433,28 @@
 
             is_contraction: a boolean indicating if twitch velocities to be calculating are for the
                 twitch contraction or relaxation
 
         Returns:
             DataFrame floats that are the velocities of each twitch
         """
-        coord_type = "contraction" if is_contraction else "relaxation"
+        if is_contraction:
+            coord_type = "contraction"
+            twitch_base = self.baseline_widths[0]
+            twitch_top = 90
+        else:
+            coord_type = "relaxation"
+            twitch_base = self.baseline_widths[1]
+            twitch_top = 10
 
-        Y_end = coordinate_df["force", coord_type, self.velocity_start]
-        Y_start = coordinate_df["force", coord_type, self.velocity_end]
+        Y_end = coordinate_df["force", coord_type, twitch_top]
+        Y_start = coordinate_df["force", coord_type, twitch_base]
 
-        X_end = coordinate_df["time", coord_type, self.velocity_start]
-        X_start = coordinate_df["time", coord_type, self.velocity_end]
+        X_end = coordinate_df["time", coord_type, twitch_top]
+        X_start = coordinate_df["time", coord_type, twitch_base]
 
         # change in force / change in time
         velocity = abs((Y_end - Y_start) / (X_end - X_start))
         velocity *= MICRO_TO_BASE_CONVERSION
 
         return velocity
```

### Comparing `Pulse3D-0.33.5/src/pulse3D/nb_peak_detection.py` & `Pulse3D-0.33.6/src/pulse3D/nb_peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.6/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.6/src/pulse3D/plate_recording.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/plotting.py` & `Pulse3D-0.33.6/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/stimulation.py` & `Pulse3D-0.33.6/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/transforms.py` & `Pulse3D-0.33.6/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.5/src/pulse3D/utils.py` & `Pulse3D-0.33.6/src/pulse3D/utils.py`

 * *Files identical despite different names*

