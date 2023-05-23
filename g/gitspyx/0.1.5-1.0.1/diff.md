# Comparing `tmp/gitspyx-0.1.5.tar.gz` & `tmp/gitspyx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitspyx-0.1.5.tar", last modified: Thu May 18 22:59:51 2023, max compression
+gzip compressed data, was "gitspyx-1.0.1.tar", last modified: Tue May 23 16:46:49 2023, max compression
```

## Comparing `gitspyx-0.1.5.tar` & `gitspyx-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-18 22:59:51.023616 gitspyx-0.1.5/
--rw-r--r--   0 alex      (1000) alex      (1000)     1059 2023-05-18 21:59:47.000000 gitspyx-0.1.5/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     1093 2023-05-18 22:59:51.023616 gitspyx-0.1.5/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     3350 2023-05-18 22:59:24.000000 gitspyx-0.1.5/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-18 22:59:51.023616 gitspyx-0.1.5/gitspyx/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-18 21:56:40.000000 gitspyx-0.1.5/gitspyx/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6761 2023-05-18 22:59:16.000000 gitspyx-0.1.5/gitspyx/gitspyx.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-18 22:59:51.023616 gitspyx-0.1.5/gitspyx.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     1093 2023-05-18 22:59:50.000000 gitspyx-0.1.5/gitspyx.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      253 2023-05-18 22:59:50.000000 gitspyx-0.1.5/gitspyx.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-18 22:59:50.000000 gitspyx-0.1.5/gitspyx.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       49 2023-05-18 22:59:50.000000 gitspyx-0.1.5/gitspyx.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-18 22:59:50.000000 gitspyx-0.1.5/gitspyx.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        8 2023-05-18 22:59:50.000000 gitspyx-0.1.5/gitspyx.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-18 22:59:51.023616 gitspyx-0.1.5/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)     1369 2023-05-18 22:59:04.000000 gitspyx-0.1.5/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-23 16:46:49.660384 gitspyx-1.0.1/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1059 2023-05-18 21:59:47.000000 gitspyx-1.0.1/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     1093 2023-05-23 16:46:49.660384 gitspyx-1.0.1/PKG-INFO
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-23 16:46:49.660384 gitspyx-1.0.1/gitspyx/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-18 21:56:40.000000 gitspyx-1.0.1/gitspyx/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7682 2023-05-23 16:21:14.000000 gitspyx-1.0.1/gitspyx/gitspyx.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-23 16:46:49.660384 gitspyx-1.0.1/gitspyx.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1093 2023-05-23 16:46:49.000000 gitspyx-1.0.1/gitspyx.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-05-23 16:46:49.000000 gitspyx-1.0.1/gitspyx.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-23 16:46:49.000000 gitspyx-1.0.1/gitspyx.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       49 2023-05-23 16:46:49.000000 gitspyx-1.0.1/gitspyx.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-23 16:46:49.000000 gitspyx-1.0.1/gitspyx.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        8 2023-05-23 16:46:49.000000 gitspyx-1.0.1/gitspyx.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-23 16:46:49.660384 gitspyx-1.0.1/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)     1369 2023-05-23 16:46:20.000000 gitspyx-1.0.1/setup.py
```

### Comparing `gitspyx-0.1.5/LICENSE` & `gitspyx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitspyx-0.1.5/PKG-INFO` & `gitspyx-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitspyx
-Version: 0.1.5
+Version: 1.0.1
 Summary: Get Github user profile details
 Home-page: https://github.com/MrHacker-X/GitSpyX.git/
 Author: Alex Butler 🚩
 Author-email: mrhackerxofficial@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gitspyx-0.1.5/gitspyx.egg-info/PKG-INFO` & `gitspyx-1.0.1/gitspyx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitspyx
-Version: 0.1.5
+Version: 1.0.1
 Summary: Get Github user profile details
 Home-page: https://github.com/MrHacker-X/GitSpyX.git/
 Author: Alex Butler 🚩
 Author-email: mrhackerxofficial@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gitspyx-0.1.5/setup.py` & `gitspyx-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gitspyx',
-    version='0.1.5',
+    version='1.0.1',
     author='Alex Butler 🚩',
     author_email='mrhackerxofficial@gmail.com',
     description='Get Github user profile details',
     long_description='''GitSpyX: Simplify GitHub analysis with user profiles, repository details, contributor insights, and powerful visualizations. Effortlessly extract valuable information and gain insights for informed decision-making. Accelerate your GitHub repository analysis workflow with GitSpyX.''',
     long_description_content_type='text/plain',
     url='https://github.com/MrHacker-X/GitSpyX.git/',
     packages=find_packages(),
```

