# Comparing `tmp/kbib-0.1.6.tar.gz` & `tmp/kbib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbib-0.1.6.tar", last modified: Mon Apr 24 05:27:00 2023, max compression
+gzip compressed data, was "kbib-0.1.7.tar", last modified: Tue May 23 14:40:30 2023, max compression
```

## Comparing `kbib-0.1.6.tar` & `kbib-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:27:00.901289 kbib-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-24 05:26:43.000000 kbib-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 05:26:43.000000 kbib-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 05:27:00.901289 kbib-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-24 05:26:43.000000 kbib-0.1.6/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:27:00.901289 kbib-0.1.6/kbib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:26:43.000000 kbib-0.1.6/kbib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-24 05:26:43.000000 kbib-0.1.6/kbib/parseRefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-04-24 05:26:43.000000 kbib-0.1.6/kbib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:27:00.901289 kbib-0.1.6/kbib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:27:00.901289 kbib-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-24 05:26:43.000000 kbib-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:30.042519 kbib-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 14:40:09.000000 kbib-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 14:40:09.000000 kbib-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-23 14:40:30.042519 kbib-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-23 14:40:09.000000 kbib-0.1.7/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:30.042519 kbib-0.1.7/kbib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:09.000000 kbib-0.1.7/kbib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-23 14:40:09.000000 kbib-0.1.7/kbib/parseRefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-23 14:40:09.000000 kbib-0.1.7/kbib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:30.042519 kbib-0.1.7/kbib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:40:29.000000 kbib-0.1.7/kbib.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:40:30.042519 kbib-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-23 14:40:09.000000 kbib-0.1.7/setup.py
```

### Comparing `kbib-0.1.6/LICENSE` & `kbib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kbib-0.1.6/PKG-INFO` & `kbib-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.6
+Version: 0.1.7
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kbib-0.1.6/Readme.md` & `kbib-0.1.7/Readme.md`

 * *Files identical despite different names*

### Comparing `kbib-0.1.6/kbib/parseRefs.py` & `kbib-0.1.7/kbib/parseRefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             f.write(bibs)
     else:
         print(bibs)
 
 
 def CommandsGiven(args):
     # check if any commands are given
-    for elem in ['bib','ref','pdf','ren']:
+    for elem in ['bib','ref','pdf','ren','dup']:
         if getattr(args,elem):
             return True
     return False
 
 
 def main():
     parser = createParser()
```

### Comparing `kbib-0.1.6/kbib/utils.py` & `kbib-0.1.7/kbib/utils.py`

 * *Files identical despite different names*

### Comparing `kbib-0.1.6/kbib.egg-info/PKG-INFO` & `kbib-0.1.7/kbib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.6
+Version: 0.1.7
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kbib-0.1.6/setup.py` & `kbib-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('Readme.md') as f:
     txt = f.read()
 
 setup(name='kbib',
-    version='0.1.6',
+    version='0.1.7',
     description='A command line tool to get bibtex information from DOIs and PDFs',
     long_description=txt,
     long_description_content_type='text/markdown',
     author='Koushik Naskar',
     author_email='koushik.naskar9@gmail.com',
     license="MIT",
     classifiers=[
```

