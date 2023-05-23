# Comparing `tmp/MacFSEvents-0.8.3.tar.gz` & `tmp/MacFSEvents-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MacFSEvents-0.8.3.tar", last modified: Tue May 23 06:43:38 2023, max compression
+gzip compressed data, was "MacFSEvents-0.8.4.tar", last modified: Tue May 23 07:46:16 2023, max compression
```

## Comparing `MacFSEvents-0.8.3.tar` & `MacFSEvents-0.8.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-23 06:43:38.599276 MacFSEvents-0.8.3/
--rw-r--r--   0 mborch     (503) staff       (20)     2382 2023-05-23 06:43:32.000000 MacFSEvents-0.8.3/CHANGES.rst
--rw-r--r--   0 mborch     (503) staff       (20)     1287 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/LICENSE.txt
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-23 06:43:38.599003 MacFSEvents-0.8.3/MacFSEvents.egg-info/
--rw-r--r--   0 mborch     (503) staff       (20)     8029 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/PKG-INFO
--rw-r--r--   0 mborch     (503) staff       (20)      250 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/SOURCES.txt
--rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/dependency_links.txt
--rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-22 20:16:14.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/not-zip-safe
--rw-r--r--   0 mborch     (503) staff       (20)       19 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/top_level.txt
--rw-r--r--   0 mborch     (503) staff       (20)     8029 2023-05-23 06:43:38.599159 MacFSEvents-0.8.3/PKG-INFO
--rw-r--r--   0 mborch     (503) staff       (20)     4718 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/README.rst
--rw-r--r--   0 mborch     (503) staff       (20)    10752 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/_fsevents.c
--rw-r--r--   0 mborch     (503) staff       (20)     1182 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/compat.c
--rw-r--r--   0 mborch     (503) staff       (20)     9607 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/fsevents.py
--rw-r--r--   0 mborch     (503) staff       (20)       38 2023-05-23 06:43:38.599316 MacFSEvents-0.8.3/setup.cfg
--rw-r--r--   0 mborch     (503) staff       (20)     1776 2023-05-23 06:43:10.000000 MacFSEvents-0.8.3/setup.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-23 07:46:16.233217 MacFSEvents-0.8.4/
+-rw-r--r--   0 mborch     (503) staff       (20)     2468 2023-05-23 07:45:20.000000 MacFSEvents-0.8.4/CHANGES.rst
+-rw-r--r--   0 mborch     (503) staff       (20)     1287 2023-05-22 20:13:46.000000 MacFSEvents-0.8.4/LICENSE.txt
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-23 07:46:16.232719 MacFSEvents-0.8.4/MacFSEvents.egg-info/
+-rw-r--r--   0 mborch     (503) staff       (20)     8216 2023-05-23 07:46:16.000000 MacFSEvents-0.8.4/MacFSEvents.egg-info/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)      259 2023-05-23 07:46:16.000000 MacFSEvents-0.8.4/MacFSEvents.egg-info/SOURCES.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-23 07:46:16.000000 MacFSEvents-0.8.4/MacFSEvents.egg-info/dependency_links.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-22 20:16:14.000000 MacFSEvents-0.8.4/MacFSEvents.egg-info/not-zip-safe
+-rw-r--r--   0 mborch     (503) staff       (20)       19 2023-05-23 07:46:16.000000 MacFSEvents-0.8.4/MacFSEvents.egg-info/top_level.txt
+-rw-r--r--   0 mborch     (503) staff       (20)     8216 2023-05-23 07:46:16.233052 MacFSEvents-0.8.4/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)     4718 2023-05-22 20:13:46.000000 MacFSEvents-0.8.4/README.rst
+-rw-r--r--   0 mborch     (503) staff       (20)    10752 2023-05-23 07:44:49.000000 MacFSEvents-0.8.4/_fsevents.c
+-rw-r--r--   0 mborch     (503) staff       (20)     1182 2023-05-22 20:13:46.000000 MacFSEvents-0.8.4/compat.c
+-rw-r--r--   0 mborch     (503) staff       (20)     1662 2023-05-22 20:13:46.000000 MacFSEvents-0.8.4/compat.h
+-rw-r--r--   0 mborch     (503) staff       (20)     9607 2023-05-23 07:32:01.000000 MacFSEvents-0.8.4/fsevents.py
+-rw-r--r--   0 mborch     (503) staff       (20)       38 2023-05-23 07:46:16.233271 MacFSEvents-0.8.4/setup.cfg
+-rw-r--r--   0 mborch     (503) staff       (20)     1925 2023-05-23 07:46:01.000000 MacFSEvents-0.8.4/setup.py
```

### Comparing `MacFSEvents-0.8.3/CHANGES.rst` & `MacFSEvents-0.8.4/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.8.4 (2023-05-23)
+------------------
+
+- Fix test compatibility with newer Python 3.
+
 0.8.3 (2023-05-23)
 ------------------
 
 - Fix brown-bag release.
 
 0.8.2 (2023-05-22)
 ------------------
```

### Comparing `MacFSEvents-0.8.3/LICENSE.txt` & `MacFSEvents-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.3/MacFSEvents.egg-info/PKG-INFO` & `MacFSEvents-0.8.4/MacFSEvents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MacFSEvents
-Version: 0.8.3
+Version: 0.8.4
 Summary: Thread-based interface to file system observation primitives.
 Home-page: https://github.com/malthe/macfsevents
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD
 Platform: Mac OS X
 Classifier: Development Status :: 4 - Beta
@@ -12,16 +12,18 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 2.4
 Classifier: Programming Language :: Python :: 2.5
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 License-File: LICENSE.txt
 
 .. contents::
 
 Overview
@@ -170,14 +172,19 @@
 
 .. [#] See `FSEventStreamEventFlags <http://developer.apple.com/mac/library/documentation/Darwin/Reference/FSEvents_Ref/FSEvents_h/index.html#//apple_ref/c/tag/FSEventStreamEventFlags>`_ for a reference. To check for a particular mask, use the *bitwise and* operator ``&``.
 
 
 Changelog
 =========
 
+0.8.4 (2023-05-23)
+------------------
+
+- Fix test compatibility with newer Python 3.
+
 0.8.3 (2023-05-23)
 ------------------
 
 - Fix brown-bag release.
 
 0.8.2 (2023-05-22)
 ------------------
```

### Comparing `MacFSEvents-0.8.3/PKG-INFO` & `MacFSEvents-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MacFSEvents
-Version: 0.8.3
+Version: 0.8.4
 Summary: Thread-based interface to file system observation primitives.
 Home-page: https://github.com/malthe/macfsevents
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD
 Platform: Mac OS X
 Classifier: Development Status :: 4 - Beta
@@ -12,16 +12,18 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 2.4
 Classifier: Programming Language :: Python :: 2.5
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 License-File: LICENSE.txt
 
 .. contents::
 
 Overview
@@ -170,14 +172,19 @@
 
 .. [#] See `FSEventStreamEventFlags <http://developer.apple.com/mac/library/documentation/Darwin/Reference/FSEvents_Ref/FSEvents_h/index.html#//apple_ref/c/tag/FSEventStreamEventFlags>`_ for a reference. To check for a particular mask, use the *bitwise and* operator ``&``.
 
 
 Changelog
 =========
 
+0.8.4 (2023-05-23)
+------------------
+
+- Fix test compatibility with newer Python 3.
+
 0.8.3 (2023-05-23)
 ------------------
 
 - Fix brown-bag release.
 
 0.8.2 (2023-05-22)
 ------------------
```

### Comparing `MacFSEvents-0.8.3/README.rst` & `MacFSEvents-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.3/_fsevents.c` & `MacFSEvents-0.8.4/_fsevents.c`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.3/compat.c` & `MacFSEvents-0.8.4/compat.c`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.3/fsevents.py` & `MacFSEvents-0.8.4/fsevents.py`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.3/setup.py` & `MacFSEvents-0.8.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,23 @@
               sources = ['_fsevents.c', 'compat.c'],
               extra_link_args = ["-framework","CoreFoundation",
                                "-framework","CoreServices"],
              ),
     ]
 
 setup(name = "MacFSEvents",
-      version = "0.8.3",
+      version = "0.8.4",
       description = "Thread-based interface to file system observation primitives.",
       long_description = "\n\n".join((read('README.rst'), read('CHANGES.rst'))),
       license = "BSD",
-      data_files = [("", ["LICENSE.txt", "CHANGES.rst"])],
+      data_files = [("", [
+          "compat.h",
+          "LICENSE.txt",
+          "CHANGES.rst"
+      ])],
       author = "Malthe Borch",
       author_email = "mborch@gmail.com",
       url = 'https://github.com/malthe/macfsevents',
       cmdclass = dict(build_ext=build_ext),
       ext_modules = ext_modules,
       platforms = ["Mac OS X"],
       classifiers = [
@@ -34,16 +38,18 @@
         'License :: OSI Approved :: BSD License',
         'Operating System :: MacOS :: MacOS X',
         'Programming Language :: C',
         'Programming Language :: Python :: 2.4',
         'Programming Language :: Python :: 2.5',
         'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.2',
-        'Programming Language :: Python :: 3.3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Filesystems',
       ],
       zip_safe=False,
       test_suite="tests",
       py_modules=['fsevents'],
      )
```

