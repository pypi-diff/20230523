# Comparing `tmp/translateabc-1.0.1.tar.gz` & `tmp/translateabc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translateabc-1.0.1.tar", last modified: Tue May 23 12:06:26 2023, max compression
+gzip compressed data, was "translateabc-1.0.2.tar", last modified: Tue May 23 12:31:33 2023, max compression
```

## Comparing `translateabc-1.0.1.tar` & `translateabc-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 12:06:26.398101 translateabc-1.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-23 11:45:45.000000 translateabc-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      491 2023-05-23 12:06:26.397096 translateabc-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-23 11:45:51.000000 translateabc-1.0.1/README.md
--rw-rw-rw-   0        0        0       88 2023-05-23 11:45:30.000000 translateabc-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 12:06:26.398101 translateabc-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-05-23 12:05:24.000000 translateabc-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:06:26.385088 translateabc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:06:26.391592 translateabc-1.0.1/src/translateabc/
--rw-rw-rw-   0        0        0       69 2023-05-23 11:44:44.000000 translateabc-1.0.1/src/translateabc/__init__.py
--rw-rw-rw-   0        0        0      386 2023-05-23 11:44:03.000000 translateabc-1.0.1/src/translateabc/translateabc.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:06:26.396596 translateabc-1.0.1/src/translateabc.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-23 12:06:26.000000 translateabc-1.0.1/src/translateabc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-23 12:06:26.000000 translateabc-1.0.1/src/translateabc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 12:06:26.000000 translateabc-1.0.1/src/translateabc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 12:06:26.000000 translateabc-1.0.1/src/translateabc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.201017 translateabc-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.168428 translateabc-1.0.2/.idea/
+-rw-rw-rw-   0        0        0      184 2023-05-23 11:40:39.000000 translateabc-1.0.2/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.169429 translateabc-1.0.2/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      174 2023-05-23 11:40:38.000000 translateabc-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      182 2023-05-23 11:48:08.000000 translateabc-1.0.2/.idea/misc.xml
+-rw-rw-rw-   0        0        0      283 2023-05-23 11:40:38.000000 translateabc-1.0.2/.idea/modules.xml
+-rw-rw-rw-   0        0        0      318 2023-05-23 11:48:08.000000 translateabc-1.0.2/.idea/translateabc.iml
+-rw-rw-rw-   0        0        0     4010 2023-05-23 12:31:12.000000 translateabc-1.0.2/.idea/workspace.xml
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:45:45.000000 translateabc-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-23 12:30:23.000000 translateabc-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      491 2023-05-23 12:31:33.201017 translateabc-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:45:51.000000 translateabc-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.173456 translateabc-1.0.2/dist/
+-rw-rw-rw-   0        0        0  1675410 2023-05-23 12:31:15.000000 translateabc-1.0.2/dist/translateabc-1.0.2.tar.gz
+-rw-rw-rw-   0        0        0   531223 2023-05-23 12:31:15.000000 translateabc-1.0.2/dist/translateabc-1.0.2.win-amd64.zip
+-rw-rw-rw-   0        0        0       88 2023-05-23 11:45:30.000000 translateabc-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 12:31:33.201535 translateabc-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-23 12:31:12.000000 translateabc-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.155399 translateabc-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.175958 translateabc-1.0.2/src/translateabc/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.156901 translateabc-1.0.2/src/translateabc/READMEhh/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.156400 translateabc-1.0.2/src/translateabc/READMEhh/ai35/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.187475 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/
+-rw-rw-rw-   0        0        0     2469 2023-05-22 14:26:06.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/1.ipynb
+-rw-rw-rw-   0        0        0     5078 2023-05-22 14:26:04.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/2.ipynb
+-rw-rw-rw-   0        0        0     2661 2023-05-22 14:30:18.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/3.ipynb
+-rw-rw-rw-   0        0        0    12943 2023-05-22 14:36:23.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/4.ipynb
+-rw-rw-rw-   0        0        0     4965 2023-05-22 14:48:13.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/5.ipynb
+-rw-rw-rw-   0        0        0     3570 2023-05-22 15:10:05.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/6.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.188984 translateabc-1.0.2/src/translateabc/READMEhh/ai35/02/
+-rw-rw-rw-   0        0        0        0 2023-05-22 14:53:43.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/02/01.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.189985 translateabc-1.0.2/src/translateabc/READMEhh/moni/
+-rw-rw-rw-   0        0        0  4928289 2022-08-06 03:19:14.000000 translateabc-1.0.2/src/translateabc/READMEhh/moni/bankmarketing.csv
+-r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.2/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.199013 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/
+-rw-rw-rw-   0        0        0      124 2023-05-22 15:56:25.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/1.csv
+-rw-rw-rw-   0        0        0     5625 2023-05-22 16:09:33.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/1.ipynb
+-rw-rw-rw-   0        0        0       53 2023-05-22 15:56:19.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/2.csv
+-rw-rw-rw-   0        0        0      167 2023-05-22 15:59:00.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/output.csv
+-rw-rw-rw-   0        0        0       69 2023-05-23 11:44:44.000000 translateabc-1.0.2/src/translateabc/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-05-23 11:44:03.000000 translateabc-1.0.2/src/translateabc/translateabc.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.179962 translateabc-1.0.2/src/translateabc.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.232976 translateabc-1.0.2/translateabc-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.232976 translateabc-1.0.2/translateabc-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.232976 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.233980 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.276650 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/
+-r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
```

### Comparing `translateabc-1.0.1/setup.py` & `translateabc-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="translateabc",
-    version="1.0.1",
+    version="1.0.2",
     author="Linvery",
     author_email="1253445120@qq.com",
     description="translateabc",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    include_package_data=True,
     url="https://github.com/pypa/sampleproject",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

