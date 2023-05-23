# Comparing `tmp/tKot-0.2.1.tar.gz` & `tmp/tKot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tKot-0.2.1.tar", last modified: Wed May  3 11:35:39 2023, max compression
+gzip compressed data, was "tKot-0.3.0.tar", last modified: Tue May 23 06:07:24 2023, max compression
```

## Comparing `tKot-0.2.1.tar` & `tKot-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:35:39.951607 tKot-0.2.1/
--rw-rw-rw-   0        0        0      483 2023-05-03 11:35:39.950608 tKot-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.2.1/README.md
--rw-rw-rw-   0        0        0      602 2023-05-03 11:35:24.000000 tKot-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 11:35:39.951607 tKot-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:35:39.888307 tKot-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:35:39.899308 tKot-0.2.1/src/tKot/
--rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.2.1/src/tKot/__init__.py
--rw-rw-rw-   0        0        0      874 2023-05-03 11:18:28.000000 tKot-0.2.1/src/tKot/buttons.py
--rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.2.1/src/tKot/frames.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:35:39.947608 tKot-0.2.1/src/tKot.egg-info/
--rw-rw-rw-   0        0        0      483 2023-05-03 11:35:39.000000 tKot-0.2.1/src/tKot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-03 11:35:39.000000 tKot-0.2.1/src/tKot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:35:39.000000 tKot-0.2.1/src/tKot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 11:35:39.000000 tKot-0.2.1/src/tKot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 11:35:39.000000 tKot-0.2.1/src/tKot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.749444 tKot-0.3.0/
+-rw-rw-rw-   0        0        0      483 2023-05-23 06:07:24.748443 tKot-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.3.0/README.md
+-rw-rw-rw-   0        0        0      602 2023-05-23 06:00:55.000000 tKot-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 06:07:24.749444 tKot-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.724443 tKot-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.735463 tKot-0.3.0/src/tKot/
+-rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.3.0/src/tKot/__init__.py
+-rw-rw-rw-   0        0        0     2487 2023-05-23 06:06:44.000000 tKot-0.3.0/src/tKot/buttons.py
+-rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.3.0/src/tKot/frames.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.746443 tKot-0.3.0/src/tKot.egg-info/
+-rw-rw-rw-   0        0        0      483 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/top_level.txt
```

### Comparing `tKot-0.2.1/pyproject.toml` & `tKot-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backed = "setuptools.build_meta"
 
 [project]
 name = "tKot"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tKot-0.2.1/src/tKot/frames.py` & `tKot-0.3.0/src/tKot/frames.py`

 * *Files identical despite different names*

