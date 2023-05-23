# Comparing `tmp/nexus-utilities-0.5.2.tar.gz` & `tmp/nexus-utilities-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.5.2.tar", last modified: Tue May 23 12:58:25 2023, max compression
+gzip compressed data, was "nexus-utilities-0.5.3.tar", last modified: Tue May 23 13:14:59 2023, max compression
```

## Comparing `nexus-utilities-0.5.2.tar` & `nexus-utilities-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:58:25.714488 nexus-utilities-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 12:58:25.714488 nexus-utilities-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:58:25.714488 nexus-utilities-0.5.2/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 12:58:25.000000 nexus-utilities-0.5.2/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-23 12:58:25.000000 nexus-utilities-0.5.2/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:58:25.000000 nexus-utilities-0.5.2/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 12:58:25.000000 nexus-utilities-0.5.2/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 12:58:25.000000 nexus-utilities-0.5.2/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:58:25.714488 nexus-utilities-0.5.2/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/nexus_utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:58:25.714488 nexus-utilities-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-23 12:58:09.000000 nexus-utilities-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-23 13:14:59.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/setup.py
```

### Comparing `nexus-utilities-0.5.2/LICENSE.txt` & `nexus-utilities-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/PKG-INFO` & `nexus-utilities-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.5.2
+Version: 0.5.3
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.5.2/README.md` & `nexus-utilities-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.5.3/nexus_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.5.2
+Version: 0.5.3
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.5.2/nexus_utils/config_utils.py` & `nexus-utilities-0.5.3/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/nexus_utils/database_utils.py` & `nexus-utilities-0.5.3/nexus_utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/nexus_utils/datetime_utils.py` & `nexus-utilities-0.5.3/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/nexus_utils/flatfile_utils.py` & `nexus-utilities-0.5.3/nexus_utils/flatfile_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         # Determine the encoding of the content
         result = chardet.detect(content)
 
     encoding = result['encoding']
 
     # If the detected encoding is ASCII, read the entire file to confirm the encoding
     if encoding.lower() == 'ascii':
-        with open(file_path, 'r', encoding=encoding) as f:
+        with open(file_path, 'rb') as f:
             content = f.read()
             # Determine the encoding of the entire file
             result = chardet.detect(content)
             encoding = result['encoding']
 
     return encoding
```

### Comparing `nexus-utilities-0.5.2/nexus_utils/package_utils.py` & `nexus-utilities-0.5.3/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/nexus_utils/password_utils.py` & `nexus-utilities-0.5.3/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/nexus_utils/string_utils.py` & `nexus-utilities-0.5.3/nexus_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.2/setup.py` & `nexus-utilities-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.5.2',
+    version='0.5.3',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

