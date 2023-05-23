# Comparing `tmp/dfmodule-0.0.2.tar.gz` & `tmp/dfmodule-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.2.tar", last modified: Tue May 23 04:57:35 2023, max compression
+gzip compressed data, was "dfmodule-0.0.3.tar", last modified: Tue May 23 08:38:56 2023, max compression
```

## Comparing `dfmodule-0.0.2.tar` & `dfmodule-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 04:57:35.279952 dfmodule-0.0.2/
--rw-rw-rw-   0        0        0      478 2023-05-23 04:57:35.279952 dfmodule-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-05-23 03:07:30.000000 dfmodule-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 04:57:35.269952 dfmodule-0.0.2/common/
--rw-rw-rw-   0        0        0       96 2023-05-23 04:57:29.000000 dfmodule-0.0.2/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 04:57:35.278952 dfmodule-0.0.2/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      478 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 04:57:35.279952 dfmodule-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-05-23 04:57:17.000000 dfmodule-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:38:56.877254 dfmodule-0.0.3/
+-rw-rw-rw-   0        0        0      478 2023-05-23 08:38:56.876253 dfmodule-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1401 2023-05-23 08:36:52.000000 dfmodule-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 08:38:56.861254 dfmodule-0.0.3/common/
+-rw-rw-rw-   0        0        0      149 2023-05-23 08:36:49.000000 dfmodule-0.0.3/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:38:56.875256 dfmodule-0.0.3/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-05-23 08:38:56.000000 dfmodule-0.0.3/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-23 08:38:56.000000 dfmodule-0.0.3/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:38:56.000000 dfmodule-0.0.3/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.3/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-23 08:38:56.000000 dfmodule-0.0.3/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:38:56.877254 dfmodule-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-05-23 08:38:34.000000 dfmodule-0.0.3/setup.py
```

### Comparing `dfmodule-0.0.2/setup.py` & `dfmodule-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.2',
+    version='0.0.3',
     description='PYPI tutorial package by howardHamm',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
     install_requires=[],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
```

