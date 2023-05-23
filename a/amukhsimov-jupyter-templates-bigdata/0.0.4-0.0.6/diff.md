# Comparing `tmp/amukhsimov-jupyter-templates-bigdata-0.0.4.tar.gz` & `tmp/amukhsimov-jupyter-templates-bigdata-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.4.tar", last modified: Tue May 23 10:08:48 2023, max compression
+gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.6.tar", last modified: Tue May 23 10:22:41 2023, max compression
```

## Comparing `amukhsimov-jupyter-templates-bigdata-0.0.4.tar` & `amukhsimov-jupyter-templates-bigdata-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:08:48.710603 amukhsimov-jupyter-templates-bigdata-0.0.4/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 10:08:48.710433 amukhsimov-jupyter-templates-bigdata-0.0.4/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1883 2023-05-23 09:21:25.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/README.md
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:08:48.709606 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:08:48.710243 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)      579 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 10:08:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       77 2023-05-23 10:07:36.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/amukhsimov_jupyter_templates_bigdata/amukhsimov_jupyter_templates_bigdata.py
--rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 10:08:48.710654 amukhsimov-jupyter-templates-bigdata-0.0.4/setup.cfg
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1009 2023-05-23 10:07:49.000000 amukhsimov-jupyter-templates-bigdata-0.0.4/setup.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:22:41.221314 amukhsimov-jupyter-templates-bigdata-0.0.6/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 10:22:41.221157 amukhsimov-jupyter-templates-bigdata-0.0.6/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     1883 2023-05-23 09:21:25.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/README.md
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 10:22:41.221360 amukhsimov-jupyter-templates-bigdata-0.0.6/setup.cfg
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      944 2023-05-23 10:21:57.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/setup.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:22:41.219637 amukhsimov-jupyter-templates-bigdata-0.0.6/src/
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:22:41.220390 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       79 2023-05-23 10:17:48.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata/__init__.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     9792 2023-05-23 10:18:03.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata/connectors.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      808 2023-05-23 08:22:13.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata/crypto.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 10:22:41.220983 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata.egg-info/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 10:22:40.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      496 2023-05-23 10:22:41.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 10:22:40.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 10:22:41.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 10:22:41.000000 amukhsimov-jupyter-templates-bigdata-0.0.6/src/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.4/README.md` & `amukhsimov-jupyter-templates-bigdata-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.4/setup.py` & `amukhsimov-jupyter-templates-bigdata-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.6'
 DESCRIPTION = 'amukhsimov-jupyter-templates-bigdata'
 LONG_DESCRIPTION = 'No description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="amukhsimov-jupyter-templates-bigdata",
     version=VERSION,
     author="Akmal Mukhsimov",
     author_email="a.mukhsimov@hamkorlab.club",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
     install_requires=['python-dotenv', 'pyspark', 'cx-Oracle',
                       'cryptography', 'psycopg2'],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    py_modules=["amukhsimov_jupyter_templates_bigdata"],
-    package_dir={'': 'amukhsimov_jupyter_templates_bigdata'},
+    packages=['amukhsimov_jupyter_templates_bigdata'],
+    package_dir={'': 'src'},
     python_requires=">=3.6"
 )
```

