# Comparing `tmp/ebeer-0.0.17.tar.gz` & `tmp/ebeer-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.17.tar", last modified: Mon May 22 18:36:36 2023, max compression
+gzip compressed data, was "ebeer-0.0.18.tar", last modified: Mon May 22 22:27:59 2023, max compression
```

## Comparing `ebeer-0.0.17.tar` & `ebeer-0.0.18.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:36:36.233986 ebeer-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 18:35:31.000000 ebeer-0.0.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 18:35:31.000000 ebeer-0.0.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 18:36:36.233986 ebeer-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 18:35:31.000000 ebeer-0.0.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-22 18:35:31.000000 ebeer-0.0.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:36:36.233986 ebeer-0.0.17/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:36:36.225986 ebeer-0.0.17/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 18:35:31.000000 ebeer-0.0.17/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:36:36.225986 ebeer-0.0.17/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 18:35:31.000000 ebeer-0.0.17/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-22 18:35:31.000000 ebeer-0.0.17/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-22 18:35:31.000000 ebeer-0.0.17/src/ebeer/label_index.py
--rw-r--r--   0 runner    (1001) docker     (123)  6684424 2023-05-22 18:35:31.000000 ebeer-0.0.17/src/ebeer/trained_model.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:36:36.233986 ebeer-0.0.17/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 18:36:36.000000 ebeer-0.0.17/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 18:36:36.000000 ebeer-0.0.17/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:36:36.000000 ebeer-0.0.17/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 18:36:36.000000 ebeer-0.0.17/src/ebeer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 18:36:36.000000 ebeer-0.0.17/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:36:36.233986 ebeer-0.0.17/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-22 18:35:31.000000 ebeer-0.0.17/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.690166 ebeer-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 22:26:45.000000 ebeer-0.0.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 22:26:45.000000 ebeer-0.0.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 22:27:59.690166 ebeer-0.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 22:26:45.000000 ebeer-0.0.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-22 22:26:45.000000 ebeer-0.0.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:27:59.690166 ebeer-0.0.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.682165 ebeer-0.0.18/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.682165 ebeer-0.0.18/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/label_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)  6684424 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/trained_model.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.690166 ebeer-0.0.18/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.690166 ebeer-0.0.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-22 22:26:45.000000 ebeer-0.0.18/tests/test_classify.py
```

### Comparing `ebeer-0.0.17/LICENSE` & `ebeer-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.17/PKG-INFO` & `ebeer-0.0.18/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebeer
-Version: 0.0.17
+Version: 0.0.18
 Summary: CNN Trained to predict brazilian beers
 Author-email: diego vasque maldonado <diegoomal13@gmail.com>
 Project-URL: Homepage, https://github.com/Diegoomal/proj_integrado_trabalho_final
 Project-URL: Bug Tracker, https://github.com/Diegoomal/proj_integrado_trabalho_final/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ebeer-0.0.17/pyproject.toml` & `ebeer-0.0.18/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 requires = [
     "setuptools>=61.0", "wheel", "build"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ebeer"
-version = "0.0.17"
+version = "0.0.18"
 authors = [
     { name="diego vasque maldonado", email="diegoomal13@gmail.com" }
 ]
 description = "CNN Trained to predict brazilian beers"
 readme = "src/README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy", "tensorflow", "Pillow"
+    "numpy", "tensorflow", "Pillow", "importlib_resources"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Diegoomal/proj_integrado_trabalho_final"
 "Bug Tracker" = "https://github.com/Diegoomal/proj_integrado_trabalho_final/issues"
```

### Comparing `ebeer-0.0.17/src/ebeer/beer_classifier.py` & `ebeer-0.0.18/src/ebeer/beer_classifier.py`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.17/src/ebeer/label_index.py` & `ebeer-0.0.18/src/ebeer/label_index.py`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.17/src/ebeer/trained_model.h5` & `ebeer-0.0.18/src/ebeer/trained_model.h5`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.17/src/ebeer.egg-info/PKG-INFO` & `ebeer-0.0.18/src/ebeer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebeer
-Version: 0.0.17
+Version: 0.0.18
 Summary: CNN Trained to predict brazilian beers
 Author-email: diego vasque maldonado <diegoomal13@gmail.com>
 Project-URL: Homepage, https://github.com/Diegoomal/proj_integrado_trabalho_final
 Project-URL: Bug Tracker, https://github.com/Diegoomal/proj_integrado_trabalho_final/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ebeer-0.0.17/tests/test_classify.py` & `ebeer-0.0.18/tests/test_classify.py`

 * *Files identical despite different names*

