# Comparing `tmp/lpynn-0.0.2.1.tar.gz` & `tmp/lpynn-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpynn-0.0.2.1.tar", last modified: Tue Apr 25 23:49:15 2023, max compression
+gzip compressed data, was "lpynn-0.0.2.2.tar", last modified: Sat May  6 13:53:29 2023, max compression
```

## Comparing `lpynn-0.0.2.1.tar` & `lpynn-0.0.2.2.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.507017 lpynn-0.0.2.1/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)     1197 2023-04-25 23:49:15.506910 lpynn-0.0.2.1/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      746 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/README.md
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.506084 lpynn-0.0.2.1/lpynn/
--rw-r--r--   0 ubaid      (501) staff       (20)        0 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/lpynn/__init__.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.506753 lpynn-0.0.2.1/lpynn/perceptron/
--rw-r--r--   0 ubaid      (501) staff       (20)      132 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/lpynn/perceptron/__init__.py
--rw-r--r--   0 ubaid      (501) staff       (20)     4153 2023-04-25 23:48:43.000000 lpynn-0.0.2.1/lpynn/perceptron/perceptron_main.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.506525 lpynn-0.0.2.1/lpynn.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)     1197 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      225 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        6 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-25 23:49:15.507049 lpynn-0.0.2.1/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1908 2023-04-25 23:48:34.000000 lpynn-0.0.2.1/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:53:29.128991 lpynn-0.0.2.2/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpynn-0.0.2.2/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)     1197 2023-05-06 13:53:29.128879 lpynn-0.0.2.2/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      746 2023-05-06 13:52:09.000000 lpynn-0.0.2.2/README.md
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:53:29.128717 lpynn-0.0.2.2/lpynn.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1197 2023-05-06 13:53:29.000000 lpynn-0.0.2.2/lpynn.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      170 2023-05-06 13:53:29.000000 lpynn-0.0.2.2/lpynn.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-06 13:53:29.000000 lpynn-0.0.2.2/lpynn.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       18 2023-05-06 13:53:29.000000 lpynn-0.0.2.2/lpynn.egg-info/requires.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-06 13:53:29.000000 lpynn-0.0.2.2/lpynn.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-05-06 13:53:29.129027 lpynn-0.0.2.2/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1927 2023-05-06 13:52:28.000000 lpynn-0.0.2.2/setup.py
```

### Comparing `lpynn-0.0.2.1/LICENSE` & `lpynn-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lpynn-0.0.2.1/PKG-INFO` & `lpynn-0.0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpynn
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: A basic neural networks python package
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ubaid Shaikh
 Author-email: shaikhubaid769@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 This is a basic neural network package consisting of a single perceptron node. It can do binary classification.
 ## Usage
 
 **Example:**
 ```python
 from lpynn.perceptron import init_perceptron, print_perceptron, normalize_input_vectors, Perceptron, train_dataset
-from lptypes import i32, f64
+from lpython import i32, f64
 
 def main0():
     p: Perceptron = Perceptron(0, [0.0], 0.0, 0, 0.0, 0.0, 0)
     init_perceptron(p, 2, 0.05, 10000, 90.0)
     print_perceptron(p)
     print("=================================")
```

### Comparing `lpynn-0.0.2.1/README.md` & `lpynn-0.0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This is a basic neural network package consisting of a single perceptron node. It can do binary classification.
 ## Usage
 
 **Example:**
 ```python
 from lpynn.perceptron import init_perceptron, print_perceptron, normalize_input_vectors, Perceptron, train_dataset
-from lptypes import i32, f64
+from lpython import i32, f64
 
 def main0():
     p: Perceptron = Perceptron(0, [0.0], 0.0, 0, 0.0, 0.0, 0)
     init_perceptron(p, 2, 0.05, 10000, 90.0)
     print_perceptron(p)
     print("=================================")
```

### Comparing `lpynn-0.0.2.1/lpynn.egg-info/PKG-INFO` & `lpynn-0.0.2.2/lpynn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpynn
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: A basic neural networks python package
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ubaid Shaikh
 Author-email: shaikhubaid769@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 This is a basic neural network package consisting of a single perceptron node. It can do binary classification.
 ## Usage
 
 **Example:**
 ```python
 from lpynn.perceptron import init_perceptron, print_perceptron, normalize_input_vectors, Perceptron, train_dataset
-from lptypes import i32, f64
+from lpython import i32, f64
 
 def main0():
     p: Perceptron = Perceptron(0, [0.0], 0.0, 0, 0.0, 0.0, 0)
     init_perceptron(p, 2, 0.05, 10000, 90.0)
     print_perceptron(p)
     print("=================================")
```

### Comparing `lpynn-0.0.2.1/setup.py` & `lpynn-0.0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # The setup.py file is used as the build script for setuptools. Setuptools is a
 # package that allows you to easily build and distribute Python distributions.
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
-REQUIRED_PACKAGES=[]
+REQUIRED_PACKAGES=["lpython_emulation"]
 
-VERSION="0.0.2.1"
+VERSION="0.0.2.2"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpynn",                                               # name of project
```

