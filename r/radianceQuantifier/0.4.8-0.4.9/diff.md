# Comparing `tmp/radianceQuantifier-0.4.8.tar.gz` & `tmp/radianceQuantifier-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radianceQuantifier-0.4.8.tar", last modified: Wed Mar  2 20:46:51 2022, max compression
+gzip compressed data, was "radianceQuantifier-0.4.9.tar", last modified: Wed Mar  2 21:03:40 2022, max compression
```

## Comparing `radianceQuantifier-0.4.8.tar` & `radianceQuantifier-0.4.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 20:46:51.544089 radianceQuantifier-0.4.8/
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    35149 2021-10-20 07:17:23.000000 radianceQuantifier-0.4.8/LICENSE.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       88 2021-10-20 07:51:09.000000 radianceQuantifier-0.4.8/MANIFEST.in
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1521 2022-03-02 20:46:51.543786 radianceQuantifier-0.4.8/PKG-INFO
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      833 2021-12-11 19:38:50.000000 radianceQuantifier-0.4.8/README.md
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 20:46:51.525247 radianceQuantifier-0.4.8/radianceQuantifier/
--rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-10-20 00:42:33.000000 radianceQuantifier-0.4.8/radianceQuantifier/__init__.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     9914 2022-03-02 20:46:05.000000 radianceQuantifier-0.4.8/radianceQuantifier/__main__.py
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 20:46:51.533118 radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/__init__.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    28020 2022-02-11 00:17:19.000000 radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/inVivoRadianceImagePlotting.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    47786 2022-02-13 04:36:02.000000 radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/inVivoRadianceProcessing.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    16092 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/miscFunctions.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     3971 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/survivalProcessing.py
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 20:46:51.538573 radianceQuantifier-0.4.8/radianceQuantifier/plotting/
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/__init__.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5431 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlot1D.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     3268 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlot2D.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     7976 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlot3D.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    10282 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlotCategorical.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27353 2021-12-11 23:32:06.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlotLibrary.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27445 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/interactiveGUIElements.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    60210 2022-01-20 16:27:29.000000 radianceQuantifier-0.4.8/radianceQuantifier/plotting/plottingGUI.py
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)   212214 2021-10-16 20:08:05.000000 radianceQuantifier-0.4.8/radianceQuantifier/radianceQuantifierLogo.png
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 20:46:51.543277 radianceQuantifier-0.4.8/radianceQuantifier/setup/
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/setup/__init__.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     6451 2021-12-11 23:07:42.000000 radianceQuantifier-0.4.8/radianceQuantifier/setup/experimentCreationGUI.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5797 2021-12-11 23:12:42.000000 radianceQuantifier-0.4.8/radianceQuantifier/setup/experimentSetupGUI.py
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     2853 2022-01-12 04:21:23.000000 radianceQuantifier-0.4.8/radianceQuantifier/setup/processExperimentGUI.py
--rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1289 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.8/radianceQuantifier/setup/removeExperiment.py
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 20:46:51.529848 radianceQuantifier-0.4.8/radianceQuantifier.egg-info/
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1521 2022-03-02 20:46:51.000000 radianceQuantifier-0.4.8/radianceQuantifier.egg-info/PKG-INFO
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1278 2022-03-02 20:46:51.000000 radianceQuantifier-0.4.8/radianceQuantifier.egg-info/SOURCES.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        1 2022-03-02 20:46:51.000000 radianceQuantifier-0.4.8/radianceQuantifier.egg-info/dependency_links.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       72 2022-03-02 20:46:51.000000 radianceQuantifier-0.4.8/radianceQuantifier.egg-info/entry_points.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      138 2022-03-02 20:46:51.000000 radianceQuantifier-0.4.8/radianceQuantifier.egg-info/requires.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       19 2022-03-02 20:46:51.000000 radianceQuantifier-0.4.8/radianceQuantifier.egg-info/top_level.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       38 2022-03-02 20:46:51.544214 radianceQuantifier-0.4.8/setup.cfg
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1456 2022-03-02 20:46:37.000000 radianceQuantifier-0.4.8/setup.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 21:03:40.400979 radianceQuantifier-0.4.9/
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    35149 2021-10-20 07:17:23.000000 radianceQuantifier-0.4.9/LICENSE.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       88 2021-10-20 07:51:09.000000 radianceQuantifier-0.4.9/MANIFEST.in
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1521 2022-03-02 21:03:40.400442 radianceQuantifier-0.4.9/PKG-INFO
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      833 2021-12-11 19:38:50.000000 radianceQuantifier-0.4.9/README.md
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 21:03:40.375496 radianceQuantifier-0.4.9/radianceQuantifier/
+-rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-10-20 00:42:33.000000 radianceQuantifier-0.4.9/radianceQuantifier/__init__.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     9846 2022-03-02 21:02:18.000000 radianceQuantifier-0.4.9/radianceQuantifier/__main__.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 21:03:40.384744 radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/__init__.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    28020 2022-02-11 00:17:19.000000 radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/inVivoRadianceImagePlotting.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    47786 2022-02-13 04:36:02.000000 radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/inVivoRadianceProcessing.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    16092 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/miscFunctions.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     3971 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/survivalProcessing.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 21:03:40.392733 radianceQuantifier-0.4.9/radianceQuantifier/plotting/
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/__init__.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5431 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlot1D.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     3268 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlot2D.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     7976 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlot3D.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    10282 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlotCategorical.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27353 2021-12-11 23:32:06.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlotLibrary.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27445 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/interactiveGUIElements.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    60210 2022-01-20 16:27:29.000000 radianceQuantifier-0.4.9/radianceQuantifier/plotting/plottingGUI.py
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)   212214 2021-10-16 20:08:05.000000 radianceQuantifier-0.4.9/radianceQuantifier/radianceQuantifierLogo.png
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 21:03:40.399349 radianceQuantifier-0.4.9/radianceQuantifier/setup/
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/setup/__init__.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     6451 2021-12-11 23:07:42.000000 radianceQuantifier-0.4.9/radianceQuantifier/setup/experimentCreationGUI.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5797 2021-12-11 23:12:42.000000 radianceQuantifier-0.4.9/radianceQuantifier/setup/experimentSetupGUI.py
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     2853 2022-01-12 04:21:23.000000 radianceQuantifier-0.4.9/radianceQuantifier/setup/processExperimentGUI.py
+-rw-rw-r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1289 2021-12-11 23:01:00.000000 radianceQuantifier-0.4.9/radianceQuantifier/setup/removeExperiment.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2022-03-02 21:03:40.379499 radianceQuantifier-0.4.9/radianceQuantifier.egg-info/
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1521 2022-03-02 21:03:40.000000 radianceQuantifier-0.4.9/radianceQuantifier.egg-info/PKG-INFO
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1278 2022-03-02 21:03:40.000000 radianceQuantifier-0.4.9/radianceQuantifier.egg-info/SOURCES.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        1 2022-03-02 21:03:40.000000 radianceQuantifier-0.4.9/radianceQuantifier.egg-info/dependency_links.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       72 2022-03-02 21:03:40.000000 radianceQuantifier-0.4.9/radianceQuantifier.egg-info/entry_points.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      138 2022-03-02 21:03:40.000000 radianceQuantifier-0.4.9/radianceQuantifier.egg-info/requires.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       19 2022-03-02 21:03:40.000000 radianceQuantifier-0.4.9/radianceQuantifier.egg-info/top_level.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       38 2022-03-02 21:03:40.401291 radianceQuantifier-0.4.9/setup.cfg
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1456 2022-03-02 21:03:03.000000 radianceQuantifier-0.4.9/setup.py
```

### Comparing `radianceQuantifier-0.4.8/LICENSE.txt` & `radianceQuantifier-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/PKG-INFO` & `radianceQuantifier-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radianceQuantifier
-Version: 0.4.8
+Version: 0.4.9
 Summary: Automatically crops mice and quantifies their tumor luminescences from raw IVIS images
 Home-page: https://github.com/soorajachar/radianceQuantifier
 Author: Sooraj Achar
 Author-email: acharsr@nih.gov
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `radianceQuantifier-0.4.8/README.md` & `radianceQuantifier-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/__main__.py` & `radianceQuantifier-0.4.9/radianceQuantifier/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,15 @@
             experiments = sorted(experiments)[::-1]
             self.experimentMenu['values'] = experiments
             if len(experiments) == 1:
                 self.experimentMenu.set(self.experimentMenu['values'][0])
             self.experimentMenu['width'] = len(max(experiments,key=len))
         
         if 'misc' not in os.listdir(master.homedirectory):
-            os.mkdir(master.homedirectory+'misc'])
-            #subprocess.run(['mkdir',master.homedirectory+'misc'])
+            os.mkdir(master.homedirectory+'misc')
         if 'pathDict.pkl' not in os.listdir(master.homedirectory+'misc'):
             self.pathDict = {}
         else:
             self.pathDict = pickle.load(open(master.homedirectory+'misc/pathDict.pkl','rb'))
         projects = list(self.pathDict.keys())
         self.projectMenu = tkinter.ttk.Combobox(expSelectionFrame,values = projects)
         if len(self.pathDict) > 0:
```

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/inVivoRadianceImagePlotting.py` & `radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/inVivoRadianceImagePlotting.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/inVivoRadianceProcessing.py` & `radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/inVivoRadianceProcessing.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/miscFunctions.py` & `radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/miscFunctions.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/dataprocessing/survivalProcessing.py` & `radianceQuantifier-0.4.9/radianceQuantifier/dataprocessing/survivalProcessing.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlot1D.py` & `radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlot1D.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlot2D.py` & `radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlot2D.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlot3D.py` & `radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlot3D.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlotCategorical.py` & `radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlotCategorical.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/plotting/facetPlotLibrary.py` & `radianceQuantifier-0.4.9/radianceQuantifier/plotting/facetPlotLibrary.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/plotting/interactiveGUIElements.py` & `radianceQuantifier-0.4.9/radianceQuantifier/plotting/interactiveGUIElements.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/plotting/plottingGUI.py` & `radianceQuantifier-0.4.9/radianceQuantifier/plotting/plottingGUI.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/radianceQuantifierLogo.png` & `radianceQuantifier-0.4.9/radianceQuantifier/radianceQuantifierLogo.png`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/setup/experimentCreationGUI.py` & `radianceQuantifier-0.4.9/radianceQuantifier/setup/experimentCreationGUI.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/setup/experimentSetupGUI.py` & `radianceQuantifier-0.4.9/radianceQuantifier/setup/experimentSetupGUI.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/setup/processExperimentGUI.py` & `radianceQuantifier-0.4.9/radianceQuantifier/setup/processExperimentGUI.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier/setup/removeExperiment.py` & `radianceQuantifier-0.4.9/radianceQuantifier/setup/removeExperiment.py`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier.egg-info/PKG-INFO` & `radianceQuantifier-0.4.9/radianceQuantifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radianceQuantifier
-Version: 0.4.8
+Version: 0.4.9
 Summary: Automatically crops mice and quantifies their tumor luminescences from raw IVIS images
 Home-page: https://github.com/soorajachar/radianceQuantifier
 Author: Sooraj Achar
 Author-email: acharsr@nih.gov
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `radianceQuantifier-0.4.8/radianceQuantifier.egg-info/SOURCES.txt` & `radianceQuantifier-0.4.9/radianceQuantifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radianceQuantifier-0.4.8/setup.py` & `radianceQuantifier-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="radianceQuantifier",
-    version="0.4.8",
+    version="0.4.9",
     author = "Sooraj Achar",
     author_email = "acharsr@nih.gov",
     description = "Automatically crops mice and quantifies their tumor luminescences from raw IVIS images",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/soorajachar/radianceQuantifier",
     classifiers = classifiers,
```

