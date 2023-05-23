# Comparing `tmp/large-image-source-multi-1.21.0.tar.gz` & `tmp/large-image-source-multi-1.21.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-multi-1.21.0.tar", last modified: Tue May 23 14:21:11 2023, max compression
+gzip compressed data, was "large-image-source-multi-1.21.1.dev2.tar", last modified: Tue May 23 18:52:45 2023, max compression
```

## Comparing `large-image-source-multi-1.21.0.tar` & `large-image-source-multi-1.21.1.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 14:21:11.573232 large-image-source-multi-1.21.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-05-23 14:21:11.573232 large-image-source-multi-1.21.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 14:21:11.573232 large-image-source-multi-1.21.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-05-23 14:19:58.000000 large-image-source-multi-1.21.0/docs/specification.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 14:21:11.573232 large-image-source-multi-1.21.0/large_image_source_multi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45283 2023-05-23 14:19:58.000000 large-image-source-multi-1.21.0/large_image_source_multi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-23 14:19:58.000000 large-image-source-multi-1.21.0/large_image_source_multi/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 14:21:11.573232 large-image-source-multi-1.21.0/large_image_source_multi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/large_image_source_multi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/large_image_source_multi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/large_image_source_multi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/large_image_source_multi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/large_image_source_multi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-23 14:21:11.000000 large-image-source-multi-1.21.0/large_image_source_multi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-23 14:21:11.573232 large-image-source-multi-1.21.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-05-23 14:19:58.000000 large-image-source-multi-1.21.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 18:52:45.437438 large-image-source-multi-1.21.1.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2023-05-23 18:52:45.437438 large-image-source-multi-1.21.1.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 18:52:45.437438 large-image-source-multi-1.21.1.dev2/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-05-23 18:51:23.000000 large-image-source-multi-1.21.1.dev2/docs/specification.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 18:52:45.437438 large-image-source-multi-1.21.1.dev2/large_image_source_multi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45283 2023-05-23 18:51:23.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-23 18:51:23.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 18:52:45.437438 large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-23 18:52:45.000000 large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-23 18:52:45.437438 large-image-source-multi-1.21.1.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-05-23 18:51:23.000000 large-image-source-multi-1.21.1.dev2/setup.py
```

### Comparing `large-image-source-multi-1.21.0/LICENSE` & `large-image-source-multi-1.21.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.21.0/PKG-INFO` & `large-image-source-multi-1.21.1.dev2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.21.0
+Version: 1.21.1.dev2
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.21.0/README.rst` & `large-image-source-multi-1.21.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.21.0/docs/specification.rst` & `large-image-source-multi-1.21.1.dev2/docs/specification.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.21.0/large_image_source_multi/__init__.py` & `large-image-source-multi-1.21.1.dev2/large_image_source_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.21.0/large_image_source_multi/girder_source.py` & `large-image-source-multi-1.21.1.dev2/large_image_source_multi/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.21.0/large_image_source_multi.egg-info/PKG-INFO` & `large-image-source-multi-1.21.1.dev2/large_image_source_multi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.21.0
+Version: 1.21.1.dev2
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.21.0/setup.py` & `large-image-source-multi-1.21.1.dev2/setup.py`

 * *Files identical despite different names*

