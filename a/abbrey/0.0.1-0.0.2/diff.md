# Comparing `tmp/abbrey-0.0.1.tar.gz` & `tmp/abbrey-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abbrey-0.0.1.tar", last modified: Tue May 23 04:04:51 2023, max compression
+gzip compressed data, was "abbrey-0.0.2.tar", last modified: Tue May 23 04:32:36 2023, max compression
```

## Comparing `abbrey-0.0.1.tar` & `abbrey-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 04:04:51.011231 abbrey-0.0.1/
--rw-rw-r--   0 vmo       (1000) vmo       (1000)     1172 2023-05-23 03:34:57.000000 abbrey-0.0.1/LICENSE.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      745 2023-05-23 04:04:51.011231 abbrey-0.0.1/PKG-INFO
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      266 2023-05-23 03:43:36.000000 abbrey-0.0.1/README.md
-drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 04:04:51.011231 abbrey-0.0.1/abbrey/
--rw-rw-r--   0 vmo       (1000) vmo       (1000)       33 2023-05-23 03:51:32.000000 abbrey-0.0.1/abbrey/__init__.py
--rw-rw-r--   0 vmo       (1000) vmo       (1000)    62788 2023-05-23 02:26:41.000000 abbrey-0.0.1/abbrey/acronyms_ver0.1.csv
--rw-rw-r--   0 vmo       (1000) vmo       (1000)     1281 2023-05-23 03:50:47.000000 abbrey-0.0.1/abbrey/decoder.py
-drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 04:04:51.011231 abbrey-0.0.1/abbrey.egg-info/
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      745 2023-05-23 04:04:50.000000 abbrey-0.0.1/abbrey.egg-info/PKG-INFO
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      253 2023-05-23 04:04:50.000000 abbrey-0.0.1/abbrey.egg-info/SOURCES.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)        1 2023-05-23 04:04:50.000000 abbrey-0.0.1/abbrey.egg-info/dependency_links.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)        7 2023-05-23 04:04:50.000000 abbrey-0.0.1/abbrey.egg-info/requires.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)        7 2023-05-23 04:04:50.000000 abbrey-0.0.1/abbrey.egg-info/top_level.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)       79 2023-05-23 04:04:51.011231 abbrey-0.0.1/setup.cfg
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      967 2023-05-23 04:03:44.000000 abbrey-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:32:36.367399 abbrey-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-23 04:32:26.000000 abbrey-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:32:36.371399 abbrey-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 04:32:26.000000 abbrey-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:32:36.367399 abbrey-0.0.2/abbrey/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 04:32:26.000000 abbrey-0.0.2/abbrey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62788 2023-05-23 04:32:26.000000 abbrey-0.0.2/abbrey/acronyms_ver0.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-23 04:32:26.000000 abbrey-0.0.2/abbrey/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:32:36.367399 abbrey-0.0.2/abbrey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 04:32:36.000000 abbrey-0.0.2/abbrey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 04:32:36.371399 abbrey-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 04:32:26.000000 abbrey-0.0.2/setup.py
```

### Comparing `abbrey-0.0.1/LICENSE.txt` & `abbrey-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abbrey-0.0.1/PKG-INFO` & `abbrey-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abbrey
-Version: 0.0.1
+Version: 0.0.2
 Summary: Abbreviation decoder
 Author: pdd
 Author-email: dungphamdang99@gmail.com
 License: MIT
 Keywords: abbreviation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `abbrey-0.0.1/abbrey/acronyms_ver0.1.csv` & `abbrey-0.0.2/abbrey/acronyms_ver0.1.csv`

 * *Files identical despite different names*

### Comparing `abbrey-0.0.1/abbrey/decoder.py` & `abbrey-0.0.2/abbrey/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,8 +38,7 @@
         """
         tokens = sentence.split(" ")
 
         def _get_abbr_if_any(abbr: str):
             return self.abbr_dict.get(abbr, abbr)
 
         return " ".join(map(_get_abbr_if_any, tokens))
-        return " ".join(map(_get_abbr_if_any, tokens))
```

### Comparing `abbrey-0.0.1/abbrey.egg-info/PKG-INFO` & `abbrey-0.0.2/abbrey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abbrey
-Version: 0.0.1
+Version: 0.0.2
 Summary: Abbreviation decoder
 Author: pdd
 Author-email: dungphamdang99@gmail.com
 License: MIT
 Keywords: abbreviation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `abbrey-0.0.1/setup.py` & `abbrey-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="abbrey",
     packages=["abbrey"],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     description="Abbreviation decoder",
     author="pdd",
     author_email="dungphamdang99@gmail.com",
     # url="https://github.com/user/reponame",  # TODO
     # download_url="https://github.com/user/reponame/archive/v_01.tar.gz",  # TODO
     keywords=["abbreviation"],
```

