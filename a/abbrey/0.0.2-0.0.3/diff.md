# Comparing `tmp/abbrey-0.0.2.tar.gz` & `tmp/abbrey-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abbrey-0.0.2.tar", last modified: Tue May 23 04:32:36 2023, max compression
+gzip compressed data, was "abbrey-0.0.3.tar", last modified: Tue May 23 04:38:41 2023, max compression
```

## Comparing `abbrey-0.0.2.tar` & `abbrey-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:32:36.367399 abbrey-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-23 04:32:26.000000 abbrey-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:32:36.371399 abbrey-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 04:32:26.000000 abbrey-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:32:36.367399 abbrey-0.0.2/abbrey/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 04:32:26.000000 abbrey-0.0.2/abbrey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62788 2023-05-23 04:32:26.000000 abbrey-0.0.2/abbrey/acronyms_ver0.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-23 04:32:26.000000 abbrey-0.0.2/abbrey/decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:32:36.367399 abbrey-0.0.2/abbrey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 04:32:36.371399 abbrey-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 04:32:26.000000 abbrey-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:38:41.598154 abbrey-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-23 04:38:29.000000 abbrey-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:38:41.598154 abbrey-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 04:38:29.000000 abbrey-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:38:41.598154 abbrey-0.0.3/abbrey/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 04:38:29.000000 abbrey-0.0.3/abbrey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62788 2023-05-23 04:38:29.000000 abbrey-0.0.3/abbrey/acronyms_ver0.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-23 04:38:29.000000 abbrey-0.0.3/abbrey/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:38:41.598154 abbrey-0.0.3/abbrey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:38:41.000000 abbrey-0.0.3/abbrey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 04:38:41.598154 abbrey-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 04:38:29.000000 abbrey-0.0.3/setup.py
```

### Comparing `abbrey-0.0.2/LICENSE.txt` & `abbrey-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abbrey-0.0.2/PKG-INFO` & `abbrey-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abbrey
-Version: 0.0.2
+Version: 0.0.3
 Summary: Abbreviation decoder
 Author: pdd
 Author-email: dungphamdang99@gmail.com
 License: MIT
 Keywords: abbreviation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `abbrey-0.0.2/abbrey/acronyms_ver0.1.csv` & `abbrey-0.0.3/abbrey/acronyms_ver0.1.csv`

 * *Files identical despite different names*

### Comparing `abbrey-0.0.2/abbrey/decoder.py` & `abbrey-0.0.3/abbrey/decoder.py`

 * *Files identical despite different names*

### Comparing `abbrey-0.0.2/abbrey.egg-info/PKG-INFO` & `abbrey-0.0.3/abbrey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abbrey
-Version: 0.0.2
+Version: 0.0.3
 Summary: Abbreviation decoder
 Author: pdd
 Author-email: dungphamdang99@gmail.com
 License: MIT
 Keywords: abbreviation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `abbrey-0.0.2/setup.py` & `abbrey-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="abbrey",
     packages=["abbrey"],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     description="Abbreviation decoder",
     author="pdd",
     author_email="dungphamdang99@gmail.com",
     # url="https://github.com/user/reponame",  # TODO
     # download_url="https://github.com/user/reponame/archive/v_01.tar.gz",  # TODO
     keywords=["abbreviation"],
```

