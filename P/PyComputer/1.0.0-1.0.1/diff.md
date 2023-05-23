# Comparing `tmp/PyComputer-1.0.0.tar.gz` & `tmp/PyComputer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComputer-1.0.0.tar", last modified: Mon May 22 18:35:08 2023, max compression
+gzip compressed data, was "PyComputer-1.0.1.tar", last modified: Tue May 23 03:47:27 2023, max compression
```

## Comparing `PyComputer-1.0.0.tar` & `PyComputer-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 18:35:08.938445 PyComputer-1.0.0/
--rw-rw-rw-   0        0        0     2662 2023-05-22 12:41:42.000000 PyComputer-1.0.0/CREDITS.md
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyComputer-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      309 2023-05-18 06:46:41.000000 PyComputer-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2627 2023-05-22 18:35:08.936457 PyComputer-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 18:35:08.920535 PyComputer-1.0.0/PyComputer/
--rw-rw-rw-   0        0        0     5139 2023-05-22 12:38:02.000000 PyComputer-1.0.0/PyComputer/LicensePlate.py
--rw-rw-rw-   0        0        0     4008 2023-05-22 12:36:11.000000 PyComputer-1.0.0/PyComputer/PeopleDetection.py
--rw-rw-rw-   0        0        0     3887 2023-05-22 12:37:38.000000 PyComputer-1.0.0/PyComputer/VehicleDetection.py
--rw-rw-rw-   0        0        0       59 2023-05-22 12:24:38.000000 PyComputer-1.0.0/PyComputer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 18:35:08.934455 PyComputer-1.0.0/PyComputer.egg-info/
--rw-rw-rw-   0        0        0     2627 2023-05-22 18:35:08.000000 PyComputer-1.0.0/PyComputer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-22 18:35:08.000000 PyComputer-1.0.0/PyComputer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 18:35:08.000000 PyComputer-1.0.0/PyComputer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 18:35:08.000000 PyComputer-1.0.0/PyComputer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 18:35:08.000000 PyComputer-1.0.0/PyComputer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2090 2023-05-22 12:43:06.000000 PyComputer-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 18:35:08.938445 PyComputer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-05-22 18:32:57.000000 PyComputer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:47:27.443489 PyComputer-1.0.1/
+-rw-rw-rw-   0        0        0      600 2023-05-23 03:31:34.000000 PyComputer-1.0.1/CREDITS.md
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyComputer-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       98 2023-05-23 03:32:25.000000 PyComputer-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2689 2023-05-23 03:47:27.442579 PyComputer-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 03:47:27.406860 PyComputer-1.0.1/PyComputer/
+-rw-rw-rw-   0        0        0      453 2023-05-23 03:27:34.000000 PyComputer-1.0.1/PyComputer/Brightness.py
+-rw-rw-rw-   0        0        0     1339 2023-05-23 03:25:52.000000 PyComputer-1.0.1/PyComputer/Volume.py
+-rw-rw-rw-   0        0        0       60 2023-05-23 02:07:40.000000 PyComputer-1.0.1/PyComputer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:47:27.425570 PyComputer-1.0.1/PyComputer/assets/
+-rwxrwxrwx   0        0        0   899784 2023-05-23 02:05:42.000000 PyComputer-1.0.1/PyComputer/assets/SetVol.exe
+drwxrwxrwx   0        0        0        0 2023-05-23 03:47:27.422693 PyComputer-1.0.1/PyComputer.egg-info/
+-rw-rw-rw-   0        0        0     2689 2023-05-23 03:47:26.000000 PyComputer-1.0.1/PyComputer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-05-23 03:47:26.000000 PyComputer-1.0.1/PyComputer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 03:47:26.000000 PyComputer-1.0.1/PyComputer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-23 03:47:26.000000 PyComputer-1.0.1/PyComputer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-23 03:47:26.000000 PyComputer-1.0.1/PyComputer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2097 2023-05-23 03:43:50.000000 PyComputer-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 03:47:27.444485 PyComputer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2023-05-23 03:42:39.000000 PyComputer-1.0.1/setup.py
```

### Comparing `PyComputer-1.0.0/LICENSE.txt` & `PyComputer-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyComputer-1.0.0/PKG-INFO` & `PyComputer-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: PyComputer
-Version: 1.0.0
-Summary: PyComputer
-Home-page: https://github.com/Anikethc/PyTraffic
-Download-URL: https://pypi.org/project/PyTraffic
+Version: 1.0.1
+Summary: PyComputer is an advanced Python package that manages and alters your computer's settings.
+Home-page: https://github.com/Anikethc/PyComputer
+Download-URL: https://pypi.org/project/PyComputer
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
-Keywords: Traffic,Traffic Density,Traffic Density Estimation,License Plates,License Plate Detection,License Plate Recognition,Vehicles,Vehicle Detection
+Keywords: Computer,Settings
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyTraffic
+# PyComputer
 
 ## Introduction
 
-PyTraffic is an advanced Python package to work on traffic-related functions and use cases.
+PyComputer is an advanced Python package that manages and alters your computer's settings.
 
-Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
+Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pycomputer-docs).
 
 ## Package Information
 
-**Name** - PyTraffic</br>
-**Version** - 1.1.6</br>
-**Description** - PyTraffic is an advanced Python package to work on traffic-related functions and use cases.</br>
+**Name** - PyComputer</br>
+**Version** - 1.0.1</br>
+**Description** - PyComputer is an advanced Python package that manages and alters your computer's settings.</br>
 **Author** - Aniketh Chavare</br>
-**GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
-**Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
-**Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
+**GitHub URL** - [https://github.com/Anikethc/PyComputer](https://github.com/Anikethc/PyComputer)</br>
+**Pypi.org URL** - [https://pypi.org/project/PyComputer](https://pypi.org/project/PyComputer)</br>
+**Docs URL** - [https://aniketh-chavare.gitbook.io/pycomputer-docs](https://aniketh-chavare.gitbook.io/pycomputer-docs)
 
 ## License
 
 MIT License
 
 Copyright (c) 2023 Aniketh Chavare
```

### Comparing `PyComputer-1.0.0/PyComputer.egg-info/PKG-INFO` & `PyComputer-1.0.1/PyComputer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: PyComputer
-Version: 1.0.0
-Summary: PyComputer
-Home-page: https://github.com/Anikethc/PyTraffic
-Download-URL: https://pypi.org/project/PyTraffic
+Version: 1.0.1
+Summary: PyComputer is an advanced Python package that manages and alters your computer's settings.
+Home-page: https://github.com/Anikethc/PyComputer
+Download-URL: https://pypi.org/project/PyComputer
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
-Keywords: Traffic,Traffic Density,Traffic Density Estimation,License Plates,License Plate Detection,License Plate Recognition,Vehicles,Vehicle Detection
+Keywords: Computer,Settings
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyTraffic
+# PyComputer
 
 ## Introduction
 
-PyTraffic is an advanced Python package to work on traffic-related functions and use cases.
+PyComputer is an advanced Python package that manages and alters your computer's settings.
 
-Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
+Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pycomputer-docs).
 
 ## Package Information
 
-**Name** - PyTraffic</br>
-**Version** - 1.1.6</br>
-**Description** - PyTraffic is an advanced Python package to work on traffic-related functions and use cases.</br>
+**Name** - PyComputer</br>
+**Version** - 1.0.1</br>
+**Description** - PyComputer is an advanced Python package that manages and alters your computer's settings.</br>
 **Author** - Aniketh Chavare</br>
-**GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
-**Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
-**Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
+**GitHub URL** - [https://github.com/Anikethc/PyComputer](https://github.com/Anikethc/PyComputer)</br>
+**Pypi.org URL** - [https://pypi.org/project/PyComputer](https://pypi.org/project/PyComputer)</br>
+**Docs URL** - [https://aniketh-chavare.gitbook.io/pycomputer-docs](https://aniketh-chavare.gitbook.io/pycomputer-docs)
 
 ## License
 
 MIT License
 
 Copyright (c) 2023 Aniketh Chavare
```

### Comparing `PyComputer-1.0.0/README.md` & `PyComputer-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# PyTraffic
+# PyComputer
 
 ## Introduction
 
-PyTraffic is an advanced Python package to work on traffic-related functions and use cases.
+PyComputer is an advanced Python package that manages and alters your computer's settings.
 
-Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
+Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pycomputer-docs).
 
 ## Package Information
 
-**Name** - PyTraffic</br>
-**Version** - 1.1.6</br>
-**Description** - PyTraffic is an advanced Python package to work on traffic-related functions and use cases.</br>
+**Name** - PyComputer</br>
+**Version** - 1.0.1</br>
+**Description** - PyComputer is an advanced Python package that manages and alters your computer's settings.</br>
 **Author** - Aniketh Chavare</br>
-**GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
-**Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
-**Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
+**GitHub URL** - [https://github.com/Anikethc/PyComputer](https://github.com/Anikethc/PyComputer)</br>
+**Pypi.org URL** - [https://pypi.org/project/PyComputer](https://pypi.org/project/PyComputer)</br>
+**Docs URL** - [https://aniketh-chavare.gitbook.io/pycomputer-docs](https://aniketh-chavare.gitbook.io/pycomputer-docs)
 
 ## License
 
 MIT License
 
 Copyright (c) 2023 Aniketh Chavare
```

### Comparing `PyComputer-1.0.0/setup.py` & `PyComputer-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,27 +8,33 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyComputer",
-    version="1.0.0",
-    description="PyComputer",
+    version="1.0.1",
+    description="PyComputer is an advanced Python package that manages and alters your computer's settings.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
     author_email="anikethchavare@outlook.com",
-    keywords=["Traffic", "Traffic Density", "Traffic Density Estimation", "License Plates", "License Plate Detection", "License Plate Recognition", "Vehicles", "Vehicle Detection"],
-    url="https://github.com/Anikethc/PyTraffic",
-    download_url="https://pypi.org/project/PyTraffic"
+    keywords=["Computer", "Settings"],
+    url="https://github.com/Anikethc/PyComputer",
+    download_url="https://pypi.org/project/PyComputer"
 )
 
+# Classifiers
+classifiers = [
+    "Operating System :: Microsoft :: Windows",
+    "Programming Language :: Python"
+]
+
 # Install Requires
-install_requires = ["imutils"]
+install_requires = ["screen-brightness-control"]
 
 # Run the Setup File
 if __name__ == "__main__":
-    setup(**setup_args, install_requires=install_requires)
+    setup(**setup_args, install_requires=install_requires, classifiers=classifiers)
```

