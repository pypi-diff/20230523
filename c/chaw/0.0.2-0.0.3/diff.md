# Comparing `tmp/chaw-0.0.2.tar.gz` & `tmp/chaw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaw-0.0.2.tar", last modified: Tue May 23 17:51:49 2023, max compression
+gzip compressed data, was "chaw-0.0.3.tar", last modified: Tue May 23 17:56:31 2023, max compression
```

## Comparing `chaw-0.0.2.tar` & `chaw-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:51:49.336552 chaw-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 17:51:49.336552 chaw-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-23 17:51:38.000000 chaw-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:51:49.336552 chaw-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 17:51:38.000000 chaw-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:51:49.332552 chaw-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:51:49.332552 chaw-0.0.2/src/chaw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:51:38.000000 chaw-0.0.2/src/chaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-23 17:51:38.000000 chaw-0.0.2/src/chaw/chaw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:51:49.336552 chaw-0.0.2/src/chaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 17:51:49.000000 chaw-0.0.2/src/chaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 17:51:49.000000 chaw-0.0.2/src/chaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:51:49.000000 chaw-0.0.2/src/chaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 17:51:49.000000 chaw-0.0.2/src/chaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 17:51:49.000000 chaw-0.0.2/src/chaw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:31.540473 chaw-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 17:56:31.540473 chaw-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-23 17:56:19.000000 chaw-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:56:31.540473 chaw-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 17:56:19.000000 chaw-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:31.536473 chaw-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:31.540473 chaw-0.0.3/src/chaw/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 17:56:19.000000 chaw-0.0.3/src/chaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-23 17:56:19.000000 chaw-0.0.3/src/chaw/chaw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:31.540473 chaw-0.0.3/src/chaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 17:56:31.000000 chaw-0.0.3/src/chaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 17:56:31.000000 chaw-0.0.3/src/chaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:56:31.000000 chaw-0.0.3/src/chaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 17:56:31.000000 chaw-0.0.3/src/chaw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 17:56:31.000000 chaw-0.0.3/src/chaw.egg-info/top_level.txt
```

### Comparing `chaw-0.0.2/setup.py` & `chaw-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Wrapper for the Companies House API'
 LONG_DESCRIPTION = 'Wrapper for the Companies House API'
 
 setup(
         name="chaw", 
         version=VERSION,
         author="Morgan Thomas",
```

### Comparing `chaw-0.0.2/src/chaw/chaw.py` & `chaw-0.0.3/src/chaw/chaw.py`

 * *Files identical despite different names*

