# Comparing `tmp/tailraiders-0.0.5.tar.gz` & `tmp/tailraiders-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailraiders-0.0.5.tar", last modified: Tue May 23 09:46:09 2023, max compression
+gzip compressed data, was "tailraiders-0.0.6.tar", last modified: Tue May 23 09:56:50 2023, max compression
```

## Comparing `tailraiders-0.0.5.tar` & `tailraiders-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.075492 tailraiders-0.0.5/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1012 2023-05-23 09:46:09.073388 tailraiders-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      687 2023-05-23 09:45:39.000000 tailraiders-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 09:46:09.075492 tailraiders-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-05-23 09:45:44.000000 tailraiders-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.013311 tailraiders-0.0.5/tailraiders/
--rw-rw-rw-   0        0        0      933 2023-05-23 09:45:31.000000 tailraiders-0.0.5/tailraiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.056805 tailraiders-0.0.5/tailraiders/boaboa/
--rw-rw-rw-   0        0        0      141 2023-05-23 09:34:49.000000 tailraiders-0.0.5/tailraiders/boaboa/__init__.py
--rw-rw-rw-   0        0        0     2521 2023-05-23 09:27:58.000000 tailraiders-0.0.5/tailraiders/boaboa/doc.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.058802 tailraiders-0.0.5/tailraiders/bugtrapper/
--rw-rw-rw-   0        0        0      110 2023-05-23 09:36:01.000000 tailraiders-0.0.5/tailraiders/bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.062393 tailraiders-0.0.5/tailraiders/gajalaka/
--rw-rw-rw-   0        0        0      132 2023-05-23 09:35:13.000000 tailraiders-0.0.5/tailraiders/gajalaka/__init__.py
--rw-rw-rw-   0        0        0     6178 2023-05-23 09:20:00.000000 tailraiders-0.0.5/tailraiders/gajalaka/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.064864 tailraiders-0.0.5/tailraiders/plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.5/tailraiders/plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.068363 tailraiders-0.0.5/tailraiders/protector/
--rw-rw-rw-   0        0        0      135 2023-05-23 09:35:05.000000 tailraiders-0.0.5/tailraiders/protector/__init__.py
--rw-rw-rw-   0        0        0     3635 2023-05-23 09:24:23.000000 tailraiders-0.0.5/tailraiders/protector/nan.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.070854 tailraiders-0.0.5/tailraiders/trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.5/tailraiders/trouper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:46:09.051538 tailraiders-0.0.5/tailraiders.egg-info/
--rw-rw-rw-   0        0        0     1012 2023-05-23 09:46:07.000000 tailraiders-0.0.5/tailraiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-23 09:46:08.000000 tailraiders-0.0.5/tailraiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:46:07.000000 tailraiders-0.0.5/tailraiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-23 09:46:08.000000 tailraiders-0.0.5/tailraiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-23 09:46:08.000000 tailraiders-0.0.5/tailraiders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.247678 tailraiders-0.0.6/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1012 2023-05-23 09:56:50.246673 tailraiders-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2023-05-23 09:56:17.000000 tailraiders-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:56:50.248688 tailraiders-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-05-23 09:56:11.000000 tailraiders-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.182431 tailraiders-0.0.6/tailraiders/
+-rw-rw-rw-   0        0        0      932 2023-05-23 09:55:55.000000 tailraiders-0.0.6/tailraiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.224047 tailraiders-0.0.6/tailraiders/boaboa/
+-rw-rw-rw-   0        0        0      141 2023-05-23 09:34:49.000000 tailraiders-0.0.6/tailraiders/boaboa/__init__.py
+-rw-rw-rw-   0        0        0     2521 2023-05-23 09:27:58.000000 tailraiders-0.0.6/tailraiders/boaboa/doc.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.227050 tailraiders-0.0.6/tailraiders/bugtrapper/
+-rw-rw-rw-   0        0        0      110 2023-05-23 09:36:01.000000 tailraiders-0.0.6/tailraiders/bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.232767 tailraiders-0.0.6/tailraiders/gajalaka/
+-rw-rw-rw-   0        0        0      132 2023-05-23 09:35:13.000000 tailraiders-0.0.6/tailraiders/gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     6178 2023-05-23 09:20:00.000000 tailraiders-0.0.6/tailraiders/gajalaka/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.235130 tailraiders-0.0.6/tailraiders/plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.6/tailraiders/plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.240148 tailraiders-0.0.6/tailraiders/protector/
+-rw-rw-rw-   0        0        0      135 2023-05-23 09:35:05.000000 tailraiders-0.0.6/tailraiders/protector/__init__.py
+-rw-rw-rw-   0        0        0     3635 2023-05-23 09:24:23.000000 tailraiders-0.0.6/tailraiders/protector/nan.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.243331 tailraiders-0.0.6/tailraiders/trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.6/tailraiders/trouper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:56:50.218523 tailraiders-0.0.6/tailraiders.egg-info/
+-rw-rw-rw-   0        0        0     1012 2023-05-23 09:56:48.000000 tailraiders-0.0.6/tailraiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-23 09:56:49.000000 tailraiders-0.0.6/tailraiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:56:48.000000 tailraiders-0.0.6/tailraiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-23 09:56:49.000000 tailraiders-0.0.6/tailraiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 09:56:49.000000 tailraiders-0.0.6/tailraiders.egg-info/top_level.txt
```

### Comparing `tailraiders-0.0.5/LICENSE` & `tailraiders-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.5/PKG-INFO` & `tailraiders-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,14 +12,14 @@
 # Tailraiders
 Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
 You can install the package by using the following code:<br>
 **pip install tailraiders**
 
-## New additions: Version 0.0.5
+## New additions: Version 0.0.6
 - All functionalities can be imported from tailraiders, no need for calling the subpackages at this point in time
 - docstring function now has inputs
 - Plot now has an additional child-class: MeltPlot
 - Nan is moved to tailraiders.protector
 - Nan now has a function to read from csv-files: df_from_file
```

### Comparing `tailraiders-0.0.5/README.md` & `tailraiders-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tailraiders
 Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
 You can install the package by using the following code:<br>
 **pip install tailraiders**
 
-## New additions: Version 0.0.5
+## New additions: Version 0.0.6
 - All functionalities can be imported from tailraiders, no need for calling the subpackages at this point in time
 - docstring function now has inputs
 - Plot now has an additional child-class: MeltPlot
 - Nan is moved to tailraiders.protector
 - Nan now has a function to read from csv-files: df_from_file
```

### Comparing `tailraiders-0.0.5/setup.py` & `tailraiders-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier, versions with 0.0.x are trials and tests',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     name = 'tailraiders',
-    version = '0.0.5',
+    version = '0.0.6',
     packages = find_packages(include = ['tailraiders', 'tailraiders.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

### Comparing `tailraiders-0.0.5/tailraiders/__init__.py` & `tailraiders-0.0.6/tailraiders/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,9 @@
         __import__(module)
     #Raise an error when it fails, telling them to install the failed module
     except ImportError:
         raise ImportError(f"The required package {module} was not found. Please install it.")
     
 #Making it so you can, for certain parts, just import tailraiders
 from tailraiders.boaboa.doc import docstring
-from tailraiders.gajalaka.plots import Plots, MeltPlot
+from tailraiders.gajalaka.plots import Plot, MeltPlot
 from tailraiders.protector.nan import Nan
```

### Comparing `tailraiders-0.0.5/tailraiders/boaboa/doc.py` & `tailraiders-0.0.6/tailraiders/boaboa/doc.py`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.5/tailraiders/gajalaka/plots.py` & `tailraiders-0.0.6/tailraiders/gajalaka/plots.py`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.5/tailraiders/protector/nan.py` & `tailraiders-0.0.6/tailraiders/protector/nan.py`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.5/tailraiders.egg-info/PKG-INFO` & `tailraiders-0.0.6/tailraiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,14 +12,14 @@
 # Tailraiders
 Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
 You can install the package by using the following code:<br>
 **pip install tailraiders**
 
-## New additions: Version 0.0.5
+## New additions: Version 0.0.6
 - All functionalities can be imported from tailraiders, no need for calling the subpackages at this point in time
 - docstring function now has inputs
 - Plot now has an additional child-class: MeltPlot
 - Nan is moved to tailraiders.protector
 - Nan now has a function to read from csv-files: df_from_file
```

### Comparing `tailraiders-0.0.5/tailraiders.egg-info/SOURCES.txt` & `tailraiders-0.0.6/tailraiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

