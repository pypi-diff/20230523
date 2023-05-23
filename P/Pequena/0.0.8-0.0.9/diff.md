# Comparing `tmp/Pequena-0.0.8.tar.gz` & `tmp/Pequena-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pequena-0.0.8.tar", last modified: Sun Mar 19 18:01:05 2023, max compression
+gzip compressed data, was "Pequena-0.0.9.tar", last modified: Sun Mar 19 18:12:57 2023, max compression
```

## Comparing `Pequena-0.0.8.tar` & `Pequena-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 18:01:05.701153 Pequena-0.0.8/
--rw-rw-rw-   0        0        0      733 2023-03-19 18:01:05.700156 Pequena-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-19 18:01:05.676220 Pequena-0.0.8/Pequena/
--rw-rw-rw-   0        0        0      119 2023-03-16 16:00:16.000000 Pequena-0.0.8/Pequena/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-12 10:14:57.000000 Pequena-0.0.8/Pequena/compile.py
--rw-rw-rw-   0        0        0     4758 2023-03-19 18:00:25.000000 Pequena-0.0.8/Pequena/window.py
-drwxrwxrwx   0        0        0        0 2023-03-19 18:01:05.699159 Pequena-0.0.8/Pequena.egg-info/
--rw-rw-rw-   0        0        0      733 2023-03-19 18:01:05.000000 Pequena-0.0.8/Pequena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-03-19 18:01:05.000000 Pequena-0.0.8/Pequena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 18:01:05.000000 Pequena-0.0.8/Pequena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-19 18:01:05.000000 Pequena-0.0.8/Pequena.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-19 18:01:05.000000 Pequena-0.0.8/Pequena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-19 18:01:05.701153 Pequena-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-03-19 18:00:54.000000 Pequena-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-19 18:12:57.590094 Pequena-0.0.9/
+-rw-rw-rw-   0        0        0      733 2023-03-19 18:12:57.590094 Pequena-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-03-19 18:12:57.575134 Pequena-0.0.9/Pequena/
+-rw-rw-rw-   0        0        0      119 2023-03-16 16:00:16.000000 Pequena-0.0.9/Pequena/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-12 10:14:57.000000 Pequena-0.0.9/Pequena/compile.py
+-rw-rw-rw-   0        0        0     4758 2023-03-19 18:00:25.000000 Pequena-0.0.9/Pequena/window.py
+drwxrwxrwx   0        0        0        0 2023-03-19 18:12:57.589096 Pequena-0.0.9/Pequena.egg-info/
+-rw-rw-rw-   0        0        0      733 2023-03-19 18:12:57.000000 Pequena-0.0.9/Pequena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-03-19 18:12:57.000000 Pequena-0.0.9/Pequena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-19 18:12:57.000000 Pequena-0.0.9/Pequena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-03-19 18:12:57.000000 Pequena-0.0.9/Pequena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-03-19 18:12:57.000000 Pequena-0.0.9/Pequena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-19 18:12:57.591091 Pequena-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-03-19 18:12:55.000000 Pequena-0.0.9/setup.py
```

### Comparing `Pequena-0.0.8/PKG-INFO` & `Pequena-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pequena
-Version: 0.0.8
+Version: 0.0.9
 Summary: Lightweight desktop app framework
 Author: borecjeborec1
 Author-email: <atzuki@protonmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pequena-0.0.8/Pequena/window.py` & `Pequena-0.0.9/Pequena/window.py`

 * *Files identical despite different names*

### Comparing `Pequena-0.0.8/Pequena.egg-info/PKG-INFO` & `Pequena-0.0.9/Pequena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pequena
-Version: 0.0.8
+Version: 0.0.9
 Summary: Lightweight desktop app framework
 Author: borecjeborec1
 Author-email: <atzuki@protonmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pequena-0.0.8/setup.py` & `Pequena-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = "0.0.9"
 DESCRIPTION = 'Lightweight desktop app framework'
 with open("Readme.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name="Pequena",
     version=VERSION,
```

