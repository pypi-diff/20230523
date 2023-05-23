# Comparing `tmp/dbtgenlib-0.0.8.tar.gz` & `tmp/dbtgenlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbtgenlib-0.0.8.tar", last modified: Sun May 21 22:40:48 2023, max compression
+gzip compressed data, was "dist/dbtgenlib-0.0.9.tar", last modified: Mon May 22 14:56:23 2023, max compression
```

## Comparing `dbtgenlib-0.0.8.tar` & `dbtgenlib-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      183 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       12 2023-05-21 22:08:14.000000 dbtgenlib-0.0.8/README.md
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      281 2023-05-21 22:40:45.000000 dbtgenlib-0.0.8/setup.py
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/setup.cfg
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib.egg-info/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      183 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib.egg-info/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      261 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib.egg-info/SOURCES.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       84 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib.egg-info/entry_points.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib.egg-info/requires.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       10 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib.egg-info/top_level.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib.egg-info/dependency_links.txt
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-21 22:40:48.000000 dbtgenlib-0.0.8/dbtgenlib/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 14:43:00.000000 dbtgenlib-0.0.8/dbtgenlib/__init__.py
--rw-r--r--   0 patrykpacholek   (501) staff       (20)     1700 2023-05-21 22:07:27.000000 dbtgenlib-0.0.8/dbtgenlib/yml_gen.py
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      183 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       12 2023-05-21 22:08:14.000000 dbtgenlib-0.0.9/README.md
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      278 2023-05-22 14:56:21.000000 dbtgenlib-0.0.9/setup.py
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/setup.cfg
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib.egg-info/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      183 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib.egg-info/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      261 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib.egg-info/SOURCES.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       81 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib.egg-info/entry_points.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib.egg-info/requires.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       10 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib.egg-info/top_level.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib.egg-info/dependency_links.txt
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-22 14:56:23.000000 dbtgenlib-0.0.9/dbtgenlib/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 14:43:00.000000 dbtgenlib-0.0.9/dbtgenlib/__init__.py
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)     1700 2023-05-21 22:07:27.000000 dbtgenlib-0.0.9/dbtgenlib/yml_gen.py
```

### Comparing `dbtgenlib-0.0.8/dbtgenlib/yml_gen.py` & `dbtgenlib-0.0.9/dbtgenlib/yml_gen.py`

 * *Files identical despite different names*

