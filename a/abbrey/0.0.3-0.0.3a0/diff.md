# Comparing `tmp/abbrey-0.0.3.tar.gz` & `tmp/abbrey-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abbrey-0.0.3.tar", last modified: Tue May 23 04:38:41 2023, max compression
+gzip compressed data, was "abbrey-0.0.3a0.tar", last modified: Tue May 23 05:03:43 2023, max compression
```

## Comparing `abbrey-0.0.3.tar` & `abbrey-0.0.3a0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:38:41.598154 abbrey-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-23 04:38:29.000000 abbrey-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:38:41.598154 abbrey-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 04:38:29.000000 abbrey-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:38:41.598154 abbrey-0.0.3/abbrey/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 04:38:29.000000 abbrey-0.0.3/abbrey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62788 2023-05-23 04:38:29.000000 abbrey-0.0.3/abbrey/acronyms_ver0.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-23 04:38:29.000000 abbrey-0.0.3/abbrey/decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:38:41.598154 abbrey-0.0.3/abbrey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 04:38:41.598154 abbrey-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 04:38:29.000000 abbrey-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:03:43.168438 abbrey-0.0.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-23 05:03:33.000000 abbrey-0.0.3a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-23 05:03:43.168438 abbrey-0.0.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 05:03:33.000000 abbrey-0.0.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:03:43.168438 abbrey-0.0.3a0/abbrey/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 05:03:33.000000 abbrey-0.0.3a0/abbrey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-23 05:03:33.000000 abbrey-0.0.3a0/abbrey/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:03:43.168438 abbrey-0.0.3a0/abbrey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-23 05:03:43.000000 abbrey-0.0.3a0/abbrey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 05:03:43.000000 abbrey-0.0.3a0/abbrey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 05:03:43.000000 abbrey-0.0.3a0/abbrey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 05:03:43.000000 abbrey-0.0.3a0/abbrey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 05:03:43.000000 abbrey-0.0.3a0/abbrey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 05:03:43.168438 abbrey-0.0.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-23 05:03:33.000000 abbrey-0.0.3a0/setup.py
```

### Comparing `abbrey-0.0.3/LICENSE.txt` & `abbrey-0.0.3a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abbrey-0.0.3/abbrey/decoder.py` & `abbrey-0.0.3a0/abbrey/decoder.py`

 * *Files identical despite different names*

