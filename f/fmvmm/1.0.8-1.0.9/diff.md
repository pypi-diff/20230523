# Comparing `tmp/fmvmm-1.0.8.tar.gz` & `tmp/fmvmm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmvmm-1.0.8.tar", last modified: Tue May 23 09:24:24 2023, max compression
+gzip compressed data, was "fmvmm-1.0.9.tar", last modified: Tue May 23 10:02:30 2023, max compression
```

## Comparing `fmvmm-1.0.8.tar` & `fmvmm-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:24.345208 fmvmm-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 09:24:10.000000 fmvmm-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 09:24:24.345208 fmvmm-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:24.345208 fmvmm-1.0.8/fmvmm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 09:24:24.000000 fmvmm-1.0.8/fmvmm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:24:24.000000 fmvmm-1.0.8/fmvmm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:24:24.000000 fmvmm-1.0.8/fmvmm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 09:24:24.000000 fmvmm-1.0.8/fmvmm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 09:24:24.000000 fmvmm-1.0.8/fmvmm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:24:24.000000 fmvmm-1.0.8/fmvmm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:24.345208 fmvmm-1.0.8/mixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-23 09:24:10.000000 fmvmm-1.0.8/mixtures/DMM_Class.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-05-23 09:24:10.000000 fmvmm-1.0.8/mixtures/DMM_Soft_Class.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:10.000000 fmvmm-1.0.8/mixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:24:24.345208 fmvmm-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 09:24:10.000000 fmvmm-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:24.345208 fmvmm-1.0.8/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:10.000000 fmvmm-1.0.8/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-23 09:24:10.000000 fmvmm-1.0.8/utils/utils_dmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-23 09:24:10.000000 fmvmm-1.0.8/utils/utils_fmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-23 09:24:10.000000 fmvmm-1.0.8/utils/utils_mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:30.684698 fmvmm-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 10:02:19.000000 fmvmm-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 10:02:30.684698 fmvmm-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:30.684698 fmvmm-1.0.9/fmvmm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:30.684698 fmvmm-1.0.9/fmvmm/mixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/mixtures/DMM_Class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/mixtures/DMM_Soft_Class.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/mixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:30.684698 fmvmm-1.0.9/fmvmm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/utils/utils_dmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/utils/utils_fmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-23 10:02:19.000000 fmvmm-1.0.9/fmvmm/utils/utils_mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:02:30.684698 fmvmm-1.0.9/fmvmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 10:02:30.000000 fmvmm-1.0.9/fmvmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-23 10:02:30.000000 fmvmm-1.0.9/fmvmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:02:30.000000 fmvmm-1.0.9/fmvmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 10:02:30.000000 fmvmm-1.0.9/fmvmm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 10:02:30.000000 fmvmm-1.0.9/fmvmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 10:02:30.000000 fmvmm-1.0.9/fmvmm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:02:30.684698 fmvmm-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 10:02:19.000000 fmvmm-1.0.9/setup.py
```

### Comparing `fmvmm-1.0.8/LICENSE` & `fmvmm-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fmvmm-1.0.8/mixtures/DMM_Class.py` & `fmvmm-1.0.9/fmvmm/mixtures/DMM_Class.py`

 * *Files identical despite different names*

### Comparing `fmvmm-1.0.8/mixtures/DMM_Soft_Class.py` & `fmvmm-1.0.9/fmvmm/mixtures/DMM_Soft_Class.py`

 * *Files identical despite different names*

### Comparing `fmvmm-1.0.8/setup.py` & `fmvmm-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fmvmm',
-    version='1.0.8',
+    version='1.0.9',
     author='Samyajoy Pal',
     author_email='palsamyajoy@gmail.com',
     description="flexible multivariate mixture model",
     long_description="mixture model with different distributions",
     packages=find_packages(),
     install_requires=[
         'numpy',
```

### Comparing `fmvmm-1.0.8/utils/utils_dmm.py` & `fmvmm-1.0.9/fmvmm/utils/utils_dmm.py`

 * *Files identical despite different names*

### Comparing `fmvmm-1.0.8/utils/utils_fmm.py` & `fmvmm-1.0.9/fmvmm/utils/utils_fmm.py`

 * *Files identical despite different names*

### Comparing `fmvmm-1.0.8/utils/utils_mixture.py` & `fmvmm-1.0.9/fmvmm/utils/utils_mixture.py`

 * *Files identical despite different names*

