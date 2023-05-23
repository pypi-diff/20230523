# Comparing `tmp/crabpy-1.2.3.tar.gz` & `tmp/crabpy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy-1.2.3.tar", last modified: Mon May 15 12:05:47 2023, max compression
+gzip compressed data, was "crabpy-1.2.4.tar", last modified: Tue May 23 09:15:03 2023, max compression
```

## Comparing `crabpy-1.2.3.tar` & `crabpy-1.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-15 12:05:47.293972 crabpy-1.2.3/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6790 2023-05-15 12:05:37.000000 crabpy-1.2.3/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.2.3/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.2.3/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8441 2023-05-15 12:05:47.293972 crabpy-1.2.3/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.2.3/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-15 12:05:47.289972 crabpy-1.2.3/crabpy/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.3/crabpy/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7552 2023-05-15 12:05:37.000000 crabpy-1.2.3/crabpy/client.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-15 12:05:47.293972 crabpy-1.2.3/crabpy/data/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   238209 2023-05-03 12:29:06.000000 crabpy-1.2.3/crabpy/data/deelgemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.2.3/crabpy/data/gemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.2.3/crabpy/data/gewesten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.2.3/crabpy/data/provincies.json
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-15 12:05:47.293972 crabpy-1.2.3/crabpy/gateway/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.3/crabpy/gateway/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    30229 2023-05-04 13:36:14.000000 crabpy-1.2.3/crabpy/gateway/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.2.3/crabpy/gateway/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.2.3/crabpy/gateway/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.2.3/crabpy/gateway/exception.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.2.3/crabpy/wsa.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.2.3/crabpy/wsse.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-15 12:05:47.289972 crabpy-1.2.3/crabpy.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8441 2023-05-15 12:05:47.000000 crabpy-1.2.3/crabpy.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-05-15 12:05:47.000000 crabpy-1.2.3/crabpy.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-15 12:05:47.000000 crabpy-1.2.3/crabpy.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-05-15 12:05:47.000000 crabpy-1.2.3/crabpy.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.2.3/crabpy.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-05-15 12:05:47.000000 crabpy-1.2.3/crabpy.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-05-15 12:05:47.000000 crabpy-1.2.3/crabpy.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-05-15 12:05:47.293972 crabpy-1.2.3/setup.cfg
--rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-05-15 12:05:37.000000 crabpy-1.2.3/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:15:03.156770 crabpy-1.2.4/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6878 2023-05-23 09:14:50.000000 crabpy-1.2.4/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.2.4/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.2.4/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8529 2023-05-23 09:15:03.156770 crabpy-1.2.4/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.2.4/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:15:03.152770 crabpy-1.2.4/crabpy/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.4/crabpy/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7552 2023-05-15 12:05:37.000000 crabpy-1.2.4/crabpy/client.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:15:03.156770 crabpy-1.2.4/crabpy/data/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    97092 2023-05-23 09:14:50.000000 crabpy-1.2.4/crabpy/data/deelgemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.2.4/crabpy/data/gemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.2.4/crabpy/data/gewesten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.2.4/crabpy/data/provincies.json
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:15:03.156770 crabpy-1.2.4/crabpy/gateway/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.4/crabpy/gateway/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    30229 2023-05-04 13:36:14.000000 crabpy-1.2.4/crabpy/gateway/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.2.4/crabpy/gateway/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.2.4/crabpy/gateway/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.2.4/crabpy/gateway/exception.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.2.4/crabpy/wsa.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.2.4/crabpy/wsse.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:15:03.156770 crabpy-1.2.4/crabpy.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8529 2023-05-23 09:15:03.000000 crabpy-1.2.4/crabpy.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-05-23 09:15:03.000000 crabpy-1.2.4/crabpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-23 09:15:03.000000 crabpy-1.2.4/crabpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-05-23 09:15:03.000000 crabpy-1.2.4/crabpy.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.2.4/crabpy.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-05-23 09:15:03.000000 crabpy-1.2.4/crabpy.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-05-23 09:15:03.000000 crabpy-1.2.4/crabpy.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-05-23 09:15:03.156770 crabpy-1.2.4/setup.cfg
+-rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-05-23 09:14:50.000000 crabpy-1.2.4/setup.py
```

### Comparing `crabpy-1.2.3/CHANGES.rst` & `crabpy-1.2.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.2.4 (23-05-2023)
+------------------
+
+- Foute lijst van deelgemeenten gebruikt (#225)
+
 1.2.3 (15-05-2023)
 ------------------
 
 - Limiet van list op 1000 items (#221)
 
 1.2.2 (09-05-2023)
 ------------------
```

### Comparing `crabpy-1.2.3/LICENSE` & `crabpy-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/PKG-INFO` & `crabpy-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.2.3
+Version: 1.2.4
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.2.4 (23-05-2023)
+------------------
+
+- Foute lijst van deelgemeenten gebruikt (#225)
+
 1.2.3 (15-05-2023)
 ------------------
 
 - Limiet van list op 1000 items (#221)
 
 1.2.2 (09-05-2023)
 ------------------
```

### Comparing `crabpy-1.2.3/README.rst` & `crabpy-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/client.py` & `crabpy-1.2.4/crabpy/client.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/data/gemeenten.json` & `crabpy-1.2.4/crabpy/data/gemeenten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/data/gewesten.json` & `crabpy-1.2.4/crabpy/data/gewesten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/data/provincies.json` & `crabpy-1.2.4/crabpy/data/provincies.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/gateway/adressenregister.py` & `crabpy-1.2.4/crabpy/gateway/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/gateway/capakey.py` & `crabpy-1.2.4/crabpy/gateway/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/gateway/crab.py` & `crabpy-1.2.4/crabpy/gateway/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/gateway/exception.py` & `crabpy-1.2.4/crabpy/gateway/exception.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/wsa.py` & `crabpy-1.2.4/crabpy/wsa.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy/wsse.py` & `crabpy-1.2.4/crabpy/wsse.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/crabpy.egg-info/PKG-INFO` & `crabpy-1.2.4/crabpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.2.3
+Version: 1.2.4
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.2.4 (23-05-2023)
+------------------
+
+- Foute lijst van deelgemeenten gebruikt (#225)
+
 1.2.3 (15-05-2023)
 ------------------
 
 - Limiet van list op 1000 items (#221)
 
 1.2.2 (09-05-2023)
 ------------------
```

### Comparing `crabpy-1.2.3/crabpy.egg-info/SOURCES.txt` & `crabpy-1.2.4/crabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.3/setup.py` & `crabpy-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "crabpy",
 ]
 
 requires = ["suds-py3>=1.4.4.1", "dogpile.cache", "requests"]
 
 setup(
     name="crabpy",
-    version="1.2.3",
+    version="1.2.4",
     description="Interact with geographical webservices by Informatie Vlaanderen.",
     long_description=open("README.rst").read() + "\n\n" + open("CHANGES.rst").read(),
     author="Onroerend Erfgoed",
     author_email="ict@onroerenderfgoed.be",
     url="http://github.com/onroerenderfgoed/crabpy",
     packages=find_packages(exclude=["tests*"]),
     package_data={"": ["LICENSE"]},
```

