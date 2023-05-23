# Comparing `tmp/fmvmm-1.0.5.tar.gz` & `tmp/fmvmm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmvmm-1.0.5.tar", last modified: Tue May 23 08:36:20 2023, max compression
+gzip compressed data, was "fmvmm-1.0.7.tar", last modified: Tue May 23 09:16:24 2023, max compression
```

## Comparing `fmvmm-1.0.5.tar` & `fmvmm-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:36:20.638819 fmvmm-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 08:36:09.000000 fmvmm-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 08:36:20.638819 fmvmm-1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:36:20.638819 fmvmm-1.0.5/fmvmm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:36:20.638819 fmvmm-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 08:36:09.000000 fmvmm-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:16:24.006468 fmvmm-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 09:16:12.000000 fmvmm-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 09:16:24.006468 fmvmm-1.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:16:24.006468 fmvmm-1.0.7/fmvmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 09:16:23.000000 fmvmm-1.0.7/fmvmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:16:24.000000 fmvmm-1.0.7/fmvmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:16:23.000000 fmvmm-1.0.7/fmvmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 09:16:23.000000 fmvmm-1.0.7/fmvmm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 09:16:23.000000 fmvmm-1.0.7/fmvmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:16:23.000000 fmvmm-1.0.7/fmvmm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:16:24.006468 fmvmm-1.0.7/mixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-23 09:16:12.000000 fmvmm-1.0.7/mixtures/DMM_Class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-05-23 09:16:12.000000 fmvmm-1.0.7/mixtures/DMM_Soft_Class.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:16:12.000000 fmvmm-1.0.7/mixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:16:24.006468 fmvmm-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 09:16:12.000000 fmvmm-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:16:24.006468 fmvmm-1.0.7/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:16:12.000000 fmvmm-1.0.7/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-23 09:16:12.000000 fmvmm-1.0.7/utils/utils_dmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-23 09:16:12.000000 fmvmm-1.0.7/utils/utils_fmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-23 09:16:12.000000 fmvmm-1.0.7/utils/utils_mixture.py
```

### Comparing `fmvmm-1.0.5/LICENSE` & `fmvmm-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fmvmm-1.0.5/setup.py` & `fmvmm-1.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fmvmm',
-    version='1.0.5',
+    version='1.0.7',
     author='Samyajoy Pal',
     author_email='palsamyajoy@gmail.com',
     description="flexible multivariate mixture model",
     long_description="mixture model with different distributions",
     packages=find_packages(),
     install_requires=[
         'numpy',
```

