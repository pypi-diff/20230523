# Comparing `tmp/superfluid-0.0.4.tar.gz` & `tmp/superfluid-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.0.4.tar", last modified: Tue May 23 15:50:57 2023, max compression
+gzip compressed data, was "superfluid-0.0.5.tar", last modified: Tue May 23 16:07:04 2023, max compression
```

## Comparing `superfluid-0.0.4.tar` & `superfluid-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 15:50:57.174252 superfluid-0.0.4/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.4/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2821 2023-05-23 15:50:57.171175 superfluid-0.0.4/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.4/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 15:50:57.168715 superfluid-0.0.4/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 15:50:57.170982 superfluid-0.0.4/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2821 2023-05-23 15:50:57.000000 superfluid-0.0.4/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      224 2023-05-23 15:50:57.000000 superfluid-0.0.4/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 15:50:57.000000 superfluid-0.0.4/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 15:50:57.000000 superfluid-0.0.4/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 15:50:57.000000 superfluid-0.0.4/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 15:50:57.174309 superfluid-0.0.4/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      827 2023-05-23 15:49:48.000000 superfluid-0.0.4/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:07:04.878229 superfluid-0.0.5/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.5/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:07:04.877992 superfluid-0.0.5/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.5/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:07:04.875935 superfluid-0.0.5/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:07:04.877255 superfluid-0.0.5/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      224 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:07:04.000000 superfluid-0.0.5/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:07:04.878273 superfluid-0.0.5/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      824 2023-05-23 16:06:59.000000 superfluid-0.0.5/setup.py
```

### Comparing `superfluid-0.0.4/LICENSE.txt` & `superfluid-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.4/PKG-INFO` & `superfluid-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <h1 align="center">Welcome to Superfluid Python SDK 👋
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.5 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
+Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
                                [Superfluid logo]
                     [License:_MIT] [Twitter:_Superfluid_HQ]
 ### ð  [Homepage](https://superfluid.finance) ### â¨ [Superfluid App](https:
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)
```

### Comparing `superfluid-0.0.4/README.md` & `superfluid-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.4/main/superfluid.egg-info/PKG-INFO` & `superfluid-0.0.5/main/superfluid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <h1 align="center">Welcome to Superfluid Python SDK 👋
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.5 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
+Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
                                [Superfluid logo]
                     [License:_MIT] [Twitter:_Superfluid_HQ]
 ### ð  [Homepage](https://superfluid.finance) ### â¨ [Superfluid App](https:
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)
```

### Comparing `superfluid-0.0.4/setup.py` & `superfluid-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.0.4",
+    version="0.0.5",
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
-        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
     ],
     install_requires=["web3 == 6.3.0"],
     extras_require={
         "dev": ["twine>=4.0.2"]
     },
     python_requires=">=3"
```

