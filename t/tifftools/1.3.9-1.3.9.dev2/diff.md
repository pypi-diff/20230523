# Comparing `tmp/tifftools-1.3.9.tar.gz` & `tmp/tifftools-1.3.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifftools-1.3.9.tar", last modified: Tue Feb 28 18:33:26 2023, max compression
+gzip compressed data, was "tifftools-1.3.9.dev2.tar", last modified: Tue Feb 28 18:11:35 2023, max compression
```

## Comparing `tifftools-1.3.9.tar` & `tifftools-1.3.9.dev2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:33:26.807555 tifftools-1.3.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:33:26.799555 tifftools-1.3.9/.circleci/
--rw-r--r--   0 root         (0) root         (0)     4313 2023-02-28 18:33:03.000000 tifftools-1.3.9/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2023-02-28 18:33:03.000000 tifftools-1.3.9/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      596 2023-02-28 18:33:03.000000 tifftools-1.3.9/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3020 2023-02-28 18:33:03.000000 tifftools-1.3.9/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)      549 2023-02-28 18:33:03.000000 tifftools-1.3.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      148 2023-02-28 18:33:03.000000 tifftools-1.3.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8878 2023-02-28 18:33:26.803555 tifftools-1.3.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7973 2023-02-28 18:33:03.000000 tifftools-1.3.9/README.rst
--rw-r--r--   0 root         (0) root         (0)      424 2023-02-28 18:33:03.000000 tifftools-1.3.9/codecov.yml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 18:33:26.807555 tifftools-1.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2091 2023-02-28 18:33:03.000000 tifftools-1.3.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:33:26.803555 tifftools-1.3.9/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:33:26.803555 tifftools-1.3.9/tests/data/
--rw-r--r--   0 root         (0) root         (0)      630 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_datatype.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_double_reference.tif
--rw-r--r--   0 root         (0) root         (0)      653 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_header1.tif
--rw-r--r--   0 root         (0) root         (0)      815 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_header2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_ifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      360 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      616 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_jpeg2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_strip_offset.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_subifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      653 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_tag_offset.tif
--rw-r--r--   0 root         (0) root         (0)      641 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/bad_unicode.tif
--rw-r--r--   0 root         (0) root         (0)      616 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/good_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      453 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/data/good_single.tif
--rw-r--r--   0 root         (0) root         (0)     2114 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     3059 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_constants.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_dump.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)      848 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_options.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_path_or_fobj.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_read_tiff.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_readme.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_set.py
--rw-r--r--   0 root         (0) root         (0)     3992 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-02-28 18:33:03.000000 tifftools-1.3.9/tests/test_write_tiff.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:33:26.803555 tifftools-1.3.9/tifftools/
--rw-r--r--   0 root         (0) root         (0)     1170 2023-02-28 18:33:03.000000 tifftools-1.3.9/tifftools/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-02-28 18:33:03.000000 tifftools-1.3.9/tifftools/__main__.py
--rw-r--r--   0 root         (0) root         (0)    31100 2023-02-28 18:33:03.000000 tifftools-1.3.9/tifftools/commands.py
--rw-r--r--   0 root         (0) root         (0)    56913 2023-02-28 18:33:03.000000 tifftools-1.3.9/tifftools/constants.py
--rw-r--r--   0 root         (0) root         (0)      265 2023-02-28 18:33:03.000000 tifftools-1.3.9/tifftools/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-02-28 18:33:03.000000 tifftools-1.3.9/tifftools/path_or_fobj.py
--rwxr-xr-x   0 root         (0) root         (0)    24826 2023-02-28 18:33:03.000000 tifftools-1.3.9/tifftools/tifftools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:33:26.803555 tifftools-1.3.9/tifftools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8878 2023-02-28 18:33:26.000000 tifftools-1.3.9/tifftools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2023-02-28 18:33:26.000000 tifftools-1.3.9/tifftools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 18:33:26.000000 tifftools-1.3.9/tifftools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-28 18:33:26.000000 tifftools-1.3.9/tifftools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 18:33:16.000000 tifftools-1.3.9/tifftools.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-28 18:33:26.000000 tifftools-1.3.9/tifftools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-02-28 18:33:26.000000 tifftools-1.3.9/tifftools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1729 2023-02-28 18:33:03.000000 tifftools-1.3.9/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:11:35.373013 tifftools-1.3.9.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:11:35.365013 tifftools-1.3.9.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)      549 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      148 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8883 2023-02-28 18:11:35.373013 tifftools-1.3.9.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7973 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      424 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 18:11:35.373013 tifftools-1.3.9.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:11:35.365013 tifftools-1.3.9.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:11:35.369013 tifftools-1.3.9.dev2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_datatype.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_double_reference.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_header1.tif
+-rw-r--r--   0 root         (0) root         (0)      815 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_header2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_ifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      360 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_jpeg2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_strip_offset.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_subifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_tag_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      641 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/bad_unicode.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/good_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/data/good_single.tif
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_constants.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_dump.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)      848 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_options.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_path_or_fobj.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_read_tiff.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_readme.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_set.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tests/test_write_tiff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:11:35.369013 tifftools-1.3.9.dev2/tifftools/
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tifftools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tifftools/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    31100 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tifftools/commands.py
+-rw-r--r--   0 root         (0) root         (0)    56913 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tifftools/constants.py
+-rw-r--r--   0 root         (0) root         (0)      265 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tifftools/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tifftools/path_or_fobj.py
+-rwxr-xr-x   0 root         (0) root         (0)    24826 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tifftools/tifftools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 18:11:35.373013 tifftools-1.3.9.dev2/tifftools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8883 2023-02-28 18:11:35.000000 tifftools-1.3.9.dev2/tifftools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-02-28 18:11:35.000000 tifftools-1.3.9.dev2/tifftools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 18:11:35.000000 tifftools-1.3.9.dev2/tifftools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-02-28 18:11:35.000000 tifftools-1.3.9.dev2/tifftools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 18:11:24.000000 tifftools-1.3.9.dev2/tifftools.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-02-28 18:11:35.000000 tifftools-1.3.9.dev2/tifftools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-02-28 18:11:35.000000 tifftools-1.3.9.dev2/tifftools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-02-28 18:11:09.000000 tifftools-1.3.9.dev2/tox.ini
```

### Comparing `tifftools-1.3.9/.circleci/config.yml` & `tifftools-1.3.9.dev2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/.gitignore` & `tifftools-1.3.9.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/CHANGELOG.md` & `tifftools-1.3.9.dev2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/LICENSE` & `tifftools-1.3.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/PKG-INFO` & `tifftools-1.3.9.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.3.9
+Version: 1.3.9.dev2
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.3.9/README.rst` & `tifftools-1.3.9.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/setup.py` & `tifftools-1.3.9.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_datatype.tif` & `tifftools-1.3.9.dev2/tests/data/bad_datatype.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_double_reference.tif` & `tifftools-1.3.9.dev2/tests/data/bad_double_reference.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_header1.tif` & `tifftools-1.3.9.dev2/tests/data/bad_header1.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_header2.tif` & `tifftools-1.3.9.dev2/tests/data/bad_header2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_jpeg2.tif` & `tifftools-1.3.9.dev2/tests/data/bad_jpeg2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_subifd_offset.tif` & `tifftools-1.3.9.dev2/tests/data/bad_subifd_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_tag_offset.tif` & `tifftools-1.3.9.dev2/tests/data/bad_tag_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/bad_unicode.tif` & `tifftools-1.3.9.dev2/tests/data/bad_unicode.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/data/good_jpeg.tif` & `tifftools-1.3.9.dev2/tests/data/good_jpeg.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/datastore.py` & `tifftools-1.3.9.dev2/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_constants.py` & `tifftools-1.3.9.dev2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_dump.py` & `tifftools-1.3.9.dev2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_main.py` & `tifftools-1.3.9.dev2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_options.py` & `tifftools-1.3.9.dev2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_path_or_fobj.py` & `tifftools-1.3.9.dev2/tests/test_path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_read_tiff.py` & `tifftools-1.3.9.dev2/tests/test_read_tiff.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_readme.py` & `tifftools-1.3.9.dev2/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_set.py` & `tifftools-1.3.9.dev2/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_split.py` & `tifftools-1.3.9.dev2/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tests/test_write_tiff.py` & `tifftools-1.3.9.dev2/tests/test_write_tiff.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tifftools/__init__.py` & `tifftools-1.3.9.dev2/tifftools/__init__.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tifftools/commands.py` & `tifftools-1.3.9.dev2/tifftools/commands.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tifftools/constants.py` & `tifftools-1.3.9.dev2/tifftools/constants.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tifftools/path_or_fobj.py` & `tifftools-1.3.9.dev2/tifftools/path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tifftools/tifftools.py` & `tifftools-1.3.9.dev2/tifftools/tifftools.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tifftools.egg-info/PKG-INFO` & `tifftools-1.3.9.dev2/tifftools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.3.9
+Version: 1.3.9.dev2
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.3.9/tifftools.egg-info/SOURCES.txt` & `tifftools-1.3.9.dev2/tifftools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tifftools-1.3.9/tox.ini` & `tifftools-1.3.9.dev2/tox.ini`

 * *Files identical despite different names*

