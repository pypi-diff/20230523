# Comparing `tmp/psychopy-usbToBNC-0.0.2.tar.gz` & `tmp/psychopy-usbToBNC-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psychopy-usbToBNC-0.0.2.tar", last modified: Tue May 23 15:12:16 2023, max compression
+gzip compressed data, was "dist\psychopy-usbToBNC-0.0.3.tar", last modified: Tue May 23 15:17:19 2023, max compression
```

## Comparing `psychopy-usbToBNC-0.0.2.tar` & `psychopy-usbToBNC-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 15:12:16.866390 psychopy-usbToBNC-0.0.2/
--rw-rw-rw-   0        0        0      611 2023-05-23 15:12:16.866390 psychopy-usbToBNC-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 15:12:16.849316 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC/
--rw-rw-rw-   0        0        0      389 2023-05-20 01:52:07.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:12:16.865391 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC/usbToBNC/
--rw-rw-rw-   0        0        0    11487 2023-05-20 01:52:53.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC/usbToBNC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:12:16.864387 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/
--rw-rw-rw-   0        0        0      611 2023-05-23 15:12:16.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-23 15:12:16.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 15:12:16.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-23 15:12:16.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 15:12:16.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-23 15:12:16.000000 psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 15:12:16.866390 psychopy-usbToBNC-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      992 2023-05-23 15:12:01.000000 psychopy-usbToBNC-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.929342 psychopy-usbToBNC-0.0.3/
+-rw-rw-rw-   0        0        0      608 2023-05-23 15:17:19.929342 psychopy-usbToBNC-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.910337 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/
+-rw-rw-rw-   0        0        0      389 2023-05-20 01:52:07.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.928342 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/usbToBNC/
+-rw-rw-rw-   0        0        0    11487 2023-05-20 01:52:53.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/usbToBNC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.927346 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 15:17:19.929342 psychopy-usbToBNC-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      989 2023-05-23 15:17:16.000000 psychopy-usbToBNC-0.0.3/setup.py
```

### Comparing `psychopy-usbToBNC-0.0.2/PKG-INFO` & `psychopy-usbToBNC-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: psychopy-usbToBNC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Coming soon
 Home-page: UNKNOWN
 Author: Labeo Technologies(Christophe Cloutier-Tremblay)
 Author-email: <Christophe@labeotech.com>
 License: UNKNOWN
 Description: todo
 Keywords: python
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `psychopy-usbToBNC-0.0.2/psychopy_usbToBNC/usbToBNC/__init__.py` & `psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/usbToBNC/__init__.py`

 * *Files identical despite different names*

### Comparing `psychopy-usbToBNC-0.0.2/psychopy_usbToBNC.egg-info/PKG-INFO` & `psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: psychopy-usbToBNC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Coming soon
 Home-page: UNKNOWN
 Author: Labeo Technologies(Christophe Cloutier-Tremblay)
 Author-email: <Christophe@labeotech.com>
 License: UNKNOWN
 Description: todo
 Keywords: python
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `psychopy-usbToBNC-0.0.2/setup.py` & `psychopy-usbToBNC-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Coming soon'
 LONG_DESCRIPTION = 'todo'
 
 # Setting up
 setup(
     name="psychopy-usbToBNC",
     version=VERSION,
@@ -19,15 +19,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['Psychopy'],
     keywords=['python'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

