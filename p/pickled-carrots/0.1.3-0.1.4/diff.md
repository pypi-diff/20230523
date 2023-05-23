# Comparing `tmp/pickled_carrots-0.1.3.tar.gz` & `tmp/pickled_carrots-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-0.1.3.tar", max compression
+gzip compressed data, was "pickled_carrots-0.1.4.tar", max compression
```

## Comparing `pickled_carrots-0.1.3.tar` & `pickled_carrots-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,18 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.1.3/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.1.3/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.1.3/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.1.3/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.1.3/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.1.3/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.1.3/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.1.3/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.1.3/pickled_carrots/plot.py
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.1.3/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0      192 2023-05-20 10:55:17.702165 pickled_carrots-0.1.3/pickled_carrots/vinegar/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13078 2023-05-20 11:08:06.265611 pickled_carrots-0.1.3/pickled_carrots/vinegar/__pycache__/core.cpython-39.pyc
--rw-r--r--   0        0        0     3553 2023-05-19 17:56:34.158359 pickled_carrots-0.1.3/pickled_carrots/vinegar/__pycache__/event.cpython-39.pyc
--rw-r--r--   0        0        0    15989 2023-05-20 11:21:14.081943 pickled_carrots-0.1.3/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     5481 2023-05-19 17:53:39.362318 pickled_carrots-0.1.3/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.1.3/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0      650 2023-05-19 21:07:21.294282 pickled_carrots-0.1.3/pickled_carrots/vinegar/tests/read_hsf.py
--rw-r--r--   0        0        0   138903 2023-05-19 21:13:13.562541 pickled_carrots-0.1.3/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-05-20 11:36:44.460851 pickled_carrots-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pickled_carrots-0.1.3/setup.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.1.4/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.1.4/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.1.4/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.1.4/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.1.4/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.1.4/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.1.4/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.1.4/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.1.4/pickled_carrots/plot.py
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.1.4/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    15989 2023-05-20 11:21:14.081943 pickled_carrots-0.1.4/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     5481 2023-05-19 17:53:39.362318 pickled_carrots-0.1.4/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.1.4/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0      650 2023-05-19 21:07:21.294282 pickled_carrots-0.1.4/pickled_carrots/vinegar/tests/read_hsf.py
+-rw-r--r--   0        0        0   138903 2023-05-19 21:13:13.562541 pickled_carrots-0.1.4/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-05-23 14:37:50.380891 pickled_carrots-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pickled_carrots-0.1.4/setup.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.1.4/PKG-INFO
```

### Comparing `pickled_carrots-0.1.3/README.md` & `pickled_carrots-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/DPData.py` & `pickled_carrots-0.1.4/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/DPPlot.py` & `pickled_carrots-0.1.4/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/DPUtil.py` & `pickled_carrots-0.1.4/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/database.py` & `pickled_carrots-0.1.4/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/dataclass.py` & `pickled_carrots-0.1.4/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/mathutil.py` & `pickled_carrots-0.1.4/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/plot.py` & `pickled_carrots-0.1.4/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/vinegar/core.py` & `pickled_carrots-0.1.4/pickled_carrots/vinegar/core.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/vinegar/event.py` & `pickled_carrots-0.1.4/pickled_carrots/vinegar/event.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-0.1.4/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/vinegar/tests/read_hsf.py` & `pickled_carrots-0.1.4/pickled_carrots/vinegar/tests/read_hsf.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pickled_carrots/waveforms.py` & `pickled_carrots-0.1.4/pickled_carrots/waveforms.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.3/pyproject.toml` & `pickled_carrots-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

### Comparing `pickled_carrots-0.1.3/setup.py` & `pickled_carrots-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'pytz>=2023.3,<2024.0',
  'shapely>=2.0.1,<3.0.0',
  'statsmodels>=0.14.0,<0.15.0',
  'uquake>=1.2.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pickled-carrots',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': "# ESG_Research\n\nThis repository contains Python and C# code which is used for various different functions. In this document we will go through what each folder contains.\n\n__Analytics_Notebooks__\n\nThis folder contains Jupyter notebooks which have various different functionalities. More notebooks can be found on the DataShare, under Frac4/Notebooks.\n\n&nbsp;\n\n\n__ESG-dash__\n\nA dash-based dashboard for evaluating sensor quality for mining sites.\n\n&nbsp;\n\n\n__ESG__\n\nThe main module folder for our Python codes. The files within this folder are used in most of our jupyter notebooks. More details on what each file contains can be found in the folder.\n\n&nbsp;\n\n__ITG-FMC__\n\nContains the tiltmeter processing dashboard written in Python, a Fiber processing C# app, a DPA and DPA-RTA C# app, and a copy of the Stress Inversion python package (which has since been merged into the main ESG repo.\n\n&nbsp;\n\n__Scripts__\n\nContains various Python scripts which are used to automated processes such as HypoDD or noise analysis.\n\n&nbsp;\n\n__build/lib, dist, esg_das, esg_dts__\n\nPython code for processing Fiber data. \n\n&nbsp;\n\n__Miscellaneous__\n\nThere are some additional files in this folder which are related to replicated anaconda environments. The requirements.txt file can be used to create ESG's default environment.\n",
     'author': 'pickled cattots team',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pickled_carrots-0.1.3/PKG-INFO` & `pickled_carrots-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

