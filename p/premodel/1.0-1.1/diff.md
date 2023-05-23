# Comparing `tmp/premodel-1.0.tar.gz` & `tmp/premodel-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "premodel-1.0.tar", last modified: Mon May 22 10:52:10 2023, max compression
+gzip compressed data, was "premodel-1.1.tar", last modified: Tue May 23 11:23:24 2023, max compression
```

## Comparing `premodel-1.0.tar` & `premodel-1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:52:10.718411 premodel-1.0/
--rw-rw-rw-   0        0        0     1091 2023-05-19 06:36:47.000000 premodel-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      534 2023-05-22 10:52:10.716413 premodel-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 premodel-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 10:52:10.718411 premodel-1.0/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-05-22 10:51:23.000000 premodel-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:52:10.655678 premodel-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 10:52:10.669683 premodel-1.0/src/premodel/
--rw-rw-rw-   0        0        0     1738 2023-05-22 10:28:35.000000 premodel-1.0/src/premodel/KNN.py
--rw-rw-rw-   0        0        0        0 2023-05-22 10:24:24.000000 premodel-1.0/src/premodel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:52:10.714414 premodel-1.0/src/premodel.egg-info/
--rw-rw-rw-   0        0        0      534 2023-05-22 10:52:10.000000 premodel-1.0/src/premodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-05-22 10:52:10.000000 premodel-1.0/src/premodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:52:10.000000 premodel-1.0/src/premodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-22 10:52:10.000000 premodel-1.0/src/premodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 10:52:10.000000 premodel-1.0/src/premodel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 11:23:24.561537 premodel-1.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-19 06:36:47.000000 premodel-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      718 2023-05-23 11:23:24.560507 premodel-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 premodel-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 11:23:24.562618 premodel-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-05-23 11:22:45.000000 premodel-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:23:24.485511 premodel-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 11:23:24.521575 premodel-1.1/src/premodel/
+-rw-rw-rw-   0        0        0     1738 2023-05-22 10:28:35.000000 premodel-1.1/src/premodel/KNN.py
+-rw-rw-rw-   0        0        0     1395 2023-05-23 11:22:13.000000 premodel-1.1/src/premodel/Linear_Regression.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:24:24.000000 premodel-1.1/src/premodel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:23:24.558051 premodel-1.1/src/premodel.egg-info/
+-rw-rw-rw-   0        0        0      718 2023-05-23 11:23:24.000000 premodel-1.1/src/premodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-23 11:23:24.000000 premodel-1.1/src/premodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:23:24.000000 premodel-1.1/src/premodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-23 11:23:24.000000 premodel-1.1/src/premodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 11:23:24.000000 premodel-1.1/src/premodel.egg-info/top_level.txt
```

### Comparing `premodel-1.0/LICENSE.txt` & `premodel-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `premodel-1.0/setup.py` & `premodel-1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from setuptools import find_packages, setup
 
 if __name__ == "__main__":
     setup(
     name = "premodel",
     author = "Akshat Sabharwal",
-    version = "1.0",
+    version = "1.1",
     package_dir={"":"src"},
     package=['premodel'],
     author_email = "akshatsabharwal35@gmail.com",
     description="Pre-built Machine Learning Models",
     long_description = """
-    \bK-Nearest Neighbours\b
+    K-Nearest Neighbours
 
-    predict: Returns the predicted value
-    visualize: Returns  a matplotlib scatter plot of the data along with the predicted point and its value. (Requires the calling of predict() method first)
-    euclidean: Returns the Euclidean distance of the given point from all the points given in the dataset""",
+    \n\npredict: Returns the predicted value
+    \n\nvisualize: Returns  a matplotlib scatter plot of the data along with the predicted point and its value. (Requires the calling of predict() method first)
+    \n\neuclidean: Returns the Euclidean distance of the given point from all the points given in the dataset
+    
+    \n\n\nLinear Regression
+
+    \n\nfit: Trains the model to the given data and return the slope and intercept values
+    \n\npredict: Returns the predicted value""",
     install_requires = [
         'numpy',
         'matplotlib',
         'random2',
         'pandas'
     ]
     )
```

### Comparing `premodel-1.0/src/premodel/KNN.py` & `premodel-1.1/src/premodel/KNN.py`

 * *Files identical despite different names*

