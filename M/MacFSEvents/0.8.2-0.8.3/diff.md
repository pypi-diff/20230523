# Comparing `tmp/MacFSEvents-0.8.2.tar.gz` & `tmp/MacFSEvents-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MacFSEvents-0.8.2.tar", last modified: Mon May 22 20:16:14 2023, max compression
+gzip compressed data, was "MacFSEvents-0.8.3.tar", last modified: Tue May 23 06:43:38 2023, max compression
```

## Comparing `MacFSEvents-0.8.2.tar` & `MacFSEvents-0.8.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-22 20:16:14.787247 MacFSEvents-0.8.2/
--rw-r--r--   0 mborch     (503) staff       (20)     1287 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/LICENSE.txt
-drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-22 20:16:14.786979 MacFSEvents-0.8.2/MacFSEvents.egg-info/
--rw-r--r--   0 mborch     (503) staff       (20)     7964 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/PKG-INFO
--rw-r--r--   0 mborch     (503) staff       (20)      238 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/SOURCES.txt
--rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/dependency_links.txt
--rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/not-zip-safe
--rw-r--r--   0 mborch     (503) staff       (20)       19 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/top_level.txt
--rw-r--r--   0 mborch     (503) staff       (20)     7964 2023-05-22 20:16:14.787132 MacFSEvents-0.8.2/PKG-INFO
--rw-r--r--   0 mborch     (503) staff       (20)     4718 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/README.rst
--rw-r--r--   0 mborch     (503) staff       (20)    10752 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/_fsevents.c
--rw-r--r--   0 mborch     (503) staff       (20)     1182 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/compat.c
--rw-r--r--   0 mborch     (503) staff       (20)     9607 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/fsevents.py
--rw-r--r--   0 mborch     (503) staff       (20)       38 2023-05-22 20:16:14.787294 MacFSEvents-0.8.2/setup.cfg
--rw-r--r--   0 mborch     (503) staff       (20)     1761 2023-05-22 20:15:53.000000 MacFSEvents-0.8.2/setup.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-23 06:43:38.599276 MacFSEvents-0.8.3/
+-rw-r--r--   0 mborch     (503) staff       (20)     2382 2023-05-23 06:43:32.000000 MacFSEvents-0.8.3/CHANGES.rst
+-rw-r--r--   0 mborch     (503) staff       (20)     1287 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/LICENSE.txt
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-23 06:43:38.599003 MacFSEvents-0.8.3/MacFSEvents.egg-info/
+-rw-r--r--   0 mborch     (503) staff       (20)     8029 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)      250 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/SOURCES.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/dependency_links.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-22 20:16:14.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/not-zip-safe
+-rw-r--r--   0 mborch     (503) staff       (20)       19 2023-05-23 06:43:38.000000 MacFSEvents-0.8.3/MacFSEvents.egg-info/top_level.txt
+-rw-r--r--   0 mborch     (503) staff       (20)     8029 2023-05-23 06:43:38.599159 MacFSEvents-0.8.3/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)     4718 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/README.rst
+-rw-r--r--   0 mborch     (503) staff       (20)    10752 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/_fsevents.c
+-rw-r--r--   0 mborch     (503) staff       (20)     1182 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/compat.c
+-rw-r--r--   0 mborch     (503) staff       (20)     9607 2023-05-22 20:13:46.000000 MacFSEvents-0.8.3/fsevents.py
+-rw-r--r--   0 mborch     (503) staff       (20)       38 2023-05-23 06:43:38.599316 MacFSEvents-0.8.3/setup.cfg
+-rw-r--r--   0 mborch     (503) staff       (20)     1776 2023-05-23 06:43:10.000000 MacFSEvents-0.8.3/setup.py
```

### Comparing `MacFSEvents-0.8.2/LICENSE.txt` & `MacFSEvents-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.2/MacFSEvents.egg-info/PKG-INFO` & `MacFSEvents-0.8.3/MacFSEvents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MacFSEvents
-Version: 0.8.2
+Version: 0.8.3
 Summary: Thread-based interface to file system observation primitives.
 Home-page: https://github.com/malthe/macfsevents
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD
 Platform: Mac OS X
 Classifier: Development Status :: 4 - Beta
@@ -170,14 +170,19 @@
 
 .. [#] See `FSEventStreamEventFlags <http://developer.apple.com/mac/library/documentation/Darwin/Reference/FSEvents_Ref/FSEvents_h/index.html#//apple_ref/c/tag/FSEventStreamEventFlags>`_ for a reference. To check for a particular mask, use the *bitwise and* operator ``&``.
 
 
 Changelog
 =========
 
+0.8.3 (2023-05-23)
+------------------
+
+- Fix brown-bag release.
+
 0.8.2 (2023-05-22)
 ------------------
 
 - Fix file mask string method missing return value (#43).
 
 0.8.1 (2018-02-21)
 ------------------
```

### Comparing `MacFSEvents-0.8.2/PKG-INFO` & `MacFSEvents-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MacFSEvents
-Version: 0.8.2
+Version: 0.8.3
 Summary: Thread-based interface to file system observation primitives.
 Home-page: https://github.com/malthe/macfsevents
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD
 Platform: Mac OS X
 Classifier: Development Status :: 4 - Beta
@@ -170,14 +170,19 @@
 
 .. [#] See `FSEventStreamEventFlags <http://developer.apple.com/mac/library/documentation/Darwin/Reference/FSEvents_Ref/FSEvents_h/index.html#//apple_ref/c/tag/FSEventStreamEventFlags>`_ for a reference. To check for a particular mask, use the *bitwise and* operator ``&``.
 
 
 Changelog
 =========
 
+0.8.3 (2023-05-23)
+------------------
+
+- Fix brown-bag release.
+
 0.8.2 (2023-05-22)
 ------------------
 
 - Fix file mask string method missing return value (#43).
 
 0.8.1 (2018-02-21)
 ------------------
```

### Comparing `MacFSEvents-0.8.2/README.rst` & `MacFSEvents-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.2/_fsevents.c` & `MacFSEvents-0.8.3/_fsevents.c`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.2/compat.c` & `MacFSEvents-0.8.3/compat.c`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.2/fsevents.py` & `MacFSEvents-0.8.3/fsevents.py`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.2/setup.py` & `MacFSEvents-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
               sources = ['_fsevents.c', 'compat.c'],
               extra_link_args = ["-framework","CoreFoundation",
                                "-framework","CoreServices"],
              ),
     ]
 
 setup(name = "MacFSEvents",
-      version = "0.8.2",
+      version = "0.8.3",
       description = "Thread-based interface to file system observation primitives.",
       long_description = "\n\n".join((read('README.rst'), read('CHANGES.rst'))),
       license = "BSD",
-      data_files = [("", ["LICENSE.txt"])],
+      data_files = [("", ["LICENSE.txt", "CHANGES.rst"])],
       author = "Malthe Borch",
       author_email = "mborch@gmail.com",
       url = 'https://github.com/malthe/macfsevents',
       cmdclass = dict(build_ext=build_ext),
       ext_modules = ext_modules,
       platforms = ["Mac OS X"],
       classifiers = [
```

