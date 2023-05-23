# Comparing `tmp/libquantum-1.5.1.tar.gz` & `tmp/libquantum-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquantum-1.5.1.tar", last modified: Fri Apr 28 19:53:35 2023, max compression
+gzip compressed data, was "libquantum-1.5.2.tar", last modified: Tue May 23 20:13:24 2023, max compression
```

## Comparing `libquantum-1.5.1.tar` & `libquantum-1.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.519199 libquantum-1.5.1/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.1/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-04-28 19:53:35.519199 libquantum-1.5.1/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2989 2023-04-28 19:47:14.000000 libquantum-1.5.1/README.md
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.517199 libquantum-1.5.1/libquantum/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.1/libquantum/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    22119 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/atoms.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/atoms_inverse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/blast_pulse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/doppler.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/dyadics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/entropy.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/export.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4322 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/gabor_box.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.518199 libquantum-1.5.1/libquantum/plot_templates/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.1/libquantum/plot_templates/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_picks.py
--rw-r--r--   0 opq       (1000) opq       (1000)    41024 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_reps.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42082 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_reps_black.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4092 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/rms_envelope.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/scales.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.1/libquantum/spectra.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10324 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/stockwell_orig.py
--rw-r--r--   0 opq       (1000) opq       (1000)    33732 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_cwt.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19514 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_fft.py
--rw-r--r--   0 opq       (1000) opq       (1000)    11380 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_stx.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8438 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_stx_loopy.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14611 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/synthetics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/tfr_gate_pick.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19522 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.517199 libquantum-1.5.1/libquantum.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     1039 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      104 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       23 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/top_level.txt
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.518199 libquantum-1.5.1/libquantum2/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum2/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15727 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum2/benchmark_signals.py
--rw-r--r--   0 opq       (1000) opq       (1000)      864 2023-04-28 19:51:16.000000 libquantum-1.5.1/pyproject.toml
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-28 19:53:35.519199 libquantum-1.5.1/setup.cfg
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.519199 libquantum-1.5.1/tests/
--rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.1/tests/test_quantum.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.1/tests/test_spectra.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:13:24.044037 libquantum-1.5.2/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.2/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-05-23 20:13:24.044037 libquantum-1.5.2/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2989 2023-04-28 19:47:14.000000 libquantum-1.5.2/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:13:24.042038 libquantum-1.5.2/libquantum/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.2/libquantum/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    22119 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/atoms.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/atoms_inverse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/blast_pulse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/doppler.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/dyadics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/entropy.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/export.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4322 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/gabor_box.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:13:24.043038 libquantum-1.5.2/libquantum/plot_templates/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.2/libquantum/plot_templates/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/plot_templates/plot_time_frequency_picks.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    41024 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/plot_templates/plot_time_frequency_reps.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    42082 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/plot_templates/plot_time_frequency_reps_black.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4092 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/rms_envelope.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/scales.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.2/libquantum/spectra.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    10324 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/stockwell_orig.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    33732 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/styx_cwt.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19514 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/styx_fft.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    11380 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/styx_stx.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8438 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/styx_stx_loopy.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14611 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/synthetics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.2/libquantum/tfr_gate_pick.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19522 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum/utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:13:24.043038 libquantum-1.5.2/libquantum.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-05-23 20:13:24.000000 libquantum-1.5.2/libquantum.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     1039 2023-05-23 20:13:24.000000 libquantum-1.5.2/libquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-05-23 20:13:24.000000 libquantum-1.5.2/libquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      104 2023-05-23 20:13:24.000000 libquantum-1.5.2/libquantum.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       23 2023-05-23 20:13:24.000000 libquantum-1.5.2/libquantum.egg-info/top_level.txt
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:13:24.043038 libquantum-1.5.2/libquantum2/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum2/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15727 2023-04-28 19:47:14.000000 libquantum-1.5.2/libquantum2/benchmark_signals.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      864 2023-05-23 20:12:16.000000 libquantum-1.5.2/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-05-23 20:13:24.044037 libquantum-1.5.2/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:13:24.044037 libquantum-1.5.2/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.2/tests/test_quantum.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.2/tests/test_spectra.py
```

### Comparing `libquantum-1.5.1/LICENSE` & `libquantum-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/PKG-INFO` & `libquantum-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.1
+Version: 1.5.2
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.1/README.md` & `libquantum-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/atoms.py` & `libquantum-1.5.2/libquantum/atoms.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/atoms_inverse.py` & `libquantum-1.5.2/libquantum/atoms_inverse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/blast_pulse.py` & `libquantum-1.5.2/libquantum/blast_pulse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/doppler.py` & `libquantum-1.5.2/libquantum/doppler.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/dyadics.py` & `libquantum-1.5.2/libquantum/dyadics.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/entropy.py` & `libquantum-1.5.2/libquantum/entropy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/export.py` & `libquantum-1.5.2/libquantum/export.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/gabor_box.py` & `libquantum-1.5.2/libquantum/gabor_box.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py` & `libquantum-1.5.2/libquantum/plot_templates/plot_geo_scatter_2d_3d.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_picks.py` & `libquantum-1.5.2/libquantum/plot_templates/plot_time_frequency_picks.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_reps.py` & `libquantum-1.5.2/libquantum/plot_templates/plot_time_frequency_reps.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_reps_black.py` & `libquantum-1.5.2/libquantum/plot_templates/plot_time_frequency_reps_black.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/rms_envelope.py` & `libquantum-1.5.2/libquantum/rms_envelope.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/scales.py` & `libquantum-1.5.2/libquantum/scales.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/spectra.py` & `libquantum-1.5.2/libquantum/spectra.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/stockwell_orig.py` & `libquantum-1.5.2/libquantum/stockwell_orig.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/styx_cwt.py` & `libquantum-1.5.2/libquantum/styx_cwt.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/styx_fft.py` & `libquantum-1.5.2/libquantum/styx_fft.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/styx_stx.py` & `libquantum-1.5.2/libquantum/styx_stx.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/styx_stx_loopy.py` & `libquantum-1.5.2/libquantum/styx_stx_loopy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/synthetics.py` & `libquantum-1.5.2/libquantum/synthetics.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/tfr_gate_pick.py` & `libquantum-1.5.2/libquantum/tfr_gate_pick.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum/utils.py` & `libquantum-1.5.2/libquantum/utils.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum.egg-info/PKG-INFO` & `libquantum-1.5.2/libquantum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.1
+Version: 1.5.2
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.1/libquantum.egg-info/SOURCES.txt` & `libquantum-1.5.2/libquantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/libquantum2/benchmark_signals.py` & `libquantum-1.5.2/libquantum2/benchmark_signals.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.1/pyproject.toml` & `libquantum-1.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "libquantum"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library for implementing standardized time-frequency representations."
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file = "LICENSE" }
 
 dependencies = [
     "librosa==0.10.0.post2",
-    "redvox==3.4.0",
+    "redvox==3.4.2",
     "libwwz==1.3.0",
     "redvox-base[matplotlib,numpy,pandas,scipy]==2023.4.27"
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/libquantum"
 PyPI = "https://pypi.org/project/libquantum/"
```

### Comparing `libquantum-1.5.1/tests/test_spectra.py` & `libquantum-1.5.2/tests/test_spectra.py`

 * *Files identical despite different names*

