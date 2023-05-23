# Comparing `tmp/licensekeygentest-0.2.1.tar.gz` & `tmp/licensekeygentest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-0.2.1.tar", last modified: Tue May  9 11:24:57 2023, max compression
+gzip compressed data, was "licensekeygentest-1.0.1.tar", last modified: Tue May 23 16:33:50 2023, max compression
```

## Comparing `licensekeygentest-0.2.1.tar` & `licensekeygentest-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 11:24:57.893829 licensekeygentest-0.2.1/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.2.1/LICENSE
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      695 2023-05-09 11:24:57.893829 licensekeygentest-0.2.1/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      152 2023-05-09 09:30:18.000000 licensekeygentest-0.2.1/README.md
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 11:24:57.893829 licensekeygentest-0.2.1/licensekeygentest/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.2.1/licensekeygentest/__init__.py
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1897 2023-05-09 11:24:32.000000 licensekeygentest-0.2.1/licensekeygentest/main.py
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 11:24:57.893829 licensekeygentest-0.2.1/licensekeygentest.egg-info/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      695 2023-05-09 11:24:57.000000 licensekeygentest-0.2.1/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 11:24:57.000000 licensekeygentest-0.2.1/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 11:24:57.000000 licensekeygentest-0.2.1/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 11:24:57.000000 licensekeygentest-0.2.1/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 11:24:57.000000 licensekeygentest-0.2.1/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 11:24:57.893829 licensekeygentest-0.2.1/setup.cfg
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 11:24:47.000000 licensekeygentest-0.2.1/setup.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-23 16:33:50.373928 licensekeygentest-1.0.1/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 11:20:36.000000 licensekeygentest-1.0.1/LICENSE
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-23 16:33:50.373928 licensekeygentest-1.0.1/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      152 2023-05-23 11:20:36.000000 licensekeygentest-1.0.1/README.md
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-23 16:33:50.369928 licensekeygentest-1.0.1/licensekeygentest/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       43 2023-05-23 11:20:36.000000 licensekeygentest-1.0.1/licensekeygentest/__init__.py
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     2356 2023-05-23 16:31:06.000000 licensekeygentest-1.0.1/licensekeygentest/main.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-23 16:33:50.369928 licensekeygentest-1.0.1/licensekeygentest.egg-info/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      286 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        1 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        9 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       18 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       38 2023-05-23 16:33:50.373928 licensekeygentest-1.0.1/setup.cfg
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 16:32:02.000000 licensekeygentest-1.0.1/setup.py
```

### Comparing `licensekeygentest-0.2.1/LICENSE` & `licensekeygentest-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-0.2.1/PKG-INFO` & `licensekeygentest-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.2.1
-Summary: POC for keygen authentication
+Version: 1.0.1
+Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `licensekeygentest-0.2.1/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-1.0.1/licensekeygentest.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.2.1
-Summary: POC for keygen authentication
+Version: 1.0.1
+Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `licensekeygentest-0.2.1/setup.py` & `licensekeygentest-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.1'
-DESCRIPTION = 'POC for keygen authentication'
+VERSION = '1.0.1'
+DESCRIPTION = 'POC for license validation checks'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
     author="Rahul R",
     author_email="<rahulranjan25.RR@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['requests', 'py-machineid'],
+    install_requires=['requests'],
     keywords=['python', 'authentication', 'licensing'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

