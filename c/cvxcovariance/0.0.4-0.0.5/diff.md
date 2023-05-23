# Comparing `tmp/cvxcovariance-0.0.4.tar.gz` & `tmp/cvxcovariance-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxcovariance-0.0.4.tar", max compression
+gzip compressed data, was "cvxcovariance-0.0.5.tar", max compression
```

## Comparing `cvxcovariance-0.0.4.tar` & `cvxcovariance-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11375 2023-05-23 17:19:48.663657 cvxcovariance-0.0.4/LICENSE
--rw-r--r--   0        0        0      542 2023-05-23 17:19:48.663657 cvxcovariance-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-23 17:19:48.691657 cvxcovariance-0.0.4/cvx/covariance/__init__.py
--rw-r--r--   0        0        0     6737 2023-05-23 17:19:48.691657 cvxcovariance-0.0.4/cvx/covariance/covariance_combination.py
--rw-r--r--   0        0        0     6542 2023-05-23 17:19:48.691657 cvxcovariance-0.0.4/cvx/covariance/ewma.py
--rw-r--r--   0        0        0     8440 2023-05-23 17:19:48.691657 cvxcovariance-0.0.4/cvx/covariance/iterated_ewma_vec.py
--rw-r--r--   0        0        0      600 2023-05-23 17:20:17.871481 cvxcovariance-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 cvxcovariance-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-05-23 18:05:21.231819 cvxcovariance-0.0.5/LICENSE
+-rw-r--r--   0        0        0      542 2023-05-23 18:05:21.231819 cvxcovariance-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/__init__.py
+-rw-r--r--   0        0        0     6737 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/covariance_combination.py
+-rw-r--r--   0        0        0     6542 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/ewma.py
+-rw-r--r--   0        0        0     8440 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/iterated_ewma_vec.py
+-rw-r--r--   0        0        0      600 2023-05-23 18:05:51.312697 cvxcovariance-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 cvxcovariance-0.0.5/PKG-INFO
```

### Comparing `cvxcovariance-0.0.4/LICENSE` & `cvxcovariance-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.4/README.md` & `cvxcovariance-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.4/cvx/covariance/covariance_combination.py` & `cvxcovariance-0.0.5/cvx/covariance/covariance_combination.py`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.4/cvx/covariance/ewma.py` & `cvxcovariance-0.0.5/cvx/covariance/ewma.py`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.4/cvx/covariance/iterated_ewma_vec.py` & `cvxcovariance-0.0.5/cvx/covariance/iterated_ewma_vec.py`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.4/pyproject.toml` & `cvxcovariance-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxcovariance"
-version = "v0.0.4"             # Don't touch, leave at 0.0.0
+version = "v0.0.5"             # Don't touch, leave at 0.0.0
 description = "..."
 authors = ["Kasper", "Thomas"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cov_pred_finance"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxcovariance-0.0.4/PKG-INFO` & `cvxcovariance-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxcovariance
-Version: 0.0.4
+Version: 0.0.5
 Summary: ...
 Home-page: https://github.com/cvxgrp/cov_pred_finance
 Author: Kasper
 Requires-Python: >=3.8.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

