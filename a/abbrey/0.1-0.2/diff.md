# Comparing `tmp/abbrey-0.1.tar.gz` & `tmp/abbrey-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abbrey-0.1.tar", last modified: Tue May 23 03:40:32 2023, max compression
+gzip compressed data, was "abbrey-0.2.tar", last modified: Tue May 23 03:44:41 2023, max compression
```

## Comparing `abbrey-0.1.tar` & `abbrey-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 03:40:32.607850 abbrey-0.1/
--rw-rw-r--   0 vmo       (1000) vmo       (1000)     1172 2023-05-23 03:34:57.000000 abbrey-0.1/LICENSE.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      435 2023-05-23 03:40:32.607850 abbrey-0.1/PKG-INFO
--rw-rw-r--   0 vmo       (1000) vmo       (1000)        0 2023-05-23 03:26:11.000000 abbrey-0.1/README.md
-drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 03:40:32.607850 abbrey-0.1/abbrey/
--rw-rw-r--   0 vmo       (1000) vmo       (1000)       31 2023-05-23 03:24:47.000000 abbrey-0.1/abbrey/__init__.py
--rw-rw-r--   0 vmo       (1000) vmo       (1000)     1130 2023-05-23 03:37:56.000000 abbrey-0.1/abbrey/decoder.py
-drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 03:40:32.607850 abbrey-0.1/abbrey.egg-info/
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      435 2023-05-23 03:40:32.000000 abbrey-0.1/abbrey.egg-info/PKG-INFO
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      226 2023-05-23 03:40:32.000000 abbrey-0.1/abbrey.egg-info/SOURCES.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)        1 2023-05-23 03:40:32.000000 abbrey-0.1/abbrey.egg-info/dependency_links.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)        7 2023-05-23 03:40:32.000000 abbrey-0.1/abbrey.egg-info/requires.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)        7 2023-05-23 03:40:32.000000 abbrey-0.1/abbrey.egg-info/top_level.txt
--rw-rw-r--   0 vmo       (1000) vmo       (1000)       79 2023-05-23 03:40:32.607850 abbrey-0.1/setup.cfg
--rw-rw-r--   0 vmo       (1000) vmo       (1000)      708 2023-05-23 03:40:14.000000 abbrey-0.1/setup.py
+drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 03:44:41.083406 abbrey-0.2/
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)     1172 2023-05-23 03:34:57.000000 abbrey-0.2/LICENSE.txt
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)      435 2023-05-23 03:44:41.083406 abbrey-0.2/PKG-INFO
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)      266 2023-05-23 03:43:36.000000 abbrey-0.2/README.md
+drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 03:44:41.083406 abbrey-0.2/abbrey/
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)       31 2023-05-23 03:24:47.000000 abbrey-0.2/abbrey/__init__.py
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)     1130 2023-05-23 03:37:56.000000 abbrey-0.2/abbrey/decoder.py
+drwxrwxr-x   0 vmo       (1000) vmo       (1000)        0 2023-05-23 03:44:41.083406 abbrey-0.2/abbrey.egg-info/
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)      435 2023-05-23 03:44:41.000000 abbrey-0.2/abbrey.egg-info/PKG-INFO
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)      226 2023-05-23 03:44:41.000000 abbrey-0.2/abbrey.egg-info/SOURCES.txt
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)        1 2023-05-23 03:44:41.000000 abbrey-0.2/abbrey.egg-info/dependency_links.txt
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)        7 2023-05-23 03:44:41.000000 abbrey-0.2/abbrey.egg-info/requires.txt
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)        7 2023-05-23 03:44:41.000000 abbrey-0.2/abbrey.egg-info/top_level.txt
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)       79 2023-05-23 03:44:41.083406 abbrey-0.2/setup.cfg
+-rw-rw-r--   0 vmo       (1000) vmo       (1000)      708 2023-05-23 03:44:38.000000 abbrey-0.2/setup.py
```

### Comparing `abbrey-0.1/LICENSE.txt` & `abbrey-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abbrey-0.1/abbrey/decoder.py` & `abbrey-0.2/abbrey/decoder.py`

 * *Files identical despite different names*

### Comparing `abbrey-0.1/setup.py` & `abbrey-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name="abbrey",
     packages=["abbrey"],
-    version="0.1",
+    version="0.2",
     license="MIT",
     description="Abbreivation decoder",
     author="pdd",
     author_email="dungphamdang99@gmail.com",
     # url="https://github.com/user/reponame",  # TODO
     # download_url="https://github.com/user/reponame/archive/v_01.tar.gz",  # TODO
     keywords=["abbreviation"],
```

