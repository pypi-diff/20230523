# Comparing `tmp/problexity-0.5.6.tar.gz` & `tmp/problexity-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problexity-0.5.6.tar", last modified: Thu Oct 13 20:01:19 2022, max compression
+gzip compressed data, was "problexity-0.5.7.tar", last modified: Tue May 23 15:01:45 2023, max compression
```

## Comparing `problexity-0.5.6.tar` & `problexity-0.5.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 joana      (501) staff       (20)        0 2022-10-13 20:01:19.551554 problexity-0.5.6/
--rw-r--r--   0 joana      (501) staff       (20)    34502 2022-06-16 16:05:05.000000 problexity-0.5.6/LICENSE
--rw-r--r--   0 joana      (501) staff       (20)     7484 2022-10-13 20:01:19.551641 problexity-0.5.6/PKG-INFO
--rw-r--r--   0 joana      (501) staff       (20)     6496 2022-10-13 08:48:46.000000 problexity-0.5.6/README.md
-drwxr-xr-x   0 joana      (501) staff       (20)        0 2022-10-13 20:01:19.548115 problexity-0.5.6/problexity/
--rw-r--r--   0 joana      (501) staff       (20)    14936 2022-10-10 10:17:39.000000 problexity-0.5.6/problexity/ComplexityCalculator.py
--rw-r--r--   0 joana      (501) staff       (20)      781 2022-10-06 09:30:47.000000 problexity-0.5.6/problexity/__init__.py
--rw-r--r--   0 joana      (501) staff       (20)       44 2022-10-13 19:57:47.000000 problexity-0.5.6/problexity/_version.py
-drwxr-xr-x   0 joana      (501) staff       (20)        0 2022-10-13 20:01:19.550517 problexity-0.5.6/problexity/classification/
--rw-r--r--   0 joana      (501) staff       (20)      501 2022-10-04 10:45:11.000000 problexity-0.5.6/problexity/classification/__init__.py
--rw-r--r--   0 joana      (501) staff       (20)     1130 2022-06-17 13:00:21.000000 problexity-0.5.6/problexity/classification/class_imbalance.py
--rw-r--r--   0 joana      (501) staff       (20)     1976 2022-06-19 20:19:56.000000 problexity-0.5.6/problexity/classification/dimensionality.py
--rw-r--r--   0 joana      (501) staff       (20)     6662 2022-10-13 19:56:59.000000 problexity-0.5.6/problexity/classification/feature_based.py
--rw-r--r--   0 joana      (501) staff       (20)     5507 2022-09-26 10:54:21.000000 problexity-0.5.6/problexity/classification/gower.py
--rw-r--r--   0 joana      (501) staff       (20)     3261 2022-06-19 20:27:30.000000 problexity-0.5.6/problexity/classification/linearity.py
--rw-r--r--   0 joana      (501) staff       (20)     8020 2022-07-26 16:14:00.000000 problexity-0.5.6/problexity/classification/neighborhood.py
--rw-r--r--   0 joana      (501) staff       (20)     4015 2022-10-04 10:44:39.000000 problexity-0.5.6/problexity/classification/network.py
-drwxr-xr-x   0 joana      (501) staff       (20)        0 2022-10-13 20:01:19.551103 problexity-0.5.6/problexity/regression/
--rw-r--r--   0 joana      (501) staff       (20)      274 2022-10-04 10:50:56.000000 problexity-0.5.6/problexity/regression/__init__.py
--rw-r--r--   0 joana      (501) staff       (20)     7592 2022-10-07 10:55:38.000000 problexity-0.5.6/problexity/regression/correlation.py
--rw-r--r--   0 joana      (501) staff       (20)     3806 2022-10-07 10:57:03.000000 problexity-0.5.6/problexity/regression/geometry.py
--rw-r--r--   0 joana      (501) staff       (20)     1813 2022-10-03 19:42:24.000000 problexity-0.5.6/problexity/regression/linearity.py
--rw-r--r--   0 joana      (501) staff       (20)     3437 2022-10-07 10:56:13.000000 problexity-0.5.6/problexity/regression/smoothness.py
-drwxr-xr-x   0 joana      (501) staff       (20)        0 2022-10-13 20:01:19.551450 problexity-0.5.6/problexity/tests/
--rw-r--r--   0 joana      (501) staff       (20)        0 2022-06-16 16:05:05.000000 problexity-0.5.6/problexity/tests/__init__.py
--rw-r--r--   0 joana      (501) staff       (20)    19208 2022-10-13 19:57:25.000000 problexity-0.5.6/problexity/tests/test_classification.py
--rw-r--r--   0 joana      (501) staff       (20)     3039 2022-10-13 19:58:36.000000 problexity-0.5.6/problexity/tests/test_regression.py
-drwxr-xr-x   0 joana      (501) staff       (20)        0 2022-10-13 20:01:19.549576 problexity-0.5.6/problexity.egg-info/
--rw-r--r--   0 joana      (501) staff       (20)     7484 2022-10-13 20:01:19.000000 problexity-0.5.6/problexity.egg-info/PKG-INFO
--rw-r--r--   0 joana      (501) staff       (20)      890 2022-10-13 20:01:19.000000 problexity-0.5.6/problexity.egg-info/SOURCES.txt
--rw-r--r--   0 joana      (501) staff       (20)        1 2022-10-13 20:01:19.000000 problexity-0.5.6/problexity.egg-info/dependency_links.txt
--rw-r--r--   0 joana      (501) staff       (20)       50 2022-10-13 20:01:19.000000 problexity-0.5.6/problexity.egg-info/requires.txt
--rw-r--r--   0 joana      (501) staff       (20)       11 2022-10-13 20:01:19.000000 problexity-0.5.6/problexity.egg-info/top_level.txt
--rw-r--r--   0 joana      (501) staff       (20)      330 2022-10-13 20:01:19.552898 problexity-0.5.6/setup.cfg
--rw-r--r--   0 joana      (501) staff       (20)     1884 2022-10-04 12:03:19.000000 problexity-0.5.6/setup.py
+drwxr-xr-x   0 joana      (501) staff       (20)        0 2023-05-23 15:01:45.031122 problexity-0.5.7/
+-rw-r--r--   0 joana      (501) staff       (20)    34502 2022-06-16 16:05:05.000000 problexity-0.5.7/LICENSE
+-rw-r--r--   0 joana      (501) staff       (20)     7502 2023-05-23 15:01:45.031221 problexity-0.5.7/PKG-INFO
+-rw-r--r--   0 joana      (501) staff       (20)     6534 2023-01-24 12:35:37.000000 problexity-0.5.7/README.md
+drwxr-xr-x   0 joana      (501) staff       (20)        0 2023-05-23 15:01:45.025082 problexity-0.5.7/problexity/
+-rw-r--r--   0 joana      (501) staff       (20)    14936 2022-10-10 10:17:39.000000 problexity-0.5.7/problexity/ComplexityCalculator.py
+-rw-r--r--   0 joana      (501) staff       (20)      781 2022-10-06 09:30:47.000000 problexity-0.5.7/problexity/__init__.py
+-rw-r--r--   0 joana      (501) staff       (20)       44 2023-05-23 14:58:26.000000 problexity-0.5.7/problexity/_version.py
+drwxr-xr-x   0 joana      (501) staff       (20)        0 2023-05-23 15:01:45.028419 problexity-0.5.7/problexity/classification/
+-rw-r--r--   0 joana      (501) staff       (20)      501 2022-10-04 10:45:11.000000 problexity-0.5.7/problexity/classification/__init__.py
+-rw-r--r--   0 joana      (501) staff       (20)     1130 2022-06-17 13:00:21.000000 problexity-0.5.7/problexity/classification/class_imbalance.py
+-rw-r--r--   0 joana      (501) staff       (20)     1976 2022-06-19 20:19:56.000000 problexity-0.5.7/problexity/classification/dimensionality.py
+-rw-r--r--   0 joana      (501) staff       (20)     6665 2023-05-09 07:07:51.000000 problexity-0.5.7/problexity/classification/feature_based.py
+-rw-r--r--   0 joana      (501) staff       (20)     5507 2022-09-26 10:54:21.000000 problexity-0.5.7/problexity/classification/gower.py
+-rw-r--r--   0 joana      (501) staff       (20)     3261 2022-06-19 20:27:30.000000 problexity-0.5.7/problexity/classification/linearity.py
+-rw-r--r--   0 joana      (501) staff       (20)     8020 2022-07-26 16:14:00.000000 problexity-0.5.7/problexity/classification/neighborhood.py
+-rw-r--r--   0 joana      (501) staff       (20)     4015 2022-10-04 10:44:39.000000 problexity-0.5.7/problexity/classification/network.py
+drwxr-xr-x   0 joana      (501) staff       (20)        0 2023-05-23 15:01:45.029983 problexity-0.5.7/problexity/regression/
+-rw-r--r--   0 joana      (501) staff       (20)      274 2022-10-04 10:50:56.000000 problexity-0.5.7/problexity/regression/__init__.py
+-rw-r--r--   0 joana      (501) staff       (20)     7592 2022-10-07 10:55:38.000000 problexity-0.5.7/problexity/regression/correlation.py
+-rw-r--r--   0 joana      (501) staff       (20)     3806 2022-10-07 10:57:03.000000 problexity-0.5.7/problexity/regression/geometry.py
+-rw-r--r--   0 joana      (501) staff       (20)     1813 2022-10-03 19:42:24.000000 problexity-0.5.7/problexity/regression/linearity.py
+-rw-r--r--   0 joana      (501) staff       (20)     3437 2022-10-07 10:56:13.000000 problexity-0.5.7/problexity/regression/smoothness.py
+drwxr-xr-x   0 joana      (501) staff       (20)        0 2023-05-23 15:01:45.030858 problexity-0.5.7/problexity/tests/
+-rw-r--r--   0 joana      (501) staff       (20)        0 2022-06-16 16:05:05.000000 problexity-0.5.7/problexity/tests/__init__.py
+-rw-r--r--   0 joana      (501) staff       (20)    19208 2022-10-13 19:57:25.000000 problexity-0.5.7/problexity/tests/test_classification.py
+-rw-r--r--   0 joana      (501) staff       (20)     3039 2022-10-13 19:58:36.000000 problexity-0.5.7/problexity/tests/test_regression.py
+drwxr-xr-x   0 joana      (501) staff       (20)        0 2023-05-23 15:01:45.025864 problexity-0.5.7/problexity.egg-info/
+-rw-r--r--   0 joana      (501) staff       (20)     7502 2023-05-23 15:01:44.000000 problexity-0.5.7/problexity.egg-info/PKG-INFO
+-rw-r--r--   0 joana      (501) staff       (20)      890 2023-05-23 15:01:44.000000 problexity-0.5.7/problexity.egg-info/SOURCES.txt
+-rw-r--r--   0 joana      (501) staff       (20)        1 2023-05-23 15:01:44.000000 problexity-0.5.7/problexity.egg-info/dependency_links.txt
+-rw-r--r--   0 joana      (501) staff       (20)       50 2023-05-23 15:01:44.000000 problexity-0.5.7/problexity.egg-info/requires.txt
+-rw-r--r--   0 joana      (501) staff       (20)       11 2023-05-23 15:01:44.000000 problexity-0.5.7/problexity.egg-info/top_level.txt
+-rw-r--r--   0 joana      (501) staff       (20)      330 2023-05-23 15:01:45.031579 problexity-0.5.7/setup.cfg
+-rw-r--r--   0 joana      (501) staff       (20)     1884 2022-10-04 12:03:19.000000 problexity-0.5.7/setup.py
```

### Comparing `problexity-0.5.6/LICENSE` & `problexity-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/PKG-INFO` & `problexity-0.5.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: problexity
-Version: 0.5.6
+Version: 0.5.7
 Summary: The problexity module is an open-source python library containing the implementation of measures describing the complexity of the classification problem.
 Home-page: https://w4k2.github.io/problexity/
+Download-URL: https://github.com/w4k2/problexity
 Maintainer: J. Komorniczak
 Maintainer-email: joanna.komorniczak@vp.pl
 License: GPL-3.0
-Download-URL: https://github.com/w4k2/problexity
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -30,19 +29,22 @@
 The `problexity` module is an open-source python library containing the implementation of measures describing the complexity of the classification and regression problems. The package contains a ComplexityCalculator model, allowing the calculation, analysis and visualization of problem complexity measures.
 
 ## Citation policy
 
 If you use problexity in a scientific publication, We would appreciate citation to the following papers, including introduction of library and original introduction of used measures:
 
 ```
-@article{komorniczak2022complexity,
-  title={problexity — an open-source Python library for binary classification problem complexity assessment},
-  author={Komorniczak, Joanna and and Ksieniewicz, Pawel},
-  journal={arXiv preprint arXiv:2207.06709},
-  year={2022}
+@article{komorniczak2023problexity,
+  title={problexity—An open-source Python library for supervised learning problem complexity assessment},
+  author={Komorniczak, Joanna and Ksieniewicz, Pawe{\l}},
+  journal={Neurocomputing},
+  volume={521},
+  pages={126--136},
+  year={2023},
+  publisher={Elsevier}
 }
 ```
 
 ```
 @article{lorena2018complex,
   title={How complex is your classification problem},
   author={Lorena, A and Garcia, L and Lehmann, Jens and Souto, M and Ho, T},
@@ -174,9 +176,7 @@
 # Generate plot describing the dataset
 cc.plot(fig, (1,1,1))
 ```
 
 An example of a complexity graph is shown below.
 
 ![Example graph](example_graph.png)
-
-
```

### Comparing `problexity-0.5.6/README.md` & `problexity-0.5.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 The `problexity` module is an open-source python library containing the implementation of measures describing the complexity of the classification and regression problems. The package contains a ComplexityCalculator model, allowing the calculation, analysis and visualization of problem complexity measures.
 
 ## Citation policy
 
 If you use problexity in a scientific publication, We would appreciate citation to the following papers, including introduction of library and original introduction of used measures:
 
 ```
-@article{komorniczak2022complexity,
-  title={problexity — an open-source Python library for binary classification problem complexity assessment},
-  author={Komorniczak, Joanna and and Ksieniewicz, Pawel},
-  journal={arXiv preprint arXiv:2207.06709},
-  year={2022}
+@article{komorniczak2023problexity,
+  title={problexity—An open-source Python library for supervised learning problem complexity assessment},
+  author={Komorniczak, Joanna and Ksieniewicz, Pawe{\l}},
+  journal={Neurocomputing},
+  volume={521},
+  pages={126--136},
+  year={2023},
+  publisher={Elsevier}
 }
 ```
 
 ```
 @article{lorena2018complex,
   title={How complex is your classification problem},
   author={Lorena, A and Garcia, L and Lehmann, Jens and Souto, M and Ho, T},
```

### Comparing `problexity-0.5.6/problexity/ComplexityCalculator.py` & `problexity-0.5.7/problexity/ComplexityCalculator.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/__init__.py` & `problexity-0.5.7/problexity/__init__.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/classification/class_imbalance.py` & `problexity-0.5.7/problexity/classification/class_imbalance.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/classification/dimensionality.py` & `problexity-0.5.7/problexity/classification/dimensionality.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/classification/feature_based.py` & `problexity-0.5.7/problexity/classification/feature_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     X_0_std = np.std(X_0, axis = 0)
     X_1_std = np.std(X_1, axis = 0)
 
     l = (X_0_prop*X_1_prop*np.power((X_0_mean - X_1_mean),2)) + (X_1_prop*X_0_prop*np.power((X_1_mean - X_0_mean),2))
     m = (X_0_prop*(np.power(X_0_std,2))) + (X_1_prop*(np.power(X_1_std,2)))
     r_all = l/m
     
-    return 1 / (1+np.max(r_all))
+    return 1 / (1+np.nanmax(r_all))
 
 def f1v(X, y):
     """
     Calculates the Directional vector maximum Fisher's discriminant ratio (F1v) metric.
 
     .. math::
 
@@ -134,15 +134,15 @@
     maxmin = np.max((np.min(X_0, axis=0), np.min(X_1, axis=0)), axis=0)
     maxmax = np.max((np.max(X_0, axis=0), np.max(X_1, axis=0)), axis=0)
     minmin = np.min((np.min(X_0, axis=0), np.min(X_1, axis=0)), axis=0)
 
     f_overlap = np.max((np.zeros((X.shape[1])), (minmax - maxmin)), axis=0)
     f_range = maxmax - minmin
 
-    return np.product(f_overlap/f_range)
+    return np.nanprod(f_overlap/f_range)
 
 def f3(X, y):
     """
     Calculates the Maximum individual feature efficiency (F3) metric.
 
     Measure describes the efficiency of each feature in the separation of classes. It considers the maximum value among all features.
```

### Comparing `problexity-0.5.6/problexity/classification/gower.py` & `problexity-0.5.7/problexity/classification/gower.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/classification/linearity.py` & `problexity-0.5.7/problexity/classification/linearity.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/classification/neighborhood.py` & `problexity-0.5.7/problexity/classification/neighborhood.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/classification/network.py` & `problexity-0.5.7/problexity/classification/network.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/regression/correlation.py` & `problexity-0.5.7/problexity/regression/correlation.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/regression/geometry.py` & `problexity-0.5.7/problexity/regression/geometry.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/regression/linearity.py` & `problexity-0.5.7/problexity/regression/linearity.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/regression/smoothness.py` & `problexity-0.5.7/problexity/regression/smoothness.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/tests/test_classification.py` & `problexity-0.5.7/problexity/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity/tests/test_regression.py` & `problexity-0.5.7/problexity/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/problexity.egg-info/PKG-INFO` & `problexity-0.5.7/problexity.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: problexity
-Version: 0.5.6
+Version: 0.5.7
 Summary: The problexity module is an open-source python library containing the implementation of measures describing the complexity of the classification problem.
 Home-page: https://w4k2.github.io/problexity/
+Download-URL: https://github.com/w4k2/problexity
 Maintainer: J. Komorniczak
 Maintainer-email: joanna.komorniczak@vp.pl
 License: GPL-3.0
-Download-URL: https://github.com/w4k2/problexity
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -30,19 +29,22 @@
 The `problexity` module is an open-source python library containing the implementation of measures describing the complexity of the classification and regression problems. The package contains a ComplexityCalculator model, allowing the calculation, analysis and visualization of problem complexity measures.
 
 ## Citation policy
 
 If you use problexity in a scientific publication, We would appreciate citation to the following papers, including introduction of library and original introduction of used measures:
 
 ```
-@article{komorniczak2022complexity,
-  title={problexity — an open-source Python library for binary classification problem complexity assessment},
-  author={Komorniczak, Joanna and and Ksieniewicz, Pawel},
-  journal={arXiv preprint arXiv:2207.06709},
-  year={2022}
+@article{komorniczak2023problexity,
+  title={problexity—An open-source Python library for supervised learning problem complexity assessment},
+  author={Komorniczak, Joanna and Ksieniewicz, Pawe{\l}},
+  journal={Neurocomputing},
+  volume={521},
+  pages={126--136},
+  year={2023},
+  publisher={Elsevier}
 }
 ```
 
 ```
 @article{lorena2018complex,
   title={How complex is your classification problem},
   author={Lorena, A and Garcia, L and Lehmann, Jens and Souto, M and Ho, T},
@@ -174,9 +176,7 @@
 # Generate plot describing the dataset
 cc.plot(fig, (1,1,1))
 ```
 
 An example of a complexity graph is shown below.
 
 ![Example graph](example_graph.png)
-
-
```

### Comparing `problexity-0.5.6/problexity.egg-info/SOURCES.txt` & `problexity-0.5.7/problexity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `problexity-0.5.6/setup.py` & `problexity-0.5.7/setup.py`

 * *Files identical despite different names*

