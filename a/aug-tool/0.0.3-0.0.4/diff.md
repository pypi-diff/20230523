# Comparing `tmp/aug-tool-0.0.3.tar.gz` & `tmp/aug-tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug-tool-0.0.3.tar", last modified: Sun Apr 23 16:33:57 2023, max compression
+gzip compressed data, was "aug-tool-0.0.4.tar", last modified: Tue May 23 17:43:30 2023, max compression
```

## Comparing `aug-tool-0.0.3.tar` & `aug-tool-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.699164 aug-tool-0.0.3/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:14:24.000000 aug-tool-0.0.3/LICENCE
--rw-rw-rw-   0        0        0       26 2023-04-23 16:29:48.000000 aug-tool-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2725 2023-04-23 16:33:57.700160 aug-tool-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2059 2023-04-15 13:31:22.000000 aug-tool-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-04-14 20:14:26.000000 aug-tool-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      805 2023-04-23 16:33:57.701158 aug-tool-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.673072 aug-tool-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.692191 aug-tool-0.0.3/src/aug_tool/
--rw-rw-rw-   0        0        0     6540 2023-04-23 15:20:48.000000 aug-tool-0.0.3/src/aug_tool/Augmentation.py
--rw-rw-rw-   0        0        0        0 2023-04-14 18:48:21.000000 aug-tool-0.0.3/src/aug_tool/__init__.py
--rw-rw-rw-   0        0        0     3832 2023-04-23 15:46:09.000000 aug-tool-0.0.3/src/aug_tool/aug_tool.py
--rw-rw-rw-   0        0        0   142539 2023-01-17 19:52:24.000000 aug-tool-0.0.3/src/aug_tool/effect_1.png
--rw-rw-rw-   0        0        0    62735 2023-01-17 19:56:01.000000 aug-tool-0.0.3/src/aug_tool/effect_2.png
--rw-rw-rw-   0        0        0      617 2023-04-23 15:47:09.000000 aug-tool-0.0.3/src/aug_tool/example.py
--rw-rw-rw-   0        0        0   182306 2023-02-05 15:48:52.000000 aug-tool-0.0.3/src/aug_tool/logo.png
--rw-rw-rw-   0        0        0    20616 2023-04-15 10:14:20.000000 aug-tool-0.0.3/src/aug_tool/logo2.png
-drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.698171 aug-tool-0.0.3/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0     2725 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.708980 aug-tool-0.0.4/
+-rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug-tool-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0       20 2023-05-13 18:17:23.000000 aug-tool-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2616 2023-05-23 17:43:30.708980 aug-tool-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2059 2023-05-13 18:17:23.000000 aug-tool-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-13 18:17:23.000000 aug-tool-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      696 2023-05-23 17:43:30.710974 aug-tool-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.649273 aug-tool-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.661009 aug-tool-0.0.4/src/aug-tool/
+-rw-rw-rw-   0        0        0        0 2023-05-12 19:34:11.000000 aug-tool-0.0.4/src/aug-tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.669354 aug-tool-0.0.4/src/aug-tool/dataAugmentor/
+-rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/annAug.py
+-rw-rw-rw-   0        0        0      505 2023-05-17 20:04:01.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/dataAug.py
+-rw-rw-rw-   0        0        0     1975 2023-05-16 18:30:28.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/imgAug.py
+-rw-rw-rw-   0        0        0      954 2023-05-17 20:04:00.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/txtAug.py
+-rw-rw-rw-   0        0        0     1738 2023-05-17 19:15:02.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/xmlAug.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.686499 aug-tool-0.0.4/src/aug-tool/dataOpener/
+-rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/annOp.py
+-rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/dataOp.py
+-rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/imgOp.py
+-rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/txtOp.py
+-rw-rw-rw-   0        0        0     1535 2023-05-15 19:34:16.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/xmlOp.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.701464 aug-tool-0.0.4/src/aug-tool/dataSaver/
+-rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/annSav.py
+-rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/dataSav.py
+-rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/imgSav.py
+-rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/txtSav.py
+-rw-rw-rw-   0        0        0      473 2023-05-14 10:12:53.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/xmlSav.py
+-rw-rw-rw-   0        0        0      518 2023-05-17 20:04:00.000000 aug-tool-0.0.4/src/aug-tool/deneme.py
+-rw-rw-rw-   0        0        0     5523 2023-05-23 17:32:49.000000 aug-tool-0.0.4/src/aug-tool/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.707980 aug-tool-0.0.4/src/aug_tool.egg-info/
+-rw-rw-rw-   0        0        0     2616 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/top_level.txt
```

### Comparing `aug-tool-0.0.3/LICENCE` & `aug-tool-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.3/PKG-INFO` & `aug-tool-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.0.3
-Summary: Our library is now available on PyPI for easy installation and integration. Don t settle for limited training data - try our library today and take your ML projects to new heights!
+Version: 0.0.4
+Summary: A small package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aug-tool-0.0.3/README.md` & `aug-tool-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.3/src/aug_tool.egg-info/PKG-INFO` & `aug-tool-0.0.4/src/aug_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.0.3
-Summary: Our library is now available on PyPI for easy installation and integration. Don t settle for limited training data - try our library today and take your ML projects to new heights!
+Version: 0.0.4
+Summary: A small package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

