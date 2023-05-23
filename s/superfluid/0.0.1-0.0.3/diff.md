# Comparing `tmp/superfluid-0.0.1.tar.gz` & `tmp/superfluid-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.0.1.tar", last modified: Tue May 23 08:40:11 2023, max compression
+gzip compressed data, was "superfluid-0.0.3.tar", last modified: Tue May 23 15:18:20 2023, max compression
```

## Comparing `superfluid-0.0.1.tar` & `superfluid-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 08:40:11.718618 superfluid-0.0.1/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.1/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2824 2023-05-23 08:40:11.718485 superfluid-0.0.1/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.1/README.md
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 08:40:11.718657 superfluid-0.0.1/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      828 2023-05-23 08:39:55.000000 superfluid-0.0.1/setup.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 08:40:11.715566 superfluid-0.0.1/src/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 08:40:11.718273 superfluid-0.0.1/src/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2824 2023-05-23 08:40:11.000000 superfluid-0.0.1/src/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      219 2023-05-23 08:40:11.000000 superfluid-0.0.1/src/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 08:40:11.000000 superfluid-0.0.1/src/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 08:40:11.000000 superfluid-0.0.1/src/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 08:40:11.000000 superfluid-0.0.1/src/superfluid.egg-info/top_level.txt
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 15:18:20.214954 superfluid-0.0.3/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.3/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2824 2023-05-23 15:18:20.214827 superfluid-0.0.3/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.3/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 15:18:20.213561 superfluid-0.0.3/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 15:18:20.214572 superfluid-0.0.3/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2824 2023-05-23 15:18:20.000000 superfluid-0.0.3/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      224 2023-05-23 15:18:20.000000 superfluid-0.0.3/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 15:18:20.000000 superfluid-0.0.3/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 15:18:20.000000 superfluid-0.0.3/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 15:18:20.000000 superfluid-0.0.3/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 15:18:20.214989 superfluid-0.0.3/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      830 2023-05-23 15:18:13.000000 superfluid-0.0.3/setup.py
```

### Comparing `superfluid-0.0.1/LICENSE.txt` & `superfluid-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.1/PKG-INFO` & `superfluid-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.1
+Version: 0.0.3
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <h1 align="center">Welcome to Superfluid Python SDK 👋
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.3 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.10 Classifier: Operating System :: OS
+Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
                                [Superfluid logo]
                     [License:_MIT] [Twitter:_Superfluid_HQ]
 ### ð  [Homepage](https://superfluid.finance) ### â¨ [Superfluid App](https:
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)
```

### Comparing `superfluid-0.0.1/README.md` & `superfluid-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.1/setup.py` & `superfluid-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.0.1",
+    version="0.0.3",
     description="Python SDK for the Superfluid Protocol",
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
+    package_dir={"": "main"},
+    packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
     author_email="Godspowereze260@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent"
     ],
     install_requires=["web3 == 6.3.0"],
     extras_require={
         "dev": ["twine>=4.0.2"]
     },
     python_requires=">=3.11"
```

### Comparing `superfluid-0.0.1/src/superfluid.egg-info/PKG-INFO` & `superfluid-0.0.3/main/superfluid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.1
+Version: 0.0.3
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <h1 align="center">Welcome to Superfluid Python SDK 👋
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.3 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.10 Classifier: Operating System :: OS
+Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
                                [Superfluid logo]
                     [License:_MIT] [Twitter:_Superfluid_HQ]
 ### ð  [Homepage](https://superfluid.finance) ### â¨ [Superfluid App](https:
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)
```

