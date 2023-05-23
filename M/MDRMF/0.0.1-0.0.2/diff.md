# Comparing `tmp/MDRMF-0.0.1.tar.gz` & `tmp/MDRMF-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDRMF-0.0.1.tar", last modified: Thu May 18 06:12:59 2023, max compression
+gzip compressed data, was "MDRMF-0.0.2.tar", last modified: Tue May 23 11:39:05 2023, max compression
```

## Comparing `MDRMF-0.0.1.tar` & `MDRMF-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 06:12:59.446217 MDRMF-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-18 06:12:59.416865 MDRMF-0.0.1/MDRMF/
--rw-rw-rw-   0        0        0      153 2023-05-15 18:57:14.000000 MDRMF-0.0.1/MDRMF/__init__.py
--rw-rw-rw-   0        0        0      920 2023-05-15 18:57:39.000000 MDRMF-0.0.1/MDRMF/dataset.py
--rw-rw-rw-   0        0        0     3808 2023-05-15 19:01:09.000000 MDRMF-0.0.1/MDRMF/featurizer.py
--rw-rw-rw-   0        0        0     2634 2023-05-15 18:57:32.000000 MDRMF-0.0.1/MDRMF/moleculeloader.py
-drwxrwxrwx   0        0        0        0 2023-05-18 06:12:59.444038 MDRMF-0.0.1/MDRMF.egg-info/
--rw-rw-rw-   0        0        0      371 2023-05-18 06:12:59.000000 MDRMF-0.0.1/MDRMF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-18 06:12:59.000000 MDRMF-0.0.1/MDRMF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 06:12:59.000000 MDRMF-0.0.1/MDRMF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 06:12:59.000000 MDRMF-0.0.1/MDRMF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      371 2023-05-18 06:12:59.446060 MDRMF-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 06:12:59.447071 MDRMF-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      537 2023-05-18 06:11:03.000000 MDRMF-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.872810 MDRMF-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.816806 MDRMF-0.0.2/MDRMF/
+-rw-rw-rw-   0        0        0      153 2023-05-23 10:29:57.000000 MDRMF-0.0.2/MDRMF/__init__.py
+-rw-rw-rw-   0        0        0     2702 2023-05-23 10:04:01.000000 MDRMF-0.0.2/MDRMF/dataset.py
+-rw-rw-rw-   0        0        0     3808 2023-05-15 19:01:09.000000 MDRMF-0.0.2/MDRMF/featurizer.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.866810 MDRMF-0.0.2/MDRMF/models/
+-rw-rw-rw-   0        0        0       86 2023-05-23 10:56:06.000000 MDRMF-0.0.2/MDRMF/models/__init__.py
+-rw-rw-rw-   0        0        0     1736 2023-05-23 11:07:29.000000 MDRMF-0.0.2/MDRMF/models/modeller.py
+-rw-rw-rw-   0        0        0     1847 2023-05-23 11:12:03.000000 MDRMF-0.0.2/MDRMF/models/rfmodeller.py
+-rw-rw-rw-   0        0        0     2634 2023-05-15 18:57:32.000000 MDRMF-0.0.2/MDRMF/moleculeloader.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.860949 MDRMF-0.0.2/MDRMF.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      436 2023-05-23 11:39:05.871812 MDRMF-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 11:39:05.873810 MDRMF-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-05-23 11:37:14.000000 MDRMF-0.0.2/setup.py
```

### Comparing `MDRMF-0.0.1/MDRMF/featurizer.py` & `MDRMF-0.0.2/MDRMF/featurizer.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.1/MDRMF/moleculeloader.py` & `MDRMF-0.0.2/MDRMF/moleculeloader.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.1/setup.py` & `MDRMF-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='MDRMF',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     description='Multidrug Resistance Machine Fishing',
     author='Jacob Molin Nielsen',
-    author_email='xsj110@sund.ku.dk',
+    author_email='jacob.molin@me.com',
     url='https://github.com/MolinDiscovery/MDRMF',  # use the URL to the github repo
-    download_url='https://github.com/MolinDiscovery/MDRMF/archive/0.1.tar.gz',  # I'll explain this in a second
-    keywords=['some', 'keywords'],  # arbitrary keywords
+    download_url='https://github.com/MolinDiscovery/MDRMF/archive/v0.0.2.tar.gz',  # I'll explain this in a second
+    keywords=['machine fishing', 'drug discovery', 'machine learning', 'pool based active learning'],  # arbitrary keywords
     classifiers=[],
 )
```

