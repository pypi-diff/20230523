# Comparing `tmp/ditty-0.1.tar.gz` & `tmp/ditty-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.1.tar", last modified: Tue May 23 03:51:48 2023, max compression
+gzip compressed data, was "ditty-0.1.1.tar", last modified: Tue May 23 04:02:38 2023, max compression
```

## Comparing `ditty-0.1.tar` & `ditty-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 03:51:48.817218 ditty-0.1/
--rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.1/LICENSE
--rw-rw-r--   0 crow      (1000) crow      (1000)      254 2023-05-23 03:51:48.817218 ditty-0.1/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)     2834 2023-05-23 03:23:04.000000 ditty-0.1/README.md
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 03:51:48.817218 ditty-0.1/lib/
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 03:51:48.817218 ditty-0.1/lib/ditty.egg-info/
--rw-rw-r--   0 crow      (1000) crow      (1000)      254 2023-05-23 03:51:48.000000 ditty-0.1/lib/ditty.egg-info/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)      200 2023-05-23 03:51:48.000000 ditty-0.1/lib/ditty.egg-info/SOURCES.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 03:51:48.000000 ditty-0.1/lib/ditty.egg-info/dependency_links.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-23 03:51:48.000000 ditty-0.1/lib/ditty.egg-info/requires.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 03:51:48.000000 ditty-0.1/lib/ditty.egg-info/top_level.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-23 03:51:48.817218 ditty-0.1/setup.cfg
--rw-rw-r--   0 crow      (1000) crow      (1000)      533 2023-05-23 03:50:34.000000 ditty-0.1/setup.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:02:38.965366 ditty-0.1.1/
+-rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.1.1/LICENSE
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3132 2023-05-23 04:02:38.965366 ditty-0.1.1/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)     2834 2023-05-23 03:23:04.000000 ditty-0.1.1/README.md
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:02:38.965366 ditty-0.1.1/lib/
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:02:38.965366 ditty-0.1.1/lib/ditty.egg-info/
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3132 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)      200 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/SOURCES.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/dependency_links.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/requires.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 04:02:38.000000 ditty-0.1.1/lib/ditty.egg-info/top_level.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-23 04:02:38.965366 ditty-0.1.1/setup.cfg
+-rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-23 04:02:34.000000 ditty-0.1.1/setup.py
```

### Comparing `ditty-0.1/LICENSE` & `ditty-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.1/README.md` & `ditty-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ditty-0.1/setup.py` & `ditty-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.1',
+    version='0.1.1',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
+    long_description=open('README.md', 'r').read(),
+    long_description_content_type='text/markdown',
     url='https://github.com/iantbutler01/ditty',
     keywords='finetuning, llm, nlp, machine learning',
     install_requires=[
           'accelerate',
           'transformers',
           'datasets',
           'bitsandbytes',
           'fire',
           'peft'
       ],
 
-)
+)
```

