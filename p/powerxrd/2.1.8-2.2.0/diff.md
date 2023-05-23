# Comparing `tmp/powerxrd-2.1.8.tar.gz` & `tmp/powerxrd-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/powerxrd-2.1.8.tar", last modified: Wed Nov 30 17:33:28 2022, max compression
+gzip compressed data, was "powerxrd-2.2.0.tar", max compression
```

## Comparing `powerxrd-2.1.8.tar` & `powerxrd-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 17:33:28.839047 powerxrd-2.1.8/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1077 2022-05-27 17:32:21.000000 powerxrd-2.1.8/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1735 2022-11-30 17:33:28.839047 powerxrd-2.1.8/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1017 2022-11-22 18:57:11.000000 powerxrd-2.1.8/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 17:33:28.839047 powerxrd-2.1.8/powerxrd/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       28 2022-11-18 17:25:26.000000 powerxrd-2.1.8/powerxrd/__init__.py
--rwxrwxr-x   0 andrew    (1000) andrew    (1000)    11809 2022-11-30 17:31:15.000000 powerxrd-2.1.8/powerxrd/main.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 17:33:28.839047 powerxrd-2.1.8/powerxrd.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1735 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      223 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2022-11-30 17:33:28.839047 powerxrd-2.1.8/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1417 2022-11-30 17:32:31.000000 powerxrd-2.1.8/setup.py
+-rw-r--r--   0        0        0     1077 2023-05-16 16:25:42.299134 powerxrd-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1063 2023-05-16 16:25:42.299134 powerxrd-2.2.0/README.md
+-rw-r--r--   0        0        0       28 2023-05-16 16:25:42.311134 powerxrd-2.2.0/powerxrd/__init__.py
+-rwxr-xr-x   0        0        0    18306 2023-05-23 20:46:55.112411 powerxrd-2.2.0/powerxrd/main.py
+-rw-r--r--   0        0        0      446 2023-05-23 20:47:10.784739 powerxrd-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 powerxrd-2.2.0/PKG-INFO
```

### Comparing `powerxrd-2.1.8/LICENSE` & `powerxrd-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powerxrd-2.1.8/PKG-INFO` & `powerxrd-2.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 Metadata-Version: 2.1
 Name: powerxrd
-Version: 2.1.8
+Version: 2.2.0
 Summary: Simple tools to handle powder XRD (and XRD) data with Python.
-Home-page: https://github.com/andrewrgarcia/powerxrd
-Author: Andrew Garcia, PhD
 License: MIT
-Classifier: Intended Audience :: Science/Research
+Author: andrewrgarcia
+Author-email: garcia.gtr@gmail.com
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: lmfit (>=1.1.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
+Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # powerxrd
-Simple tools to handle powder XRD (and XRD) data
+A Python package made to handle powder XRD (and XRD) data. 
+The only known open-source Github project with a Rietveld refinement method in development. 
+
+<img src="https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/powerxrd.svg" width="400">
 
 
 ## Installation
 
 ```bash
 pip install powerxrd
 ```
 
-## Just starting? Check out the Colab notebook (click on below icon)
+## Just starting? Check out the below options
+
+<a href="https://powerxrd.readthedocs.io/en/latest">
+<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/readthedocs.png?raw=true" width="250" ></a>
 
 <a href="https://colab.research.google.com/drive/1_Eq-cW6LSPPnaRjkbeHaC81Wfbd8mQS-?usp=sharing">
-<img src="https://github.com/andrewrgarcia/powerxrd/blob/main/img/colab.png?raw=true" width="300" ></a>
+<img src="https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/docs/img/colaboratory.svg?raw=true" width="300" ></a>
 
 
-## Stand-alone Usage
-On your Terminal ("command line"), copy-paste the following lines:
-```bash 
-cd Desktop   		
-mkdir pxrd		
-cd pxrd		
-wget https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/sample1.xy	
-wget https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/tests/test_module.py   
-python test_module.py   
-```
-
 ## Contributing
 
 1. Fork it (<https://github.com/your-github-user/powerxrd/fork>)
 2. Create your feature branch (`git checkout -b my-new-feature`)
 3. Commit your changes (`git commit -am 'Add some feature'`)
 4. Push to the branch (`git push origin my-new-feature`)
 5. Create a new Pull Request
 
+
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: powerxrd Version: 2.1.8 Summary: Simple tools to
-handle powder XRD (and XRD) data with Python. Home-page: https://github.com/
-andrewrgarcia/powerxrd Author: Andrew Garcia, PhD License: MIT Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-MIT License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE # powerxrd Simple tools to handle powder XRD
-(and XRD) data ## Installation ```bash pip install powerxrd ``` ## Just
-starting? Check out the Colab notebook (click on below icon) [https://
-github.com/andrewrgarcia/powerxrd/blob/main/img/colab.png?raw=true] ## Stand-
-alone Usage On your Terminal ("command line"), copy-paste the following lines:
-```bash cd Desktop mkdir pxrd cd pxrd wget https://raw.githubusercontent.com/
-andrewrgarcia/powerxrd/main/sample1.xy wget https://raw.githubusercontent.com/
-andrewrgarcia/powerxrd/main/tests/test_module.py python test_module.py ``` ##
-Contributing 1. Fork it (
+Metadata-Version: 2.1 Name: powerxrd Version: 2.2.0 Summary: Simple tools to
+handle powder XRD (and XRD) data with Python. License: MIT Author:
+andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: lmfit (>=1.1.0,<2.0.0) Requires-Dist: matplotlib
+(>=3.6.3,<4.0.0) Requires-Dist: numpy (>=1.24.1,<2.0.0) Requires-Dist: pandas
+(>=1.5.3,<2.0.0) Requires-Dist: scipy (>=1.10.0,<2.0.0) Description-Content-
+Type: text/markdown # powerxrd A Python package made to handle powder XRD (and
+XRD) data. The only known open-source Github project with a Rietveld refinement
+method in development. [https://raw.githubusercontent.com/andrewrgarcia/
+powerxrd/main/powerxrd.svg] ## Installation ```bash pip install powerxrd ``` ##
+Just starting? Check out the below options [https://raw.githubusercontent.com/
+andrewrgarcia/voxelmap/main/docs/img/readthedocs.png?raw=true] [https://
+raw.githubusercontent.com/andrewrgarcia/powerxrd/main/docs/img/
+colaboratory.svg?raw=true] ## Contributing 1. Fork it (
 github.com/your-github-user/powerxrd/fork>) 2. Create your feature branch (`git
 checkout -b my-new-feature`) 3. Commit your changes (`git commit -am 'Add some
 feature'`) 4. Push to the branch (`git push origin my-new-feature`) 5. Create a
 new Pull Request
```

### Comparing `powerxrd-2.1.8/README.md` & `powerxrd-2.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # powerxrd
-Simple tools to handle powder XRD (and XRD) data
+A Python package made to handle powder XRD (and XRD) data. 
+The only known open-source Github project with a Rietveld refinement method in development. 
+
+<img src="https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/powerxrd.svg" width="400">
 
 
 ## Installation
 
 ```bash
 pip install powerxrd
 ```
 
-## Just starting? Check out the Colab notebook (click on below icon)
+## Just starting? Check out the below options
 
-<a href="https://colab.research.google.com/drive/1_Eq-cW6LSPPnaRjkbeHaC81Wfbd8mQS-?usp=sharing">
-<img src="https://github.com/andrewrgarcia/powerxrd/blob/main/img/colab.png?raw=true" width="300" ></a>
+<a href="https://powerxrd.readthedocs.io/en/latest">
+<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/readthedocs.png?raw=true" width="250" ></a>
 
+<a href="https://colab.research.google.com/drive/1_Eq-cW6LSPPnaRjkbeHaC81Wfbd8mQS-?usp=sharing">
+<img src="https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/docs/img/colaboratory.svg?raw=true" width="300" ></a>
 
-## Stand-alone Usage
-On your Terminal ("command line"), copy-paste the following lines:
-```bash 
-cd Desktop   		
-mkdir pxrd		
-cd pxrd		
-wget https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/sample1.xy	
-wget https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/tests/test_module.py   
-python test_module.py   
-```
 
 ## Contributing
 
 1. Fork it (<https://github.com/your-github-user/powerxrd/fork>)
 2. Create your feature branch (`git checkout -b my-new-feature`)
 3. Commit your changes (`git commit -am 'Add some feature'`)
 4. Push to the branch (`git push origin my-new-feature`)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-# powerxrd Simple tools to handle powder XRD (and XRD) data ## Installation
-```bash pip install powerxrd ``` ## Just starting? Check out the Colab notebook
-(click on below icon) [https://github.com/andrewrgarcia/powerxrd/blob/main/img/
-colab.png?raw=true] ## Stand-alone Usage On your Terminal ("command line"),
-copy-paste the following lines: ```bash cd Desktop mkdir pxrd cd pxrd wget
-https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/sample1.xy wget
-https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/tests/
-test_module.py python test_module.py ``` ## Contributing 1. Fork it (
+# powerxrd A Python package made to handle powder XRD (and XRD) data. The only
+known open-source Github project with a Rietveld refinement method in
+development. [https://raw.githubusercontent.com/andrewrgarcia/powerxrd/main/
+powerxrd.svg] ## Installation ```bash pip install powerxrd ``` ## Just
+starting? Check out the below options [https://raw.githubusercontent.com/
+andrewrgarcia/voxelmap/main/docs/img/readthedocs.png?raw=true] [https://
+raw.githubusercontent.com/andrewrgarcia/powerxrd/main/docs/img/
+colaboratory.svg?raw=true] ## Contributing 1. Fork it (
 github.com/your-github-user/powerxrd/fork>) 2. Create your feature branch (`git
 checkout -b my-new-feature`) 3. Commit your changes (`git commit -am 'Add some
 feature'`) 4. Push to the branch (`git push origin my-new-feature`) 5. Create a
 new Pull Request
```

