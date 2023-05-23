# Comparing `tmp/tenforce-0.1.0.tar.gz` & `tmp/tenforce-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenforce-0.1.0.tar", last modified: Tue May 23 03:49:06 2023, max compression
+gzip compressed data, was "tenforce-0.1.0b0.tar", last modified: Tue May 23 03:57:45 2023, max compression
```

## Comparing `tenforce-0.1.0.tar` & `tenforce-0.1.0b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:49:06.048527 tenforce-0.1.0/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     1071 2023-05-23 03:05:36.000000 tenforce-0.1.0/LICENSE.md
--rw-r--r--   0 hunterlafaille   (501) staff       (20)       29 2023-05-22 15:11:35.000000 tenforce-0.1.0/MANIFEST.in
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      138 2023-05-23 03:49:06.048410 tenforce-0.1.0/PKG-INFO
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     1635 2023-05-23 03:11:36.000000 tenforce-0.1.0/README.md
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      328 2023-05-23 03:48:35.000000 tenforce-0.1.0/pyproject.toml
--rw-r--r--   0 hunterlafaille   (501) staff       (20)       38 2023-05-23 03:49:06.048565 tenforce-0.1.0/setup.cfg
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      152 2023-05-23 03:42:27.000000 tenforce-0.1.0/setup.py
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:49:06.047413 tenforce-0.1.0/tenforce/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)        0 2023-05-21 20:05:52.000000 tenforce-0.1.0/tenforce/__init__.py
--rw-r--r--   0 hunterlafaille   (501) staff       (20)   390946 2023-05-23 03:49:05.000000 tenforce-0.1.0/tenforce/enforcer.c
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     6337 2023-05-23 02:50:27.000000 tenforce-0.1.0/tenforce/enforcer.pyx
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      551 2023-05-23 02:18:21.000000 tenforce-0.1.0/tenforce/exceptions.py
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:49:06.048029 tenforce-0.1.0/tenforce.egg-info/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      138 2023-05-23 03:49:06.000000 tenforce-0.1.0/tenforce.egg-info/PKG-INFO
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      284 2023-05-23 03:49:06.000000 tenforce-0.1.0/tenforce.egg-info/SOURCES.txt
--rw-r--r--   0 hunterlafaille   (501) staff       (20)        1 2023-05-23 03:49:06.000000 tenforce-0.1.0/tenforce.egg-info/dependency_links.txt
--rw-r--r--   0 hunterlafaille   (501) staff       (20)        9 2023-05-23 03:49:06.000000 tenforce-0.1.0/tenforce.egg-info/top_level.txt
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:49:06.048133 tenforce-0.1.0/tests/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     2127 2023-05-23 03:08:35.000000 tenforce-0.1.0/tests/test.py
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:57:45.709740 tenforce-0.1.0b0/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     1071 2023-05-23 03:05:36.000000 tenforce-0.1.0b0/LICENSE.md
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)       29 2023-05-22 15:11:35.000000 tenforce-0.1.0b0/MANIFEST.in
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      194 2023-05-23 03:57:45.709635 tenforce-0.1.0b0/PKG-INFO
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     1635 2023-05-23 03:11:36.000000 tenforce-0.1.0b0/README.md
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      329 2023-05-23 03:57:32.000000 tenforce-0.1.0b0/pyproject.toml
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)       38 2023-05-23 03:57:45.709782 tenforce-0.1.0b0/setup.cfg
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      298 2023-05-23 03:57:15.000000 tenforce-0.1.0b0/setup.py
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:57:45.708714 tenforce-0.1.0b0/tenforce/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)        0 2023-05-21 20:05:52.000000 tenforce-0.1.0b0/tenforce/__init__.py
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)   390946 2023-05-23 03:57:45.000000 tenforce-0.1.0b0/tenforce/enforcer.c
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     6337 2023-05-23 02:50:27.000000 tenforce-0.1.0b0/tenforce/enforcer.pyx
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      551 2023-05-23 02:18:21.000000 tenforce-0.1.0b0/tenforce/exceptions.py
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:57:45.709239 tenforce-0.1.0b0/tenforce.egg-info/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      194 2023-05-23 03:57:45.000000 tenforce-0.1.0b0/tenforce.egg-info/PKG-INFO
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      284 2023-05-23 03:57:45.000000 tenforce-0.1.0b0/tenforce.egg-info/SOURCES.txt
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)        1 2023-05-23 03:57:45.000000 tenforce-0.1.0b0/tenforce.egg-info/dependency_links.txt
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)        9 2023-05-23 03:57:45.000000 tenforce-0.1.0b0/tenforce.egg-info/top_level.txt
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 03:57:45.709352 tenforce-0.1.0b0/tests/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     2127 2023-05-23 03:08:35.000000 tenforce-0.1.0b0/tests/test.py
```

### Comparing `tenforce-0.1.0/LICENSE.md` & `tenforce-0.1.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.0/README.md` & `tenforce-0.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.0/tenforce/enforcer.c` & `tenforce-0.1.0b0/tenforce/enforcer.c`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.0/tenforce/enforcer.pyx` & `tenforce-0.1.0b0/tenforce/enforcer.pyx`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.0/tenforce/exceptions.py` & `tenforce-0.1.0b0/tenforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.0/tests/test.py` & `tenforce-0.1.0b0/tests/test.py`

 * *Files identical despite different names*

