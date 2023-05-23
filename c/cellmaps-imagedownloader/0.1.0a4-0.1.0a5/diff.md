# Comparing `tmp/cellmaps_imagedownloader-0.1.0a4.tar.gz` & `tmp/cellmaps_imagedownloader-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_imagedownloader-0.1.0a4.tar", last modified: Fri May 19 22:50:41 2023, max compression
+gzip compressed data, was "dist/cellmaps_imagedownloader-0.1.0a5.tar", last modified: Tue May 23 16:32:00 2023, max compression
```

## Comparing `cellmaps_imagedownloader-0.1.0a4.tar` & `cellmaps_imagedownloader-0.1.0a5.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.050034 cellmaps_imagedownloader-0.1.0a4/
--rw-r--r--   0 churas     (504) staff       (20)      150 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3731 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a4/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-11 22:14:34.000000 cellmaps_imagedownloader-0.1.0a4/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5278 2023-05-19 22:50:41.050269 cellmaps_imagedownloader-0.1.0a4/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3347 2023-05-16 20:59:48.000000 cellmaps_imagedownloader-0.1.0a4/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.040468 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/
--rw-r--r--   0 churas     (504) staff       (20)      341 2023-05-19 22:24:12.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     9182 2023-05-11 21:43:55.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)      145 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    13239 2023-05-08 16:57:23.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/gene.py
--rw-r--r--   0 churas     (504) staff       (20)    25679 2023-05-19 22:22:34.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.041794 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5278 2023-05-19 22:50:40.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1321 2023-05-19 22:50:41.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-19 22:50:40.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-19 22:50:40.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       36 2023-05-19 22:50:40.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       25 2023-05-19 22:50:40.000000 cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.046455 cellmaps_imagedownloader-0.1.0a4/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.036943 cellmaps_imagedownloader-0.1.0a4/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.037118 cellmaps_imagedownloader-0.1.0a4/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.047208 cellmaps_imagedownloader-0.1.0a4/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a4/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a4/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a4/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1029 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/cellmaps_downloader.rst
--rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-03 22:58:28.000000 cellmaps_imagedownloader-0.1.0a4/docs/cellmaps_imagedownloader.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6113 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      939 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a4/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      407 2023-05-19 22:50:41.050863 cellmaps_imagedownloader-0.1.0a4/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1899 2023-05-18 20:34:04.000000 cellmaps_imagedownloader-0.1.0a4/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-19 22:50:41.049750 cellmaps_imagedownloader-0.1.0a4/tests/
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a4/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1429 2023-05-04 23:17:17.000000 cellmaps_imagedownloader-0.1.0a4/tests/test_cellmaps_imagedownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)     7543 2023-05-11 21:09:17.000000 cellmaps_imagedownloader-0.1.0a4/tests/test_cellmapsimagedownloader.py
--rw-r--r--   0 churas     (504) staff       (20)     2245 2023-05-04 00:03:34.000000 cellmaps_imagedownloader-0.1.0a4/tests/test_genenodegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     2235 2023-05-04 00:03:55.000000 cellmaps_imagedownloader-0.1.0a4/tests/test_genequery.py
--rw-r--r--   0 churas     (504) staff       (20)    12726 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/tests/test_imagegenenodegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a4/tests/test_integration_cellmaps_downloader.py
--rw-r--r--   0 churas     (504) staff       (20)     1018 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a4/tests/test_multiprocessimagedownloader.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.955100 cellmaps_imagedownloader-0.1.0a5/
+-rw-r--r--   0 churas     (504) staff       (20)      150 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3731 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-11 22:14:34.000000 cellmaps_imagedownloader-0.1.0a5/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5191 2023-05-23 16:32:00.955244 cellmaps_imagedownloader-0.1.0a5/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3284 2023-05-22 22:23:15.000000 cellmaps_imagedownloader-0.1.0a5/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.938564 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/
+-rw-r--r--   0 churas     (504) staff       (20)      341 2023-05-23 16:21:03.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     9182 2023-05-11 21:43:55.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      145 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    14323 2023-05-22 22:15:28.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/gene.py
+-rw-r--r--   0 churas     (504) staff       (20)    27797 2023-05-23 16:31:16.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.940710 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5191 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1360 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       36 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       25 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.948811 cellmaps_imagedownloader-0.1.0a5/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.934265 cellmaps_imagedownloader-0.1.0a5/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.934335 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.949701 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-03 22:58:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/cellmaps_imagedownloader.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6214 2023-05-22 22:22:34.000000 cellmaps_imagedownloader-0.1.0a5/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      243 2023-05-22 21:38:15.000000 cellmaps_imagedownloader-0.1.0a5/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-22 23:09:36.000000 cellmaps_imagedownloader-0.1.0a5/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      407 2023-05-23 16:32:00.955705 cellmaps_imagedownloader-0.1.0a5/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1899 2023-05-18 20:34:04.000000 cellmaps_imagedownloader-0.1.0a5/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.953964 cellmaps_imagedownloader-0.1.0a5/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.954726 cellmaps_imagedownloader-0.1.0a5/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)      166 2023-05-22 20:49:48.000000 cellmaps_imagedownloader-0.1.0a5/tests/data/test_single_sample.tsv
+-rw-r--r--   0 churas     (504) staff       (20)      122 2023-05-22 20:51:02.000000 cellmaps_imagedownloader-0.1.0a5/tests/data/test_single_unique.tsv
+-rw-r--r--   0 churas     (504) staff       (20)     1429 2023-05-22 21:41:10.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_cellmaps_imagedownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     7543 2023-05-11 21:09:17.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_cellmapsimagedownloader.py
+-rw-r--r--   0 churas     (504) staff       (20)     2245 2023-05-04 00:03:34.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_genenodegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     2739 2023-05-22 21:29:59.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_genequery.py
+-rw-r--r--   0 churas     (504) staff       (20)     8830 2023-05-22 21:58:39.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_imagegenenodegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_integration_cellmaps_downloader.py
+-rw-r--r--   0 churas     (504) staff       (20)     1018 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_multiprocessimagedownloader.py
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/CONTRIBUTING.rst` & `cellmaps_imagedownloader-0.1.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/LICENSE` & `cellmaps_imagedownloader-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/PKG-INFO` & `cellmaps_imagedownloader-0.1.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_imagedownloader
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Downloads IF data needed for CM4AI MuSIC pipeline
 Home-page: https://github.com/idekerlab/cellmaps_imagedownloader
 Author: Gege Qian
 Author-email: geqian@ucsd.edu
 License: MIT license
 Description: =========================
         cellmaps_imagedownloader
@@ -18,28 +18,25 @@
             :target: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader
         
         .. image:: https://readthedocs.org/projects/cellmaps-downloader/badge/?version=latest
                 :target: https://cellmaps-imagedownloader.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        
-        
         Downloads IF data needed for CM4AI MuSIC pipeline
         
         
         * Free software: MIT license
         * Documentation: https://cellmaps-imagedownloader.readthedocs.io.
         
         
         Dependencies
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
-        * `fairscape-cli <https://pypi.org/project/fairscape-cli>`__
         * `requests <https://pypi.org/project/requests>`__
         * `mygene <https://pypi.org/project/mygene>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         
         Compatibility
         -------------
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/README.rst` & `cellmaps_imagedownloader-0.1.0a5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,25 @@
     :target: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader
 
 .. image:: https://readthedocs.org/projects/cellmaps-downloader/badge/?version=latest
         :target: https://cellmaps-imagedownloader.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
-
-
 Downloads IF data needed for CM4AI MuSIC pipeline
 
 
 * Free software: MIT license
 * Documentation: https://cellmaps-imagedownloader.readthedocs.io.
 
 
 Dependencies
 ------------
 
 * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
-* `fairscape-cli <https://pypi.org/project/fairscape-cli>`__
 * `requests <https://pypi.org/project/requests>`__
 * `mygene <https://pypi.org/project/mygene>`__
 * `tqdm <https://pypi.org/project/tqdm>`__
 
 Compatibility
 -------------
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py` & `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/gene.py` & `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/gene.py`

 * *Files 14% similar despite different names*

```diff
@@ -130,52 +130,116 @@
     Creates Image Gene Node Attributes table
     """
 
     SAMPLES_HEADER_COLS = ['filename', 'if_plate_id',
                            'position', 'sample', 'status',
                            'locations', 'antibody',
                            'ensembl_ids', 'gene_names']
+    """
+    Column labels for samples file
+    """
 
     UNIQUE_HEADER_COLS = ['antibody', 'ensembl_ids',
                           'gene_names', 'atlas_name',
                           'locations',
                           'n_location']
+    """
+    Column labels for unique file
+    """
 
     def __init__(self, samples_list=None,
                  unique_list=None,
                  genequery=GeneQuery()):
         """
         Constructor
+
+        **samples_list** is expected to be a list of :py:class:`dict`
+        objects with this format:
+
+        # TODO: Move this to a separate data document
+
+        .. code-block::
+
+            {
+             'filename': HPA FILENAME,
+             'if_plate_id': HPA PLATE ID,
+             'position': POSITION,
+             'sample': SAMPLE,
+             'status': STATUS,
+             'locations': COMMA DELIMITED LOCATIONS,
+             'antibody': ANTIBODY_ID,
+             'ensembl_ids': COMMA DELIMITED ENSEMBLID IDS,
+             'gene_names': COMMA DELIMITED GENE SYMBOLS
+            }
+
+        **Example:**
+
+        .. code-block::
+
+            {
+             'filename': '/archive/1/1_A1_1_',
+             'if_plate_id': '1',
+             'position': 'A1',
+             'sample': '1',
+             'status': '35',
+             'locations': 'Golgi apparatus',
+             'antibody': 'HPA000992',
+             'ensembl_ids': 'ENSG00000066455',
+             'gene_names': 'GOLGA5'
+            }
+
+        **unique_list** is expected to be a list of :py:class:`dict`
+        objects with this format:
+
+        .. code-block::
+
+            {
+             'antibody': ANTIBODY,
+             'ensembl_ids': COMMA DELIMITED ENSEMBL IDS,
+             'gene_names': COMMA DELIMITED GENE SYMBOLS,
+             'atlas_name': ATLAS NAME?,
+             'locations': COMMA DELIMITED LOCATIONS IN CELL,
+             'n_location': NUMBER OF LOCATIONS IN CELL,
+             }
+
+        **Example:**
+
+        .. code-block::
+
+            {
+             'antibody': 'HPA040086',
+             'ensembl_ids': 'ENSG00000094914',
+             'gene_names': 'AAAS',
+             'atlas_name': 'U-2',
+             'locations': 'OS,Nuclear membrane',
+             'n_location': '2',
+             }
+
+
+        :param samples_list: List of samples
+        :type samples_list: list
+        :param unique_list: List of unique samples
+        :type unique_list: list
+        :param genequery: Object to query for updated gene symbols
+        :type genequery: :py:class:`~cellmaps_imagedownloader.gene.GeneQuery`
         """
         super().__init__()
         self._samples_list = samples_list
         self._unique_list = unique_list
         self._genequery = genequery
 
     def get_samples_list(self):
         """
-        Gets samples_list passed in via the constructor
+        Gets **samples_list** passed in via the constructor
 
-        :return:
-        """
-        return self._samples_list
 
-    def write_samples_as_csvfile(self, outfile=None):
+        :return: list of samples set via constructor
+        :rtype: list
         """
-
-        :param outfile:
-        :return:
-        """
-        if self._samples_list is None:
-            raise CellMapsImageDownloaderError('samples list is None')
-        with open(outfile, 'w', newline='') as f:
-            writer = csv.DictWriter(f, fieldnames=ImageGeneNodeAttributeGenerator.SAMPLES_HEADER_COLS)
-            writer.writeheader()
-            for sample in self._samples_list:
-                writer.writerow(sample)
+        return self._samples_list
 
     @staticmethod
     def get_samples_from_csvfile(csvfile=None):
         """
 
         :param tsvfile:
         :return:
@@ -197,49 +261,32 @@
         """
         Gets antibodies_list passed in via the constructor
 
         :return:
         """
         return self._unique_list
 
-    def write_unique_list_as_csvfile(self, outfile=None):
-        """
-
-        :param outfile:
-        :return:
-        """
-        if self._unique_list is None:
-            raise CellMapsImageDownloaderError('unique list is None')
-
-        with open(outfile, 'w', newline='') as f:
-            writer = csv.DictWriter(f, fieldnames=ImageGeneNodeAttributeGenerator.UNIQUE_HEADER_COLS)
-            writer.writeheader()
-            for u in self._unique_list:
-                writer.writerow(u)
-
     @staticmethod
     def get_unique_list_from_csvfile(csvfile=None):
         """
 
         :param csvfile:
         :return:
         """
         if csvfile is None:
             raise CellMapsImageDownloaderError('csvfile is None')
 
         u_list = []
         with open(csvfile, 'r') as f:
             reader = csv.DictReader(f, delimiter=',')
             for row in reader:
-                u_list.append({'antibody': row['antibody'],
-                               'ensembl_ids': row['ensembl_ids'],
-                               'gene_names': row['gene_names'],
-                               'atlas_name': row['atlas_name'],
-                               'locations': row['locations'],
-                               'n_location': row['n_location']})
+                unique_entry = {}
+                for key in ImageGeneNodeAttributeGenerator.UNIQUE_HEADER_COLS:
+                    unique_entry[key] = row[key]
+                u_list.append(unique_entry)
         return u_list
 
     def _get_set_of_antibodies_from_unique_list(self):
         """
         Extract a unique set of antibodies from antibodies list
         passed in via constructor
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader/runner.py` & `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,76 +39,96 @@
 
 
 def download_file(downloadtuple):
     """
     Downloads file pointed to by 'download_url' to
     'destfile'
 
-    :param downloadtuple: (download link, dest file path)
+    .. note::
+
+        Default download function used by :py:class:`~MultiProcessImageDownloader`
+
+    :param downloadtuple: `(download link, dest file path)`
     :type downloadtuple: tuple
-    :raises Exception: from requests library if there is an error or non 200 status
     :return: None upon success otherwise:
-             (requests status code, text from request, downloadtuple)
+             `(requests status code, text from request, downloadtuple)`
     :rtype: tuple
     """
     logger.debug('Downloading ' + downloadtuple[0] + ' to ' + downloadtuple[1])
-    with requests.get(downloadtuple[0], stream=True) as r:
-        if r.status_code != 200:
-            return r.status_code, r.text, downloadtuple
-        with open(downloadtuple[1], 'wb') as f:
-            for chunk in r.iter_content(chunk_size=8192):
-                if chunk:  # filter out keep-alive new chunks
-                    f.write(chunk)
-    return None
+    try:
+        with requests.get(downloadtuple[0], stream=True) as r:
+            if r.status_code != 200:
+                return r.status_code, r.text, downloadtuple
+            with open(downloadtuple[1], 'wb') as f:
+                for chunk in r.iter_content(chunk_size=8192):
+                    if chunk:  # filter out keep-alive new chunks
+                        f.write(chunk)
+        return None
+    except requests.exceptions.HTTPError as e:
+        return -1, str(e), downloadtuple
+    except requests.exceptions.ConnectionError as e:
+        return -2, str(e), downloadtuple
+    except requests.exceptions.Timeout as e:
+        return -3, str(e), downloadtuple
+    except requests.exceptions.RequestException as e:
+        return -4, str(e), downloadtuple
+    except Exception as e:
+        return -5, str(e), downloadtuple
 
 
 class ImageDownloader(object):
     """
+    Abstract class that defines interface for classes that download images
 
     """
     def __init__(self):
         """
 
         """
         pass
 
     def download_images(self, download_list=None):
         """
         Subclasses should implement
+
         :param download_list: list of tuples where first element is
                               full URL of image to download and 2nd
                               element is destination path
         :type download_list: list
         :return: 
         """
         raise CellMapsImageDownloaderError('Subclasses should implement this')
 
 
 class FakeImageDownloader(ImageDownloader):
     """
-    Creates completely fake download by downloading
-    the first image in each color and then just makes
-    renamed copies
+    Creates fake download by downloading
+    the first image in each color from
+    `Human Protein Atlas <https://www.proteinatlas.org/>`__
+    and making renamed copies. The :py:func:`download_file` function
+    is used to download the first image of each color
+
     """
     def __abs__(self):
         """
+        Constructor
 
-        :return:
         """
         super().__init__()
         warnings.warn('This downloader generates FAKE images\n'
                       'You have been warned!!!\n'
                       'Have a nice day')
 
     def download_images(self, download_list=None):
         """
         Downloads 1st image from server and then
         and makes renamed copies for subsequent images
 
         :param download_list:
+        :type download_list: list of tuple
         :return:
         """
         num_to_download = len(download_list)
         logger.info(str(num_to_download) + ' images to download')
         t = tqdm(total=num_to_download, desc='Download',
                  unit='images')
 
@@ -130,37 +150,64 @@
             shutil.copy(src_image_dict[color], entry[1])
         return []
 
 
 class MultiProcessImageDownloader(ImageDownloader):
     """
     Uses multiprocess package to download images in parallel
+
     """
 
     def __init__(self, poolsize=4, skip_existing=False,
                  override_dfunc=None):
         """
         Constructor
+
+        .. warning::
+
+            Exceeding **poolsize** of ``4`` causes errors from Human Protein Atlas site
+
+        :param poolsize: Number of concurrent downloaders to use.
+        :type poolsize: int
+        :param skip_existing: If ``True`` skip download if image file exists and has size
+                              greater then ``0``
+        :type skip_existing: bool
+        :param override_dfunc: Function that takes a tuple `(image URL, download str path)`
+                               and downloads the image. If ``None`` :py:func:`download_file`
+                               function is used
+        :type override_dfunc: :py:class:`function`
         """
         super().__init__()
         self._poolsize = poolsize
         if override_dfunc is not None:
             self._dfunc = override_dfunc
         else:
             self._dfunc = download_file
             if skip_existing is True:
                 self._dfunc = download_file_skip_existing
 
     def download_images(self, download_list=None):
         """
         Downloads images returning a list of failed downloads
 
-        :param download_list:
-        :return: of tuples (`http status code`, `text of error`, (`link`, `destfile`))
-        :rtype: list
+        .. code-block::
+
+            from cellmaps_imagedownloader.runner import MultiProcessImageDownloader
+
+            dloader = MultiProcessImageDownloader(poolsize=2)
+
+            d_list = [('https://images.proteinatlas.org/992/1_A1_1_red.jpg',
+                       '/tmp/1_A1_1_red.jpg')]
+            failed = dloader.download_images(download_list=d_list)
+
+        :param download_list: Each tuple of format `(image URL, dest file path)`
+        :type download_list: list of tuple
+        :return: Failed downloads, format of tuple
+                 (`http status code`, `text of error`, (`link`, `destfile`))
+        :rtype: list of tuple
         """
         failed_downloads = []
         logger.debug('Poolsize for image downloader set to: ' +
                      str(self._poolsize))
         with Pool(processes=self._poolsize) as pool:
             num_to_download = len(download_list)
             logger.info(str(num_to_download) + ' images to download')
@@ -174,26 +221,19 @@
                         logger.debug('Failed download: ' + str(i))
                     failed_downloads.append(i)
         return failed_downloads
 
 
 class CellmapsImageDownloader(object):
     """
-    Class to run algorithm
-    """
-    SAMPLES_CSVFILE = 'samples.csv'
-    """
-    Copy of input csv file that is stored in output
-    directory by the :py:meth:`~cellmaps_imagedownloader.runner.CellmapsImageDownloader.run`
-    """
+    Downloads Immunofluorescent images from
+    `Human Protein Atlas <https://www.proteinatlas.org>`__
+    storing them in an output directory that is locally
+    registered as an `RO-Crate <https://www.researchobject.org/ro-crate>`__
 
-    UNIQUE_CSVFILE = 'unique.csv'
-    """
-    Copy of input csv file that is stored in output
-    directory by the :py:meth:`~cellmaps_imagedownloader.runner.CellmapsImageDownloader.run`
     """
 
     SAMPLES_FILEKEY = 'samples'
     UNIQUE_FILEKEY = 'unique'
 
     def __init__(self, outdir=None,
                  imgsuffix='.jpg',
@@ -212,22 +252,26 @@
         :type outdir: str
         :param imgsuffix: suffix to append to image file names
         :type imgsuffix: str
         :param imagedownloader: object that will perform image downloads
         :type imagedownloader: :py:class:`~cellmaps_downloader.runner.ImageDownloader`
         :param imagegen: gene node attribute generator for IF image data
         :type imagegen: :py:class:`~cellmaps_imagedownloader.gene.ImageGeneNodeAttributeGenerator`
-        :param image_url: Base URL for image download
+        :param image_url: Base URL for image download from Human Protein Atlas
         :type image_url: str
-        :param skip_logging:
+        :param skip_logging: If ``True`` skip logging
         :type skip_logging: bool
         :param provenance:
         :type provenance: dict
         :param input_data_dict:
         :type input_data_dict: dict
+        :param provenance_utils: Wrapper for `fairscape-cli <https://pypi.org/project/fairscape-cli>`__
+                                 which is used for
+                                 `RO-Crate <https://www.researchobject.org/ro-crate>`__ creation and population
+        :type provenance_utils: :py:class:`~cellmaps_utils.provenance.ProvenanceUtil`
         """
         if outdir is None:
             raise CellMapsImageDownloaderError('outdir is None')
         self._outdir = os.path.abspath(outdir)
         self._imagedownloader = imagedownloader
         self._imgsuffix = imgsuffix
         self._start_time = int(time.time())
@@ -285,22 +329,21 @@
         Creates output directory if it does not already exist
 
         :raises CellmapsDownloaderError: If output directory is None or if directory already exists
         """
         if os.path.isdir(self._outdir):
             raise CellMapsImageDownloaderError(self._outdir + ' already exists')
 
+        os.makedirs(self._outdir, mode=0o755)
         for cur_color in constants.COLORS:
             cdir = os.path.join(self._outdir, cur_color)
             if not os.path.isdir(cdir):
                 logger.debug('Creating directory: ' + cdir)
                 os.makedirs(cdir,
                             mode=0o755)
-            else:
-                logger.debug(cdir + ' already exists')
 
     def _register_software(self):
         """
         Registers this tool
 
         :raises CellMapsProvenanceError: If fairscape call fails
         """
@@ -517,14 +560,15 @@
         logger.debug('Failed download counts by http error code: ' + str(error_code_map))
         return self._imagedownloader.download_images(downloads_to_retry)
 
     def _download_images(self, max_retry=5):
         """
         Uses downloader specified in constructor to download images noted in
         tsvfile file also specified in constructor
+
         :raises CellMapsImageDownloaderError: if image downloader is ``None`` or
                                          if there are failed downloads
         :return: 0 upon success otherwise, failure
         :rtype: int
         """
         if self._imagedownloader is None:
             raise CellMapsImageDownloaderError('Image downloader is None')
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/cellmaps_imagedownloader.egg-info/PKG-INFO` & `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-imagedownloader
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Downloads IF data needed for CM4AI MuSIC pipeline
 Home-page: https://github.com/idekerlab/cellmaps_imagedownloader
 Author: Gege Qian
 Author-email: geqian@ucsd.edu
 License: MIT license
 Description: =========================
         cellmaps_imagedownloader
@@ -18,28 +18,25 @@
             :target: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader
         
         .. image:: https://readthedocs.org/projects/cellmaps-downloader/badge/?version=latest
                 :target: https://cellmaps-imagedownloader.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        
-        
         Downloads IF data needed for CM4AI MuSIC pipeline
         
         
         * Free software: MIT license
         * Documentation: https://cellmaps-imagedownloader.readthedocs.io.
         
         
         Dependencies
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
-        * `fairscape-cli <https://pypi.org/project/fairscape-cli>`__
         * `requests <https://pypi.org/project/requests>`__
         * `mygene <https://pypi.org/project/mygene>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         
         Compatibility
         -------------
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/Makefile` & `cellmaps_imagedownloader-0.1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/cellmaps_downloader.rst` & `cellmaps_imagedownloader-0.1.0a5/docs/cellmaps_imagedownloader.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 cellmaps\_imagedownloader package
-===================================
+=================================
 
 Submodules
 ----------
 
-cellmaps\_imagedownloader.cellmaps\_downloadercmd module
-----------------------------------------------------------
+cellmaps\_imagedownloader.cellmaps\_imagedownloadercmd module
+-------------------------------------------------------------
 
 .. automodule:: cellmaps_imagedownloader.cellmaps_imagedownloadercmd
    :members:
    :undoc-members:
    :show-inheritance:
 
 cellmaps\_imagedownloader.exceptions module
-----------------------------------------------
+-------------------------------------------
 
 .. automodule:: cellmaps_imagedownloader.exceptions
    :members:
    :undoc-members:
    :show-inheritance:
 
 cellmaps\_imagedownloader.gene module
----------------------------------------
+-------------------------------------
 
 .. automodule:: cellmaps_imagedownloader.gene
    :members:
    :undoc-members:
    :show-inheritance:
 
 cellmaps\_imagedownloader.runner module
-------------------------------------------
+---------------------------------------
 
 .. automodule:: cellmaps_imagedownloader.runner
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/conf.py` & `cellmaps_imagedownloader-0.1.0a5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
               'sphinx.ext.viewcode']
 
 # intersphinx mapping
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None),
                        "requests": ("https://requests.readthedocs.io/en/latest/", None),
                        "networkx": ("http://networkx.org/documentation/stable/", None),
                        "pandas": ("https://pandas.pydata.org/docs/", None),
-                       "numpy": ("https://numpy.org/doc/stable/", None)
+                       "numpy": ("https://numpy.org/doc/stable/", None),
+                       "cellmaps_utils": ("https://cellmaps_utils.readthedocs.io/en/latest/", None)
                       }
 
 # prefix document on section labels for references
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/installation.rst` & `cellmaps_imagedownloader-0.1.0a5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/make.bat` & `cellmaps_imagedownloader-0.1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/newrelease.rst` & `cellmaps_imagedownloader-0.1.0a5/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/pypircfile.rst` & `cellmaps_imagedownloader-0.1.0a5/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/usage.rst` & `cellmaps_imagedownloader-0.1.0a5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/docs/versioningscheme.rst` & `cellmaps_imagedownloader-0.1.0a5/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/setup.py` & `cellmaps_imagedownloader-0.1.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/tests/test_cellmaps_imagedownloadercmd.py` & `cellmaps_imagedownloader-0.1.0a5/tests/test_cellmaps_imagedownloadercmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/tests/test_cellmapsimagedownloader.py` & `cellmaps_imagedownloader-0.1.0a5/tests/test_cellmapsimagedownloader.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/tests/test_genenodegenerator.py` & `cellmaps_imagedownloader-0.1.0a5/tests/test_genenodegenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/tests/test_genequery.py` & `cellmaps_imagedownloader-0.1.0a5/tests/test_genequery.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,25 @@
                               fields=['field1'],
                               species='human')
         self.assertEqual({}, res)
         mockquery.querymany.assert_called_once_with(['hi'], scopes='thescope',
                                                     fields=['field1'],
                                                     species='human')
 
+    def test_get_symbols_for_genes(self):
+        mockquery = MagicMock()
+
+        mockquery.querymany = MagicMock(return_value={})
+        query = GeneQuery(mygeneinfo=mockquery)
+        res = query.get_symbols_for_genes(genelist=['g1'])
+        self.assertEqual({}, res)
+        mockquery.querymany.assert_called_once_with(['g1'], scopes='_id',
+                                                    fields=['ensembl.gene', 'symbol'],
+                                                    species='human')
+
     @unittest.skipUnless(os.getenv('CELLMAPS_DOWNLOADER_INTEGRATION_TEST') is not None, SKIP_REASON)
     def test_simple_query(self):
         query = GeneQuery()
         res = query.querymany([2, 16], scopes='_id', species='human',
                               fields=['ensembl.gene','symbol'])
         self.assertEqual(2, len(res))
         for entry in res:
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/tests/test_imagegenenodegenerator.py` & `cellmaps_imagedownloader-0.1.0a5/tests/test_imagegenenodegenerator.py`

 * *Files 24% similar despite different names*

```diff
@@ -116,93 +116,14 @@
                                 'locations': 'CA2', 'n_location': '2'},
                                {'antibody': 'GHI',
                                 'ensembl_ids': 'ENSG00000172137',
                                 'gene_names': 'DLG4', 'atlas_name': 'Brain',
                                 'locations': 'CA3', 'n_location': '3'}]
             self.assertEqual(result, expected_result)
 
-    def test_write_samples_as_csvfile(self):
-        temp_dir = tempfile.mkdtemp()
-        try:
-            # test write when samples is None
-            try:
-                imagegen = ImageGeneNodeAttributeGenerator()
-                imagegen.write_samples_as_csvfile(os.path.join(temp_dir, 'foo.csv'))
-                self.fail('Expected exception')
-            except CellMapsImageDownloaderError as ce:
-                self.assertEqual('samples list is None', str(ce))
-
-                # test with empty samples
-                imagegen = ImageGeneNodeAttributeGenerator(samples_list=[])
-                out_file = os.path.join(temp_dir, 'emptyfile.csv')
-                imagegen.write_samples_as_csvfile(outfile=os.path.join(temp_dir, out_file))
-
-                with open(out_file, 'r') as f:
-                    data = f.read()
-                    self.assertEqual(','.join(ImageGeneNodeAttributeGenerator.SAMPLES_HEADER_COLS) + '\n', data)
-
-                # test with a row
-                sample = {}
-                for key in ImageGeneNodeAttributeGenerator.SAMPLES_HEADER_COLS:
-                    sample[key] = key + '_' + str(len(key))
-
-                imagegen = ImageGeneNodeAttributeGenerator(samples_list=[sample])
-                one_line_file = os.path.join(temp_dir, 'oneline.csv')
-                imagegen.write_samples_as_csvfile(outfile=os.path.join(temp_dir, one_line_file))
-
-                with open(one_line_file, 'r') as f:
-                    data = f.readline()
-                    self.assertEqual(','.join(ImageGeneNodeAttributeGenerator.SAMPLES_HEADER_COLS) + '\n', data)
-                    data = f.readline()
-                    self.assertEqual('filename_8,if_plate_id_11,position_8,'
-                                     'sample_6,status_6,locations_9,'
-                                     'antibody_8,ensembl_ids_11,'
-                                     'gene_names_10\n', data)
-        finally:
-            shutil.rmtree(temp_dir)
-
-    def test_write_unique_list_as_csvfile(self):
-        temp_dir = tempfile.mkdtemp()
-        try:
-            # test write when samples is None
-            try:
-                imagegen = ImageGeneNodeAttributeGenerator()
-                imagegen.write_unique_list_as_csvfile(os.path.join(temp_dir, 'foo.csv'))
-                self.fail('Expected exception')
-            except CellMapsImageDownloaderError as ce:
-                self.assertEqual('unique list is None', str(ce))
-
-                # test with empty unique
-                imagegen = ImageGeneNodeAttributeGenerator(unique_list=[])
-                out_file = os.path.join(temp_dir, 'emptyfile.csv')
-                imagegen.write_unique_list_as_csvfile(outfile=os.path.join(temp_dir, out_file))
-
-                with open(out_file, 'r') as f:
-                    data = f.read()
-                    self.assertEqual(','.join(ImageGeneNodeAttributeGenerator.UNIQUE_HEADER_COLS) + '\n', data)
-
-                # test with a row
-                unique = {}
-                for key in ImageGeneNodeAttributeGenerator.UNIQUE_HEADER_COLS:
-                    unique[key] = key + '_' + str(len(key))
-
-                imagegen = ImageGeneNodeAttributeGenerator(unique_list=[unique])
-                one_line_file = os.path.join(temp_dir, 'oneline.csv')
-                imagegen.write_unique_list_as_csvfile(outfile=os.path.join(temp_dir, one_line_file))
-
-                with open(one_line_file, 'r') as f:
-                    data = f.readline()
-                    self.assertEqual(','.join(ImageGeneNodeAttributeGenerator.UNIQUE_HEADER_COLS) + '\n', data)
-                    data = f.readline()
-                    self.assertEqual('antibody_8,ensembl_ids_11,'
-                                     'gene_names_10,atlas_name_10,'
-                                     'locations_9,n_location_10\n', data)
-        finally:
-            shutil.rmtree(temp_dir)
-
     def test_get_set_of_antibodies_from_unique_list(self):
         # try with None for unique list
         try:
             imagegen = ImageGeneNodeAttributeGenerator()
             imagegen._get_set_of_antibodies_from_unique_list()
             self.fail('Expected Exception')
         except CellMapsImageDownloaderError as ce:
```

### Comparing `cellmaps_imagedownloader-0.1.0a4/tests/test_integration_cellmaps_downloader.py` & `cellmaps_imagedownloader-0.1.0a5/tests/test_integration_cellmaps_downloader.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a4/tests/test_multiprocessimagedownloader.py` & `cellmaps_imagedownloader-0.1.0a5/tests/test_multiprocessimagedownloader.py`

 * *Files identical despite different names*

