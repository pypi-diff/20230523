# Comparing `tmp/TorchPIV-0.1.0.tar.gz` & `tmp/TorchPIV-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchPIV-0.1.0.tar", last modified: Tue May 23 03:15:34 2023, max compression
+gzip compressed data, was "TorchPIV-0.1.1.tar", last modified: Tue May 23 03:33:44 2023, max compression
```

## Comparing `TorchPIV-0.1.0.tar` & `TorchPIV-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:34.633422 TorchPIV-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-05-22 09:07:57.000000 TorchPIV-0.1.0/LICENCE.txt
--rw-rw-rw-   0        0        0     2448 2023-05-23 03:15:34.633422 TorchPIV-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1922 2023-05-23 03:15:11.000000 TorchPIV-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2023-05-22 09:16:41.000000 TorchPIV-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1038 2023-05-23 03:15:34.639406 TorchPIV-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:34.595798 TorchPIV-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:34.622451 TorchPIV-0.1.0/src/TorchPIV.egg-info/
--rw-rw-rw-   0        0        0     2448 2023-05-23 03:15:34.000000 TorchPIV-0.1.0/src/TorchPIV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-05-23 03:15:34.000000 TorchPIV-0.1.0/src/TorchPIV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      195 2023-05-23 03:15:34.000000 TorchPIV-0.1.0/src/TorchPIV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-23 03:15:34.000000 TorchPIV-0.1.0/src/TorchPIV.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 03:15:34.000000 TorchPIV-0.1.0/src/TorchPIV.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:34.631427 TorchPIV-0.1.0/src/torchPIV/
--rw-rw-rw-   0        0        0    17240 2023-05-22 10:05:56.000000 TorchPIV-0.1.0/src/torchPIV/ControlsWidgets.py
--rw-rw-rw-   0        0        0    31145 2023-05-22 10:02:28.000000 TorchPIV-0.1.0/src/torchPIV/PIVbackend.py
--rw-rw-rw-   0        0        0    11894 2023-05-22 10:04:04.000000 TorchPIV-0.1.0/src/torchPIV/PIVwidgets.py
--rw-rw-rw-   0        0        0     5481 2023-05-22 14:35:51.000000 TorchPIV-0.1.0/src/torchPIV/PlotterFunctions.py
--rw-rw-rw-   0        0        0       84 2023-05-22 10:07:12.000000 TorchPIV-0.1.0/src/torchPIV/__init__.py
--rw-rw-rw-   0        0        0     9264 2023-05-22 10:05:31.000000 TorchPIV-0.1.0/src/torchPIV/mainWindow.py
--rw-rw-rw-   0        0        0      391 2023-05-22 15:16:46.000000 TorchPIV-0.1.0/src/torchPIV/settings.json
--rw-rw-rw-   0        0        0      606 2023-05-22 09:09:13.000000 TorchPIV-0.1.0/src/torchPIV/watchman.py
--rw-rw-rw-   0        0        0     6918 2023-05-22 10:03:07.000000 TorchPIV-0.1.0/src/torchPIV/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.780071 TorchPIV-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 09:07:57.000000 TorchPIV-0.1.1/LICENCE.txt
+-rw-rw-rw-   0        0        0     2660 2023-05-23 03:33:44.780071 TorchPIV-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2134 2023-05-23 03:32:06.000000 TorchPIV-0.1.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-22 09:16:41.000000 TorchPIV-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      815 2023-05-23 03:33:44.781068 TorchPIV-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.749153 TorchPIV-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.768103 TorchPIV-0.1.1/src/TorchPIV.egg-info/
+-rw-rw-rw-   0        0        0     2660 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.778077 TorchPIV-0.1.1/src/torchPIV/
+-rw-rw-rw-   0        0        0    17240 2023-05-22 10:05:56.000000 TorchPIV-0.1.1/src/torchPIV/ControlsWidgets.py
+-rw-rw-rw-   0        0        0    31145 2023-05-22 10:02:28.000000 TorchPIV-0.1.1/src/torchPIV/PIVbackend.py
+-rw-rw-rw-   0        0        0    11894 2023-05-22 10:04:04.000000 TorchPIV-0.1.1/src/torchPIV/PIVwidgets.py
+-rw-rw-rw-   0        0        0     5481 2023-05-22 14:35:51.000000 TorchPIV-0.1.1/src/torchPIV/PlotterFunctions.py
+-rw-rw-rw-   0        0        0       84 2023-05-22 10:07:12.000000 TorchPIV-0.1.1/src/torchPIV/__init__.py
+-rw-rw-rw-   0        0        0     9264 2023-05-22 10:05:31.000000 TorchPIV-0.1.1/src/torchPIV/mainWindow.py
+-rw-rw-rw-   0        0        0      391 2023-05-22 15:16:46.000000 TorchPIV-0.1.1/src/torchPIV/settings.json
+-rw-rw-rw-   0        0        0      606 2023-05-22 09:09:13.000000 TorchPIV-0.1.1/src/torchPIV/watchman.py
+-rw-rw-rw-   0        0        0     6918 2023-05-22 10:03:07.000000 TorchPIV-0.1.1/src/torchPIV/workers.py
```

### Comparing `TorchPIV-0.1.0/LICENCE.txt` & `TorchPIV-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/PKG-INFO` & `TorchPIV-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchPIV
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package for PIV data analysis
 Home-page: https://github.com/NikNazarov/TorchPIV
 Author: Nikita Nazarov
 Author-email: nazarov.nik.an@gmail.com
 Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,21 @@
 9. Supported image formats (bmp, jpg, tiff, ect.)
 10. Options for saving program results
 
 __Installation:__    
 It is easier to use conda environment.
 1. Install nvidia CUDA Toolkit https://developer.nvidia.com/cuda-toolkit to ensure latest nvidia driver usage
 2. Install pytorch with GPU support https://pytorch.org/ . Matching your CUDA version is not critical since PyTorch installs it's own cudatoolkit.  
+3. In your environment or command line <code>pip install TorchPIV</code>
+
+__Usage:__  
+Start GUI version from terminal  
+<code>python</code>  
+<code>import torchPIV</code>  
+<code>torchPIV.runGUI()</code>
 
 Tested on Windows
 
 __Performance__:  
 This method allows processing 4 thousand pairs of images with a size of 4 MP each with a search window of 64, overlap of 50%, two iterations with re-arranging (an increase in the number of vectors by 4 times) in less than 10 minutes. The first iteration of the algorithm (~[4000, 64, 64] subimage tensor) takes ~15 ms on a Geforce GTX 1660 Ti GPU.
 
 __Futhure plans__:
```

### Comparing `TorchPIV-0.1.0/README.md` & `TorchPIV-0.1.1/src/TorchPIV.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: TorchPIV
+Version: 0.1.1
+Summary: Package for PIV data analysis
+Home-page: https://github.com/NikNazarov/TorchPIV
+Author: Nikita Nazarov
+Author-email: nazarov.nik.an@gmail.com
+Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 # PyTorch accelerated Particle Image Velocimetry
 This program implements the basic algorithms of the PIV method, such as an iterative cross-correlation method based on FFT with an integer and continuous displacement __(DWS, CWS)__ of the interrogation windows, filtering and interpolation of the pair loss effect, and so on. At this stage, the __graphical interface__ is available, the ability to select PIV hyperparameters. The key feature of the project is the use of graphics accelerators due to the __torch__ library. PIV algorithm is completely vectorized, what results in a very high performance using the GPU, but still has a room for improvement.
 
 __Parameters of the program:__
 1. Interrogation window size
 2. Window overlap size
 3. Coordinate scale
@@ -13,14 +28,21 @@
 9. Supported image formats (bmp, jpg, tiff, ect.)
 10. Options for saving program results
 
 __Installation:__    
 It is easier to use conda environment.
 1. Install nvidia CUDA Toolkit https://developer.nvidia.com/cuda-toolkit to ensure latest nvidia driver usage
 2. Install pytorch with GPU support https://pytorch.org/ . Matching your CUDA version is not critical since PyTorch installs it's own cudatoolkit.  
+3. In your environment or command line <code>pip install TorchPIV</code>
+
+__Usage:__  
+Start GUI version from terminal  
+<code>python</code>  
+<code>import torchPIV</code>  
+<code>torchPIV.runGUI()</code>
 
 Tested on Windows
 
 __Performance__:  
 This method allows processing 4 thousand pairs of images with a size of 4 MP each with a search window of 64, overlap of 50%, two iterations with re-arranging (an increase in the number of vectors by 4 times) in less than 10 minutes. The first iteration of the algorithm (~[4000, 64, 64] subimage tensor) takes ~15 ms on a Geforce GTX 1660 Ti GPU.
 
 __Futhure plans__:
```

### Comparing `TorchPIV-0.1.0/src/TorchPIV.egg-info/SOURCES.txt` & `TorchPIV-0.1.1/src/TorchPIV.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/src/torchPIV/ControlsWidgets.py` & `TorchPIV-0.1.1/src/torchPIV/ControlsWidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/src/torchPIV/PIVbackend.py` & `TorchPIV-0.1.1/src/torchPIV/PIVbackend.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/src/torchPIV/PIVwidgets.py` & `TorchPIV-0.1.1/src/torchPIV/PIVwidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/src/torchPIV/PlotterFunctions.py` & `TorchPIV-0.1.1/src/torchPIV/PlotterFunctions.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/src/torchPIV/mainWindow.py` & `TorchPIV-0.1.1/src/torchPIV/mainWindow.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/src/torchPIV/watchman.py` & `TorchPIV-0.1.1/src/torchPIV/watchman.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.0/src/torchPIV/workers.py` & `TorchPIV-0.1.1/src/torchPIV/workers.py`

 * *Files identical despite different names*

