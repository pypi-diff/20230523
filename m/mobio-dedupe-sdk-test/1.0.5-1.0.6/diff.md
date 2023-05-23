# Comparing `tmp/mobio-dedupe-sdk-test-1.0.5.tar.gz` & `tmp/mobio-dedupe-sdk-test-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-dedupe-sdk-test-1.0.5.tar", last modified: Tue May 23 08:49:58 2023, max compression
+gzip compressed data, was "mobio-dedupe-sdk-test-1.0.6.tar", last modified: Tue May 23 08:58:03 2023, max compression
```

## Comparing `mobio-dedupe-sdk-test-1.0.5.tar` & `mobio-dedupe-sdk-test-1.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:49:58.279209 mobio-dedupe-sdk-test-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 08:49:58.279209 mobio-dedupe-sdk-test-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:49:58.245208 mobio-dedupe-sdk-test-1.0.5/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:49:58.249209 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:49:58.265209 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/__init__.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/_init.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/_typing.py
--rw-r--r--   0 root         (0) root         (0)    55436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/api.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/backport.py
--rw-r--r--   0 root         (0) root         (0)    11058 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/blocking.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/canonical.py
--rw-r--r--   0 root         (0) root         (0)     2603 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/canopy_index.py
--rw-r--r--   0 root         (0) root         (0)    12932 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/clustering.py
--rw-r--r--   0 root         (0) root         (0)    11718 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/convenience.py
--rw-r--r--   0 root         (0) root         (0)     9307 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/core.py
--rw-r--r--   0 root         (0) root         (0)     8410 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/datamodel.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/index.py
--rw-r--r--   0 root         (0) root         (0)    15883 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/labeler.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/levenshtein.py
--rw-r--r--   0 root         (0) root         (0)     6898 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/predicate_functions.py
--rw-r--r--   0 root         (0) root         (0)    11150 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/predicates.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/tfidf.py
--rw-r--r--   0 root         (0) root         (0)    14462 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:49:58.274209 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/base.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/categorical_type.py
--rw-r--r--   0 root         (0) root         (0)      390 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/exact.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/exists.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/interaction.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/latlong.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/price.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/set.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:49:58.278209 mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 08:49:58.000000 mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1334 2023-05-23 08:49:58.000000 mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 08:49:58.000000 mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 08:49:58.000000 mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      656 2023-05-23 08:49:58.000000 mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 08:49:58.000000 mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 08:49:58.279209 mobio-dedupe-sdk-test-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    10310 2023-05-23 08:49:57.000000 mobio-dedupe-sdk-test-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:58:03.713090 mobio-dedupe-sdk-test-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 08:58:03.712089 mobio-dedupe-sdk-test-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:58:03.670088 mobio-dedupe-sdk-test-1.0.6/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:58:03.676089 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:58:03.696089 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/_init.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/_typing.py
+-rw-r--r--   0 root         (0) root         (0)    55436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/api.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/backport.py
+-rw-r--r--   0 root         (0) root         (0)    11058 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/blocking.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/canonical.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/canopy_index.py
+-rw-r--r--   0 root         (0) root         (0)    12932 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/clustering.py
+-rw-r--r--   0 root         (0) root         (0)    11718 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/convenience.py
+-rw-r--r--   0 root         (0) root         (0)     9307 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/core.py
+-rw-r--r--   0 root         (0) root         (0)     8410 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/datamodel.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/index.py
+-rw-r--r--   0 root         (0) root         (0)    15883 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/labeler.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/levenshtein.py
+-rw-r--r--   0 root         (0) root         (0)     6898 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/predicate_functions.py
+-rw-r--r--   0 root         (0) root         (0)    11150 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/predicates.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/tfidf.py
+-rw-r--r--   0 root         (0) root         (0)    14462 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:58:03.705089 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/base.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/categorical_type.py
+-rw-r--r--   0 root         (0) root         (0)      390 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/exact.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/exists.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/interaction.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/latlong.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/price.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/set.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 08:58:03.711089 mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 08:58:03.000000 mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-05-23 08:58:03.000000 mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 08:58:03.000000 mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 08:58:03.000000 mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-23 08:58:03.000000 mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 08:58:03.000000 mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 08:58:03.713090 mobio-dedupe-sdk-test-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    10322 2023-05-23 08:58:02.000000 mobio-dedupe-sdk-test-1.0.6/setup.py
```

### Comparing `mobio-dedupe-sdk-test-1.0.5/PKG-INFO` & `mobio-dedupe-sdk-test-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-dedupe-sdk-test
-Version: 1.0.5
+Version: 1.0.6
 Summary: Mobio dedupe SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/_typing.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/_typing.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/api.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/api.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/blocking.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/blocking.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/canonical.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/canonical.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/canopy_index.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/canopy_index.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/clustering.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/clustering.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/convenience.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/convenience.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/core.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/core.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/datamodel.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/datamodel.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/index.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/index.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/labeler.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/labeler.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/levenshtein.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/levenshtein.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/predicate_functions.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/predicate_functions.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/predicates.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/predicates.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/serializer.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/serializer.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/tfidf.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/tfidf.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/training.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/training.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/base.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/base.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/categorical_type.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/categorical_type.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/exists.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/exists.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/interaction.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/interaction.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/price.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/price.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/set.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/set.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio/sdks/dedupe/variables/string.py` & `mobio-dedupe-sdk-test-1.0.6/mobio/sdks/dedupe/variables/string.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/PKG-INFO` & `mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-dedupe-sdk-test
-Version: 1.0.5
+Version: 1.0.6
 Summary: Mobio dedupe SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/SOURCES.txt` & `mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/mobio_dedupe_sdk_test.egg-info/requires.txt` & `mobio-dedupe-sdk-test-1.0.6/mobio_dedupe_sdk_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.5/setup.py` & `mobio-dedupe-sdk-test-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                         'pycodestyle==2.9.1', 'pycparser==2.21', 'pyflakes==2.5.0', 'pyhacrf-datamade==0.2.6',
                         'PyLBFGS==0.2.0.14', 'python-dateutil==2.8.2', 'scikit-learn==1.2.2', 'scipy==1.10.1',
                         'simplecosine==1.2', 'six==1.16.0', 'threadpoolctl==3.1.0', 'toml==0.10.2',
                         'typing_extensions==4.5.0', 'zope.index==6.0', 'zope.interface==6.0']
         return requirements
 
 
-version_dev='1.0.5'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_dev='1.0.6'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 version_prod='1.0.0'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -57,15 +57,15 @@
     name="mobio-dedupe-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.5',  # Required, Phần này cũng không được format file.
+    version='1.0.6',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio dedupe SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -137,15 +137,15 @@
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
     packages=find_namespace_packages(include=["mobio.*"]),  # Required
-    package_data={"mobio": ['mobio/*.c', 'mobio/*.py', "mobio/*.so", "mobio/*.pyx"]},  # Required
+    package_data={"mobio": ['mobio/**/*.c', 'mobio/**/*.py', "mobio/**/*.so", "mobio/**/*.pyx"]},  # Required
     namespace_packages=["mobio"],  # Optional
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
     python_requires=">=3",
     # This field lists other packages that your project depends on to run.
```

