# Comparing `tmp/comex-0.0.3.tar.gz` & `tmp/comex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.0.3.tar", last modified: Sat May 20 03:39:17 2023, max compression
+gzip compressed data, was "comex-0.0.4.tar", last modified: Tue May 23 15:38:00 2023, max compression
```

## Comparing `comex-0.0.3.tar` & `comex-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:39:17.600000 comex-0.0.3/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.3/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)     7952 2023-05-20 03:39:17.600000 comex-0.0.3/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     7335 2023-05-20 03:38:54.000000 comex-0.0.3/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-20 03:39:17.600000 comex-0.0.3/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.3/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:39:17.600000 comex-0.0.3/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:39:17.600000 comex-0.0.3/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)     7952 2023-05-20 03:39:17.000000 comex-0.0.3/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)      236 2023-05-20 03:39:17.000000 comex-0.0.3/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-20 03:39:17.000000 comex-0.0.3/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-20 03:39:17.000000 comex-0.0.3/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-20 03:39:17.000000 comex-0.0.3/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-20 03:39:17.000000 comex-0.0.3/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-23 15:38:00.290000 comex-0.0.4/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.4/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)     7952 2023-05-23 15:38:00.290000 comex-0.0.4/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     7335 2023-05-20 03:38:54.000000 comex-0.0.4/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-23 15:38:00.300000 comex-0.0.4/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.4/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-23 15:38:00.290000 comex-0.0.4/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-23 15:38:00.290000 comex-0.0.4/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)     7952 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)      236 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.0.3/LICENSE` & `comex-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.0.3/PKG-INFO` & `comex-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `comex-0.0.3/README.md` & `comex-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `comex-0.0.3/setup.cfg` & `comex-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.0.3
+version = 0.0.4
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.0.3/src/comex.egg-info/PKG-INFO` & `comex-0.0.4/src/comex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

