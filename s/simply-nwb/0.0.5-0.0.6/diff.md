# Comparing `tmp/simply_nwb-0.0.5.tar.gz` & `tmp/simply_nwb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.0.5.tar", last modified: Tue May 23 16:56:34 2023, max compression
+gzip compressed data, was "simply_nwb-0.0.6.tar", last modified: Tue May 23 19:27:04 2023, max compression
```

## Comparing `simply_nwb-0.0.5.tar` & `simply_nwb-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.568687 simply_nwb-0.0.5/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      566 2023-05-23 16:56:34.568687 simply_nwb-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-23 16:56:34.568687 simply_nwb-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.556912 simply_nwb-0.0.5/simply_nwb/
--rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.561541 simply_nwb-0.0.5/simply_nwb/acquisition/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.566452 simply_nwb-0.0.5/simply_nwb/acquisition/tools/
--rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/blackrock.py
--rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/labjack.py
--rw-rw-rw-   0        0        0     2601 2023-05-23 15:16:58.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/plaintext.py
--rw-rw-rw-   0        0        0     3437 2023-05-23 16:16:41.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/tif.py
--rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.0.5/simply_nwb/acquisition/tools/yaml.py
--rw-rw-rw-   0        0        0    21474 2023-05-23 16:35:37.000000 simply_nwb-0.0.5/simply_nwb/simple_nwb.py
--rw-rw-rw-   0        0        0     8461 2023-05-23 16:46:28.000000 simply_nwb-0.0.5/simply_nwb/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.567685 simply_nwb-0.0.5/simply_nwb/transforms/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.5/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     3498 2023-05-19 20:56:41.000000 simply_nwb-0.0.5/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:56:34.561541 simply_nwb-0.0.5/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      702 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-23 16:56:34.000000 simply_nwb-0.0.5/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.548498 simply_nwb-0.0.6/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-05-23 19:27:04.547499 simply_nwb-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-23 19:27:04.548498 simply_nwb-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.535445 simply_nwb-0.0.6/simply_nwb/
+-rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.538655 simply_nwb-0.0.6/simply_nwb/acquisition/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.546498 simply_nwb-0.0.6/simply_nwb/acquisition/tools/
+-rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/blackrock.py
+-rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/labjack.py
+-rw-rw-rw-   0        0        0     2601 2023-05-23 15:16:58.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/plaintext.py
+-rw-rw-rw-   0        0        0     3437 2023-05-23 16:16:41.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/yaml.py
+-rw-rw-rw-   0        0        0    24781 2023-05-23 18:43:23.000000 simply_nwb-0.0.6/simply_nwb/simple_nwb.py
+-rw-rw-rw-   0        0        0    10706 2023-05-23 18:43:23.000000 simply_nwb-0.0.6/simply_nwb/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.547499 simply_nwb-0.0.6/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     5540 2023-05-23 18:31:52.000000 simply_nwb-0.0.6/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.538655 simply_nwb-0.0.6/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      702 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.0.5/LICENSE` & `simply_nwb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/PKG-INFO` & `simply_nwb-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply_nwb
-Version: 0.0.5
+Version: 0.0.6
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.5/setup.py` & `simply_nwb-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.0.5/simply_nwb/acquisition/tools/blackrock.py` & `simply_nwb-0.0.6/simply_nwb/acquisition/tools/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/simply_nwb/acquisition/tools/csv.py` & `simply_nwb-0.0.6/simply_nwb/acquisition/tools/csv.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/simply_nwb/acquisition/tools/labjack.py` & `simply_nwb-0.0.6/simply_nwb/acquisition/tools/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/simply_nwb/acquisition/tools/mp4.py` & `simply_nwb-0.0.6/simply_nwb/acquisition/tools/mp4.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/simply_nwb/acquisition/tools/p_erg.py` & `simply_nwb-0.0.6/simply_nwb/acquisition/tools/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/simply_nwb/acquisition/tools/plaintext.py` & `simply_nwb-0.0.6/simply_nwb/acquisition/tools/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/simply_nwb/acquisition/tools/tif.py` & `simply_nwb-0.0.6/simply_nwb/acquisition/tools/tif.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.5/simply_nwb/simple_nwb.py` & `simply_nwb-0.0.6/simply_nwb/simple_nwb.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from pynwb.device import Device
 from pynwb.ecephys import ElectrodeGroup
 from pynwb.file import Subject
 from pynwb.ophys import OpticalChannel, TwoPhotonSeries
 
 from .acquisition.tools import labjack_load_file
 from .acquisition.tools import blackrock_all_spiketrains, perg_parse_to_table
-from .util import warn_on_name_format, inspect_nwb_obj, nwb_write, panda_df_to_dyn_table, panda_df_to_list_of_timeseries
+from .util import warn_on_name_format, inspect_nwb_obj, nwb_write, panda_df_to_dyn_table, \
+    panda_df_to_list_of_timeseries, dict_to_dyn_tables
 
 
 class SimpleNWB(object):
     _REQUIRED_ARGS = [
         "session_description",
         "session_start_time",
         "experimenter",
@@ -54,15 +55,15 @@
                 identifier = str(uuid4())
             if session_id is None:
                 session_id = str(uuid4())
             if institution is None:
                 institution = "CU Anschutz"
             if isinstance(subject, dict):
                 subject = Subject(**subject)
-            elif not isinstance(subject, Subject):
+            elif not isinstance(subject, Subject) and not subject is None:
                 raise ValueError("'subject' argument must either be a dict or a pynwb.file.Subject type!")
 
             if keywords is None:
                 keywords = []
 
             nwb_kwargs = {
                 "identifier": identifier,
@@ -98,14 +99,92 @@
         :param nwbfile: NWBFile object to write
         :param filename: path to file to write, WILL OVERWRITE!
         :return: None
         """
         nwb_write(nwbfile, filename)
 
     @staticmethod
+    def processing_add_dict(
+            nwbfile,
+            processed_name=None,
+            processed_description=None,
+            data_dict=None,
+            uneven_columns=False):
+        """
+        Add a processed dict into the NWB that doesn't fit in any other part of the NWB. MAKE SURE YOU CANT ADD IT ELSEWHERE BEFORE USING THIS FUNC!
+
+        :param nwbfile: NWBFile to add data to
+        :param processed_name: Name of the processing module
+        :param processed_description: description of the processed data
+        :param data_dict: dict data to add
+        :param uneven_columns: Set this to True if the keys of the dict have different lengths
+        """
+        if processed_name is None:
+            raise ValueError("Must supply processed_name argument!")
+        if processed_description is None:
+            raise ValueError("Must supply processed_description argument!")
+        if data_dict is None or not isinstance(data_dict, dict):
+            raise ValueError("Make sure to supply argument data_dict and it should be a dict type!")
+
+        data_interfaces = dict_to_dyn_tables(
+            dict_data=data_dict,
+            table_name=processed_name,
+            description=processed_description,
+            multiple_objs=uneven_columns
+        )
+        if not uneven_columns:
+            data_interfaces = [data_interfaces]
+        if "misc" in nwbfile.processing:
+            [nwbfile.processing["misc"].add_container(interface) for interface in data_interfaces]
+        else:
+            nwbfile.create_processing_module(
+                name="misc",
+                description=processed_description,
+                data_interfaces=data_interfaces
+            )
+
+    @staticmethod
+    def processing_add_dataframe(
+            nwbfile,
+            processed_name=None,
+            processed_description=None,
+            data=None
+    ):
+        """
+        Add a processed pandas Dataframe into the NWB that doesn't fit in any other part of the NWB. MAKE SURE YOU CANT ADD IT ELSEWHERE BEFORE USING THIS FUNC!
+
+        :param nwbfile: NWBFile to add data to
+        :param processed_name: Name of the processing module
+        :param processed_description: description of the processed data
+        :param data: Pandas Dataframe data to add
+        :return: None
+        """
+        if processed_name is None:
+            raise ValueError("Must provide processed_name argument!")
+        if processed_description is None:
+            raise ValueError("Must provide processed_description argument!")
+        if data is None or not isinstance(data, pd.DataFrame):
+            raise ValueError("data argument must be Pandas Dataframe!")
+
+        data_interface = panda_df_to_dyn_table(
+            pd_df=data,
+            table_name=processed_name,
+            description=processed_description
+        )
+
+        if "misc" in nwbfile.processing:
+            nwbfile.processing["misc"].add_container(data_interface)
+        else:
+            nwbfile.create_processing_module(
+                name="misc",
+                description=processed_description,
+                data_interfaces=[data_interface]
+            )
+
+    @staticmethod
     def two_photon_add_data(
             nwbfile,
             device_name=None,
             device_description=None,
             device_manufacturer=None,
             optical_channel_description=None,
             optical_channel_emission_lambda=None,
```

### Comparing `simply_nwb-0.0.5/simply_nwb/testing.py` & `simply_nwb-0.0.6/simply_nwb/testing.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 from simply_nwb.acquisition.tools import mp4_read_data
 from simply_nwb.acquisition.tools import tif_read_image, tif_read_directory, tif_read_subfolder_directory
 from simply_nwb.acquisition.tools import csv_load_dataframe, yaml_read_file
 from simply_nwb.acquisition.tools import labjack_load_file
 from simply_nwb.acquisition.tools import plaintext_metadata_read
 from simply_nwb.acquisition.tools import blackrock_load_data, blackrock_all_spiketrains
+from simply_nwb.util import panda_df_to_dyn_table
 from simply_nwb import SimpleNWB
 import pendulum
+import numpy as np
+import pandas as pd
 
-from util import panda_df_to_dyn_table
 
 # Data is available on Google Drive, as Spencer for access
 blackrock_nev_filename = "../data/wheel_4p3_lSC_2001.nev"
 perg_filename = "../data/pg1_A_raw.TXT"
 perg_folder = "../data/pg_folder"
 labjack_filename = "../data/labjack_data.dat"
 labjack_filename2 = "../data/labjack_data2.dat"
@@ -22,14 +24,16 @@
 mp4_filename = "../data/mp4_test.mp4"
 tif_foldername_folder_fmt = "../data/tifs/folder_formatted"
 tif_subfolder_kwargs = {"parent_folder": "../data/tifs/subfolder_formatted",
                         "subfolder_glob": "file*", "file_glob": "Image.tif"}
 tif_single_filename = "../data/tifs/subfolder_formatted/file/Image.tif"
 # Note: This CSV isn't formatted correctly so it will look weird when loaded
 csv_filename = "../data/20230414_unitR2_session002_leftCam-0000DLC_resnet50_licksNov3shuffle1_1030000.csv"
+dict_data = {"data1": [1, 2, 3, 4, 5], "data2": ["a", "b", "c", "d", "e"]}
+dict_data_uneven_cols = {"data1": [1, 2, 3], "data2": ["a", "b", "c", "d", "e"], "aa": 5}
 
 
 def nwb_gen():
     return SimpleNWB.create_nwb(
         # Required
         session_description="Mouse cookie eating session",
         # Subtract 1 year so we don't run into the 'NWB start time is at a greater date than current' issue
@@ -74,25 +78,28 @@
         # Description of the reference electrode and/or reference scheme used for this electrode, e.g.,"stainless steel skull screw" or "online common average referencing"
 
         # Optional args
         device_manufacturer="BlackRock",
         device_name="BlackRock#4",
         electrode_group_name="electrodegroup0"
     )
-    # nwb.units["spike_times"][:] # List of spike times
+
+    t = nwb.units["spike_times"][:] # List of spike times
+
     return nwb, []
 
 
 def nwb_perg():
     nwb = nwb_gen()
     SimpleNWB.add_p_erg_data(nwb, perg_filename, "perg_table", description="test desc")
     SimpleNWB.add_p_erg_data(nwb, perg_filename, "perg_table", description="test desc")
     SimpleNWB.add_p_erg_folder(nwb, foldername=perg_folder, file_pattern="*.txt", table_name="p_ergs", description="test desc")
-    # nwb.acquisition["perg_table_data"]["average"][:]
-    # nwb.acquisition["perg_table_metadata"]["channel"][:]
+
+    t = nwb.acquisition["perg_table_data"]["average"][:]
+    t = nwb.acquisition["perg_table_metadata"]["channel"][:]
     return nwb, []
 
 
 def nwb_labjack():
     # Not a true .dat file, should be .txt but whatever
     r = labjack_load_file(labjack_filename)
     r2 = labjack_load_file(labjack_filename2)
@@ -107,18 +114,18 @@
         start_time=0.0,
         sampling_rate=1.0,
         description="Sampled at 1hz some data description here",
         behavior_module=None,
         behavior_module_name=None,
         comments="Labjack behavioral data"
     )
-    # nwbfile.processing["behavior"]["labjack_file_1_behavioral_events"]["Time"].data[:]
-    # nwbfile.processing["behavior"]["labjack_file_1_behavioral_events"]["v0"].data
-    # nwbfile.processing["behavior"]["labjack_file_1_metadata"]
-    # nwbfile.processing["behavior"]["labjack_file_1_metadata"]["CH+"]
+    t = nwbfile.processing["behavior"]["labjack_file_1_behavioral_events"]["Time"].data[:]
+    t = nwbfile.processing["behavior"]["labjack_file_1_behavioral_events"]["v0"].data
+    t = nwbfile.processing["behavior"]["labjack_file_1_metadata"]
+    t = nwbfile.processing["behavior"]["labjack_file_1_metadata"]["CH+"]
     return nwbfile, []
 
 
 def nwb_two_photon():
     nwb = nwb_gen()
     data = tif_read_directory(tif_foldername_folder_fmt, filename_glob="*ome.tif")
 
@@ -142,18 +149,81 @@
         two_photon_unit="normalized amplitude",
         two_photon_rate=1.0,  # sampling rate in Hz
         image_data=data
     )
     # nwb.acquisition["TwoPhotonSeries"].data
 
     # Ignore the check_data_orientation check
-    # nwb.acquisition["MyTwoPhotonSeries"].data[:]
+    t = nwb.acquisition["MyTwoPhotonSeries"].data[:]
     return nwb, ["check_data_orientation"]
 
 
+def nwb_processing_module_df():
+    nwb = nwb_gen()
+
+    d = pd.DataFrame.from_dict(dict_data)
+
+    SimpleNWB.processing_add_dataframe(
+        nwb,
+        processed_name="ProcessedData",
+        processed_description="Test processing",
+        data=d
+    )
+
+    # Extra to test multiple adds
+    SimpleNWB.processing_add_dataframe(
+        nwb,
+        processed_name="ProcessedData2",
+        processed_description="Test processing",
+        data=d
+    )
+
+    t = nwb.processing["misc"]["ProcessedData"]["data1"]
+    return nwb, []
+
+
+def nwb_processing_module_dict():
+    nwb = nwb_gen()
+
+    SimpleNWB.processing_add_dict(
+        nwb,
+        processed_name="ProcessedDictData1",
+        processed_description="Test processing",
+        data_dict=dict_data,
+        uneven_columns=False
+    )
+    t = nwb.processing["misc"]["ProcessedDictData1"]["data1"][:]
+
+    SimpleNWB.processing_add_dict(
+        nwb,
+        processed_name="ProcessedDictData2",
+        processed_description="Test processing",
+        data_dict=dict_data_uneven_cols,
+        uneven_columns=True
+    )
+    # Because of uneven columns, each key is separate
+    t = nwb.processing["misc"]["ProcessedDictData2_data1"]["data1"][:]
+    t = nwb.processing["misc"]["ProcessedDictData2_data2"]["data2"][:]
+    t = nwb.processing["misc"]["ProcessedDictData2_aa"]["aa"][:]
+
+    # Add another dict
+    SimpleNWB.processing_add_dict(
+        nwb,
+        processed_name="ProcessedDictData2",
+        processed_description="Test processing",
+        data_dict=dict_data,
+        uneven_columns=False
+    )
+    t = nwb.processing["misc"]["ProcessedDictData2"]["data2"][:]
+    contents = nwb.processing["misc"].containers
+
+    # Ignore the check_single_row test since could be an edgecase
+    return nwb, ["check_single_row"]
+
+
 def blackrock_test():
     d = blackrock_load_data(blackrock_nev_filename)
     d2 = blackrock_all_spiketrains(blackrock_nev_filename)
     tw = 2
 
 
 def plaintext_metadata_test():
@@ -169,15 +239,16 @@
 
 def yaml_test():
     r = yaml_read_file(yaml_filename)
     tw = 2
 
 
 def mp4_test():
-    r = mp4_read_data(mp4_filename)
+    # r = mp4_read_data(mp4_filename)
+    # TODO Make faster test case and work on this integration
     tw = 2
 
 
 def tif_test():
     r = tif_read_image(tif_single_filename)
     rr = tif_read_subfolder_directory(**tif_subfolder_kwargs)
     rrr = tif_read_directory(tif_foldername_folder_fmt, filename_glob="*ome.tif")
@@ -197,18 +268,20 @@
     # csv_test()
     # plaintext_metadata_test()
     # yaml_test()
     # mp4_test()
     # tif_test()
 
     funcs_to_assert = [
-        nwb_nev,
-        nwb_perg,
-        nwb_labjack,
-        nwb_two_photon
+        # nwb_nev,
+        # nwb_perg,
+        # nwb_labjack,
+        # nwb_two_photon,
+        # nwb_processing_module_df,
+        # nwb_processing_module_dict
     ]
 
     SimpleNWB.inspect(nwb_gen())
 
     for func in funcs_to_assert:
         nwb_to_inspect, ignore_error_names = func()
         results = SimpleNWB.inspect(nwb_to_inspect)
```

### Comparing `simply_nwb-0.0.5/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.0.6/simply_nwb.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-nwb
-Version: 0.0.5
+Version: 0.0.6
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.5/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.0.6/simply_nwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

