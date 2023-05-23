# Comparing `tmp/cellxgene_census-1.0.1.tar.gz` & `tmp/cellxgene_census-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.0.1.tar", last modified: Wed May 10 19:26:28 2023, max compression
+gzip compressed data, was "cellxgene_census-1.0.2.tar", last modified: Tue May 23 01:31:00 2023, max compression
```

## Comparing `cellxgene_census-1.0.1.tar` & `cellxgene_census-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:26:28.492627 cellxgene_census-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-10 19:26:28.492627 cellxgene_census-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:26:28.488627 cellxgene_census-1.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 19:26:28.492627 cellxgene_census-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:26:28.488627 cellxgene_census-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:26:28.488627 cellxgene_census-1.0.1/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:26:28.488627 cellxgene_census-1.0.1/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-10 19:26:28.000000 cellxgene_census-1.0.1/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-10 19:26:28.000000 cellxgene_census-1.0.1/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:26:28.000000 cellxgene_census-1.0.1/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 19:26:28.000000 cellxgene_census-1.0.1/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 19:26:28.000000 cellxgene_census-1.0.1/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:26:28.492627 cellxgene_census-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-10 19:26:12.000000 cellxgene_census-1.0.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.613107 cellxgene_census-1.0.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.613107 cellxgene_census-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.617107 cellxgene_census-1.0.2/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.617107 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 01:31:00.000000 cellxgene_census-1.0.2/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:31:00.621107 cellxgene_census-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25092 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 01:30:44.000000 cellxgene_census-1.0.2/tests/test_util.py
```

### Comparing `cellxgene_census-1.0.1/LICENSE` & `cellxgene_census-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/PKG-INFO` & `cellxgene_census-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.0.1
+Version: 1.0.2
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.0.1/README.md` & `cellxgene_census-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/pyproject.toml` & `cellxgene_census-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,23 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies= [
     # NOTE: the tiledbsoma version must be >= to the version used in the Census builder, to
     # ensure that the assets are readable (tiledbsoma supports backward compatible reading).
     # Make sure this version does not fall behind the builder's tiledbsoma version.
-    "tiledbsoma==1.2.3",
+    "tiledbsoma==1.2.4",
     "anndata",
     "numpy>=1.21,<1.24",  # numpy is constrained by numba and the old pip solver
     "requests",
     "typing_extensions",
     "s3fs",
     "scipy",
     # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
     "certifi",
-    # Temporary fix for https://github.com/single-cell-data/TileDB-SOMA/issues/1322, remove when we update to tiledbsoma>1.2.2
-    "tiledb",
 ]
 
 [project.urls]
 homepage = "https://github.com/chanzuckerberg/cellxgene-census"
 repository = "https://github.com/chanzuckerberg/cellxgene-census"
 
 [tool.setuptools.packages.find]
```

### Comparing `cellxgene_census-1.0.1/release_process.md` & `cellxgene_census-1.0.2/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census/__init__.py` & `cellxgene_census-1.0.2/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.0.2/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.0.2/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census/_open.py` & `cellxgene_census-1.0.2/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.0.2/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.0.2/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.0.2/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.0.1
+Version: 1.0.2
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.0.1/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.0.2/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/tests/test_acceptance.py` & `cellxgene_census-1.0.2/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/tests/test_directory.py` & `cellxgene_census-1.0.2/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/tests/test_get_anndata.py` & `cellxgene_census-1.0.2/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/tests/test_get_helpers.py` & `cellxgene_census-1.0.2/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/tests/test_open.py` & `cellxgene_census-1.0.2/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.1/tests/test_util.py` & `cellxgene_census-1.0.2/tests/test_util.py`

 * *Files identical despite different names*

