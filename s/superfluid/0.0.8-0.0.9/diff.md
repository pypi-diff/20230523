# Comparing `tmp/superfluid-0.0.8.tar.gz` & `tmp/superfluid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.0.8.tar", last modified: Tue May 23 16:29:14 2023, max compression
+gzip compressed data, was "superfluid-0.0.9.tar", last modified: Tue May 23 16:33:53 2023, max compression
```

## Comparing `superfluid-0.0.8.tar` & `superfluid-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.557785 superfluid-0.0.8/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.8/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:29:14.557644 superfluid-0.0.8/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.8/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.551634 superfluid-0.0.8/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.552183 superfluid-0.0.8/main/superfluid/
--rw-r--r--   0 godspowereze   (501) staff       (20)      118 2023-05-23 16:22:23.000000 superfluid-0.0.8/main/superfluid/__init__.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.557456 superfluid-0.0.8/main/superfluid/src/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.0.8/main/superfluid/src/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     5339 2023-05-23 07:38:08.000000 superfluid-0.0.8/main/superfluid/src/__types__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     9372 2023-05-23 16:28:15.000000 superfluid-0.0.8/main/superfluid/src/cfa.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      709 2023-05-18 07:21:56.000000 superfluid-0.0.8/main/superfluid/src/constants.py
--rw-r--r--   0 godspowereze   (501) staff       (20)       84 2023-05-10 07:50:23.000000 superfluid-0.0.8/main/superfluid/src/errors.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1014 2023-05-23 16:28:39.000000 superfluid-0.0.8/main/superfluid/src/host.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1701 2023-05-23 16:28:48.000000 superfluid-0.0.8/main/superfluid/src/operation.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      760 2023-05-23 16:28:53.000000 superfluid-0.0.8/main/superfluid/src/utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.555054 superfluid-0.0.8/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      497 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:29:14.557822 superfluid-0.0.8/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      824 2023-05-23 16:29:13.000000 superfluid-0.0.8/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.733557 superfluid-0.0.9/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.9/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:33:53.733386 superfluid-0.0.9/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.9/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.729408 superfluid-0.0.9/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.729958 superfluid-0.0.9/main/superfluid/
+-rw-r--r--   0 godspowereze   (501) staff       (20)      118 2023-05-23 16:22:23.000000 superfluid-0.0.9/main/superfluid/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.732915 superfluid-0.0.9/main/superfluid/src/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.0.9/main/superfluid/src/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     5339 2023-05-23 07:38:08.000000 superfluid-0.0.9/main/superfluid/src/__types__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     9372 2023-05-23 16:28:15.000000 superfluid-0.0.9/main/superfluid/src/cfa.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      709 2023-05-18 07:21:56.000000 superfluid-0.0.9/main/superfluid/src/constants.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)       84 2023-05-10 07:50:23.000000 superfluid-0.0.9/main/superfluid/src/errors.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1014 2023-05-23 16:28:39.000000 superfluid-0.0.9/main/superfluid/src/host.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1701 2023-05-23 16:28:48.000000 superfluid-0.0.9/main/superfluid/src/operation.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      760 2023-05-23 16:28:53.000000 superfluid-0.0.9/main/superfluid/src/utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.731001 superfluid-0.0.9/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      497 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:33:53.733598 superfluid-0.0.9/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-23 16:33:20.000000 superfluid-0.0.9/setup.py
```

### Comparing `superfluid-0.0.8/LICENSE.txt` & `superfluid-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/PKG-INFO` & `superfluid-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.8
+Version: 0.0.9
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
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.8 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.9 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
```

### Comparing `superfluid-0.0.8/README.md` & `superfluid-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/main/superfluid/src/__types__.py` & `superfluid-0.0.9/main/superfluid/src/__types__.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/main/superfluid/src/cfa.py` & `superfluid-0.0.9/main/superfluid/src/cfa.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/main/superfluid/src/constants.py` & `superfluid-0.0.9/main/superfluid/src/constants.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/main/superfluid/src/host.py` & `superfluid-0.0.9/main/superfluid/src/host.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/main/superfluid/src/operation.py` & `superfluid-0.0.9/main/superfluid/src/operation.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/main/superfluid/src/utils.py` & `superfluid-0.0.9/main/superfluid/src/utils.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.8/main/superfluid.egg-info/PKG-INFO` & `superfluid-0.0.9/main/superfluid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.8
+Version: 0.0.9
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
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.8 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.9 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
```

### Comparing `superfluid-0.0.8/setup.py` & `superfluid-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.0.8",
+    version="0.0.9",
     description="Python SDK for the Superfluid Protocol",
     package_dir={"": "main"},
     packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
     author_email="Godspowereze260@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
     ],
-    install_requires=["web3 == 6.3.0"],
+    install_requires=["web3 == 6.3.0", "python-decouple==3.8"],
     extras_require={
         "dev": ["twine>=4.0.2"]
     },
     python_requires=">=3"
 )
```

