# Comparing `tmp/MandiriUtils-0.1.tar.gz` & `tmp/MandiriUtils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MandiriUtils-0.1.tar", last modified: Tue May 23 03:00:19 2023, max compression
+gzip compressed data, was "MandiriUtils-0.2.tar", last modified: Tue May 23 03:12:09 2023, max compression
```

## Comparing `MandiriUtils-0.1.tar` & `MandiriUtils-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:00:19.842212 MandiriUtils-0.1/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.1/LICENSE.txt
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:00:19.842212 MandiriUtils-0.1/MandiriUtils/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     2457 2023-05-23 02:47:09.000000 MandiriUtils-0.1/MandiriUtils/Client.py
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       44 2023-05-23 02:47:10.000000 MandiriUtils-0.1/MandiriUtils/__init__.py
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:00:19.842212 MandiriUtils-0.1/MandiriUtils.egg-info/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 03:00:19.000000 MandiriUtils-0.1/MandiriUtils.egg-info/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      267 2023-05-23 03:00:19.000000 MandiriUtils-0.1/MandiriUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 03:00:19.000000 MandiriUtils-0.1/MandiriUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 03:00:19.000000 MandiriUtils-0.1/MandiriUtils.egg-info/requires.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 03:00:19.000000 MandiriUtils-0.1/MandiriUtils.egg-info/top_level.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 03:00:19.842212 MandiriUtils-0.1/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.1/README.md
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 03:00:19.842212 MandiriUtils-0.1/setup.cfg
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 02:59:53.000000 MandiriUtils-0.1/setup.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:12:09.379016 MandiriUtils-0.2/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.2/LICENSE.txt
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:12:09.375016 MandiriUtils-0.2/MandiriUtils/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     2457 2023-05-23 02:47:09.000000 MandiriUtils-0.2/MandiriUtils/Client.py
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.2/MandiriUtils/__init__.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:12:09.379016 MandiriUtils-0.2/MandiriUtils.egg-info/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      267 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/requires.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/top_level.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 03:12:09.379016 MandiriUtils-0.2/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.2/README.md
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 03:12:09.379016 MandiriUtils-0.2/setup.cfg
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 03:12:06.000000 MandiriUtils-0.2/setup.py
```

### Comparing `MandiriUtils-0.1/LICENSE.txt` & `MandiriUtils-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MandiriUtils-0.1/MandiriUtils/Client.py` & `MandiriUtils-0.2/MandiriUtils/Client.py`

 * *Files identical despite different names*

### Comparing `MandiriUtils-0.1/MandiriUtils.egg-info/PKG-INFO` & `MandiriUtils-0.2/MandiriUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.1
+Version: 0.2
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_03.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.1/PKG-INFO` & `MandiriUtils-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.1
+Version: 0.2
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_03.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.1/setup.py` & `MandiriUtils-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'MandiriUtils',         
   packages = ['MandiriUtils'],   
-  version = '0.1',      
+  version = '0.2',      
   license='MIT',        
   description = 'Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API',
   author = 'Hanif Amal Robbani',       
   author_email = 'dev.har07@gmail.com',
   url = 'https://github.com/har07',
-  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_02.tar.gz', 
+  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_03.tar.gz', 
   keywords = ['banking', 'signature', 'token', 'mandiri'], 
   install_requires=[
           'pycryptodome==3.17.0',
           'requests==2.22.0',
           'pyjks==20.0.0',
       ],
   classifiers=[
```

