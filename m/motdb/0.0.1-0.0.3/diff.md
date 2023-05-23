# Comparing `tmp/motdb-0.0.1.tar.gz` & `tmp/motdb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motdb-0.0.1.tar", last modified: Tue May 23 18:38:23 2023, max compression
+gzip compressed data, was "motdb-0.0.3.tar", last modified: Tue May 23 19:24:43 2023, max compression
```

## Comparing `motdb-0.0.1.tar` & `motdb-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 18:38:23.612081 motdb-0.0.1/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-18 14:54:10.000000 motdb-0.0.1/LICENSE
--rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-23 15:03:31.000000 motdb-0.0.1/MANIFEST.in
--rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-23 18:38:23.611955 motdb-0.0.1/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)       53 2023-05-23 15:39:33.000000 motdb-0.0.1/README.md
--rw-r--r--   0 mfsteele   (502) staff       (20)     1165 2023-05-23 18:32:56.000000 motdb-0.0.1/pyproject.toml
--rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-23 18:38:23.612131 motdb-0.0.1/setup.cfg
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 18:38:23.609982 motdb-0.0.1/src/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 18:38:23.610992 motdb-0.0.1/src/motdb/
--rw-r--r--   0 mfsteele   (502) staff       (20)       25 2023-05-23 18:32:56.000000 motdb-0.0.1/src/motdb/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)       89 2023-05-23 18:08:52.000000 motdb-0.0.1/src/motdb/__main__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-23 18:10:33.000000 motdb-0.0.1/src/motdb/dbx.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 18:38:23.611732 motdb-0.0.1/src/motdb.egg-info/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-23 18:38:23.000000 motdb-0.0.1/src/motdb.egg-info/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)      305 2023-05-23 18:38:23.000000 motdb-0.0.1/src/motdb.egg-info/SOURCES.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-23 18:38:23.000000 motdb-0.0.1/src/motdb.egg-info/dependency_links.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       46 2023-05-23 18:38:23.000000 motdb-0.0.1/src/motdb.egg-info/entry_points.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       81 2023-05-23 18:38:23.000000 motdb-0.0.1/src/motdb.egg-info/requires.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        6 2023-05-23 18:38:23.000000 motdb-0.0.1/src/motdb.egg-info/top_level.txt
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 19:24:43.278078 motdb-0.0.3/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-18 14:54:10.000000 motdb-0.0.3/LICENSE
+-rw-r--r--   0 mfsteele   (502) staff       (20)       81 2023-05-23 19:19:31.000000 motdb-0.0.3/MANIFEST.in
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-23 19:24:43.277939 motdb-0.0.3/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)       53 2023-05-23 15:39:33.000000 motdb-0.0.3/README.md
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-23 19:23:41.000000 motdb-0.0.3/pyproject.toml
+-rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-23 19:24:43.278117 motdb-0.0.3/setup.cfg
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 19:24:43.270175 motdb-0.0.3/src/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 19:24:43.271554 motdb-0.0.3/src/motdb/
+-rw-r--r--   0 mfsteele   (502) staff       (20)       25 2023-05-23 19:23:41.000000 motdb-0.0.3/src/motdb/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)       89 2023-05-23 18:08:52.000000 motdb-0.0.3/src/motdb/__main__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-23 18:10:33.000000 motdb-0.0.3/src/motdb/dbx.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 19:24:43.270374 motdb-0.0.3/src/motdb/inc/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 19:24:43.272601 motdb-0.0.3/src/motdb/inc/json/
+-rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 motdb-0.0.3/src/motdb/inc/json/dict_tracy.json
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 19:24:43.274726 motdb-0.0.3/src/motdb/inc/whls/
+-rw-r--r--   0 mfsteele   (502) staff       (20)   700282 2023-05-23 16:39:38.000000 motdb-0.0.3/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-23 19:24:43.272475 motdb-0.0.3/src/motdb.egg-info/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-23 19:24:43.000000 motdb-0.0.3/src/motdb.egg-info/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)      409 2023-05-23 19:24:43.000000 motdb-0.0.3/src/motdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-23 19:24:43.000000 motdb-0.0.3/src/motdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       46 2023-05-23 19:24:43.000000 motdb-0.0.3/src/motdb.egg-info/entry_points.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-23 19:24:43.000000 motdb-0.0.3/src/motdb.egg-info/requires.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        6 2023-05-23 19:24:43.000000 motdb-0.0.3/src/motdb.egg-info/top_level.txt
```

### Comparing `motdb-0.0.1/LICENSE` & `motdb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `motdb-0.0.1/PKG-INFO` & `motdb-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motdb
-Version: 0.0.1
+Version: 0.0.3
 Summary: Một Database Layer to ... Bind Them (All)
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `motdb-0.0.1/pyproject.toml` & `motdb-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motdb"
-version = "0.0.1"
+version = "0.0.3"
 description = "Một Database Layer to ... Bind Them (All)"
 readme = "README.md"
 authors = [{ name = "Mike Steele", email = "mike@mikesteele.us" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["database", "fetch", "db"]
 dependencies = [
-    'pysqlite3 >= 0.5.0',
     'tomli >= 2.0.1',
     'click >= 8.1.3'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["bumpver", "isort", "pip-tools", "pytest"]
@@ -30,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/soulrx/motdb"
 
 [project.scripts]
 motdb = "motdb.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `motdb-0.0.1/src/motdb.egg-info/PKG-INFO` & `motdb-0.0.3/src/motdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motdb
-Version: 0.0.1
+Version: 0.0.3
 Summary: Một Database Layer to ... Bind Them (All)
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

