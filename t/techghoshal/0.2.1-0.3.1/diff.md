# Comparing `tmp/techghoshal-0.2.1.tar.gz` & `tmp/techghoshal-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techghoshal-0.2.1.tar", last modified: Tue May 23 13:23:34 2023, max compression
+gzip compressed data, was "techghoshal-0.3.1.tar", last modified: Tue May 23 13:36:38 2023, max compression
```

## Comparing `techghoshal-0.2.1.tar` & `techghoshal-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:23:34.869988 techghoshal-0.2.1/
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-23 13:23:34.869988 techghoshal-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-23 12:12:53.000000 techghoshal-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:23:34.869988 techghoshal-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-23 13:23:25.000000 techghoshal-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:23:34.869988 techghoshal-0.2.1/techghoshal/
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-23 13:21:55.000000 techghoshal-0.2.1/techghoshal/__init__.py
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-23 13:15:53.000000 techghoshal-0.2.1/techghoshal/hello.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:23:34.869988 techghoshal-0.2.1/techghoshal.egg-info/
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-23 13:23:34.000000 techghoshal-0.2.1/techghoshal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-23 13:23:34.000000 techghoshal-0.2.1/techghoshal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:23:34.000000 techghoshal-0.2.1/techghoshal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-23 13:23:34.000000 techghoshal-0.2.1/techghoshal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-23 13:23:34.000000 techghoshal-0.2.1/techghoshal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:36:38.373689 techghoshal-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-23 13:36:38.373689 techghoshal-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-23 12:12:53.000000 techghoshal-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:36:38.373689 techghoshal-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-23 13:36:32.000000 techghoshal-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:36:38.369689 techghoshal-0.3.1/techghoshal/
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-23 13:36:04.000000 techghoshal-0.3.1/techghoshal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:36:38.373689 techghoshal-0.3.1/techghoshal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-23 13:36:38.000000 techghoshal-0.3.1/techghoshal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-23 13:36:38.000000 techghoshal-0.3.1/techghoshal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:36:38.000000 techghoshal-0.3.1/techghoshal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-23 13:36:38.000000 techghoshal-0.3.1/techghoshal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-23 13:36:38.000000 techghoshal-0.3.1/techghoshal.egg-info/top_level.txt
```

### Comparing `techghoshal-0.2.1/setup.py` & `techghoshal-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.1'
+VERSION = '0.3.1'
 DESCRIPTION = 'Basic Hello package'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="techghoshal",
     version=VERSION,
```

