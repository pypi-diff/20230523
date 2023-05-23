# Comparing `tmp/rcsb.utils.seqalign-0.26.tar.gz` & `tmp/rcsb.utils.seqalign-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.seqalign-0.26.tar", last modified: Mon Jan  9 17:40:01 2023, max compression
+gzip compressed data, was "rcsb.utils.seqalign-0.27.tar", last modified: Tue May 23 15:32:41 2023, max compression
```

## Comparing `rcsb.utils.seqalign-0.26.tar` & `rcsb.utils.seqalign-0.27.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:40:01.116546 rcsb.utils.seqalign-0.26/
--rw-r--r--   0 vsts      (1001) docker     (122)     1283 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      112 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1663 2023-01-09 17:40:01.116546 rcsb.utils.seqalign-0.26/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      957 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:40:01.112546 rcsb.utils.seqalign-0.26/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:40:01.116546 rcsb.utils.seqalign-0.26/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:40:01.116546 rcsb.utils.seqalign-0.26/rcsb/utils/seqalign/
--rw-r--r--   0 vsts      (1001) docker     (122)    33465 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/rcsb/utils/seqalign/MMseqsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-01-09 17:30:29.000000 rcsb.utils.seqalign-0.26/rcsb/utils/seqalign/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-09 17:40:01.116546 rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1663 2023-01-09 17:40:01.000000 rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-01-09 17:40:01.000000 rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-09 17:40:01.000000 rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-09 17:31:24.000000 rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-01-09 17:40:01.000000 rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-01-09 17:40:01.000000 rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-01-09 17:30:30.000000 rcsb.utils.seqalign-0.26/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-01-09 17:40:01.116546 rcsb.utils.seqalign-0.26/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2291 2023-01-09 17:30:30.000000 rcsb.utils.seqalign-0.26/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 15:32:41.284111 rcsb.utils.seqalign-0.27/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1351 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      112 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1663 2023-05-23 15:32:41.284111 rcsb.utils.seqalign-0.27/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      957 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 15:32:41.284111 rcsb.utils.seqalign-0.27/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 15:32:41.284111 rcsb.utils.seqalign-0.27/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 15:32:41.284111 rcsb.utils.seqalign-0.27/rcsb/utils/seqalign/
+-rw-r--r--   0 vsts      (1001) docker     (122)    33465 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/rcsb/utils/seqalign/MMseqsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/rcsb/utils/seqalign/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 15:32:41.284111 rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1663 2023-05-23 15:32:41.000000 rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-05-23 15:32:41.000000 rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 15:32:41.000000 rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 15:24:06.000000 rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-05-23 15:32:41.000000 rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-23 15:32:41.000000 rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-23 15:32:41.288111 rcsb.utils.seqalign-0.27/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2291 2023-05-23 15:22:53.000000 rcsb.utils.seqalign-0.27/setup.py
```

### Comparing `rcsb.utils.seqalign-0.26/HISTORY.txt` & `rcsb.utils.seqalign-0.27/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,8 +11,9 @@
   12-Jun-2021  - V0.19 Add bit score filtering in __getMatchResults()
   12-Jun-2021  - V0.20 Updating installation scripts
   27-Jun-2021  - V0.21 Adjust handling of defaults for formatOutput parameter in __formatSearchResults()
    4-Jul-2021  - V0.22 Add new tests for searchDatabase() and make sensitivity adjustable in tests
   11-Jul-2021  - V0.23 Add getAlignedRegions() convenience method
   11-Jul-2021  - V0.24 Add aligned regions to the default query results data structure
   29-Jul-2021  - V0.25 Disable cleanup of taxonomy download files in TaxonomyProvider()
-   9-Jan-2023  - V0.26 Configuration changes to support tox 4
+   9-Jan-2023  - V0.26 Configuration changes to support tox 4
+  22-May-2023  - V0.27 Add retries to tox task for MMseqs2 download
```

### Comparing `rcsb.utils.seqalign-0.26/LICENSE` & `rcsb.utils.seqalign-0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seqalign-0.26/PKG-INFO` & `rcsb.utils.seqalign-0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.seqalign
-Version: 0.26
+Version: 0.27
 Summary: RCSB Python Wrapper Module for Sequence Alignment Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_seqalign
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.seqalign-0.26/README.md` & `rcsb.utils.seqalign-0.27/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seqalign-0.26/rcsb/utils/seqalign/MMseqsUtils.py` & `rcsb.utils.seqalign-0.27/rcsb/utils/seqalign/MMseqsUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.seqalign-0.26/rcsb.utils.seqalign.egg-info/PKG-INFO` & `rcsb.utils.seqalign-0.27/rcsb.utils.seqalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.seqalign
-Version: 0.26
+Version: 0.27
 Summary: RCSB Python Wrapper Module for Sequence Alignment Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_seqalign
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.seqalign-0.26/setup.py` & `rcsb.utils.seqalign-0.27/setup.py`

 * *Files identical despite different names*

