# Comparing `tmp/aitomatic-1.2.6.tar.gz` & `tmp/aitomatic-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitomatic-1.2.6.tar", last modified: Thu May 18 12:27:19 2023, max compression
+gzip compressed data, was "aitomatic-1.2.7.tar", last modified: Tue May 23 00:25:13 2023, max compression
```

## Comparing `aitomatic-1.2.6.tar` & `aitomatic-1.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-18 12:27:19.214562 aitomatic-1.2.6/
--rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.2.6/LICENSE
--rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.2.6/MANIFEST.in
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-05-18 12:27:19.214711 aitomatic-1.2.6/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.2.6/README.md
--rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.2.6/pyproject.toml
--rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.2.6/requirements.txt
--rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-05-18 12:27:19.215433 aitomatic-1.2.6/setup.cfg
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-18 12:27:19.193962 aitomatic-1.2.6/src/
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-18 12:27:19.199283 aitomatic-1.2.6/src/aitomatic/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.6/src/aitomatic/__init__.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-18 12:27:19.206299 aitomatic-1.2.6/src/aitomatic/api/
--rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.2.6/src/aitomatic/api/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8709 2023-05-16 01:46:06.000000 aitomatic-1.2.6/src/aitomatic/api/build.py
--rw-r--r--   0 hungvo     (501) staff       (20)     6120 2023-05-04 14:19:17.000000 aitomatic-1.2.6/src/aitomatic/api/client.py
--rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.2.6/src/aitomatic/api/exceptions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.2.6/src/aitomatic/api/model_params.py
--rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.2.6/src/aitomatic/api/tuning_utils.py
--rw-r--r--   0 hungvo     (501) staff       (20)    15755 2023-05-16 01:46:06.000000 aitomatic-1.2.6/src/aitomatic/api/web_model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-18 12:27:19.211952 aitomatic-1.2.6/src/aitomatic/dsl/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.6/src/aitomatic/dsl/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.2.6/src/aitomatic/dsl/arl_conclusions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.2.6/src/aitomatic/dsl/arl_features.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.2.6/src/aitomatic/dsl/arl_handler.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.2.6/src/aitomatic/dsl/arl_rules.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.2.6/src/aitomatic/dsl/utils.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-18 12:27:19.213935 aitomatic-1.2.6/src/aitomatic/objects/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.2.6/src/aitomatic/objects/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-05-04 14:19:17.000000 aitomatic-1.2.6/src/aitomatic/objects/dataset.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.2.6/src/aitomatic/objects/model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-18 12:27:19.201605 aitomatic-1.2.6/src/aitomatic.egg-info/
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-05-18 12:27:19.000000 aitomatic-1.2.6/src/aitomatic.egg-info/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-05-18 12:27:19.000000 aitomatic-1.2.6/src/aitomatic.egg-info/SOURCES.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-05-18 12:27:19.000000 aitomatic-1.2.6/src/aitomatic.egg-info/dependency_links.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-05-18 12:27:19.000000 aitomatic-1.2.6/src/aitomatic.egg-info/requires.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-05-18 12:27:19.000000 aitomatic-1.2.6/src/aitomatic.egg-info/top_level.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-05-16 01:46:06.000000 aitomatic-1.2.6/version.txt
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.231569 aitomatic-1.2.7/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.2.7/LICENSE
+-rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.2.7/MANIFEST.in
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-05-23 00:25:13.232165 aitomatic-1.2.7/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.2.7/README.md
+-rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.2.7/pyproject.toml
+-rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.2.7/requirements.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-05-23 00:25:13.233625 aitomatic-1.2.7/setup.cfg
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.175027 aitomatic-1.2.7/src/
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.186465 aitomatic-1.2.7/src/aitomatic/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/__init__.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.209156 aitomatic-1.2.7/src/aitomatic/api/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8726 2023-05-23 00:24:16.000000 aitomatic-1.2.7/src/aitomatic/api/build.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     6120 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/client.py
+-rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/api/exceptions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/model_params.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/tuning_utils.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    15755 2023-05-16 01:46:06.000000 aitomatic-1.2.7/src/aitomatic/api/web_model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.222824 aitomatic-1.2.7/src/aitomatic/dsl/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_conclusions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_features.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_handler.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_rules.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.2.7/src/aitomatic/dsl/utils.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.228942 aitomatic-1.2.7/src/aitomatic/objects/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.2.7/src/aitomatic/objects/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/objects/dataset.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/objects/model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.191145 aitomatic-1.2.7/src/aitomatic.egg-info/
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/requires.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/top_level.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-05-23 00:24:58.000000 aitomatic-1.2.7/version.txt
```

### Comparing `aitomatic-1.2.6/LICENSE` & `aitomatic-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/PKG-INFO` & `aitomatic-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.6
+Version: 1.2.7
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.6/README.md` & `aitomatic-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/setup.cfg` & `aitomatic-1.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/api/__init__.py` & `aitomatic-1.2.7/src/aitomatic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/api/build.py` & `aitomatic-1.2.7/src/aitomatic/api/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return params
 
     def build_model(
         self,
         model_type: str,
         model_name: str,
         knowledge_name: str,
-        data_name: str,
+        data_name: Optional[str] = None,
         ml_models: List[Any] = [],
         label_columns: Dict[str, Optional[Any]] = {},
         threshold: Any = {},
         membership_error_width: Any = {},
         mapping_data: Any = None,
         metadata: Any = None,
     ):
```

### Comparing `aitomatic-1.2.6/src/aitomatic/api/client.py` & `aitomatic-1.2.7/src/aitomatic/api/client.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/api/model_params.py` & `aitomatic-1.2.7/src/aitomatic/api/model_params.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/api/tuning_utils.py` & `aitomatic-1.2.7/src/aitomatic/api/tuning_utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/api/web_model.py` & `aitomatic-1.2.7/src/aitomatic/api/web_model.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/dsl/arl_conclusions.py` & `aitomatic-1.2.7/src/aitomatic/dsl/arl_conclusions.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/dsl/arl_features.py` & `aitomatic-1.2.7/src/aitomatic/dsl/arl_features.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/dsl/arl_handler.py` & `aitomatic-1.2.7/src/aitomatic/dsl/arl_handler.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/dsl/arl_rules.py` & `aitomatic-1.2.7/src/aitomatic/dsl/arl_rules.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/dsl/utils.py` & `aitomatic-1.2.7/src/aitomatic/dsl/utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/objects/dataset.py` & `aitomatic-1.2.7/src/aitomatic/objects/dataset.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic/objects/model.py` & `aitomatic-1.2.7/src/aitomatic/objects/model.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.6/src/aitomatic.egg-info/PKG-INFO` & `aitomatic-1.2.7/src/aitomatic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.6
+Version: 1.2.7
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.6/src/aitomatic.egg-info/SOURCES.txt` & `aitomatic-1.2.7/src/aitomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

