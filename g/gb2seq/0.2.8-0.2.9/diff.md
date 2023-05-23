# Comparing `tmp/gb2seq-0.2.8.tar.gz` & `tmp/gb2seq-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gb2seq-0.2.8.tar", last modified: Sun May 21 14:27:17 2023, max compression
+gzip compressed data, was "gb2seq-0.2.9.tar", last modified: Sun May 21 14:42:23 2023, max compression
```

## Comparing `gb2seq-0.2.8.tar` & `gb2seq-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:27:17.608239 gb2seq-0.2.8/
--rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.8/AUTHORS
--rw-rw-r--   0 terry      (501) staff       (20)       39 2023-05-20 21:53:46.000000 gb2seq-0.2.8/MANIFEST.in
--rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:27:17.607581 gb2seq-0.2.8/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)    26621 2023-05-21 12:53:46.000000 gb2seq-0.2.8/README.md
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:27:17.594440 gb2seq-0.2.8/bin/
--rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.8/bin/annotate-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     7257 2023-05-21 10:01:54.000000 gb2seq-0.2.8/bin/describe-feature.py
--rwxrwxr-x   0 terry      (501) staff       (20)    15353 2023-05-20 07:09:01.000000 gb2seq-0.2.8/bin/describe-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     6171 2023-05-21 10:32:17.000000 gb2seq-0.2.8/bin/describe-site.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:27:17.598420 gb2seq-0.2.8/gb2seq/
--rw-rw-r--   0 terry      (501) staff       (20)       93 2023-05-21 14:26:49.000000 gb2seq-0.2.8/gb2seq/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)    41849 2023-05-21 12:40:54.000000 gb2seq-0.2.8/gb2seq/alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     7745 2023-03-24 11:55:34.000000 gb2seq-0.2.8/gb2seq/annotate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.8/gb2seq/change.py
--rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.8/gb2seq/checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    27532 2023-05-21 14:02:33.000000 gb2seq-0.2.8/gb2seq/features.py
--rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.8/gb2seq/genome.py
--rw-rw-r--   0 terry      (501) staff       (20)     2457 2023-03-24 11:55:34.000000 gb2seq-0.2.8/gb2seq/sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    20485 2023-05-21 07:41:44.000000 gb2seq-0.2.8/gb2seq/translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.8/gb2seq/variants.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:27:17.600846 gb2seq-0.2.8/gb2seq.egg-info/
--rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:27:17.000000 gb2seq-0.2.8/gb2seq.egg-info/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)      633 2023-05-21 14:27:17.000000 gb2seq-0.2.8/gb2seq.egg-info/SOURCES.txt
--rw-rw-r--   0 terry      (501) staff       (20)        1 2023-05-21 14:27:17.000000 gb2seq-0.2.8/gb2seq.egg-info/dependency_links.txt
--rw-rw-r--   0 terry      (501) staff       (20)       20 2023-05-21 14:27:17.000000 gb2seq-0.2.8/gb2seq.egg-info/requires.txt
--rw-rw-r--   0 terry      (501) staff       (20)        7 2023-05-21 14:27:17.000000 gb2seq-0.2.8/gb2seq.egg-info/top_level.txt
--rw-rw-r--   0 terry      (501) staff       (20)       38 2023-05-21 14:27:17.608417 gb2seq-0.2.8/setup.cfg
--rw-rw-r--   0 terry      (501) staff       (20)     2079 2023-05-21 13:34:44.000000 gb2seq-0.2.8/setup.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:27:17.606725 gb2seq-0.2.8/test/
--rw-rw-r--   0 terry      (501) staff       (20)    66686 2023-05-21 13:39:01.000000 gb2seq-0.2.8/test/test_alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.8/test/test_change.py
--rw-rw-r--   0 terry      (501) staff       (20)     5116 2023-05-21 13:39:38.000000 gb2seq-0.2.8/test/test_checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-03-24 11:55:34.000000 gb2seq-0.2.8/test/test_features.py
--rw-rw-r--   0 terry      (501) staff       (20)    17090 2023-05-21 13:40:07.000000 gb2seq-0.2.8/test/test_genomes.py
--rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.8/test/test_sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    21028 2023-05-21 12:34:49.000000 gb2seq-0.2.8/test/test_translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1075 2023-05-21 13:47:12.000000 gb2seq-0.2.8/test/test_variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:42:23.729535 gb2seq-0.2.9/
+-rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.9/AUTHORS
+-rw-rw-r--   0 terry      (501) staff       (20)       39 2023-05-20 21:53:46.000000 gb2seq-0.2.9/MANIFEST.in
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:42:23.729159 gb2seq-0.2.9/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)    26621 2023-05-21 12:53:46.000000 gb2seq-0.2.9/README.md
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:42:23.719590 gb2seq-0.2.9/bin/
+-rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.9/bin/annotate-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     7257 2023-05-21 10:01:54.000000 gb2seq-0.2.9/bin/describe-feature.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    15353 2023-05-20 07:09:01.000000 gb2seq-0.2.9/bin/describe-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     6171 2023-05-21 10:32:17.000000 gb2seq-0.2.9/bin/describe-site.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:42:23.723297 gb2seq-0.2.9/gb2seq/
+-rw-rw-r--   0 terry      (501) staff       (20)       93 2023-05-21 14:35:02.000000 gb2seq-0.2.9/gb2seq/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)    41849 2023-05-21 12:40:54.000000 gb2seq-0.2.9/gb2seq/alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     7745 2023-03-24 11:55:34.000000 gb2seq-0.2.9/gb2seq/annotate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.9/gb2seq/change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.9/gb2seq/checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    27529 2023-05-21 14:40:15.000000 gb2seq-0.2.9/gb2seq/features.py
+-rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.9/gb2seq/genome.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2457 2023-03-24 11:55:34.000000 gb2seq-0.2.9/gb2seq/sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    20485 2023-05-21 07:41:44.000000 gb2seq-0.2.9/gb2seq/translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.9/gb2seq/variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:42:23.725311 gb2seq-0.2.9/gb2seq.egg-info/
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:42:23.000000 gb2seq-0.2.9/gb2seq.egg-info/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)      633 2023-05-21 14:42:23.000000 gb2seq-0.2.9/gb2seq.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        1 2023-05-21 14:42:23.000000 gb2seq-0.2.9/gb2seq.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry      (501) staff       (20)       20 2023-05-21 14:42:23.000000 gb2seq-0.2.9/gb2seq.egg-info/requires.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        7 2023-05-21 14:42:23.000000 gb2seq-0.2.9/gb2seq.egg-info/top_level.txt
+-rw-rw-r--   0 terry      (501) staff       (20)       38 2023-05-21 14:42:23.729653 gb2seq-0.2.9/setup.cfg
+-rw-rw-r--   0 terry      (501) staff       (20)     2079 2023-05-21 13:34:44.000000 gb2seq-0.2.9/setup.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:42:23.728683 gb2seq-0.2.9/test/
+-rw-rw-r--   0 terry      (501) staff       (20)    66686 2023-05-21 13:39:01.000000 gb2seq-0.2.9/test/test_alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.9/test/test_change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5116 2023-05-21 13:39:38.000000 gb2seq-0.2.9/test/test_checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-03-24 11:55:34.000000 gb2seq-0.2.9/test/test_features.py
+-rw-rw-r--   0 terry      (501) staff       (20)    17090 2023-05-21 13:40:07.000000 gb2seq-0.2.9/test/test_genomes.py
+-rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.9/test/test_sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    21028 2023-05-21 12:34:49.000000 gb2seq-0.2.9/test/test_translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1075 2023-05-21 13:47:12.000000 gb2seq-0.2.9/test/test_variants.py
```

### Comparing `gb2seq-0.2.8/PKG-INFO` & `gb2seq-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
 Maintainer: Terry C. Jones
 Maintainer-email: terence.jones@charite.de
```

### Comparing `gb2seq-0.2.8/README.md` & `gb2seq-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/bin/annotate-genome.py` & `gb2seq-0.2.9/bin/annotate-genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/bin/describe-feature.py` & `gb2seq-0.2.9/bin/describe-feature.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/bin/describe-genome.py` & `gb2seq-0.2.9/bin/describe-genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/bin/describe-site.py` & `gb2seq-0.2.9/bin/describe-site.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/alignment.py` & `gb2seq-0.2.9/gb2seq/alignment.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/annotate.py` & `gb2seq-0.2.9/gb2seq/annotate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/change.py` & `gb2seq-0.2.9/gb2seq/change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/checker.py` & `gb2seq-0.2.9/gb2seq/checker.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/features.py` & `gb2seq-0.2.9/gb2seq/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from os import environ
 import itertools
 from collections import UserDict
 from pathlib import Path
 from typing import Dict, Optional, Set, Union
 
 try:
-    from importlib.resources import open_text
+    from importlib.resources import files
 except ImportError:
-    from importlib_resources import open_text
+    from importlib_resources import files
 
 
 # from warnings import warn
 import json
 import argparse
 
 from Bio import Entrez, SeqIO
@@ -75,15 +75,15 @@
     ) -> None:
         super().__init__()
         self.sars2 = sars2
         self.translatedNames: Set[str] = set()
 
         if referenceSpecification is None:
             if sars2:
-                with open_text("gb2seq.data", "NC_045512.2.gb") as fp:
+                with files("gb2seq.data").joinpath("NC_045512.2.gb") as fp:
                     try:
                         record = SeqIO.read(fp, "genbank")
                     except Exception as e:
                         print(
                             "Could not parse default SARS-CoV-2 GenBank record",
                             e,
                             file=sys.stderr,
```

### Comparing `gb2seq-0.2.8/gb2seq/genome.py` & `gb2seq-0.2.9/gb2seq/genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/sars2.py` & `gb2seq-0.2.9/gb2seq/sars2.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/translate.py` & `gb2seq-0.2.9/gb2seq/translate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq/variants.py` & `gb2seq-0.2.9/gb2seq/variants.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/gb2seq.egg-info/PKG-INFO` & `gb2seq-0.2.9/gb2seq.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
 Maintainer: Terry C. Jones
 Maintainer-email: terence.jones@charite.de
```

### Comparing `gb2seq-0.2.8/gb2seq.egg-info/SOURCES.txt` & `gb2seq-0.2.9/gb2seq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/setup.py` & `gb2seq-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/test/test_alignment.py` & `gb2seq-0.2.9/test/test_alignment.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/test/test_change.py` & `gb2seq-0.2.9/test/test_change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/test/test_checker.py` & `gb2seq-0.2.9/test/test_checker.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/test/test_features.py` & `gb2seq-0.2.9/test/test_features.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/test/test_genomes.py` & `gb2seq-0.2.9/test/test_genomes.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/test/test_translate.py` & `gb2seq-0.2.9/test/test_translate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.8/test/test_variants.py` & `gb2seq-0.2.9/test/test_variants.py`

 * *Files identical despite different names*

