# Comparing `tmp/watermark-2.4.1.tar.gz` & `tmp/watermark-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watermark-2.4.1.tar", last modified: Tue May 23 16:52:54 2023, max compression
+gzip compressed data, was "watermark-2.4.2.tar", last modified: Tue May 23 19:00:07 2023, max compression
```

## Comparing `watermark-2.4.1.tar` & `watermark-2.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 16:52:54.721265 watermark-2.4.1/
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1507 2023-05-23 16:50:16.000000 watermark-2.4.1/LICENSE
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       58 2023-05-23 16:50:46.000000 watermark-2.4.1/MANIFEST.in
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 16:52:54.721344 watermark-2.4.1/PKG-INFO
--rw-r--r--   0 sebastianraschka   (501) staff       (20)    11591 2023-05-23 16:50:16.000000 watermark-2.4.1/README.md
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       55 2023-05-23 16:50:16.000000 watermark-2.4.1/requirements.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      512 2023-05-23 16:52:54.721611 watermark-2.4.1/setup.cfg
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1476 2023-05-23 16:50:16.000000 watermark-2.4.1/setup.py
-drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 16:52:54.720444 watermark-2.4.1/watermark/
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      373 2023-05-23 16:50:16.000000 watermark-2.4.1/watermark/__init__.py
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     3842 2023-05-23 16:50:16.000000 watermark-2.4.1/watermark/magic.py
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      291 2023-05-23 16:50:16.000000 watermark-2.4.1/watermark/version.py
--rw-r--r--   0 sebastianraschka   (501) staff       (20)    10070 2023-05-23 16:50:16.000000 watermark-2.4.1/watermark/watermark.py
-drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 16:52:54.721151 watermark-2.4.1/watermark.egg-info/
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 16:52:54.000000 watermark-2.4.1/watermark.egg-info/PKG-INFO
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      314 2023-05-23 16:52:54.000000 watermark-2.4.1/watermark.egg-info/SOURCES.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)        1 2023-05-23 16:52:54.000000 watermark-2.4.1/watermark.egg-info/dependency_links.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       61 2023-05-23 16:52:54.000000 watermark-2.4.1/watermark.egg-info/requires.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       10 2023-05-23 16:52:54.000000 watermark-2.4.1/watermark.egg-info/top_level.txt
+drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 19:00:07.833177 watermark-2.4.2/
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1507 2023-05-23 16:50:16.000000 watermark-2.4.2/LICENSE
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)       58 2023-05-23 18:54:21.000000 watermark-2.4.2/MANIFEST.in
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 19:00:07.833254 watermark-2.4.2/PKG-INFO
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)    11591 2023-05-23 16:50:16.000000 watermark-2.4.2/README.md
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)       49 2023-05-23 18:58:20.000000 watermark-2.4.2/requirements.txt
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      512 2023-05-23 19:00:07.833504 watermark-2.4.2/setup.cfg
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1476 2023-05-23 16:50:16.000000 watermark-2.4.2/setup.py
+drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 19:00:07.832279 watermark-2.4.2/watermark/
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      373 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/__init__.py
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     3842 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/magic.py
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      291 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/version.py
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)    10070 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/watermark.py
+drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 19:00:07.833028 watermark-2.4.2/watermark.egg-info/
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/PKG-INFO
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      314 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)        1 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)       61 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/requires.txt
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)       10 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/top_level.txt
```

### Comparing `watermark-2.4.1/LICENSE` & `watermark-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watermark-2.4.1/PKG-INFO` & `watermark-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermark
-Version: 2.4.1
+Version: 2.4.2
 Summary: IPython magic function to print date/time stamps and various system information.
 Home-page: https://github.com/rasbt/watermark
 Author: Sebastian Raschka
 Author-email: mail@sebastianraschka.com
 License: newBSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `watermark-2.4.1/README.md` & `watermark-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `watermark-2.4.1/setup.cfg` & `watermark-2.4.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.4.1
+version = 2.4.2
 license_file = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: IPython
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `watermark-2.4.1/setup.py` & `watermark-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `watermark-2.4.1/watermark/magic.py` & `watermark-2.4.2/watermark/magic.py`

 * *Files identical despite different names*

### Comparing `watermark-2.4.1/watermark/watermark.py` & `watermark-2.4.2/watermark/watermark.py`

 * *Files identical despite different names*

### Comparing `watermark-2.4.1/watermark.egg-info/PKG-INFO` & `watermark-2.4.2/watermark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermark
-Version: 2.4.1
+Version: 2.4.2
 Summary: IPython magic function to print date/time stamps and various system information.
 Home-page: https://github.com/rasbt/watermark
 Author: Sebastian Raschka
 Author-email: mail@sebastianraschka.com
 License: newBSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

