# Comparing `tmp/at-fetch-data-1.0.0.tar.gz` & `tmp/at-fetch-data-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "at-fetch-data-1.0.0.tar", last modified: Tue May 23 12:48:09 2023, max compression
+gzip compressed data, was "at-fetch-data-1.0.1.tar", last modified: Tue May 23 12:55:38 2023, max compression
```

## Comparing `at-fetch-data-1.0.0.tar` & `at-fetch-data-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:48:09.941046 at-fetch-data-1.0.0/
--rw-r--r--   0 ctw        (501) staff       (20)      129 2023-05-23 12:48:09.940629 at-fetch-data-1.0.0/PKG-INFO
--rw-r--r--   0 ctw        (501) staff       (20)      742 2023-05-23 12:38:22.000000 at-fetch-data-1.0.0/README.md
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:48:09.939491 at-fetch-data-1.0.0/at_fetch_data.egg-info/
--rw-r--r--   0 ctw        (501) staff       (20)      129 2023-05-23 12:48:09.000000 at-fetch-data-1.0.0/at_fetch_data.egg-info/PKG-INFO
--rw-r--r--   0 ctw        (501) staff       (20)      250 2023-05-23 12:48:09.000000 at-fetch-data-1.0.0/at_fetch_data.egg-info/SOURCES.txt
--rw-r--r--   0 ctw        (501) staff       (20)        1 2023-05-23 12:48:09.000000 at-fetch-data-1.0.0/at_fetch_data.egg-info/dependency_links.txt
--rw-r--r--   0 ctw        (501) staff       (20)       40 2023-05-23 12:48:09.000000 at-fetch-data-1.0.0/at_fetch_data.egg-info/requires.txt
--rw-r--r--   0 ctw        (501) staff       (20)        6 2023-05-23 12:48:09.000000 at-fetch-data-1.0.0/at_fetch_data.egg-info/top_level.txt
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:48:09.940276 at-fetch-data-1.0.0/fetch/
--rw-r--r--   0 ctw        (501) staff       (20)        0 2023-05-23 12:37:49.000000 at-fetch-data-1.0.0/fetch/__init__.py
--rw-r--r--   0 ctw        (501) staff       (20)      367 2023-05-23 12:37:49.000000 at-fetch-data-1.0.0/fetch/const.py
--rw-r--r--   0 ctw        (501) staff       (20)     2911 2023-05-23 12:42:48.000000 at-fetch-data-1.0.0/fetch/fetch.py
--rw-r--r--   0 ctw        (501) staff       (20)       38 2023-05-23 12:48:09.941130 at-fetch-data-1.0.0/setup.cfg
--rw-r--r--   0 ctw        (501) staff       (20)      302 2023-05-23 12:48:06.000000 at-fetch-data-1.0.0/setup.py
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:55:38.268777 at-fetch-data-1.0.1/
+-rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-23 12:55:38.268597 at-fetch-data-1.0.1/PKG-INFO
+-rw-r--r--   0 ctw        (501) staff       (20)      742 2023-05-23 12:38:22.000000 at-fetch-data-1.0.1/README.md
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:55:38.267423 at-fetch-data-1.0.1/at_fetch_data.egg-info/
+-rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-23 12:55:37.000000 at-fetch-data-1.0.1/at_fetch_data.egg-info/PKG-INFO
+-rw-r--r--   0 ctw        (501) staff       (20)      250 2023-05-23 12:55:38.000000 at-fetch-data-1.0.1/at_fetch_data.egg-info/SOURCES.txt
+-rw-r--r--   0 ctw        (501) staff       (20)        1 2023-05-23 12:55:38.000000 at-fetch-data-1.0.1/at_fetch_data.egg-info/dependency_links.txt
+-rw-r--r--   0 ctw        (501) staff       (20)       40 2023-05-23 12:55:38.000000 at-fetch-data-1.0.1/at_fetch_data.egg-info/requires.txt
+-rw-r--r--   0 ctw        (501) staff       (20)        6 2023-05-23 12:55:38.000000 at-fetch-data-1.0.1/at_fetch_data.egg-info/top_level.txt
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:55:38.268118 at-fetch-data-1.0.1/fetch/
+-rw-r--r--   0 ctw        (501) staff       (20)        0 2023-05-23 12:37:49.000000 at-fetch-data-1.0.1/fetch/__init__.py
+-rw-r--r--   0 ctw        (501) staff       (20)      367 2023-05-23 12:37:49.000000 at-fetch-data-1.0.1/fetch/const.py
+-rw-r--r--   0 ctw        (501) staff       (20)     2911 2023-05-23 12:42:48.000000 at-fetch-data-1.0.1/fetch/fetch.py
+-rw-r--r--   0 ctw        (501) staff       (20)       38 2023-05-23 12:55:38.268848 at-fetch-data-1.0.1/setup.cfg
+-rw-r--r--   0 ctw        (501) staff       (20)      477 2023-05-23 12:55:26.000000 at-fetch-data-1.0.1/setup.py
```

### Comparing `at-fetch-data-1.0.0/README.md` & `at-fetch-data-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `at-fetch-data-1.0.0/fetch/fetch.py` & `at-fetch-data-1.0.1/fetch/fetch.py`

 * *Files identical despite different names*

