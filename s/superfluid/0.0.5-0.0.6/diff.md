# Comparing `tmp/superfluid-0.0.5.tar.gz` & `tmp/superfluid-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.0.5.tar", last modified: Tue May 23 16:07:04 2023, max compression
+gzip compressed data, was "superfluid-0.0.6.tar", last modified: Tue May 23 16:17:32 2023, max compression
```

## Comparing `superfluid-0.0.5.tar` & `superfluid-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:07:04.878229 superfluid-0.0.5/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.5/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:07:04.877992 superfluid-0.0.5/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.5/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:07:04.875935 superfluid-0.0.5/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:07:04.877255 superfluid-0.0.5/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      224 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:07:04.878273 superfluid-0.0.5/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      824 2023-05-23 16:06:59.000000 superfluid-0.0.5/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:17:32.497616 superfluid-0.0.6/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.6/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:17:32.497475 superfluid-0.0.6/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.6/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:17:32.493054 superfluid-0.0.6/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:17:32.493609 superfluid-0.0.6/main/superfluid/
+-rw-r--r--   0 godspowereze   (501) staff       (20)      114 2023-05-23 16:16:43.000000 superfluid-0.0.6/main/superfluid/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:17:32.497293 superfluid-0.0.6/main/superfluid/src/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.0.6/main/superfluid/src/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     5339 2023-05-23 07:38:08.000000 superfluid-0.0.6/main/superfluid/src/__types__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     9367 2023-05-23 08:19:40.000000 superfluid-0.0.6/main/superfluid/src/cfa.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      709 2023-05-18 07:21:56.000000 superfluid-0.0.6/main/superfluid/src/constants.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)       84 2023-05-10 07:50:23.000000 superfluid-0.0.6/main/superfluid/src/errors.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1011 2023-05-23 06:52:12.000000 superfluid-0.0.6/main/superfluid/src/host.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1700 2023-05-23 06:54:22.000000 superfluid-0.0.6/main/superfluid/src/operation.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      759 2023-05-23 07:47:53.000000 superfluid-0.0.6/main/superfluid/src/utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:17:32.496275 superfluid-0.0.6/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:17:32.000000 superfluid-0.0.6/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      497 2023-05-23 16:17:32.000000 superfluid-0.0.6/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:17:32.000000 superfluid-0.0.6/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 16:17:32.000000 superfluid-0.0.6/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-23 16:17:32.000000 superfluid-0.0.6/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:17:32.497654 superfluid-0.0.6/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      824 2023-05-23 16:13:54.000000 superfluid-0.0.6/setup.py
```

### Comparing `superfluid-0.0.5/LICENSE.txt` & `superfluid-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.5/PKG-INFO` & `superfluid-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.6 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
```

### Comparing `superfluid-0.0.5/README.md` & `superfluid-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.5/main/superfluid.egg-info/PKG-INFO` & `superfluid-0.0.6/main/superfluid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.6 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
```

### Comparing `superfluid-0.0.5/setup.py` & `superfluid-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.0.5",
+    version="0.0.6",
     description="Python SDK for the Superfluid Protocol",
     package_dir={"": "main"},
     packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
```

