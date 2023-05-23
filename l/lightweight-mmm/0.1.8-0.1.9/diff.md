# Comparing `tmp/lightweight_mmm-0.1.8.tar.gz` & `tmp/lightweight_mmm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_mmm-0.1.8.tar", last modified: Tue May  2 14:40:41 2023, max compression
+gzip compressed data, was "lightweight_mmm-0.1.9.tar", last modified: Tue May 23 21:24:16 2023, max compression
```

## Comparing `lightweight_mmm-0.1.8.tar` & `lightweight_mmm-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:40:41.481279 lightweight_mmm-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-02 14:40:41.481279 lightweight_mmm-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:40:41.477279 lightweight_mmm-0.1.8/lightweight_mmm/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:40:41.477279 lightweight_mmm-0.1.8/lightweight_mmm/core/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:40:41.477279 lightweight_mmm-0.1.8/lightweight_mmm/core/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/baseline/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/baseline/intercept_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/core_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/core_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:40:41.481279 lightweight_mmm-0.1.8/lightweight_mmm/core/time/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/time/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/time/seasonality_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/time/trend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/time/trend_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:40:41.481279 lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/lagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/lagging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/saturation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27388 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/lightweight_mmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/lightweight_mmm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/media_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/media_transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/optimize_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/optimize_media_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    57242 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/plot_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38304 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/lightweight_mmm/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:40:41.477279 lightweight_mmm-0.1.8/lightweight_mmm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-02 14:40:41.000000 lightweight_mmm-0.1.8/lightweight_mmm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-02 14:40:41.000000 lightweight_mmm-0.1.8/lightweight_mmm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:40:41.000000 lightweight_mmm-0.1.8/lightweight_mmm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-02 14:40:41.000000 lightweight_mmm-0.1.8/lightweight_mmm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 14:40:41.000000 lightweight_mmm-0.1.8/lightweight_mmm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:40:41.481279 lightweight_mmm-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-02 14:40:28.000000 lightweight_mmm-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:16.651072 lightweight_mmm-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-23 21:24:16.651072 lightweight_mmm-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:16.647072 lightweight_mmm-0.1.9/lightweight_mmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:16.651072 lightweight_mmm-0.1.9/lightweight_mmm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:16.651072 lightweight_mmm-0.1.9/lightweight_mmm/core/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/baseline/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/baseline/intercept_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/core_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/core_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:16.651072 lightweight_mmm-0.1.9/lightweight_mmm/core/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/time/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/time/seasonality_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/time/trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/time/trend_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:16.651072 lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/lagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/lagging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/saturation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27355 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/lightweight_mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/lightweight_mmm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/media_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/media_transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/optimize_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/optimize_media_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57242 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/plot_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38304 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/lightweight_mmm/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:16.647072 lightweight_mmm-0.1.9/lightweight_mmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-23 21:24:16.000000 lightweight_mmm-0.1.9/lightweight_mmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-23 21:24:16.000000 lightweight_mmm-0.1.9/lightweight_mmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:24:16.000000 lightweight_mmm-0.1.9/lightweight_mmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-23 21:24:16.000000 lightweight_mmm-0.1.9/lightweight_mmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 21:24:16.000000 lightweight_mmm-0.1.9/lightweight_mmm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:24:16.651072 lightweight_mmm-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-23 21:24:05.000000 lightweight_mmm-0.1.9/setup.py
```

### Comparing `lightweight_mmm-0.1.8/LICENSE` & `lightweight_mmm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/PKG-INFO` & `lightweight_mmm-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight_mmm
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for Media-Mix-Modelling
 Home-page: https://github.com/google/lightweight_mmm
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lightweight_mmm-0.1.8/README.md` & `lightweight_mmm-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/__init__.py` & `lightweight_mmm-0.1.9/lightweight_mmm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 
 """LightweightMMM library.
 
 Detailed documentation and examples can be found in the
 [Github repository](https://github.com/google/lightweight_mmm).
 """
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/conftest.py` & `lightweight_mmm-0.1.9/lightweight_mmm/conftest.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/__init__.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/baseline/__init__.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/baseline/__init__.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/baseline/intercept.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/baseline/intercept.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/baseline/intercept_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/baseline/intercept_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/core_utils.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/core_utils.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/core_utils_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/core_utils_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/priors.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/priors.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/time/__init__.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/time/__init__.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/time/seasonality.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/time/seasonality.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/time/seasonality_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/time/seasonality_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/time/trend.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/time/trend.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/time/trend_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/time/trend_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/__init__.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/identity.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/identity.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/lagging.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/lagging.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/lagging_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/lagging_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/saturation.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/saturation.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/core/transformations/saturation_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/core/transformations/saturation_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/lightweight_mmm.py` & `lightweight_mmm-0.1.9/lightweight_mmm/lightweight_mmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,25 +92,26 @@
 
   # This is pretty strict but LMMM classes don't need to compare equal unless
   # they are exact copies.
   if type(item_1) != type(item_2):
     is_equal = False
   elif isinstance(item_1, str):
     is_equal = item_1 == item_2
-  elif isinstance(item_1, (jax.Array, np.ndarray, Sequence)):
-    if all(isinstance(x, str) for x in item_1) and all(
-        isinstance(x, str) for x in item_2):
-      is_equal = item_1 == item_2
-    else:
-      is_equal = np.array_equal(item_1, item_2, equal_nan=True)
+  elif isinstance(item_1, (jax.Array, np.ndarray)) or (
+      isinstance(item_1, Sequence)
+      and not all(isinstance(x, str) for x in item_1)
+  ):
+    is_equal = np.array_equal(item_1, item_2, equal_nan=True)
   elif isinstance(item_1, MutableMapping):
-    is_equal = all([
-        _compare_equality_for_lmmm(item_1[x], item_2[x])
-        for x in item_1.keys() | item_2.keys()
-    ])
+    is_equal = all(
+        [
+            _compare_equality_for_lmmm(item_1[x], item_2[x])
+            for x in item_1.keys() | item_2.keys()
+        ]
+    )
   else:
     is_equal = item_1 == item_2
 
   return is_equal
 
 
 class NotFittedModelError(Exception):
```

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/lightweight_mmm_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/lightweight_mmm_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,20 +451,16 @@
 
     if expected_equal:
       self.assertEqual(carryover_mmm, other_mmm)
     else:
       self.assertNotEqual(carryover_mmm, other_mmm)
 
   @parameterized.named_parameters([
-      dict(
-          testcase_name="national_mmm",
-          media_mix_model="national_mmm"),
-      dict(
-          testcase_name="geo_mmm",
-          media_mix_model="geo_mmm"),
+      dict(testcase_name="national_mmm", media_mix_model="national_mmm"),
+      dict(testcase_name="geo_mmm", media_mix_model="geo_mmm"),
   ])
   def test_fitted_mmm_does_not_equal_default_mmm(self, media_mix_model):
     default_mmm_object = lightweight_mmm.LightweightMMM()
     fitted_mmm_object = getattr(self, media_mix_model)
     self.assertNotEqual(default_mmm_object, fitted_mmm_object)
 
 if __name__ == "__main__":
```

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/media_transforms.py` & `lightweight_mmm-0.1.9/lightweight_mmm/media_transforms.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/media_transforms_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/media_transforms_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/models.py` & `lightweight_mmm-0.1.9/lightweight_mmm/models.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/models_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/models_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/optimize_media.py` & `lightweight_mmm-0.1.9/lightweight_mmm/optimize_media.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/optimize_media_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/optimize_media_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/plot.py` & `lightweight_mmm-0.1.9/lightweight_mmm/plot.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/plot_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/plot_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/preprocessing.py` & `lightweight_mmm-0.1.9/lightweight_mmm/preprocessing.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/preprocessing_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/utils.py` & `lightweight_mmm-0.1.9/lightweight_mmm/utils.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm/utils_test.py` & `lightweight_mmm-0.1.9/lightweight_mmm/utils_test.py`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm.egg-info/PKG-INFO` & `lightweight_mmm-0.1.9/lightweight_mmm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight-mmm
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for Media-Mix-Modelling
 Home-page: https://github.com/google/lightweight_mmm
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lightweight_mmm-0.1.8/lightweight_mmm.egg-info/SOURCES.txt` & `lightweight_mmm-0.1.9/lightweight_mmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightweight_mmm-0.1.8/setup.py` & `lightweight_mmm-0.1.9/setup.py`

 * *Files identical despite different names*

