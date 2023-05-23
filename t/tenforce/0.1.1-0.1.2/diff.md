# Comparing `tmp/tenforce-0.1.1.tar.gz` & `tmp/tenforce-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenforce-0.1.1.tar", last modified: Tue May 23 04:03:35 2023, max compression
+gzip compressed data, was "tenforce-0.1.2.tar", last modified: Tue May 23 04:14:44 2023, max compression
```

## Comparing `tenforce-0.1.1.tar` & `tenforce-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:03:35.995012 tenforce-0.1.1/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     1071 2023-05-23 03:05:36.000000 tenforce-0.1.1/LICENSE.md
--rw-r--r--   0 hunterlafaille   (501) staff       (20)       29 2023-05-22 15:11:35.000000 tenforce-0.1.1/MANIFEST.in
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      138 2023-05-23 04:03:35.994908 tenforce-0.1.1/PKG-INFO
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     1635 2023-05-23 03:11:36.000000 tenforce-0.1.1/README.md
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      329 2023-05-23 04:01:20.000000 tenforce-0.1.1/pyproject.toml
--rw-r--r--   0 hunterlafaille   (501) staff       (20)       38 2023-05-23 04:03:35.995049 tenforce-0.1.1/setup.cfg
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      153 2023-05-23 04:01:32.000000 tenforce-0.1.1/setup.py
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:03:35.993894 tenforce-0.1.1/tenforce/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)        0 2023-05-21 20:05:52.000000 tenforce-0.1.1/tenforce/__init__.py
--rw-r--r--   0 hunterlafaille   (501) staff       (20)   390946 2023-05-23 04:03:35.000000 tenforce-0.1.1/tenforce/enforcer.c
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     6337 2023-05-23 02:50:27.000000 tenforce-0.1.1/tenforce/enforcer.pyx
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      551 2023-05-23 02:18:21.000000 tenforce-0.1.1/tenforce/exceptions.py
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:03:35.994501 tenforce-0.1.1/tenforce.egg-info/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      138 2023-05-23 04:03:35.000000 tenforce-0.1.1/tenforce.egg-info/PKG-INFO
--rw-r--r--   0 hunterlafaille   (501) staff       (20)      284 2023-05-23 04:03:35.000000 tenforce-0.1.1/tenforce.egg-info/SOURCES.txt
--rw-r--r--   0 hunterlafaille   (501) staff       (20)        1 2023-05-23 04:03:35.000000 tenforce-0.1.1/tenforce.egg-info/dependency_links.txt
--rw-r--r--   0 hunterlafaille   (501) staff       (20)        9 2023-05-23 04:03:35.000000 tenforce-0.1.1/tenforce.egg-info/top_level.txt
-drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:03:35.994619 tenforce-0.1.1/tests/
--rw-r--r--   0 hunterlafaille   (501) staff       (20)     2127 2023-05-23 03:08:35.000000 tenforce-0.1.1/tests/test.py
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:14:44.874593 tenforce-0.1.2/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     1071 2023-05-23 03:05:36.000000 tenforce-0.1.2/LICENSE.md
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)       29 2023-05-22 15:11:35.000000 tenforce-0.1.2/MANIFEST.in
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     3055 2023-05-23 04:14:44.874448 tenforce-0.1.2/PKG-INFO
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     1635 2023-05-23 03:11:36.000000 tenforce-0.1.2/README.md
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      363 2023-05-23 04:14:20.000000 tenforce-0.1.2/pyproject.toml
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)       38 2023-05-23 04:14:44.874636 tenforce-0.1.2/setup.cfg
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      153 2023-05-23 04:01:32.000000 tenforce-0.1.2/setup.py
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:14:44.873464 tenforce-0.1.2/tenforce/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)        0 2023-05-21 20:05:52.000000 tenforce-0.1.2/tenforce/__init__.py
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)   390946 2023-05-23 04:03:35.000000 tenforce-0.1.2/tenforce/enforcer.c
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     6337 2023-05-23 02:50:27.000000 tenforce-0.1.2/tenforce/enforcer.pyx
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      551 2023-05-23 02:18:21.000000 tenforce-0.1.2/tenforce/exceptions.py
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:14:44.874052 tenforce-0.1.2/tenforce.egg-info/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     3055 2023-05-23 04:14:44.000000 tenforce-0.1.2/tenforce.egg-info/PKG-INFO
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)      284 2023-05-23 04:14:44.000000 tenforce-0.1.2/tenforce.egg-info/SOURCES.txt
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)        1 2023-05-23 04:14:44.000000 tenforce-0.1.2/tenforce.egg-info/dependency_links.txt
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)        9 2023-05-23 04:14:44.000000 tenforce-0.1.2/tenforce.egg-info/top_level.txt
+drwxr-xr-x   0 hunterlafaille   (501) staff       (20)        0 2023-05-23 04:14:44.874159 tenforce-0.1.2/tests/
+-rw-r--r--   0 hunterlafaille   (501) staff       (20)     2127 2023-05-23 03:08:35.000000 tenforce-0.1.2/tests/test.py
```

### Comparing `tenforce-0.1.1/LICENSE.md` & `tenforce-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.1/README.md` & `tenforce-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.1/tenforce/enforcer.c` & `tenforce-0.1.2/tenforce/enforcer.c`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.1/tenforce/enforcer.pyx` & `tenforce-0.1.2/tenforce/enforcer.pyx`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.1/tenforce/exceptions.py` & `tenforce-0.1.2/tenforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.1/tests/test.py` & `tenforce-0.1.2/tests/test.py`

 * *Files identical despite different names*

