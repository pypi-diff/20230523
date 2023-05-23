# Comparing `tmp/install-pybci-0.1.4b9.tar.gz` & `tmp/install-pybci-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.1.4b9.tar", last modified: Mon May 22 11:54:25 2023, max compression
+gzip compressed data, was "install-pybci-0.2.0b0.tar", last modified: Tue May 23 18:35:00 2023, max compression
```

## Comparing `install-pybci-0.1.4b9.tar` & `install-pybci-0.2.0b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 11:54:25.000000 install-pybci-0.1.4b9/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14692 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:54:25.570451 install-pybci-0.1.4b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-22 11:53:52.000000 install-pybci-0.1.4b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.309146 install-pybci-0.2.0b0/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.309146 install-pybci-0.2.0b0/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.309146 install-pybci-0.2.0b0/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/setup.py
```

### Comparing `install-pybci-0.1.4b9/LICENSE` & `install-pybci-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b9/PKG-INFO` & `install-pybci-0.2.0b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b9
+Version: 0.2.0b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
+The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
 (currently using install-pybci due to pybci having name too similar with another package on pypi)
@@ -64,22 +64,17 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion.
-
-Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG", since data analysis, preprocessing and feature extraction between devices can vary greatly, this is why custom feature extraction classes can be created for each data stream maker type. 
-
-Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state).
-
-The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware. 
-
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
+Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
+Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - Combine multiple data streams for multi modal bci!
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.1.4b9/README.md` & `install-pybci-0.2.0b0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
+The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
 (currently using install-pybci due to pybci having name too similar with another package on pypi)
@@ -40,22 +40,17 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion.
-
-Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG", since data analysis, preprocessing and feature extraction between devices can vary greatly, this is why custom feature extraction classes can be created for each data stream maker type. 
-
-Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state).
-
-The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware. 
-
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
+Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
+Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - Combine multiple data streams for multi modal bci!
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.1.4b9/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.0b0/install_pybci.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b9
+Version: 0.2.0b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
 A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
+The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
 (currently using install-pybci due to pybci having name too similar with another package on pypi)
@@ -64,22 +64,17 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion.
-
-Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG", since data analysis, preprocessing and feature extraction between devices can vary greatly, this is why custom feature extraction classes can be created for each data stream maker type. 
-
-Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state).
-
-The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware. 
-
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
+Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
+Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - Combine multiple data streams for multi modal bci!
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.1.4b9/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.0b0/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b9/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.0b0/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b9/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.0b0/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b9/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.0b0/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b9/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.2.0b0/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,35 +29,40 @@
         while not self.closeEvent.is_set():
             if self.markerCountRetrieveEvent.is_set():
                 self.markerCountQueue.put(self.epochCounts)
             if self.trainTestEvent.is_set(): # We're training!
                 try:
                     #print(len(self.dataQueueTrain.get_nowait()))
                     dataFIFOs, currentMarker, sr, devCount = self.dataQueueTrain.get_nowait() #[sliceDataFIFOs, self.currentMarker, self.sr, self.devCount
-                    lastDevice = self.ReceiveMarker(currentMarker, devCount)
+                    #lastDevice = self.ReceiveMarker(currentMarker, devCount)
+                    if currentMarker in self.epochCounts:
+                        self.epochCounts[currentMarker][1] += 1
+                    else:
+                        self.epochCounts[currentMarker] = [len(self.epochCounts.keys()),1]
                     target = self.epochCounts[currentMarker][0]
                     features = self.featureExtractor.ProcessFeatures(dataFIFOs, sr, target) # allows custom epoch class to be passed
                     # add logic to ensure all devices epoch data has been received (totalDevices)
-                    if lastDevice:
-                        self.featureQueueTrain.put( [features, target, self.epochCounts] )
-                    else:
+                    #if lastDevice:
+                    self.featureQueueTrain.put( [features, devCount, target, self.epochCounts] )
+                    #else:
                         # needs logic to append features together across devices (requires flattening of channels to 1d array of features)
                         # same for test mode
-                        pass
+                    #    pass
                 except queue.Empty:
                     pass
             else:
                 try:
                     #print("we ain't dataQueueTesting: FeatureProcessorThread")
                     dataFIFOs, sr, devCount = self.dataQueueTest.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, ]
                     features = self.featureExtractor.ProcessFeatures(dataFIFOs, sr, None)
-                    self.featureQueueTest.put(features)
+                    self.featureQueueTest.put([features, devCount])
                 except queue.Empty:
                     pass
 
+    '''
     def ReceiveMarker(self, marker, devCount):
         """ Tracks count of epoch markers in dict self.epochCounts - used for syncing data between multiple devices in function self.run() """
         if self.totalDevices == 1:
             if len(self.customEpochSettings.keys())>0: #  custom marker received
                 if marker in self.customEpochSettings.keys():
                     if marker in self.epochCounts:
                         self.epochCounts[marker][1] += 1
@@ -84,8 +89,9 @@
                         self.epochCounts[marker] = [len(self.epochCounts.keys()),1]
             self.tempDeviceEpochLogger[devCount] = 1
             if all(element == 1 for element in self.tempDeviceEpochLogger): # first device of epoch received
                 self.tempDeviceEpochLogger = [0 for x in range(self.totalDevices)]
                 return True
             else:
                 return False
-            # we need to log each type of device and make sure the same number is received of each
+            # we need to log each type of device and make sure the same number is received of each
+    '''
```

### Comparing `install-pybci-0.1.4b9/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.0b0/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b9/pybci/Utils/Classifier.py` & `install-pybci-0.2.0b0/pybci/Utils/Classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         elif self.classifierLibrary == "tensor":
             if all(item == y_train[0] for item in y_train):
                 pass
             else:
                 #print(np.array(x_train).shape)
                 #print(y_train)
 
-                self.model.fit(np.array(x_train), np.array(y_train)) # epochs and batch_size should be customisable
+                self.model.fit(x_train, y_train) # epochs and batch_size should be customisable
                 self.loss, self.accuracy = self.model.evaluate(np.array(x_test), np.array(y_test))
                 #print("Classification accuracy (tf):" +str(self.accuracy))
         else:
             # no classifier library selected, print debug?
             pass
 
     def TestModel(self, x):
@@ -67,20 +67,22 @@
         #    x = np.array([x.flatten()])
         #else:
         #    x = np.array(x)
         #print(x)
         #print(x.shape)
         if self.classifierLibrary == "sklearn":
             x = np.expand_dims(x, axis=0)
+            #print(x.shape)
             return self.clf.predict(x)
             #print("we predict it's: "+str(self.y_pred))
         elif self.classifierLibrary == "tensor":
             # Predict the class labels for the test data
             #print(x)
             x = np.expand_dims(x, axis=0)
+            #print(x.shape)
             predictions = self.model.predict(x)
             if len (predictions[0]) == 1: # assume binary classification
                 return 1 if predictions[0] > 0.5 else 0
             else:    # assume multi-classification
                 return np.argmax(predictions[0])
             #print("we predict it's: "+str(y_pred))
             # Convert the predicted probabilities to class labels
```

### Comparing `install-pybci-0.1.4b9/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.0b0/pybci/Utils/FeatureExtractor.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,62 +59,62 @@
                         idx_band = np.logical_and(freqs >= band[0], freqs <= band[1])
                         #if len(psd[idx_band]) == 1: # if freq band is only in one field just pass single value instead of calculating average
                         #print(ch)
                         bp = np.mean(psd[idx_band])
                         #else:
                         #    bp = simps(psd[idx_band], dx=(freqs[1]-freqs[0])) / (band[1] - band[0])
                             #bp = simpson(psd[idx_band], dx=freq_res)
-                        features[(k*numchs)+l] = bp
+                        features[(k* self.numFeatures)+l] = bp
                     else:
-                        features[(k*numchs)+l] = 0
+                        features[(k* self.numFeatures)+l] = 0
             else:
                 freqs, psd = welch(ch, sr)# calculate for mean and median
                 l = -1 # accounts for no freqbands being selected
             if self.featureChoices.meanPSD: # mean power
                 l += 1
-                if len(freqs) > 0: features[(k*numchs)+l] = np.mean(psd) # len(freqs) can be 0 if signal is all DC
-                else: features[(k*numchs)+l] = 0
+                if len(freqs) > 0: features[(k* self.numFeatures)+l] = np.mean(psd) # len(freqs) can be 0 if signal is all DC
+                else: features[(k* self.numFeatures)+l] = 0
             if self.featureChoices.medianPSD: # median Power
                 l += 1   
-                if len(freqs) > 0: features[(k*numchs)+l] = np.median(psd) # len(freqs) can be 0 if signal is all DC
-                else: features[(k*numchs)+l] = 0
+                if len(freqs) > 0: features[(k* self.numFeatures)+l] = np.median(psd) # len(freqs) can be 0 if signal is all DC
+                else: features[(k* self.numFeatures)+l] = 0
             if self.featureChoices.appr_entropy:  # Approximate entorpy(X,M,R) X = data, M is , R is 30% standard deviation of X 
                 l += 1
-                features[(k*numchs)+l] = ant.app_entropy(ch) 
+                features[(k* self.numFeatures)+l] = ant.app_entropy(ch) 
             if self.featureChoices.perm_entropy: # permutation_entropy
                 l += 1
-                features[(k*numchs)+l] = ant.perm_entropy(ch,normalize=True)
+                features[(k* self.numFeatures)+l] = ant.perm_entropy(ch,normalize=True)
             if self.featureChoices.spec_entropy:  # spectral Entropy
                 l += 1
-                features[(k*numchs)+l] = ant.spectral_entropy(ch, sf=sr, method='welch', nperseg = len(ch), normalize=True)
+                features[(k* self.numFeatures)+l] = ant.spectral_entropy(ch, sf=sr, method='welch', nperseg = len(ch), normalize=True)
             if self.featureChoices.svd_entropy:# svd Entropy
                 l += 1
-                features[(k*numchs)+l] = ant.svd_entropy(ch, normalize=True)
+                features[(k* self.numFeatures)+l] = ant.svd_entropy(ch, normalize=True)
             if self.featureChoices.samp_entropy: # sample Entropy
                 l += 1
-                features[(k*numchs)+l] = ant.sample_entropy(ch)
+                features[(k* self.numFeatures)+l] = ant.sample_entropy(ch)
             if self.featureChoices.rms: # rms
                 l += 1
-                features[(k*numchs)+l] = np.sqrt(np.mean(np.array(ch)**2))
+                features[(k* self.numFeatures)+l] = np.sqrt(np.mean(np.array(ch)**2))
             if self.featureChoices.variance: # variance
                 l += 1    
-                features[(k*numchs)+l] =  np.var(ch)
+                features[(k* self.numFeatures)+l] =  np.var(ch)
             if self.featureChoices.meanAbs: # Mean Absolute Value 
                 l += 1
-                features[(k*numchs)+l] = sum([np.linalg.norm(c) for c in ch])/len(ch)
+                features[(k* self.numFeatures)+l] = sum([np.linalg.norm(c) for c in ch])/len(ch)
             if self.featureChoices.waveformLength: # waveformLength
                 l += 1
-                features[(k*numchs)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
+                features[(k* self.numFeatures)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
             if self.featureChoices.zeroCross: # zeroCross
                 l += 1
-                features[(k*numchs)+l] = sum([1 if c*ch[inum+1]<0 else 0 for inum, c in enumerate(ch[:-1])])
+                features[(k* self.numFeatures)+l] = sum([1 if c*ch[inum+1]<0 else 0 for inum, c in enumerate(ch[:-1])])
             if self.featureChoices.slopeSignChange: # slopeSignChange
                 l += 1    
                 ssc = sum([1 if (c-ch[inum+1])*(c-ch[inum+1])>=0.1 else 0 for inum, c in enumerate(ch[:-1])])
-                features[(k*numchs)+l] = ssc
+                features[(k* self.numFeatures)+l] = ssc
         features[np.isnan(features)] = 0 # checks for nans
         features[features == np.inf] = 0 # checks for infs
         return features
     
 class GazeFeatureExtractor():
     def __init__(self):
         super().__init__()
```

### Comparing `install-pybci-0.1.4b9/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.0b0/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b9/pybci/pybci.py` & `install-pybci-0.2.0b0/pybci/pybci.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,22 +148,22 @@
         for stream in self.dataStreams:
             self.dataQueueTrain = queue.Queue()
             self.dataQueueTest = queue.Queue()
 
             if stream.info().nominal_srate() == 0:
                 if stream.info().name() in self.streamChsDropDict.keys():
                     dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads), self.streamChsDropDict[stream.info().name()])
+                                            self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
                 else:
                     dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
                                             self.globalEpochSettings, len(self.dataThreads))
             else: # cold be desirable to capture samples only relative to timestammps with async, so maybe make this configurable?
                 if stream.info().name() in self.streamChsDropDict.keys():
                     dt = DataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads), self.streamChsDropDict[stream.info().name()])
+                                            self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
                 else:
                     dt = DataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
                                             self.globalEpochSettings, len(self.dataThreads))
 
             dt.start()
             self.dataThreads.append(dt)
             if stream.info().name() in self.streamCustomFeatureExtract.keys():
@@ -180,15 +180,15 @@
             self.ft.start()
             self.featureThreads.append(dt)
         # marker thread requires data and feature threads to push new markers too
         self.markerThread = MarkerThread(self.closeEvent,self.trainTestEvent, self.markerStream,self.dataThreads, self.featureThreads)
         self.markerThread.start()
         self.classifierThread = ClassifierThread(self.closeEvent,self.trainTestEvent, self.featureQueueTest,self.featureQueueTrain,
                                                  self.classifierInfoQueue, self.classifierInfoRetrieveEvent,
-                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent,
+                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, len(self.dataThreads),
                                                 self.minimumEpochsRequired, clf = self.clf, model = self.model)
         self.classifierThread.start()
 
     def StopThreads(self):
         self.closeEvent.set()
         self.markerThread.join()
         # wait for all threads to finish processing, probably worth pulling out finalised classifier information stored for later use.
```

### Comparing `install-pybci-0.1.4b9/setup.py` & `install-pybci-0.2.0b0/setup.py`

 * *Files identical despite different names*

