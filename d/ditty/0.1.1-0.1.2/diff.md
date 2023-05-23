# Comparing `tmp/ditty-0.1.1.tar.gz` & `tmp/ditty-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.1.1.tar", last modified: Tue May 23 04:02:38 2023, max compression
+gzip compressed data, was "ditty-0.1.2.tar", last modified: Tue May 23 04:13:11 2023, max compression
```

## Comparing `ditty-0.1.1.tar` & `ditty-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:02:38.965366 ditty-0.1.1/
--rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.1.1/LICENSE
--rw-rw-r--   0 crow      (1000) crow      (1000)     3132 2023-05-23 04:02:38.965366 ditty-0.1.1/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)     2834 2023-05-23 03:23:04.000000 ditty-0.1.1/README.md
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:02:38.965366 ditty-0.1.1/lib/
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:02:38.965366 ditty-0.1.1/lib/ditty.egg-info/
--rw-rw-r--   0 crow      (1000) crow      (1000)     3132 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)      200 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/SOURCES.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/dependency_links.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/requires.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/top_level.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-23 04:02:38.965366 ditty-0.1.1/setup.cfg
--rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-23 04:02:34.000000 ditty-0.1.1/setup.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:13:11.253512 ditty-0.1.2/
+-rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.1.2/LICENSE
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-23 04:13:11.253512 ditty-0.1.2/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)     2872 2023-05-23 04:03:46.000000 ditty-0.1.2/README.md
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:13:11.253512 ditty-0.1.2/lib/
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:13:11.253512 ditty-0.1.2/lib/ditty/
+-rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.1.2/lib/ditty/__init__.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     5020 2023-05-23 01:12:32.000000 ditty-0.1.2/lib/ditty/data.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     5434 2023-05-23 02:28:24.000000 ditty-0.1.2/lib/ditty/pipeline.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     4848 2023-05-23 03:13:21.000000 ditty-0.1.2/lib/ditty/trainer.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:13:11.253512 ditty-0.1.2/lib/ditty.egg-info/
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-23 04:13:11.000000 ditty-0.1.2/lib/ditty.egg-info/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-23 04:13:11.000000 ditty-0.1.2/lib/ditty.egg-info/SOURCES.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 04:13:11.000000 ditty-0.1.2/lib/ditty.egg-info/dependency_links.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-23 04:13:11.000000 ditty-0.1.2/lib/ditty.egg-info/requires.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-23 04:13:11.000000 ditty-0.1.2/lib/ditty.egg-info/top_level.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-23 04:13:11.253512 ditty-0.1.2/setup.cfg
+-rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-23 04:13:01.000000 ditty-0.1.2/setup.py
```

### Comparing `ditty-0.1.1/LICENSE` & `ditty-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.1.1/PKG-INFO` & `ditty-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -66,14 +66,21 @@
             ("map", truncate, {}),
         ]
     )
 ```
 
 This can be used to great effect when overriding the `dataset` method in a subclass of `Pipeline`.
 
+## Setup
+
+```
+pip install ditty
+```
+
+
 ## Tips
 
 https://github.com/google/python-fire is a tool for autogenerating CLIs from Python functions, dicts and objects.
 
 It can be combined with Pipeline to make a very quick cli for launching your process.
 
 ## Attribution / Statement of Changes
```

### Comparing `ditty-0.1.1/README.md` & `ditty-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,21 @@
             ("map", truncate, {}),
         ]
     )
 ```
 
 This can be used to great effect when overriding the `dataset` method in a subclass of `Pipeline`.
 
+## Setup
+
+```
+pip install ditty
+```
+
+
 ## Tips
 
 https://github.com/google/python-fire is a tool for autogenerating CLIs from Python functions, dicts and objects.
 
 It can be combined with Pipeline to make a very quick cli for launching your process.
 
 ## Attribution / Statement of Changes
```

### Comparing `ditty-0.1.1/lib/ditty.egg-info/PKG-INFO` & `ditty-0.1.2/lib/ditty.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -66,14 +66,21 @@
             ("map", truncate, {}),
         ]
     )
 ```
 
 This can be used to great effect when overriding the `dataset` method in a subclass of `Pipeline`.
 
+## Setup
+
+```
+pip install ditty
+```
+
+
 ## Tips
 
 https://github.com/google/python-fire is a tool for autogenerating CLIs from Python functions, dicts and objects.
 
 It can be combined with Pipeline to make a very quick cli for launching your process.
 
 ## Attribution / Statement of Changes
```

### Comparing `ditty-0.1.1/setup.py` & `ditty-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.1.1',
+    version='0.1.2',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

