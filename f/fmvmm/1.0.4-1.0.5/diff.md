# Comparing `tmp/fmvmm-1.0.4.tar.gz` & `tmp/fmvmm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmvmm-1.0.4.tar", last modified: Tue May 23 08:15:08 2023, max compression
+gzip compressed data, was "fmvmm-1.0.5.tar", last modified: Tue May 23 08:36:20 2023, max compression
```

## Comparing `fmvmm-1.0.4.tar` & `fmvmm-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:15:08.556223 fmvmm-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 08:14:57.000000 fmvmm-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 08:15:08.556223 fmvmm-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:15:08.556223 fmvmm-1.0.4/fmvmm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 08:15:08.000000 fmvmm-1.0.4/fmvmm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 08:15:08.000000 fmvmm-1.0.4/fmvmm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:15:08.000000 fmvmm-1.0.4/fmvmm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 08:15:08.000000 fmvmm-1.0.4/fmvmm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 08:15:08.000000 fmvmm-1.0.4/fmvmm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:15:08.000000 fmvmm-1.0.4/fmvmm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:15:08.560222 fmvmm-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-23 08:14:57.000000 fmvmm-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:36:20.638819 fmvmm-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 08:36:09.000000 fmvmm-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 08:36:20.638819 fmvmm-1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:36:20.638819 fmvmm-1.0.5/fmvmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:36:20.000000 fmvmm-1.0.5/fmvmm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:36:20.638819 fmvmm-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 08:36:09.000000 fmvmm-1.0.5/setup.py
```

### Comparing `fmvmm-1.0.4/LICENSE` & `fmvmm-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fmvmm-1.0.4/setup.py` & `fmvmm-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fmvmm',
-    version='1.0.4',
+    version='1.0.5',
     author='Samyajoy Pal',
     author_email='palsamyajoy@gmail.com',
     description="flexible multivariate mixture model",
     long_description="mixture model with different distributions",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'pandas',
-        'math',
-        'copy',
         'dirichlet',
         'sklearn'
     ],
     entry_points={
         'console_scripts': [
             'my_command = fmvmm.command:main',
         ],
```

