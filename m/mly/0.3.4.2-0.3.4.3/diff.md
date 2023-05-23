# Comparing `tmp/mly-0.3.4.2.tar.gz` & `tmp/mly-0.3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly-0.3.4.2.tar", last modified: Tue May 16 11:17:55 2023, max compression
+gzip compressed data, was "mly-0.3.4.3.tar", last modified: Tue May 23 11:40:00 2023, max compression
```

## Comparing `mly-0.3.4.2.tar` & `mly-0.3.4.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-16 11:17:55.028438 mly-0.3.4.2/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.3.4.2/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-05-16 11:17:55.028438 mly-0.3.4.2/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.3.4.2/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-16 11:17:54.989437 mly-0.3.4.2/mly/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.3.4.2/mly/SRD.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.3.4.2/mly/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10219 2023-05-16 10:32:51.000000 mly-0.3.4.2/mly/createFileSystem.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-16 11:17:55.004438 mly-0.3.4.2/mly/datatools/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      140 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22280 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29349 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    90481 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/generator.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-16 11:17:55.022438 mly-0.3.4.2/mly/datatools/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/tests/test_core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/tests/test_datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4570 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/datatools/tests/test_generator.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18459 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/exceptions.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.3.4.2/mly/mlTools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.3.4.2/mly/models.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.3.4.2/mly/null_energy_map.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7255 2023-05-16 11:13:14.000000 mly-0.3.4.2/mly/offlinefar.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.3.4.2/mly/plugins.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10134 2023-05-04 12:56:19.000000 mly-0.3.4.2/mly/projectwave.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.3.4.2/mly/simulateddetectornoise.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-16 11:17:55.027438 mly-0.3.4.2/mly/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.3.4.2/mly/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.3.4.2/mly/tests/test_init.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.3.4.2/mly/tests/test_tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13014 2023-05-04 12:56:19.000000 mly-0.3.4.2/mly/tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126781 2023-05-04 12:56:19.000000 mly-0.3.4.2/mly/validators.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.3.4.2/mly/waveforms.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-16 11:17:54.998438 mly-0.3.4.2/mly.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-05-16 11:17:54.000000 mly-0.3.4.2/mly.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-05-16 11:17:54.000000 mly-0.3.4.2/mly.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-16 11:17:54.000000 mly-0.3.4.2/mly.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-05-16 11:17:54.000000 mly-0.3.4.2/mly.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-16 11:17:54.000000 mly-0.3.4.2/mly.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-05-16 11:17:55.030438 mly-0.3.4.2/setup.cfg
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      956 2023-05-16 11:17:42.000000 mly-0.3.4.2/setup.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:40:00.244416 mly-0.3.4.3/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.3.4.3/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-05-23 11:40:00.245416 mly-0.3.4.3/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.3.4.3/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:40:00.177415 mly-0.3.4.3/mly/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.3.4.3/mly/SRD.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.3.4.3/mly/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10219 2023-05-16 10:32:51.000000 mly-0.3.4.3/mly/createFileSystem.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:40:00.190415 mly-0.3.4.3/mly/datatools/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      140 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22280 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29349 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    90481 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/generator.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:40:00.222415 mly-0.3.4.3/mly/datatools/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/tests/test_core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/tests/test_datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4570 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/datatools/tests/test_generator.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18459 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/exceptions.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.3.4.3/mly/mlTools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.3.4.3/mly/models.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.3.4.3/mly/null_energy_map.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7255 2023-05-23 11:33:19.000000 mly-0.3.4.3/mly/offlinefar.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.3.4.3/mly/plugins.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10134 2023-05-04 12:56:19.000000 mly-0.3.4.3/mly/projectwave.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.3.4.3/mly/simulateddetectornoise.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:40:00.243416 mly-0.3.4.3/mly/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.3.4.3/mly/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.3.4.3/mly/tests/test_init.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.3.4.3/mly/tests/test_tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13014 2023-05-04 12:56:19.000000 mly-0.3.4.3/mly/tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126771 2023-05-23 11:32:17.000000 mly-0.3.4.3/mly/validators.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.3.4.3/mly/waveforms.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:40:00.185415 mly-0.3.4.3/mly.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-05-23 11:40:00.000000 mly-0.3.4.3/mly.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-05-23 11:40:00.000000 mly-0.3.4.3/mly.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-23 11:40:00.000000 mly-0.3.4.3/mly.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-05-23 11:40:00.000000 mly-0.3.4.3/mly.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-23 11:40:00.000000 mly-0.3.4.3/mly.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-05-23 11:40:00.246416 mly-0.3.4.3/setup.cfg
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      956 2023-05-23 11:34:26.000000 mly-0.3.4.3/setup.py
```

### Comparing `mly-0.3.4.2/LICENSE` & `mly-0.3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/SRD.py` & `mly-0.3.4.3/mly/SRD.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/createFileSystem.py` & `mly-0.3.4.3/mly/createFileSystem.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/datatools/core.py` & `mly-0.3.4.3/mly/datatools/core.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/datatools/datatools.py` & `mly-0.3.4.3/mly/datatools/datatools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/datatools/generator.py` & `mly-0.3.4.3/mly/datatools/generator.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/datatools/tests/test_core.py` & `mly-0.3.4.3/mly/datatools/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/datatools/tests/test_generator.py` & `mly-0.3.4.3/mly/datatools/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/exceptions.py` & `mly-0.3.4.3/mly/exceptions.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/mlTools.py` & `mly-0.3.4.3/mly/mlTools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/models.py` & `mly-0.3.4.3/mly/models.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/null_energy_map.py` & `mly-0.3.4.3/mly/null_energy_map.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/offlinefar.py` & `mly-0.3.4.3/mly/offlinefar.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/plugins.py` & `mly-0.3.4.3/mly/plugins.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/projectwave.py` & `mly-0.3.4.3/mly/projectwave.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/simulateddetectornoise.py` & `mly-0.3.4.3/mly/simulateddetectornoise.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/tests/__init__.py` & `mly-0.3.4.3/mly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/tests/test_init.py` & `mly-0.3.4.3/mly/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/tests/test_tools.py` & `mly-0.3.4.3/mly/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/tools.py` & `mly-0.3.4.3/mly/tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly/validators.py` & `mly-0.3.4.3/mly/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import copy
 from math import ceil
 from dqsegdb2.query import query_segments
 from gwpy.io.kerberos import kinit
 
 from .simulateddetectornoise import *
 from .tools import dirlist,  fromCategorical, correlate,internalLags,circularTimeSlides
-from .datatools import DataPod, DataSet
+from .datatools import DataPod, DataSet, generator
 from gwpy.time import to_gps,from_gps
 from gwpy.segments import DataQualityFlag
 from gwpy.segments import Segment,SegmentList
 
 from gwpy.io.kerberos import kinit
 
 from gwpy.timeseries import TimeSeries
@@ -159,15 +159,15 @@
         for val in looper:
             if hrssInList==True:
 
                 kwargs['injectionHRSS']=val
             else: 
                 injectionSNR=val
 
-            DATA=DataSet.generator(duration = duration
+            DATA= generator(duration = duration
                                    ,fs = fs
                                    ,size = size
                                    ,detectors = detectors
                                    ,injectionFolder = injectionFolder
                                    ,labels = labels
                                    ,backgroundType = backgroundType
                                    ,injectionSNR = injectionSNR
@@ -314,15 +314,15 @@
             strides=1
         elif not (isinstance(strides,int) and strides <= fs and fs%strides==0):
             raise ValueError('Strides must be a divisible integer of sample frequency')
         
         preptime=time.time()
         print("PREP TIME:", preptime-t0)
         # Using a generator for the data to use for testing
-        DATA=DataSet.generator(duration=duration
+        DATA= generator(duration=duration
                                ,fs =fs
                                ,size=size
                                ,detectors=detectors
                                ,labels=labels
                                ,backgroundType=backgroundType
                                ,injectionSNR = 0
                                ,noiseSourceFile =noiseSourceFile
@@ -336,15 +336,15 @@
                                ,**kwargs)   
         t1=time.time()
         print('Time to generation: '+str(t1-t0)+' stride 0')
         t0=time.time()
 
         for st in range(1,strides):
             print('stride:',st,st*(duration/strides))
-            DATA_=DataSet.generator(duration=duration
+            DATA_= generator(duration=duration
                        ,fs =fs
                        ,size=size
                        ,detectors=detectors
                        ,labels=labels
                        ,backgroundType=backgroundType
                        ,injectionSNR = 0
                        ,noiseSourceFile =noiseSourceFile
```

### Comparing `mly-0.3.4.2/mly/waveforms.py` & `mly-0.3.4.3/mly/waveforms.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/mly.egg-info/SOURCES.txt` & `mly-0.3.4.3/mly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.2/setup.py` & `mly-0.3.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mly",
-    version="0.3.4.2",
+    version="0.3.4.3",
     author="Vasileios Skliris",
     author_email='vas.skliris@gmail.com',
     description='This tool helps you create training and testing data for ML to use for gravitational wave detection.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://pypi.python.org/pypi/mly/',
     packages=setuptools.find_packages(),
```

