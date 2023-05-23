# Comparing `tmp/amukhsimov-jupyter-templates-bigdata-0.0.3.tar.gz` & `tmp/amukhsimov-jupyter-templates-bigdata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.3.tar", last modified: Tue May 23 09:58:56 2023, max compression
+gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.4.tar", last modified: Tue May 23 10:08:48 2023, max compression
```

## Comparing `amukhsimov-jupyter-templates-bigdata-0.0.3.tar` & `amukhsimov-jupyter-templates-bigdata-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.933770 amukhsimov-jupyter-templates-bigdata-0.0.3/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      376 2023-05-23 09:58:56.933620 amukhsimov-jupyter-templates-bigdata-0.0.3/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1883 2023-05-23 09:21:25.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/README.md
--rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 09:58:56.933813 amukhsimov-jupyter-templates-bigdata-0.0.3/setup.cfg
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1013 2023-05-23 09:58:27.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/setup.py
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.932418 amukhsimov-jupyter-templates-bigdata-0.0.3/src/
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.932481 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.933456 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      376 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)      522 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:08:48.710603 amukhsimov-jupyter-templates-bigdata-0.0.4/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 10:08:48.710433 amukhsimov-jupyter-templates-bigdata-0.0.4/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     1883 2023-05-23 09:21:25.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/README.md
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:08:48.709606 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:08:48.710243 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      579 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       77 2023-05-23 10:07:36.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 10:08:48.710654 amukhsimov-jupyter-templates-bigdata-0.0.4/setup.cfg
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     1009 2023-05-23 10:07:49.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/setup.py
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.3/README.md` & `amukhsimov-jupyter-templates-bigdata-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.3/setup.py` & `amukhsimov-jupyter-templates-bigdata-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'amukhsimov-jupyter-templates-bigdata'
 LONG_DESCRIPTION = 'No description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="amukhsimov-jupyter-templates-bigdata",
@@ -19,10 +19,10 @@
     # needs to be installed along with your package. Eg: 'caer'
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     py_modules=["amukhsimov_jupyter_templates_bigdata"],
-    package_dir={'': 'src/amukhsimov_jupyter_templates_bigdata'},
+    package_dir={'': 'amukhsimov_jupyter_templates_bigdata'},
     python_requires=">=3.6"
 )
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt` & `amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 README.md
 setup.py
-src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
-src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
-src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
-src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
-src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
+amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.py
+amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
+amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
+amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
+amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
+amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
```

