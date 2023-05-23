# Comparing `tmp/mozilla-version-2.0.0.tar.gz` & `tmp/mozilla-version-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-version-2.0.0.tar", last modified: Thu Apr 20 11:56:40 2023, max compression
+gzip compressed data, was "mozilla-version-2.1.0.tar", last modified: Tue May 23 08:17:29 2023, max compression
```

## Comparing `mozilla-version-2.0.0.tar` & `mozilla-version-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15922 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/LICENSE
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      139 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/MANIFEST.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      451 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7491 2023-04-11 13:53:15.000000 mozilla-version-2.0.0/README.md
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.921603 mozilla-version-2.0.0/mozilla_version/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       60 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4961 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/balrog.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2468 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/errors.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      199 2022-08-25 14:26:48.000000 mozilla-version-2.0.0/mozilla_version/fenix.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    24783 2023-04-20 11:46:42.000000 mozilla-version-2.0.0/mozilla_version/gecko.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1988 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/maven.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9520 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/mobile.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1335 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/parser.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/mozilla_version/test/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       87 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7839 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/test_balrog.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      933 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/test_errors.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      193 2022-08-25 14:26:48.000000 mozilla-version-2.0.0/mozilla_version/test/test_fenix.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    24494 2023-04-20 11:46:42.000000 mozilla-version-2.0.0/mozilla_version/test/test_gecko.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3526 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/test/test_maven.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11948 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/test/test_mobile.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7441 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/test_version.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7929 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/version.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.921603 mozilla-version-2.0.0/mozilla_version.egg-info/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      451 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      928 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/SOURCES.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/dependency_links.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-04-11 14:24:42.000000 mozilla-version-2.0.0/mozilla_version.egg-info/not-zip-safe
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       12 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/requires.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       16 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/top_level.txt
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/requirements/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       12 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/base.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      363 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/base.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       70 2022-08-25 14:26:48.000000 mozilla-version-2.0.0/requirements/docs.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15614 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/docs.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      143 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/test.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8589 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/test.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       38 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/setup.cfg
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1194 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/setup.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        6 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/version.txt
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.100549 mozilla-version-2.1.0/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    15922 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/LICENSE
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      139 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/MANIFEST.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2023-05-23 08:17:29.100439 mozilla-version-2.1.0/PKG-INFO
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7491 2022-11-25 16:16:39.000000 mozilla-version-2.1.0/README.md
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.098031 mozilla-version-2.1.0/mozilla_version/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      262 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/__init__.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     4961 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/balrog.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     2468 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/errors.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      199 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/fenix.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    24783 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/gecko.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1988 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/maven.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     9520 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/mobile.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1335 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/parser.py
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.099702 mozilla-version-2.1.0/mozilla_version/test/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       87 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/__init__.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7839 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/test_balrog.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      268 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_default_imports.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      933 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/test_errors.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      193 2022-07-07 15:15:03.000000 mozilla-version-2.1.0/mozilla_version/test/test_fenix.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    24494 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_gecko.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     3526 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_maven.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    11948 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/test/test_mobile.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7441 2022-06-29 08:41:37.000000 mozilla-version-2.1.0/mozilla_version/test/test_version.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7929 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/mozilla_version/version.py
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.098649 mozilla-version-2.1.0/mozilla_version.egg-info/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2023-05-23 08:17:28.000000 mozilla-version-2.1.0/mozilla_version.egg-info/PKG-INFO
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      973 2023-05-23 08:17:29.000000 mozilla-version-2.1.0/mozilla_version.egg-info/SOURCES.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2023-05-23 08:17:28.000000 mozilla-version-2.1.0/mozilla_version.egg-info/dependency_links.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2022-11-25 13:12:40.000000 mozilla-version-2.1.0/mozilla_version.egg-info/not-zip-safe
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2023-05-23 08:17:29.000000 mozilla-version-2.1.0/mozilla_version.egg-info/requires.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       16 2023-05-23 08:17:29.000000 mozilla-version-2.1.0/mozilla_version.egg-info/top_level.txt
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2023-05-23 08:17:29.100285 mozilla-version-2.1.0/requirements/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/base.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      363 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/base.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       70 2022-11-25 14:28:49.000000 mozilla-version-2.1.0/requirements/docs.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    15614 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/docs.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      143 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/test.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     8589 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/requirements/test.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       38 2023-05-23 08:17:29.100584 mozilla-version-2.1.0/setup.cfg
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1194 2023-05-23 08:14:29.000000 mozilla-version-2.1.0/setup.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        6 2023-05-23 08:16:04.000000 mozilla-version-2.1.0/version.txt
```

### Comparing `mozilla-version-2.0.0/LICENSE` & `mozilla-version-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/README.md` & `mozilla-version-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/balrog.py` & `mozilla-version-2.1.0/mozilla_version/balrog.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/errors.py` & `mozilla-version-2.1.0/mozilla_version/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/gecko.py` & `mozilla-version-2.1.0/mozilla_version/gecko.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/maven.py` & `mozilla-version-2.1.0/mozilla_version/maven.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/mobile.py` & `mozilla-version-2.1.0/mozilla_version/mobile.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/parser.py` & `mozilla-version-2.1.0/mozilla_version/parser.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/test/test_balrog.py` & `mozilla-version-2.1.0/mozilla_version/test/test_balrog.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/test/test_errors.py` & `mozilla-version-2.1.0/mozilla_version/test/test_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/test/test_gecko.py` & `mozilla-version-2.1.0/mozilla_version/test/test_gecko.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/test/test_maven.py` & `mozilla-version-2.1.0/mozilla_version/test/test_maven.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/test/test_mobile.py` & `mozilla-version-2.1.0/mozilla_version/test/test_mobile.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/test/test_version.py` & `mozilla-version-2.1.0/mozilla_version/test/test_version.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version/version.py` & `mozilla-version-2.1.0/mozilla_version/version.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/mozilla_version.egg-info/SOURCES.txt` & `mozilla-version-2.1.0/mozilla_version.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 mozilla_version.egg-info/SOURCES.txt
 mozilla_version.egg-info/dependency_links.txt
 mozilla_version.egg-info/not-zip-safe
 mozilla_version.egg-info/requires.txt
 mozilla_version.egg-info/top_level.txt
 mozilla_version/test/__init__.py
 mozilla_version/test/test_balrog.py
+mozilla_version/test/test_default_imports.py
 mozilla_version/test/test_errors.py
 mozilla_version/test/test_fenix.py
 mozilla_version/test/test_gecko.py
 mozilla_version/test/test_maven.py
 mozilla_version/test/test_mobile.py
 mozilla_version/test/test_version.py
 requirements/base.in
```

### Comparing `mozilla-version-2.0.0/requirements/docs.txt` & `mozilla-version-2.1.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/requirements/test.txt` & `mozilla-version-2.1.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.0.0/setup.py` & `mozilla-version-2.1.0/setup.py`

 * *Files identical despite different names*

