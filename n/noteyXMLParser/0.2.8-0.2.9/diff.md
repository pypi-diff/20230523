# Comparing `tmp/noteyXMLParser-0.2.8.tar.gz` & `tmp/noteyXMLParser-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/noteyXMLParser-0.2.8.tar", last modified: Sat Apr 29 22:38:39 2023, max compression
+gzip compressed data, was "dist/noteyXMLParser-0.2.9.tar", last modified: Tue May 23 01:24:39 2023, max compression
```

## Comparing `noteyXMLParser-0.2.8.tar` & `noteyXMLParser-0.2.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-04-29 22:38:39.397964 noteyXMLParser-0.2.8/
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      904 2023-04-29 22:38:39.397456 noteyXMLParser-0.2.8/PKG-INFO
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      359 2023-04-11 06:22:11.000000 noteyXMLParser-0.2.8/README.md
--rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-04-29 22:38:39.398169 noteyXMLParser-0.2.8/setup.cfg
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      689 2023-04-29 22:38:32.000000 noteyXMLParser-0.2.8/setup.py
+drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-05-23 01:24:39.887789 noteyXMLParser-0.2.9/
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      904 2023-05-23 01:24:39.887514 noteyXMLParser-0.2.9/PKG-INFO
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      359 2023-04-11 06:22:11.000000 noteyXMLParser-0.2.9/README.md
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-05-23 01:24:39.887983 noteyXMLParser-0.2.9/setup.cfg
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      675 2023-05-23 01:24:22.000000 noteyXMLParser-0.2.9/setup.py
```

### Comparing `noteyXMLParser-0.2.8/PKG-INFO` & `noteyXMLParser-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noteyXMLParser
-Version: 0.2.8
+Version: 0.2.9
 Summary: Music XML Parser
 Home-page: https://github.com/mmahjoub5/NoteyXMLParser
 Author: Amin Mahjoub
 Author-email: mahjoub@usc.edu
 License: UNKNOWN
 Description: my parser
```

### Comparing `noteyXMLParser-0.2.8/setup.py` & `noteyXMLParser-0.2.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
-     name='noteyXMLParser',  
-     version='0.2.8',
-     author="Amin Mahjoub",
-     author_email="mahjoub@usc.edu",
-     description="Music XML Parser",
-     long_description=long_description,
-     package_dir={"":"/Users/aminmahjoub/NoteyXMLParser/xmlParser/src"},
-     url="https://github.com/mmahjoub5/NoteyXMLParser",
-   long_description_content_type="text/markdown",
-     packages=['noteyXMLParser'],
-     classifiers=[
-         "Programming Language :: Python :: 3",
-         "License :: OSI Approved :: MIT License",
-         "Operating System :: OS Independent",
-     ],
- )
+    name="noteyXMLParser",
+    version="0.2.9",
+    author="Amin Mahjoub",
+    author_email="mahjoub@usc.edu",
+    description="Music XML Parser",
+    long_description=long_description,
+    package_dir={"": "/Users/aminmahjoub/NoteyXMLParser/xmlParser/src"},
+    url="https://github.com/mmahjoub5/NoteyXMLParser",
+    long_description_content_type="text/markdown",
+    packages=["noteyXMLParser"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+)
```

