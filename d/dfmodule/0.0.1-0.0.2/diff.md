# Comparing `tmp/dfmodule-0.0.1.tar.gz` & `tmp/dfmodule-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule-0.0.1.tar", last modified: Tue May 23 02:49:51 2023, max compression
+gzip compressed data, was "dfmodule-0.0.2.tar", last modified: Tue May 23 04:57:35 2023, max compression
```

## Comparing `dfmodule-0.0.1.tar` & `dfmodule-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 02:49:51.562770 dfmodule-0.0.1/
--rw-rw-rw-   0        0        0      426 2023-05-23 02:49:51.562770 dfmodule-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-05-23 02:43:44.000000 dfmodule-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 02:49:51.546767 dfmodule-0.0.1/common/
--rw-rw-rw-   0        0        0       21 2023-05-23 02:38:36.000000 dfmodule-0.0.1/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 02:49:51.561765 dfmodule-0.0.1/dfmodule.egg-info/
--rw-rw-rw-   0        0        0      426 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-23 02:49:51.000000 dfmodule-0.0.1/dfmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 02:49:51.563766 dfmodule-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      643 2023-05-23 02:36:00.000000 dfmodule-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:57:35.279952 dfmodule-0.0.2/
+-rw-rw-rw-   0        0        0      478 2023-05-23 04:57:35.279952 dfmodule-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2023-05-23 03:07:30.000000 dfmodule-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 04:57:35.269952 dfmodule-0.0.2/common/
+-rw-rw-rw-   0        0        0       96 2023-05-23 04:57:29.000000 dfmodule-0.0.2/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:57:35.278952 dfmodule-0.0.2/dfmodule.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 02:49:51.000000 dfmodule-0.0.2/dfmodule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-23 04:57:35.000000 dfmodule-0.0.2/dfmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 04:57:35.279952 dfmodule-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-05-23 04:57:17.000000 dfmodule-0.0.2/setup.py
```

### Comparing `dfmodule-0.0.1/setup.py` & `dfmodule-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfmodule',
-    version='0.0.1',
+    version='0.0.2',
     description='PYPI tutorial package by howardHamm',
     author='rimmoyee',
     author_email='rimmoyee@gmail.com',
     url='',
     install_requires=[],
     packages=find_packages(exclude=[]),
     keywords=['dfmodule', 'dfmodule777'],
@@ -14,9 +14,10 @@
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

