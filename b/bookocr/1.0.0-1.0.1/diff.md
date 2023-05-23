# Comparing `tmp/bookocr-1.0.0.tar.gz` & `tmp/bookocr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookocr-1.0.0.tar", last modified: Tue May 23 00:48:55 2023, max compression
+gzip compressed data, was "bookocr-1.0.1.tar", last modified: Tue May 23 02:29:41 2023, max compression
```

## Comparing `bookocr-1.0.0.tar` & `bookocr-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 00:48:55.578035 bookocr-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-05-22 23:35:20.000000 bookocr-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1452 2023-05-23 00:48:55.577035 bookocr-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-05-23 00:41:08.000000 bookocr-1.0.0/README.md
--rw-rw-rw-   0        0        0      722 2023-05-23 00:16:30.000000 bookocr-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 00:48:55.578035 bookocr-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 00:48:55.431170 bookocr-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 00:48:55.545065 bookocr-1.0.0/src/bookocr/
--rw-rw-rw-   0        0        0       45 2023-05-16 15:03:36.000000 bookocr-1.0.0/src/bookocr/__init__.py
--rw-rw-rw-   0        0        0     2284 2023-05-19 17:50:39.000000 bookocr-1.0.0/src/bookocr/_char_ocr.py
--rw-rw-rw-   0        0        0     1230 2023-05-22 18:30:41.000000 bookocr-1.0.0/src/bookocr/_json.py
--rw-rw-rw-   0        0        0     4462 2023-05-21 17:23:34.000000 bookocr-1.0.0/src/bookocr/_service.py
--rw-rw-rw-   0        0        0    13007 2023-05-21 17:38:34.000000 bookocr-1.0.0/src/bookocr/_stats.py
--rw-rw-rw-   0        0        0     1236 2023-05-22 16:33:07.000000 bookocr-1.0.0/src/bookocr/config.py
--rw-rw-rw-   0        0        0    20769 2023-05-22 17:47:03.000000 bookocr-1.0.0/src/bookocr/ocr.py
--rw-rw-rw-   0        0        0     1089 2023-05-22 15:58:23.000000 bookocr-1.0.0/src/bookocr/stats_config.py
-drwxrwxrwx   0        0        0        0 2023-05-23 00:48:55.575037 bookocr-1.0.0/src/bookocr.egg-info/
--rw-rw-rw-   0        0        0     1452 2023-05-23 00:48:55.000000 bookocr-1.0.0/src/bookocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-23 00:48:55.000000 bookocr-1.0.0/src/bookocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 00:48:55.000000 bookocr-1.0.0/src/bookocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 00:48:55.000000 bookocr-1.0.0/src/bookocr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 02:29:41.998668 bookocr-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-22 23:35:20.000000 bookocr-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1452 2023-05-23 02:29:41.997667 bookocr-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-05-23 00:41:08.000000 bookocr-1.0.1/README.md
+-rw-rw-rw-   0        0        0      840 2023-05-23 02:29:25.000000 bookocr-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 02:29:41.998668 bookocr-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 02:29:41.953721 bookocr-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 02:29:41.981881 bookocr-1.0.1/src/bookocr/
+-rw-rw-rw-   0        0        0       45 2023-05-16 15:03:36.000000 bookocr-1.0.1/src/bookocr/__init__.py
+-rw-rw-rw-   0        0        0     2284 2023-05-19 17:50:39.000000 bookocr-1.0.1/src/bookocr/_char_ocr.py
+-rw-rw-rw-   0        0        0     1230 2023-05-22 18:30:41.000000 bookocr-1.0.1/src/bookocr/_json.py
+-rw-rw-rw-   0        0        0     4462 2023-05-21 17:23:34.000000 bookocr-1.0.1/src/bookocr/_service.py
+-rw-rw-rw-   0        0        0    13007 2023-05-21 17:38:34.000000 bookocr-1.0.1/src/bookocr/_stats.py
+-rw-rw-rw-   0        0        0     1236 2023-05-22 16:33:07.000000 bookocr-1.0.1/src/bookocr/config.py
+-rw-rw-rw-   0        0        0  2099296 2023-05-19 12:56:58.000000 bookocr-1.0.1/src/bookocr/model.h5
+-rw-rw-rw-   0        0        0    20769 2023-05-22 17:47:03.000000 bookocr-1.0.1/src/bookocr/ocr.py
+-rw-rw-rw-   0        0        0     1089 2023-05-22 15:58:23.000000 bookocr-1.0.1/src/bookocr/stats_config.py
+drwxrwxrwx   0        0        0        0 2023-05-23 02:29:41.995667 bookocr-1.0.1/src/bookocr.egg-info/
+-rw-rw-rw-   0        0        0     1452 2023-05-23 02:29:41.000000 bookocr-1.0.1/src/bookocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-23 02:29:41.000000 bookocr-1.0.1/src/bookocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 02:29:41.000000 bookocr-1.0.1/src/bookocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-23 02:29:41.000000 bookocr-1.0.1/src/bookocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 02:29:41.000000 bookocr-1.0.1/src/bookocr.egg-info/top_level.txt
```

### Comparing `bookocr-1.0.0/LICENSE` & `bookocr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/PKG-INFO` & `bookocr-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookocr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Optical character recognition (OCR) tool for printed book pages
 Author-email: Artem Poliakov <artem4250@gmail.com>
 Project-URL: Homepage, https://github.com/Artem259/bookocr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `bookocr-1.0.0/README.md` & `bookocr-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/pyproject.toml` & `bookocr-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 [build-system]
-requires = [
-    "setuptools>=61.0",
-    "opencv-python>=4.5.5.64",
-    "numpy>=1.23.5",
-    "pandas>=2.0.1",
-    "scipy>=1.10.1",
-    "tensorflow>=2.12.0",
-    "Pillow>=9.5.0"
-]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bookocr"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Artem Poliakov", email="artem4250@gmail.com" },
 ]
 description = "Optical character recognition (OCR) tool for printed book pages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "opencv-python>=4.5.5.64",
+    "numpy>=1.23.5",
+    "pandas>=2.0.1",
+    "scipy>=1.10.1",
+    "tensorflow>=2.12.0",
+    "Pillow>=9.5.0"
+]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+bookocr = ["*.h5"]
 
 [project.urls]
 "Homepage" = "https://github.com/Artem259/bookocr"
```

### Comparing `bookocr-1.0.0/src/bookocr/_char_ocr.py` & `bookocr-1.0.1/src/bookocr/_char_ocr.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/src/bookocr/_json.py` & `bookocr-1.0.1/src/bookocr/_json.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/src/bookocr/_service.py` & `bookocr-1.0.1/src/bookocr/_service.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/src/bookocr/_stats.py` & `bookocr-1.0.1/src/bookocr/_stats.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/src/bookocr/config.py` & `bookocr-1.0.1/src/bookocr/config.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/src/bookocr/ocr.py` & `bookocr-1.0.1/src/bookocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/src/bookocr/stats_config.py` & `bookocr-1.0.1/src/bookocr/stats_config.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.0/src/bookocr.egg-info/PKG-INFO` & `bookocr-1.0.1/src/bookocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookocr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Optical character recognition (OCR) tool for printed book pages
 Author-email: Artem Poliakov <artem4250@gmail.com>
 Project-URL: Homepage, https://github.com/Artem259/bookocr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

