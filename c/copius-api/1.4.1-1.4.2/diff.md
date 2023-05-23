# Comparing `tmp/copius_api-1.4.1.tar.gz` & `tmp/copius_api-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copius_api-1.4.1.tar", last modified: Tue May 23 16:06:59 2023, max compression
+gzip compressed data, was "copius_api-1.4.2.tar", last modified: Tue May 23 16:22:50 2023, max compression
```

## Comparing `copius_api-1.4.1.tar` & `copius_api-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3676 2023-05-23 16:06:59.075521 copius_api-1.4.1/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     2003 2023-05-23 15:59:18.000000 copius_api-1.4.1/README.rst
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/copius_api/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-05-23 15:39:49.000000 copius_api-1.4.1/copius_api/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1485 2023-05-23 15:41:40.000000 copius_api-1.4.1/copius_api/api.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/copius_api.egg-info/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3676 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      265 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       48 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       17 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/top_level.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2023-05-23 16:06:59.075521 copius_api-1.4.1/setup.cfg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1372 2023-05-23 16:06:32.000000 copius_api-1.4.1/setup.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/tests/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-05-23 15:39:49.000000 copius_api-1.4.1/tests/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      425 2023-05-23 15:39:49.000000 copius_api-1.4.1/tests/test_api.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:22:50.058045 copius_api-1.4.2/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3676 2023-05-23 16:22:50.058045 copius_api-1.4.2/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     2003 2023-05-23 15:59:18.000000 copius_api-1.4.2/README.rst
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:22:50.058045 copius_api-1.4.2/copius_api/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-05-23 15:39:49.000000 copius_api-1.4.2/copius_api/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1485 2023-05-23 15:41:40.000000 copius_api-1.4.2/copius_api/api.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:22:50.058045 copius_api-1.4.2/copius_api.egg-info/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3676 2023-05-23 16:22:50.000000 copius_api-1.4.2/copius_api.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      265 2023-05-23 16:22:50.000000 copius_api-1.4.2/copius_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-05-23 16:22:50.000000 copius_api-1.4.2/copius_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       72 2023-05-23 16:22:50.000000 copius_api-1.4.2/copius_api.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       17 2023-05-23 16:22:50.000000 copius_api-1.4.2/copius_api.egg-info/top_level.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2023-05-23 16:22:50.058045 copius_api-1.4.2/setup.cfg
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1452 2023-05-23 16:22:19.000000 copius_api-1.4.2/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:22:50.058045 copius_api-1.4.2/tests/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-05-23 15:39:49.000000 copius_api-1.4.2/tests/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      425 2023-05-23 15:39:49.000000 copius_api-1.4.2/tests/test_api.py
```

### Comparing `copius_api-1.4.1/PKG-INFO` & `copius_api-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: copius_api
-Version: 1.4.1
+Version: 1.4.2
 Summary: Transcription & orthography toolset
 Home-page: https://github.com/martino-vic/copius_api
 Author: Viktor Martinović
 Author-email: viktoringermany@gmail.com
 License: MIT
-Download-URL: https://github.com/martino-vic/copius_api/archive/refs/tags/v1.4.1.tar.gz
+Download-URL: https://github.com/martino-vic/copius_api/archive/refs/tags/v1.4.2.tar.gz
 Project-URL: continuous integration, https://app.circleci.com/pipelines/github/martino-vic/copius_api?branch=master
 Description: |DOI| |CircleCI|
         
         copius_api
         ==========
         
         This is a Python-api to the transcription and orthography toolset at
```

### Comparing `copius_api-1.4.1/README.rst` & `copius_api-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `copius_api-1.4.1/copius_api/api.py` & `copius_api-1.4.2/copius_api/api.py`

 * *Files identical despite different names*

### Comparing `copius_api-1.4.1/copius_api.egg-info/PKG-INFO` & `copius_api-1.4.2/copius_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: copius-api
-Version: 1.4.1
+Version: 1.4.2
 Summary: Transcription & orthography toolset
 Home-page: https://github.com/martino-vic/copius_api
 Author: Viktor Martinović
 Author-email: viktoringermany@gmail.com
 License: MIT
-Download-URL: https://github.com/martino-vic/copius_api/archive/refs/tags/v1.4.1.tar.gz
+Download-URL: https://github.com/martino-vic/copius_api/archive/refs/tags/v1.4.2.tar.gz
 Project-URL: continuous integration, https://app.circleci.com/pipelines/github/martino-vic/copius_api?branch=master
 Description: |DOI| |CircleCI|
         
         copius_api
         ==========
         
         This is a Python-api to the transcription and orthography toolset at
```

### Comparing `copius_api-1.4.1/setup.py` & `copius_api-1.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 
 setup(
   name='copius_api',
   description='Transcription & orthography toolset',
   long_description=open("README.rst").read(),
   author='Viktor Martinović',
   author_email='viktoringermany@gmail.com',
-  version='1.4.1',
+  version='1.4.2',
   packages=find_packages(),
   extras_require={
   "test": ["pytest>=7.1.2"],
   "dev": ["wheel", "twine", "sphinx"]
   },
+  install_requires=[
+          'requests',
+          'beautifulsoup4',
+      ],
   keywords=['linguistics', 'transcription'],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering',
     "Topic :: Text Processing :: Linguistic",
     'License :: OSI Approved :: MIT License',
@@ -30,15 +34,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 
   ],
   url='https://github.com/martino-vic/copius_api',
-  download_url='https://github.com/martino-vic/copius_api/archive/refs/tags/v1.4.1.tar.gz',
+  download_url='https://github.com/martino-vic/copius_api/archive/refs/tags/v1.4.2.tar.gz',
   license='MIT',
   platforms=["Linux"],
   python_requires=">=3.7",
   project_urls={
   "continuous integration": "https://app.circleci.com/pipelines/github/martino-vic/copius_api?branch=master",
   }
 )
```

