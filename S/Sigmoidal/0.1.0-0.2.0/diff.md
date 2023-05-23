# Comparing `tmp/sigmoidal-0.1.0.tar.gz` & `tmp/Sigmoidal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmoidal-0.1.0.tar", last modified: Mon May 22 21:34:34 2023, max compression
+gzip compressed data, was "Sigmoidal-0.2.0.tar", last modified: Mon May 22 21:52:35 2023, max compression
```

## Comparing `sigmoidal-0.1.0.tar` & `Sigmoidal-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-22 21:34:34.705321 sigmoidal-0.1.0/
--rw-r--r--   0 jade       (502) staff       (20)     1063 2023-05-22 21:09:43.000000 sigmoidal-0.1.0/LICENSE
--rw-r--r--   0 jade       (502) staff       (20)        0 2023-05-22 21:14:28.000000 sigmoidal-0.1.0/MANIFEST.in
--rw-r--r--   0 jade       (502) staff       (20)     1275 2023-05-22 21:34:34.704822 sigmoidal-0.1.0/PKG-INFO
--rw-r--r--   0 jade       (502) staff       (20)     1042 2023-05-22 21:14:28.000000 sigmoidal-0.1.0/README.md
--rw-r--r--   0 jade       (502) staff       (20)       38 2023-05-22 21:34:34.705352 sigmoidal-0.1.0/setup.cfg
--rw-r--r--   0 jade       (502) staff       (20)      438 2023-05-22 21:32:00.000000 sigmoidal-0.1.0/setup.py
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-22 21:34:34.704139 sigmoidal-0.1.0/sigmoidal/
--rw-r--r--   0 jade       (502) staff       (20)     4183 2023-05-22 21:14:28.000000 sigmoidal-0.1.0/sigmoidal/__init__.py
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-22 21:34:34.704671 sigmoidal-0.1.0/sigmoidal.egg-info/
--rw-r--r--   0 jade       (502) staff       (20)     1275 2023-05-22 21:34:34.000000 sigmoidal-0.1.0/sigmoidal.egg-info/PKG-INFO
--rw-r--r--   0 jade       (502) staff       (20)      224 2023-05-22 21:34:34.000000 sigmoidal-0.1.0/sigmoidal.egg-info/SOURCES.txt
--rw-r--r--   0 jade       (502) staff       (20)        1 2023-05-22 21:34:34.000000 sigmoidal-0.1.0/sigmoidal.egg-info/dependency_links.txt
--rw-r--r--   0 jade       (502) staff       (20)       28 2023-05-22 21:34:34.000000 sigmoidal-0.1.0/sigmoidal.egg-info/requires.txt
--rw-r--r--   0 jade       (502) staff       (20)       10 2023-05-22 21:34:34.000000 sigmoidal-0.1.0/sigmoidal.egg-info/top_level.txt
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-22 21:52:35.701104 Sigmoidal-0.2.0/
+-rw-r--r--   0 jade       (502) staff       (20)     1063 2023-05-22 21:09:43.000000 Sigmoidal-0.2.0/LICENSE
+-rw-r--r--   0 jade       (502) staff       (20)        0 2023-05-22 21:14:28.000000 Sigmoidal-0.2.0/MANIFEST.in
+-rw-r--r--   0 jade       (502) staff       (20)     1424 2023-05-22 21:52:35.700598 Sigmoidal-0.2.0/PKG-INFO
+-rw-r--r--   0 jade       (502) staff       (20)     1041 2023-05-22 21:50:35.000000 Sigmoidal-0.2.0/README.md
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-22 21:52:35.700160 Sigmoidal-0.2.0/Sigmoidal.egg-info/
+-rw-r--r--   0 jade       (502) staff       (20)     1424 2023-05-22 21:52:35.000000 Sigmoidal-0.2.0/Sigmoidal.egg-info/PKG-INFO
+-rw-r--r--   0 jade       (502) staff       (20)      388 2023-05-22 21:52:35.000000 Sigmoidal-0.2.0/Sigmoidal.egg-info/SOURCES.txt
+-rw-r--r--   0 jade       (502) staff       (20)        1 2023-05-22 21:52:35.000000 Sigmoidal-0.2.0/Sigmoidal.egg-info/dependency_links.txt
+-rw-r--r--   0 jade       (502) staff       (20)       28 2023-05-22 21:52:35.000000 Sigmoidal-0.2.0/Sigmoidal.egg-info/requires.txt
+-rw-r--r--   0 jade       (502) staff       (20)       10 2023-05-22 21:52:35.000000 Sigmoidal-0.2.0/Sigmoidal.egg-info/top_level.txt
+-rw-r--r--   0 jade       (502) staff       (20)       38 2023-05-22 21:52:35.701138 Sigmoidal-0.2.0/setup.cfg
+-rw-r--r--   0 jade       (502) staff       (20)      598 2023-05-22 21:50:35.000000 Sigmoidal-0.2.0/setup.py
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-22 21:52:35.700256 Sigmoidal-0.2.0/sigmoidal/
+-rw-r--r--   0 jade       (502) staff       (20)     4183 2023-05-22 21:14:28.000000 Sigmoidal-0.2.0/sigmoidal/__init__.py
```

### Comparing `sigmoidal-0.1.0/LICENSE` & `Sigmoidal-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmoidal-0.1.0/PKG-INFO` & `Sigmoidal-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: sigmoidal
-Version: 0.1.0
+Name: Sigmoidal
+Version: 0.2.0
+Summary: Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.
 Home-page: https://github.com/HelloSleuth/sigmoid
-Author: Jade Glaze
+Author: Jade Glaze, Sleuth
 Author-email: jade@hellosleuth.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sigmoid 
+# Sigmoidal 
 
-This library is intended to work like the [Numpy Polynomial](https://numpy.org/doc/stable/reference/generated/numpy.polynomial.polynomial.Polynomial.html) class where it makes sense. Specifically it supports:
+Sigmoidal is intended to work like the [Numpy Polynomial](https://numpy.org/doc/stable/reference/generated/numpy.polynomial.polynomial.Polynomial.html) class where it makes sense. Specifically it supports:
 * Using the sigmoid function in a very natural way like `y = sig(x)` including when x is a numpy array. (Once you've created a Sigmoid instance `sig = Sigmoid(...)`)
 * Fitting a Sigmoid to data just like Polynomial with `Sigmoid.fit(x, y)`.
 * Taking the first or second derivative with `deriv()`.
 * Finding the roots of the sigmoid or it's first or second derivitive with `.roots()`.
 * The convenience method `.linspace()` which can get you an array of dependent values with only the range of independent values.
 * `.copy()`
 * Operations `==`, `!=`, `str()`, `repr()`
```

### Comparing `sigmoidal-0.1.0/README.md` & `Sigmoidal-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Sigmoid 
+# Sigmoidal 
 
-This library is intended to work like the [Numpy Polynomial](https://numpy.org/doc/stable/reference/generated/numpy.polynomial.polynomial.Polynomial.html) class where it makes sense. Specifically it supports:
+Sigmoidal is intended to work like the [Numpy Polynomial](https://numpy.org/doc/stable/reference/generated/numpy.polynomial.polynomial.Polynomial.html) class where it makes sense. Specifically it supports:
 * Using the sigmoid function in a very natural way like `y = sig(x)` including when x is a numpy array. (Once you've created a Sigmoid instance `sig = Sigmoid(...)`)
 * Fitting a Sigmoid to data just like Polynomial with `Sigmoid.fit(x, y)`.
 * Taking the first or second derivative with `deriv()`.
 * Finding the roots of the sigmoid or it's first or second derivitive with `.roots()`.
 * The convenience method `.linspace()` which can get you an array of dependent values with only the range of independent values.
 * `.copy()`
 * Operations `==`, `!=`, `str()`, `repr()`
```

### Comparing `sigmoidal-0.1.0/sigmoidal/__init__.py` & `Sigmoidal-0.2.0/sigmoidal/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmoidal-0.1.0/sigmoidal.egg-info/PKG-INFO` & `Sigmoidal-0.2.0/Sigmoidal.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: sigmoidal
-Version: 0.1.0
+Name: Sigmoidal
+Version: 0.2.0
+Summary: Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.
 Home-page: https://github.com/HelloSleuth/sigmoid
-Author: Jade Glaze
+Author: Jade Glaze, Sleuth
 Author-email: jade@hellosleuth.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sigmoid 
+# Sigmoidal 
 
-This library is intended to work like the [Numpy Polynomial](https://numpy.org/doc/stable/reference/generated/numpy.polynomial.polynomial.Polynomial.html) class where it makes sense. Specifically it supports:
+Sigmoidal is intended to work like the [Numpy Polynomial](https://numpy.org/doc/stable/reference/generated/numpy.polynomial.polynomial.Polynomial.html) class where it makes sense. Specifically it supports:
 * Using the sigmoid function in a very natural way like `y = sig(x)` including when x is a numpy array. (Once you've created a Sigmoid instance `sig = Sigmoid(...)`)
 * Fitting a Sigmoid to data just like Polynomial with `Sigmoid.fit(x, y)`.
 * Taking the first or second derivative with `deriv()`.
 * Finding the roots of the sigmoid or it's first or second derivitive with `.roots()`.
 * The convenience method `.linspace()` which can get you an array of dependent values with only the range of independent values.
 * `.copy()`
 * Operations `==`, `!=`, `str()`, `repr()`
```

