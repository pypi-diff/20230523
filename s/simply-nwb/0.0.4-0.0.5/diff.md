# Comparing `tmp/simply_nwb-0.0.4.tar.gz` & `tmp/simply_nwb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.0.4.tar", last modified: Fri May 19 19:32:26 2023, max compression
+gzip compressed data, was "simply_nwb-0.0.5.tar", last modified: Tue May 23 16:56:34 2023, max compression
```

## Comparing `simply_nwb-0.0.4.tar` & `simply_nwb-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.230713 simply_nwb-0.0.4/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      566 2023-05-19 19:32:26.230713 simply_nwb-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-19 19:32:26.230713 simply_nwb-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-05-19 19:32:25.000000 simply_nwb-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.217682 simply_nwb-0.0.4/simply_nwb/
--rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.221680 simply_nwb-0.0.4/simply_nwb/acquisition/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.229205 simply_nwb-0.0.4/simply_nwb/acquisition/tools/
--rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/blackrock.py
--rw-rw-rw-   0        0        0      563 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/labjack.py
--rw-rw-rw-   0        0        0     3990 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/plaintext.py
--rw-rw-rw-   0        0        0     3382 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/tif.py
--rw-rw-rw-   0        0        0      462 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/yaml.py
--rw-rw-rw-   0        0        0      436 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/nwb_inspect_script.py
--rw-rw-rw-   0        0        0    15731 2023-05-19 17:44:29.000000 simply_nwb-0.0.4/simply_nwb/simple_nwb.py
--rw-rw-rw-   0        0        0     6651 2023-05-19 17:48:58.000000 simply_nwb-0.0.4/simply_nwb/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.229205 simply_nwb-0.0.4/simply_nwb/transforms/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     3498 2023-05-19 17:39:54.000000 simply_nwb-0.0.4/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.220691 simply_nwb-0.0.4/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.568687 simply_nwb-0.0.5/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-05-23 16:56:34.568687 simply_nwb-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-23 16:56:34.568687 simply_nwb-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.556912 simply_nwb-0.0.5/simply_nwb/
+-rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.561541 simply_nwb-0.0.5/simply_nwb/acquisition/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.566452 simply_nwb-0.0.5/simply_nwb/acquisition/tools/
+-rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/blackrock.py
+-rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/labjack.py
+-rw-rw-rw-   0        0        0     2601 2023-05-23 15:16:58.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/plaintext.py
+-rw-rw-rw-   0        0        0     3437 2023-05-23 16:16:41.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/yaml.py
+-rw-rw-rw-   0        0        0    21474 2023-05-23 16:35:37.000000 simply_nwb-0.0.5/simply_nwb/simple_nwb.py
+-rw-rw-rw-   0        0        0     8461 2023-05-23 16:46:28.000000 simply_nwb-0.0.5/simply_nwb/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.567685 simply_nwb-0.0.5/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     3498 2023-05-19 20:56:41.000000 simply_nwb-0.0.5/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.561541 simply_nwb-0.0.5/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      702 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.0.4/LICENSE` & `simply_nwb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.4/PKG-INFO` & `simply_nwb-0.0.5/simply_nwb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simply_nwb
-Version: 0.0.4
+Name: simply-nwb
+Version: 0.0.5
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.4/setup.py` & `simply_nwb-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.0.4/simply_nwb/acquisition/tools/blackrock.py` & `simply_nwb-0.0.5/simply_nwb/acquisition/tools/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.4/simply_nwb/acquisition/tools/csv.py` & `simply_nwb-0.0.5/simply_nwb/acquisition/tools/csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 import os
 
 
 def csv_load_dataframe(filename=None, **kwargs):
     """
     Simple wrapper around pd.read_csv for file checks
+
     :param filename: str filename
     :param kwargs: extra args to pass to pandas.read_csv()
     :return: pandas.DataFrame
     """
     if filename is None:
         raise ValueError("Must provide filename to load a CSV file!")
     if not os.path.exists(filename):
```

### Comparing `simply_nwb-0.0.4/simply_nwb/acquisition/tools/labjack.py` & `simply_nwb-0.0.5/simply_nwb/acquisition/tools/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.4/simply_nwb/acquisition/tools/p_erg.py` & `simply_nwb-0.0.5/simply_nwb/acquisition/tools/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.4/simply_nwb/acquisition/tools/plaintext.py` & `simply_nwb-0.0.5/simply_nwb/acquisition/tools/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.4/simply_nwb/acquisition/tools/tif.py` & `simply_nwb-0.0.5/simply_nwb/acquisition/tools/tif.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import glob
 
 
 def tif_read_image(filename=None):
     """
     Read TIF Image into a numpy array
+
     :param filename: TIF file to read
     :return: numpy array
     """
 
     if filename is None:
         raise ValueError("Must supply filename argument!")
     if not os.path.exists(filename):
@@ -18,14 +19,15 @@
 
     return np.array(Image.open(filename))
 
 
 def tif_read_directory(foldername=None, filename_glob="*.tif"):
     """
     Read a directory of TIF files, giving a filename glob for specific TIFs to grab
+
     :param foldername: Folder that contains the TIF images, directly inside
     :param filename_glob: naming scheme for the TIF files to be collected. e.g. 'image_*.tif'
     :return: numpy array
     """
     if foldername is None:
         raise ValueError("Must provide folder name argument!")
     if not os.path.exists(foldername):
@@ -36,20 +38,21 @@
         raise ValueError(f"No files found with glob '{filename_glob}' in folder {foldername}!")
     if any([os.path.isdir(ff) for ff in files]):
         raise ValueError(f"Filename Glob '{filename_glob}' includes a directory!")
 
     data = []
     for file in files:
         data.append(tif_read_image(file))
-    return data
+    return np.array(data)  # Convert our list into a numpy array
 
 
 def tif_read_subfolder_directory(parent_folder=None, subfolder_glob=None, subfolder_glob_fail_on_file_found=False, file_glob=None):
     """
     Read a directory that contains folders that contain TIFs, and read each TIF from each subfolder into memory
+
     :param parent_folder: main folder containing more folders
     :param subfolder_glob: glob to specify which subfolders to look into e.g. 'folder_num_*'
     :param subfolder_glob_fail_on_file_found: If the subfolder glob returns a file, fail the operation. Defaults to True and if a file is matched, it will ignore it
     :param file_glob: TIF file glob to specify which TIFs from the subfolders to read, e.g. 'image0*.tif'
     :return: numpy array
     """
     if parent_folder is None:
```

### Comparing `simply_nwb-0.0.4/simply_nwb/simple_nwb.py` & `simply_nwb-0.0.5/simply_nwb/simple_nwb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from uuid import uuid4
 import os
 import sys
 import glob
 
+import numpy as np
 import pandas as pd
 import pendulum
 from hdmf.common.table import DynamicTable
 from hdmf.common.table import VectorData
 from pynwb import NWBFile, TimeSeries
 from pynwb.behavior import BehavioralEvents
 from pynwb.device import Device
 from pynwb.ecephys import ElectrodeGroup
 from pynwb.file import Subject
+from pynwb.ophys import OpticalChannel, TwoPhotonSeries
 
 from .acquisition.tools import labjack_load_file
 from .acquisition.tools import blackrock_all_spiketrains, perg_parse_to_table
-from .util import warn_on_name_format, inspect_nwb_obj, write_nwb, panda_df_to_dyn_table, panda_df_to_list_of_timeseries
+from .util import warn_on_name_format, inspect_nwb_obj, nwb_write, panda_df_to_dyn_table, panda_df_to_list_of_timeseries
 
 
 class SimpleNWB(object):
     _REQUIRED_ARGS = [
         "session_description",
         "session_start_time",
         "experimenter",
@@ -93,15 +95,137 @@
     def write(nwbfile, filename=None):
         """
         Write the give NWBFile object to file
         :param nwbfile: NWBFile object to write
         :param filename: path to file to write, WILL OVERWRITE!
         :return: None
         """
-        write_nwb(nwbfile, filename)
+        nwb_write(nwbfile, filename)
+
+    @staticmethod
+    def two_photon_add_data(
+            nwbfile,
+            device_name=None,
+            device_description=None,
+            device_manufacturer=None,
+            optical_channel_description=None,
+            optical_channel_emission_lambda=None,
+            imaging_name=None,
+            imaging_rate=None,
+            excitation_lambda=None,
+            indicator=None,
+            location=None,
+            grid_spacing=None,
+            grid_spacing_unit=None,
+            origin_coords=None,
+            origin_coords_unit=None,
+            two_photon_unit=None,
+            two_photon_rate=None,
+            photon_series_name=None,
+            image_data=None,
+    ):
+        """
+        Add images from a two photon microscope to an NWB with metadata.
+        Load TIF images easily with the simply_nwb.acquisition.tools.tif module
+
+
+        :param nwbfile: NWBFile to add the data to
+        :param device_name: Name of the microscope e.g. MyMicroscope1
+        :param device_description: Description of the microscope
+        :param device_manufacturer: Manufacturer of the microscope
+        :param optical_channel_description: Description of the optical channel, electrode name
+        :param optical_channel_emission_lambda: Emission wavelength for optical channel, in nm
+        :param imaging_name: Name of this imaging dataset e.g 'my_images'
+        :param imaging_rate: Rate at which images were acquired, in Hz
+        :param excitation_lambda: Excitation wavelength in nm
+        :param indicator: Indicator, e.g. GFP
+        :param location: Location, e.g. V1
+        :param grid_spacing: Spacing of the grids used e.g. [0.1, 0.1]
+        :param grid_spacing_unit: Unit of the grid spacing e.g. 'meters'
+        :param origin_coords: Coords of the origin e.g. [0.1, 0.2] or for 3d data [0.1, 0.2, 0.3]
+        :param origin_coords_unit: Unit of the origin coords
+        :param two_photon_unit: Unit for the photon microscope, e.g. 'normalized amplitude'
+        :param two_photon_rate: two photon sampling rate in Hz
+        :param photon_series_name: Name of the two photon series for storage
+        :param image_data: Numpy array of the data in shape (samples, xres, yres, channels) if only one channel, can omit
+        :return:
+        """
+
+        if device_name is None:
+            raise ValueError("Must supply device_name argument!")
+        if device_description is None:
+            raise ValueError("Must supply device_description argument!")
+        if device_manufacturer is None:
+            raise ValueError("Must supply device_manufacturer argument!")
+        if optical_channel_description is None:
+            raise ValueError("Must supply optical_channel_description argument!")
+        if optical_channel_emission_lambda is None:
+            raise ValueError("Must supply optical_channel_emission_lambda argument!")
+        if imaging_name is None:
+            raise ValueError("Must supply imaging_name argument!")
+        if imaging_rate is None or not isinstance(imaging_rate, float):
+            raise ValueError("Must supply imaging_rate, and as a float!")
+        if excitation_lambda is None:
+            raise ValueError("Must supply excitation_lambda wavelength in nm!")
+        if indicator is None:
+            raise ValueError("Must supply indicator argument! e.g 'GFP'")
+        if location is None or not isinstance(location, str):
+            raise ValueError("Must supply location string argument")
+        if grid_spacing is None:
+            raise ValueError("Must supply grid_spacing argument!")
+        if grid_spacing_unit is None:
+            raise ValueError("Must supply grid_spacing_unit argument!")
+        if origin_coords is None:
+            raise ValueError("Must supply origin_coords argument!")
+        if origin_coords_unit is None:
+            raise ValueError("Must supply origin_coords_unit argument!")
+        if two_photon_unit is None:
+            raise ValueError("Must supply two_photon_unit argument!")
+        if two_photon_rate is None:
+            raise ValueError("Must supply two_photon_rate argument!")
+        if image_data is None or not isinstance(image_data, np.ndarray):
+            raise ValueError("Must supply image_data as numpy array!")
+
+        microscope = nwbfile.create_device(
+            name=device_name,
+            description=device_description,
+            manufacturer=device_manufacturer,
+        )
+
+        optical_channel = OpticalChannel(
+            name="OpticalChannel",
+            description=optical_channel_description,
+            emission_lambda=optical_channel_emission_lambda
+        )
+
+        imaging_plane = nwbfile.create_imaging_plane(
+            name=imaging_name,
+            optical_channel=optical_channel,
+            imaging_rate=imaging_rate,
+            description=f"Imaging plane of {location}",
+            device=microscope,
+            excitation_lambda=excitation_lambda,
+            indicator=indicator,
+            location=location,
+            grid_spacing=grid_spacing,
+            grid_spacing_unit=grid_spacing_unit,
+            origin_coords=origin_coords,
+            origin_coords_unit=origin_coords_unit,
+        )
+
+        two_photon_series = TwoPhotonSeries(
+            name=photon_series_name,
+            description="Images from a TwoPhoton microscope",
+            data=image_data,
+            imaging_plane=imaging_plane,
+            rate=two_photon_rate,
+            unit=two_photon_unit
+        )
+
+        nwbfile.add_acquisition(two_photon_series)
 
     @staticmethod
     def labjack_as_behavioral_data(
             nwbfile,
             labjack_filename=None,
             name=None,
             measured_unit_list=None,
```

### Comparing `simply_nwb-0.0.4/simply_nwb/testing.py` & `simply_nwb-0.0.5/simply_nwb/testing.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,103 +24,140 @@
 tif_subfolder_kwargs = {"parent_folder": "../data/tifs/subfolder_formatted",
                         "subfolder_glob": "file*", "file_glob": "Image.tif"}
 tif_single_filename = "../data/tifs/subfolder_formatted/file/Image.tif"
 # Note: This CSV isn't formatted correctly so it will look weird when loaded
 csv_filename = "../data/20230414_unitR2_session002_leftCam-0000DLC_resnet50_licksNov3shuffle1_1030000.csv"
 
 
-def blackrock_test():
-    d = blackrock_load_data(blackrock_nev_filename)
-    d2 = blackrock_all_spiketrains(blackrock_nev_filename)
-    tw = 2
-
-
-def gen_snwb():
+def nwb_gen():
     return SimpleNWB.create_nwb(
         # Required
-        session_description="Poked mouse with a stick",
+        session_description="Mouse cookie eating session",
         # Subtract 1 year so we don't run into the 'NWB start time is at a greater date than current' issue
         session_start_time=pendulum.now().subtract(years=1),
         experimenter=["Schmoe, Joe"],
         lab="Felsen Lab",
-        experiment_description="Poked a mouse with sticks to see if they would react",
+        experiment_description="Gave a mouse a cookie",
 
         # Optional
-        identifier="Mouse stick poke experiment",
+        identifier="cookie_0",
         subject=Subject(**{
             "subject_id": "1",
             "age": "P90D",  # ISO-8601 for 90 days duration
             "strain": "TypeOfMouseGoesHere",  # If no specific used, 'Wild Strain'
             "description": "Mouse#2 idk",
             "sex": "M",  # M - Male, F - Female, U - unknown, O - other
             # NCBI Taxonomy link or Latin Binomial (e.g.'Rattus norvegicus')
             "species": "http://purl.obolibrary.org/obo/NCBITaxon_10116",
         }),
-        session_id="Session1",
+        session_id="session0",
         institution="CU Anschutz",
         keywords=["mouse"],
 
         # related_publications="DOI::LINK GOES HERE FOR RELATED PUBLICATIONS"
     )
 
 
-def simple_nwb_nev():
-    nwb = gen_snwb()
+def nwb_nev():
+    nwb = nwb_gen()
     SimpleNWB.blackrock_spiketrains_as_units(
         nwb,
         blackrock_filename=blackrock_nev_filename,
-        device_description="BlackRock device hardward #123",
+        device_description="BlackRock device hardware #123",
         electrode_description="Electrode desc",
         electrode_location_description="location description",
         electrode_position=(0.1, 0.2, 0.3),
         # stereotaxic position of this electrode group (x, y, z) (+y is inferior)(+x is posterior)(+z is right) (required)
         electrode_impedance=0.4,  # Impedance in ohms
         electrode_brain_region="brain region desc",
-        electrode_filtering_description="filtering, thresholds descrpition",
+        electrode_filtering_description="filtering, thresholds description",
         electrode_reference_description="stainless steel skull screw",
         # Description of the reference electrode and/or reference scheme used for this electrode, e.g.,"stainless steel skull screw" or "online common average referencing"
 
         # Optional args
         device_manufacturer="BlackRock",
         device_name="BlackRock#4",
         electrode_group_name="electrodegroup0"
     )
-    return nwb
+    # nwb.units["spike_times"][:] # List of spike times
+    return nwb, []
 
 
 def nwb_perg():
-    nwb = gen_snwb()
+    nwb = nwb_gen()
     SimpleNWB.add_p_erg_data(nwb, perg_filename, "perg_table", description="test desc")
     SimpleNWB.add_p_erg_data(nwb, perg_filename, "perg_table", description="test desc")
     SimpleNWB.add_p_erg_folder(nwb, foldername=perg_folder, file_pattern="*.txt", table_name="p_ergs", description="test desc")
-    return nwb
+    # nwb.acquisition["perg_table_data"]["average"][:]
+    # nwb.acquisition["perg_table_metadata"]["channel"][:]
+    return nwb, []
 
 
 def nwb_labjack():
     # Not a true .dat file, should be .txt but whatever
     r = labjack_load_file(labjack_filename)
     r2 = labjack_load_file(labjack_filename2)
 
-    nwbfile = gen_snwb()
+    nwbfile = nwb_gen()
 
     SimpleNWB.labjack_as_behavioral_data(
         nwbfile,
         labjack_filename=labjack_filename,
         name="labjack_file_1",
         measured_unit_list=["idk units"]*9,  # 9 columns for data collected
         start_time=0.0,
         sampling_rate=1.0,
         description="Sampled at 1hz some data description here",
         behavior_module=None,
         behavior_module_name=None,
         comments="Labjack behavioral data"
     )
     # nwbfile.processing["behavior"]["labjack_file_1_behavioral_events"]["Time"].data[:]
+    # nwbfile.processing["behavior"]["labjack_file_1_behavioral_events"]["v0"].data
     # nwbfile.processing["behavior"]["labjack_file_1_metadata"]
-    return nwbfile
+    # nwbfile.processing["behavior"]["labjack_file_1_metadata"]["CH+"]
+    return nwbfile, []
+
+
+def nwb_two_photon():
+    nwb = nwb_gen()
+    data = tif_read_directory(tif_foldername_folder_fmt, filename_glob="*ome.tif")
+
+    SimpleNWB.two_photon_add_data(
+        nwb,
+        device_name="MyMicroscope",
+        device_description="The coolest microscope ever",
+        device_manufacturer="CoolMicroscopes Inc",
+        optical_channel_description="an optical channel",
+        optical_channel_emission_lambda=500.0,  # in nm
+        imaging_name="my_data",
+        imaging_rate=30.0,  # images acquired in Hz
+        excitation_lambda=600.0,  # wavelength in nm
+        indicator="GFP",
+        location="V1",
+        grid_spacing=[0.1, 0.1],
+        grid_spacing_unit="meters",
+        origin_coords=[0.1, 0.1],
+        origin_coords_unit="meters",
+        photon_series_name="MyTwoPhotonSeries",
+        two_photon_unit="normalized amplitude",
+        two_photon_rate=1.0,  # sampling rate in Hz
+        image_data=data
+    )
+    # nwb.acquisition["TwoPhotonSeries"].data
+
+    # Ignore the check_data_orientation check
+    # nwb.acquisition["MyTwoPhotonSeries"].data[:]
+    return nwb, ["check_data_orientation"]
+
+
+def blackrock_test():
+    d = blackrock_load_data(blackrock_nev_filename)
+    d2 = blackrock_all_spiketrains(blackrock_nev_filename)
+    tw = 2
 
 
 def plaintext_metadata_test():
     r = plaintext_metadata_read(metadata_filename)
     tw = 2
 
 
@@ -138,15 +175,14 @@
 def mp4_test():
     r = mp4_read_data(mp4_filename)
     tw = 2
 
 
 def tif_test():
     r = tif_read_image(tif_single_filename)
-    # tif_foldername_and_subfolder_fmt = ("../data/tifs/subfolder_formatted", "file*")
     rr = tif_read_subfolder_directory(**tif_subfolder_kwargs)
     rrr = tif_read_directory(tif_foldername_folder_fmt, filename_glob="*ome.tif")
     tw = 2
 
 
 def util_test():
     # Note: This CSV isn't formatted correctly, so it will look weird when loaded
@@ -159,20 +195,34 @@
     # util_test()
     # blackrock_test()
     # csv_test()
     # plaintext_metadata_test()
     # yaml_test()
     # mp4_test()
     # tif_test()
-    #
+
     funcs_to_assert = [
-        # gen_snwb,
-        # simple_nwb_nev,
-        # nwb_perg,
-        nwb_labjack
+        nwb_nev,
+        nwb_perg,
+        nwb_labjack,
+        nwb_two_photon
     ]
 
+    SimpleNWB.inspect(nwb_gen())
+
     for func in funcs_to_assert:
-        nwb = func()
+        nwb_to_inspect, ignore_error_names = func()
+        results = SimpleNWB.inspect(nwb_to_inspect)
+
+        # Remove ignored errors
+        idxs_to_pop = []
+        for idx, res in enumerate(results):
+            for ignore in ignore_error_names:
+                if res.check_function_name == ignore:
+                    idxs_to_pop.append(idx)
+        idxs_to_pop.reverse()
+        [results.pop(i) for i in idxs_to_pop]
+
         # Should return '[]' so anything not [] will assert False
-        assert not SimpleNWB.inspect(nwb)
+        assert not results
         print("Assert pass")
+    print("All tests passed")
```

### Comparing `simply_nwb-0.0.4/simply_nwb/util.py` & `simply_nwb-0.0.5/simply_nwb/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from hdmf.common import DynamicTable, VectorData
 from nwbinspector import inspect_nwbfile, inspect_nwbfile_object
 from pynwb import NWBHDF5IO, TimeSeries
 import warnings
 import re
 
 
-def read_nwb(filename):
+def nwb_read(filename):
     """
     Read a file from the filesystem into an NWB object
 
     :param filename: filename of an NWB file
     :return: file pointer ready to be .read() to get the nwb object
     """
     # Can't use context manager, will close file, return file pointer
     io = NWBHDF5IO(filename, mode="r")
     return io
 
 
-def write_nwb(nwb_obj, filename):
+def nwb_write(nwb_obj, filename):
     """
     Write an NWB object to a file on the local filesystem
 
     :param nwb_obj: pynwb.file.NWBFile object
     :param filename: path of a local file, doesn't need to exist
     :return: None
     """
```

### Comparing `simply_nwb-0.0.4/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simply-nwb
-Version: 0.0.4
+Name: simply_nwb
+Version: 0.0.5
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.4/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.0.5/simply_nwb.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.rst
 setup.py
 simply_nwb/__init__.py
-simply_nwb/nwb_inspect_script.py
 simply_nwb/simple_nwb.py
 simply_nwb/testing.py
 simply_nwb/util.py
 simply_nwb.egg-info/PKG-INFO
 simply_nwb.egg-info/SOURCES.txt
 simply_nwb.egg-info/dependency_links.txt
 simply_nwb.egg-info/requires.txt
```

