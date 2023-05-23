# Comparing `tmp/spectrumdevice-0.2.0.tar.gz` & `tmp/spectrumdevice-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrumdevice-0.2.0.tar", last modified: Wed Mar 23 12:30:51 2022, max compression
+gzip compressed data, was "spectrumdevice-0.3.0.tar", last modified: Tue May 23 13:58:27 2023, max compression
```

## Comparing `spectrumdevice-0.2.0.tar` & `spectrumdevice-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.170710 spectrumdevice-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11882 2022-03-23 12:30:51.170710 spectrumdevice-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10580 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-03-23 12:30:51.170710 spectrumdevice-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.166710 spectrumdevice-0.2.0/spectrum_gmbh/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrum_gmbh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrum_gmbh/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrum_gmbh/pyspcm.py
--rw-r--r--   0 runner    (1001) docker     (121)    78209 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrum_gmbh/regs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2387 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrum_gmbh/spcerr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.170710 spectrumdevice-0.2.0/spectrumdevice/
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-03-23 12:30:51.170710 spectrumdevice-0.2.0/spectrumdevice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.166710 spectrumdevice-0.2.0/spectrumdevice/devices/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.166710 spectrumdevice-0.2.0/spectrumdevice/devices/mocks/
--rw-r--r--   0 runner    (1001) docker     (121)    20874 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/mocks/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (121)    28674 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_card.py
--rw-r--r--   0 runner    (1001) docker     (121)     4263 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)    14461 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     8605 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    20352 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_star_hub.py
--rw-r--r--   0 runner    (1001) docker     (121)     4922 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_timestamper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.166710 spectrumdevice-0.2.0/spectrumdevice/settings/
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4138 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/card_dependent_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/card_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/device_modes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/io_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (121)     5736 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/transfer_buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/settings/triggering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.166710 spectrumdevice-0.2.0/spectrumdevice/spectrum_wrapper/
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/spectrum_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/spectrum_wrapper/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/spectrumdevice/spectrum_wrapper/mock_pyspcm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 12:30:51.170710 spectrumdevice-0.2.0/spectrumdevice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11882 2022-03-23 12:30:50.000000 spectrumdevice-0.2.0/spectrumdevice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-03-23 12:30:51.000000 spectrumdevice-0.2.0/spectrumdevice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 12:30:50.000000 spectrumdevice-0.2.0/spectrumdevice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 12:30:49.000000 spectrumdevice-0.2.0/spectrumdevice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-03-23 12:30:51.000000 spectrumdevice-0.2.0/spectrumdevice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-23 12:30:51.000000 spectrumdevice-0.2.0/spectrumdevice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    80044 2022-03-23 12:30:42.000000 spectrumdevice-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.588640 spectrumdevice-0.3.0/spectrum_gmbh/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrum_gmbh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrum_gmbh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrum_gmbh/pyspcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78209 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrum_gmbh/regs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrum_gmbh/spcerr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/spectrumdevice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/spectrumdevice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.588640 spectrumdevice-0.3.0/spectrumdevice/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.588640 spectrumdevice-0.3.0/spectrumdevice/devices/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/mocks/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28674 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_star_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_timestamper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/spectrumdevice/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/card_dependent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/card_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/device_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/io_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/transfer_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/settings/triggering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/spectrumdevice/spectrum_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/spectrum_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/spectrum_wrapper/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/spectrumdevice/spectrum_wrapper/mock_pyspcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/spectrumdevice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-23 13:58:27.000000 spectrumdevice-0.3.0/spectrumdevice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-23 13:58:27.000000 spectrumdevice-0.3.0/spectrumdevice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:58:27.000000 spectrumdevice-0.3.0/spectrumdevice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:58:27.000000 spectrumdevice-0.3.0/spectrumdevice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 13:58:27.000000 spectrumdevice-0.3.0/spectrumdevice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-23 13:58:27.000000 spectrumdevice-0.3.0/spectrumdevice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:58:27.592640 spectrumdevice-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/tests/test_single_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/tests/test_single_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/tests/test_star_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-23 13:58:19.000000 spectrumdevice-0.3.0/versioneer.py
```

### Comparing `spectrumdevice-0.2.0/LICENSE` & `spectrumdevice-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/PKG-INFO` & `spectrumdevice-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: spectrumdevice
-Version: 0.2.0
+Version: 0.3.0
 Summary: A high-level, object-oriented Python library for controlling Spectrum Instrumentation digitisers
 Home-page: https://github.com/KCL-BMEIS/spectrumdevice
 Author: Christian Baker, Francois Joubert
 Author-email: christian.baker@kcl.ac.uk,
 License: MIT
 Project-URL: Documentation, https://kcl-bmeis.github.io/spectrumdevice/
 Project-URL: Source, https://github.com/KCL-BMEIS/spectrumdevice
 Project-URL: Tracker, https://github.com/KCL-BMEIS/spectrumdevice/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
@@ -259,9 +259,7 @@
 
 ## Examples
 See the `example_scripts` directory.
 
 ## API Documentation
 
 See [here](https://kcl-bmeis.github.io/spectrumdevice/) for documentation for the complete API.
-
-
```

### Comparing `spectrumdevice-0.2.0/README.md` & `spectrumdevice-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/setup.cfg` & `spectrumdevice-0.3.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 	Natural Language :: English
 	Operating System :: POSIX :: Linux
 	Operating System :: Microsoft :: Windows :: Windows 10
 	Operating System :: MacOS :: MacOS X
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 	Typing :: Typed
 project_urls = 
 	Documentation = https://kcl-bmeis.github.io/spectrumdevice/
 	Source = https://github.com/KCL-BMEIS/spectrumdevice
 	Tracker = https://github.com/KCL-BMEIS/spectrumdevice/issues
 
@@ -53,23 +54,23 @@
 
 [options.extras_require]
 test = 
 	pytest == 6.2.5
 dev = 
 	flake8 == 4.0
 	flake8-bugbear == 21.9.2
-	black == 22.1.0
-	mypy == 0.931
+	black == 22.3.0
+	mypy == 1.3.0
 doc = 
 	pdoc == 8.0.1
 examples = 
 	matplotlib >= 3.5.0
 
 [mypy]
-python_version = 3.8
+python_version = 3.11
 warn_unused_configs = True
 disallow_subclassing_any = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 check_untyped_defs = True
 disallow_untyped_decorators = True
```

### Comparing `spectrumdevice-0.2.0/spectrum_gmbh/pyspcm.py` & `spectrumdevice-0.3.0/spectrum_gmbh/pyspcm.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrum_gmbh/regs.py` & `spectrumdevice-0.3.0/spectrum_gmbh/regs.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrum_gmbh/spcerr.py` & `spectrumdevice-0.3.0/spectrum_gmbh/spcerr.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/__init__.py` & `spectrumdevice-0.3.0/spectrumdevice/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/measurement.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/measurement.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/mocks/__init__.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/mocks/timestamps.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/mocks/timestamps.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_card.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_card.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_channel.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_channel.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_device.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_device.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_interface.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_interface.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_star_hub.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_star_hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,15 @@
     def set_enabled_channels(self, channels_nums: List[int]) -> None:
         """Change the currently enabled channel indices, indexed over the whole hub (from 0 to N-1, where N is the total
         number of channels available to the hub).
 
         Returns:
             channel_nums (List[int]): The indices to enable.
         """
+        channels_nums.sort()
         channels_to_enable_all_cards = channels_nums
 
         for child_card in self._child_cards:
             n_channels_in_card = len(child_card.channels)
             channels_to_enable_this_card = list(set(arange(n_channels_in_card)) & set(channels_to_enable_all_cards))
             num_channels_to_enable_this_card = len(channels_to_enable_this_card)
             child_card.set_enabled_channels(channels_to_enable_this_card)
```

### Comparing `spectrumdevice-0.2.0/spectrumdevice/devices/spectrum_timestamper.py` & `spectrumdevice-0.3.0/spectrumdevice/devices/spectrum_timestamper.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/exceptions.py` & `spectrumdevice-0.3.0/spectrumdevice/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/__init__.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/card_dependent_properties.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/card_dependent_properties.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/card_features.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/card_features.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/channel.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/channel.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/device_modes.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/device_modes.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/io_lines.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/io_lines.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/status.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/status.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/timestamps.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/timestamps.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/transfer_buffer.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/transfer_buffer.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/settings/triggering.py` & `spectrumdevice-0.3.0/spectrumdevice/settings/triggering.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/spectrum_wrapper/__init__.py` & `spectrumdevice-0.3.0/spectrumdevice/spectrum_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/spectrum_wrapper/error_handler.py` & `spectrumdevice-0.3.0/spectrumdevice/spectrum_wrapper/error_handler.py`

 * *Files identical despite different names*

### Comparing `spectrumdevice-0.2.0/spectrumdevice/spectrum_wrapper/mock_pyspcm.py` & `spectrumdevice-0.3.0/spectrumdevice/spectrum_wrapper/mock_pyspcm.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,40 +34,40 @@
 
 SPCM_BUF_DATA = 1000  # main data buffer for acquired or generated samples
 SPCM_BUF_ABA = 2000  # buffer for ABA data, holds the A-DATA (slow samples)
 SPCM_BUF_TIMESTAMP = 3000  # buffer for timestamps
 
 
 def spcm_dwGetParam_i32(handle: ctypes.c_void_p, command: int, value: Any) -> None:
-    pass
+    return
 
 
 def spcm_dwSetParam_i32(handle: ctypes.c_void_p, command: int, value: int) -> None:
-    pass
+    return
 
 
 def spcm_dwGetParam_i64(handle: ctypes.c_void_p, command: int, value: Any) -> None:
-    pass
+    return
 
 
 def spcm_dwSetParam_i64(handle: ctypes.c_void_p, command: int, value: int) -> None:
-    pass
+    return
 
 
 def spcm_hOpen(string_buffer: ctypes.c_char_p) -> ctypes.c_void_p:
-    pass
+    return ctypes.c_void_p()
 
 
 def spcm_vClose(handle: ctypes.c_void_p) -> None:
-    pass
+    return
 
 
 def spcm_dwDefTransfer_i64(
     handle: ctypes.c_void_p,
     buffer_type: int,
     direction: int,
     notify_size: int,
     buffer_pointer: ctypes.c_void_p,
     offset: int,
     length: int,
 ) -> int:
-    pass
+    return 0
```

### Comparing `spectrumdevice-0.2.0/spectrumdevice.egg-info/PKG-INFO` & `spectrumdevice-0.3.0/spectrumdevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: spectrumdevice
-Version: 0.2.0
+Version: 0.3.0
 Summary: A high-level, object-oriented Python library for controlling Spectrum Instrumentation digitisers
 Home-page: https://github.com/KCL-BMEIS/spectrumdevice
 Author: Christian Baker, Francois Joubert
 Author-email: christian.baker@kcl.ac.uk,
 License: MIT
 Project-URL: Documentation, https://kcl-bmeis.github.io/spectrumdevice/
 Project-URL: Source, https://github.com/KCL-BMEIS/spectrumdevice
 Project-URL: Tracker, https://github.com/KCL-BMEIS/spectrumdevice/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
@@ -259,9 +259,7 @@
 
 ## Examples
 See the `example_scripts` directory.
 
 ## API Documentation
 
 See [here](https://kcl-bmeis.github.io/spectrumdevice/) for documentation for the complete API.
-
-
```

### Comparing `spectrumdevice-0.2.0/spectrumdevice.egg-info/SOURCES.txt` & `spectrumdevice-0.3.0/spectrumdevice.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -41,8 +41,12 @@
 spectrumdevice/_version.py
 spectrumdevice/py.typed
 spectrumdevice.egg-info/PKG-INFO
 spectrumdevice.egg-info/SOURCES.txt
 spectrumdevice.egg-info/dependency_links.txt
 spectrumdevice.egg-info/not-zip-safe
 spectrumdevice.egg-info/requires.txt
-spectrumdevice.egg-info/top_level.txt
+spectrumdevice.egg-info/top_level.txt
+tests/test_integration.py
+tests/test_single_card.py
+tests/test_single_channel.py
+tests/test_star_hub.py
```

### Comparing `spectrumdevice-0.2.0/versioneer.py` & `spectrumdevice-0.3.0/versioneer.py`

 * *Files identical despite different names*

