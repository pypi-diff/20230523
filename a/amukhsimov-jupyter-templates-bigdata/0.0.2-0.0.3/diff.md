# Comparing `tmp/amukhsimov-jupyter-templates-bigdata-0.0.2.tar.gz` & `tmp/amukhsimov-jupyter-templates-bigdata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.2.tar", last modified: Tue May 23 09:55:32 2023, max compression
+gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.3.tar", last modified: Tue May 23 09:58:56 2023, max compression
```

## Comparing `amukhsimov-jupyter-templates-bigdata-0.0.2.tar` & `amukhsimov-jupyter-templates-bigdata-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:55:32.214684 amukhsimov-jupyter-templates-bigdata-0.0.2/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      376 2023-05-23 09:55:32.214515 amukhsimov-jupyter-templates-bigdata-0.0.2/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1883 2023-05-23 09:21:25.000000 amukhsimov-jupyter-templates-bigdata-0.0.2/README.md
--rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 09:55:32.214731 amukhsimov-jupyter-templates-bigdata-0.0.2/setup.cfg
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1013 2023-05-23 09:55:23.000000 amukhsimov-jupyter-templates-bigdata-0.0.2/setup.py
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:55:32.212923 amukhsimov-jupyter-templates-bigdata-0.0.2/src/
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:55:32.212985 amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:55:32.214323 amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      376 2023-05-23 09:55:32.000000 amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)      522 2023-05-23 09:55:32.000000 amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 09:55:32.000000 amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 09:55:32.000000 amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 09:55:32.000000 amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.933770 amukhsimov-jupyter-templates-bigdata-0.0.3/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      376 2023-05-23 09:58:56.933620 amukhsimov-jupyter-templates-bigdata-0.0.3/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     1883 2023-05-23 09:21:25.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/README.md
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 09:58:56.933813 amukhsimov-jupyter-templates-bigdata-0.0.3/setup.cfg
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     1013 2023-05-23 09:58:27.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/setup.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.932418 amukhsimov-jupyter-templates-bigdata-0.0.3/src/
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.932481 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 09:58:56.933456 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      376 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      522 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 09:58:56.000000 amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.2/README.md` & `amukhsimov-jupyter-templates-bigdata-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.2/setup.py` & `amukhsimov-jupyter-templates-bigdata-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'amukhsimov-jupyter-templates-bigdata'
 LONG_DESCRIPTION = 'No description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="amukhsimov-jupyter-templates-bigdata",
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.2/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt` & `amukhsimov-jupyter-templates-bigdata-0.0.3/src/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

