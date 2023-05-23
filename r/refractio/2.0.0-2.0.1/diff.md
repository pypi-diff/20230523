# Comparing `tmp/refractio-2.0.0.tar.gz` & `tmp/refractio-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.0.tar", last modified: Fri May 19 12:18:01 2023, max compression
+gzip compressed data, was "refractio-2.0.1.tar", last modified: Tue May 23 11:24:37 2023, max compression
```

## Comparing `refractio-2.0.0.tar` & `refractio-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-19 12:18:01.303391 refractio-2.0.0/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     2356 2023-05-19 12:18:01.303391 refractio-2.0.0/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1687 2023-05-19 12:16:37.000000 refractio-2.0.0/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-19 12:18:01.301391 refractio-2.0.0/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      231 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4707 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-19 12:16:26.000000 refractio-2.0.0/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-19 12:16:26.000000 refractio-2.0.0/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-19 12:16:26.000000 refractio-2.0.0/refractio/snowflake.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-19 12:18:01.302390 refractio-2.0.0/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     2356 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      326 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-19 12:18:01.303391 refractio-2.0.0/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-19 12:16:37.000000 refractio-2.0.0/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-23 11:24:37.214362 refractio-2.0.1/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7560 2023-05-23 11:24:37.213362 refractio-2.0.1/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6891 2023-05-23 10:14:58.000000 refractio-2.0.1/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-23 11:24:37.212361 refractio-2.0.1/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      319 2023-05-23 10:14:58.000000 refractio-2.0.1/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-23 10:14:58.000000 refractio-2.0.1/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-23 10:14:58.000000 refractio-2.0.1/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4707 2023-05-19 12:16:37.000000 refractio-2.0.1/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-19 12:16:37.000000 refractio-2.0.1/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-19 12:16:26.000000 refractio-2.0.1/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-19 12:16:26.000000 refractio-2.0.1/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-19 12:16:37.000000 refractio-2.0.1/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-19 12:16:26.000000 refractio-2.0.1/refractio/snowflake.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-23 11:24:37.213362 refractio-2.0.1/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7560 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      367 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-23 11:24:37.214362 refractio-2.0.1/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-23 10:14:58.000000 refractio-2.0.1/setup.py
```

### Comparing `refractio-2.0.0/refractio/hive.py` & `refractio-2.0.1/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.0/refractio/manager.py` & `refractio-2.0.1/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.0/refractio/mysql.py` & `refractio-2.0.1/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.0/refractio/refractio.py` & `refractio-2.0.1/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.0/refractio/sftp.py` & `refractio-2.0.1/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.0/refractio/snowflake.py` & `refractio-2.0.1/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.0/setup.py` & `refractio-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.0'
+VERSION = '2.0.1'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

