# Comparing `tmp/sql2dataframe-0.0.0.tar.gz` & `tmp/sql2dataframe-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql2dataframe-0.0.0.tar", last modified: Tue May 23 02:10:04 2023, max compression
+gzip compressed data, was "sql2dataframe-0.1.tar", last modified: Tue May 23 01:58:59 2023, max compression
```

## Comparing `sql2dataframe-0.0.0.tar` & `sql2dataframe-0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 02:10:04.084723 sql2dataframe-0.0.0/
--rw-rw-rw-   0        0        0      380 2023-05-23 02:10:04.083722 sql2dataframe-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1209 2023-05-23 01:28:33.000000 sql2dataframe-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 02:10:04.065926 sql2dataframe-0.0.0/my_package_name/
--rw-rw-rw-   0        0        0        0 2023-05-23 02:09:26.000000 sql2dataframe-0.0.0/my_package_name/__init__.py
--rw-rw-rw-   0        0        0     2177 2023-05-23 02:09:26.000000 sql2dataframe-0.0.0/my_package_name/__main__.py
--rw-rw-rw-   0        0        0       42 2023-05-23 02:10:04.084723 sql2dataframe-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-05-23 02:10:01.000000 sql2dataframe-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 02:10:04.081723 sql2dataframe-0.0.0/sql2dataframe.egg-info/
--rw-rw-rw-   0        0        0      380 2023-05-23 02:10:03.000000 sql2dataframe-0.0.0/sql2dataframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-05-23 02:10:03.000000 sql2dataframe-0.0.0/sql2dataframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 02:10:03.000000 sql2dataframe-0.0.0/sql2dataframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-23 02:10:03.000000 sql2dataframe-0.0.0/sql2dataframe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-05-23 02:10:03.000000 sql2dataframe-0.0.0/sql2dataframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-23 02:10:03.000000 sql2dataframe-0.0.0/sql2dataframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 01:58:59.365571 sql2dataframe-0.1/
+-rw-rw-rw-   0        0        0      378 2023-05-23 01:58:59.364556 sql2dataframe-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1209 2023-05-23 01:28:33.000000 sql2dataframe-0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 01:58:59.337136 sql2dataframe-0.1/my_package_name/
+-rw-rw-rw-   0        0        0     2177 2023-05-23 01:47:09.000000 sql2dataframe-0.1/my_package_name/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 01:29:24.000000 sql2dataframe-0.1/my_package_name/__main__.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 01:58:59.365571 sql2dataframe-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-05-23 01:58:56.000000 sql2dataframe-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 01:58:59.363558 sql2dataframe-0.1/sql2dataframe.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-23 01:58:58.000000 sql2dataframe-0.1/sql2dataframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-05-23 01:58:58.000000 sql2dataframe-0.1/sql2dataframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 01:58:58.000000 sql2dataframe-0.1/sql2dataframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-23 01:58:58.000000 sql2dataframe-0.1/sql2dataframe.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-05-23 01:58:58.000000 sql2dataframe-0.1/sql2dataframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 01:58:58.000000 sql2dataframe-0.1/sql2dataframe.egg-info/top_level.txt
```

### Comparing `sql2dataframe-0.0.0/README.md` & `sql2dataframe-0.1/README.md`

 * *Files identical despite different names*

### Comparing `sql2dataframe-0.0.0/my_package_name/__main__.py` & `sql2dataframe-0.1/my_package_name/__init__.py`

 * *Files identical despite different names*

### Comparing `sql2dataframe-0.0.0/setup.py` & `sql2dataframe-0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sql2dataframe',
-    version='',
+    version='0.1',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'sqlalchemy'
     ],
     entry_points={
         'console_scripts': [
```

