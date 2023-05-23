# Comparing `tmp/nrnutils-0.2.0.tar.gz` & `tmp/nrnutils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nrnutils-0.2.0.tar", last modified: Thu Jan 24 12:33:31 2013, max compression
+gzip compressed data, was "nrnutils-0.3.0.tar", last modified: Tue May 23 11:21:57 2023, max compression
```

## Comparing `nrnutils-0.2.0.tar` & `nrnutils-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 andrew     (507) staff       (20)        0 2013-01-24 12:33:31.000000 nrnutils-0.2.0/
--rw-r--r--   0 andrew     (507) staff       (20)    21097 2013-01-24 12:33:13.000000 nrnutils-0.2.0/COPYING
--rw-r--r--   0 andrew     (507) staff       (20)     3479 2013-01-24 12:33:13.000000 nrnutils-0.2.0/nrnutils.py
--rw-r--r--   0 andrew     (507) staff       (20)      745 2013-01-24 12:33:31.000000 nrnutils-0.2.0/PKG-INFO
--rw-r--r--   0 andrew     (507) staff       (20)      490 2013-01-24 12:33:13.000000 nrnutils-0.2.0/README.txt
--rw-r--r--   0 andrew     (507) staff       (20)      955 2013-01-24 12:33:13.000000 nrnutils-0.2.0/setup.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-05-23 11:21:57.204378 nrnutils-0.3.0/
+-rw-r--r--   0 adavison   (502) staff       (20)    21097 2023-05-23 11:15:54.861163 nrnutils-0.3.0/COPYING
+-rw-r--r--   0 adavison   (502) staff       (20)      740 2023-05-23 11:21:57.204509 nrnutils-0.3.0/PKG-INFO
+-rw-r--r--   0 adavison   (502) staff       (20)      486 2023-05-23 11:16:27.753017 nrnutils-0.3.0/README.txt
+-rw-r--r--   0 adavison   (502) staff       (20)     5854 2023-05-23 11:21:29.041542 nrnutils-0.3.0/nrnutils.py
+-rw-r--r--   0 adavison   (502) staff       (20)      913 2023-05-23 11:18:51.273635 nrnutils-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nrnutils-0.2.0/COPYING` & `nrnutils-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `nrnutils-0.2.0/PKG-INFO` & `nrnutils-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.1
 Name: nrnutils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Some tools for use with the NEURON simulator (http://www.neuron.yale.edu/neuron/)
-Home-page: https://bitbucket.org/apdavison/nrnutils
+Home-page: https://github.com/apdavison/nrnutils
 Author: Andrew P. Davison
-Author-email: andrewpdavison@gmail.com
+Author-email: andrew.davison@cnrs.fr
 License: CeCILL http://www.cecill.info
 Description: UNKNOWN
 Keywords: computational science neuroscience simulation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nrnutils-0.2.0/setup.py` & `nrnutils-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
-from nrnutils import __version__
 
 setup(
     name="nrnutils",
-    version=__version__,
+    version="0.3.0",
     py_modules=['nrnutils'],
     author = "Andrew P. Davison",
-    author_email = "andrewpdavison@gmail.com",
+    author_email = "andrew.davison@cnrs.fr",
     description = "Some tools for use with the NEURON simulator (http://www.neuron.yale.edu/neuron/)",
     license = "CeCILL http://www.cecill.info",
     keywords = "computational science neuroscience simulation",
-    url = "https://bitbucket.org/apdavison/nrnutils",
+    url = "https://github.com/apdavison/nrnutils",
     classifiers = ['Development Status :: 4 - Beta',
                    'Environment :: Console',
                    'Intended Audience :: Science/Research',
                    'License :: Other/Proprietary License',
                    'Natural Language :: English',
                    'Operating System :: OS Independent',
                    'Programming Language :: Python',
```

