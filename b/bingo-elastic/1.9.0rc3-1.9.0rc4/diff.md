# Comparing `tmp/bingo_elastic-1.9.0rc3-py3-none-any.whl.zip` & `tmp/bingo_elastic-1.9.0rc4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9976 bytes, number of entries: 11
--rw-r--r--  2.0 unx       26 b- defN 23-Jan-13 07:43 bingo_elastic/__init__.py
--rw-r--r--  2.0 unx    11045 b- defN 23-Jan-13 07:43 bingo_elastic/elastic.py
--rw-r--r--  2.0 unx     9694 b- defN 23-Jan-13 07:43 bingo_elastic/queries.py
--rw-r--r--  2.0 unx      431 b- defN 23-Jan-13 07:43 bingo_elastic/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-13 07:43 bingo_elastic/model/__init__.py
--rw-r--r--  2.0 unx     2800 b- defN 23-Jan-13 07:43 bingo_elastic/model/helpers.py
--rw-r--r--  2.0 unx     5770 b- defN 23-Jan-13 07:43 bingo_elastic/model/record.py
--rw-r--r--  2.0 unx     1897 b- defN 23-Jan-13 07:44 bingo_elastic-1.9.0rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-13 07:44 bingo_elastic-1.9.0rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jan-13 07:44 bingo_elastic-1.9.0rc3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      913 b- defN 23-Jan-13 07:44 bingo_elastic-1.9.0rc3.dist-info/RECORD
-11 files, 32682 bytes uncompressed, 8420 bytes compressed:  74.2%
+Zip file size: 9996 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       26 b- defN 23-Jan-17 03:05 bingo_elastic/__init__.py
+-rw-r--r--  2.0 unx    11045 b- defN 23-Jan-17 03:05 bingo_elastic/elastic.py
+-rw-r--r--  2.0 unx     9694 b- defN 23-Jan-17 03:05 bingo_elastic/queries.py
+-rw-r--r--  2.0 unx      431 b- defN 23-Jan-17 03:05 bingo_elastic/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-17 03:05 bingo_elastic/model/__init__.py
+-rw-r--r--  2.0 unx     2800 b- defN 23-Jan-17 03:05 bingo_elastic/model/helpers.py
+-rw-r--r--  2.0 unx     5770 b- defN 23-Jan-17 03:05 bingo_elastic/model/record.py
+-rw-r--r--  2.0 unx     1925 b- defN 23-Jan-17 03:06 bingo_elastic-1.9.0rc4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-17 03:06 bingo_elastic-1.9.0rc4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jan-17 03:06 bingo_elastic-1.9.0rc4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      913 b- defN 23-Jan-17 03:06 bingo_elastic-1.9.0rc4.dist-info/RECORD
+11 files, 32710 bytes uncompressed, 8440 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: bingo_elastic/model/helpers.py
 Comment: 
 
 Filename: bingo_elastic/model/record.py
 Comment: 
 
-Filename: bingo_elastic-1.9.0rc3.dist-info/METADATA
+Filename: bingo_elastic-1.9.0rc4.dist-info/METADATA
 Comment: 
 
-Filename: bingo_elastic-1.9.0rc3.dist-info/WHEEL
+Filename: bingo_elastic-1.9.0rc4.dist-info/WHEEL
 Comment: 
 
-Filename: bingo_elastic-1.9.0rc3.dist-info/top_level.txt
+Filename: bingo_elastic-1.9.0rc4.dist-info/top_level.txt
 Comment: 
 
-Filename: bingo_elastic-1.9.0rc3.dist-info/RECORD
+Filename: bingo_elastic-1.9.0rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bingo_elastic/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.9.0.rc3"
+__version__ = "1.9.0.rc4"
```

## Comparing `bingo_elastic-1.9.0rc3.dist-info/METADATA` & `bingo_elastic-1.9.0rc4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: bingo-elastic
-Version: 1.9.0rc3
+Version: 1.9.0rc4
 Summary: Cartridge that provides fast, scalable, and efficient storage and searching solution for chemical information using Elasticsearch
 Home-page: https://github.com/epam/Indigo/tree/master/bingo/bingo-elastic/python
-Download-URL: https://pypi.org/project/bingo_elastic
 Author: Ruslan Khyurri
 Author-email: ruslan_khyurri@epam.com
 License: Apache-2.0
+Download-URL: https://pypi.org/project/bingo_elastic
 Project-URL: Bug Tracker, https://github.com/epam/indigo/issues
 Project-URL: Documentation, https://github.com/epam/Indigo/tree/master/bingo/bingo-elastic/python
 Project-URL: Source Code, https://github.com/epam/indigo/
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -23,19 +24,22 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
-Requires-Dist: epam.indigo (==1.9.0.rc3)
+Requires-Dist: epam.indigo (==1.9.0.rc4)
 Requires-Dist: elasticsearch (==7.16.2)
 Provides-Extra: async
 Requires-Dist: elasticsearch[async] (==7.16.2) ; extra == 'async'
 Provides-Extra: dev
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: wheel ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: pytest-asyncio ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 
+UNKNOWN
+
+
```

## Comparing `bingo_elastic-1.9.0rc3.dist-info/RECORD` & `bingo_elastic-1.9.0rc4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-bingo_elastic/__init__.py,sha256=c9UhohUDoGHC8DYMeiPj5gmAnn5NHqaEVtQBhtFbfdc,26
+bingo_elastic/__init__.py,sha256=wNvfIXMBb_5y0n7v8LHEIHhTb6E06LmbGLAIUgH2q40,26
 bingo_elastic/elastic.py,sha256=cQkC2JeYk5nOaqjijX8VPu9ritzQu4eGvOngtmf6Ceg,11045
 bingo_elastic/queries.py,sha256=E3n0itewQyA3i4Okhr20_TBG1x8v7gzHlKST8rhGK38,9694
 bingo_elastic/utils.py,sha256=IehXeyDMRbuwgkHG1YUrYikkqTzU4YZEadjkEHWpWuM,431
 bingo_elastic/model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bingo_elastic/model/helpers.py,sha256=yLo7AEABdYH-QPBB9r8W3OczwTBQ5QeXw90r5czCMAc,2800
 bingo_elastic/model/record.py,sha256=LZYA9OYILAUoBaDZoWz2R-kknP6kmigDshCDr8h9XDs,5770
-bingo_elastic-1.9.0rc3.dist-info/METADATA,sha256=PpvSLgxuE9XRenqIyGWMaAAWy42saWxIpDF1LK8nIYg,1897
-bingo_elastic-1.9.0rc3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingo_elastic-1.9.0rc3.dist-info/top_level.txt,sha256=67ub73ySXViAI3OJN1CaNd94vwTh3zSuTZ9LHOBxoSg,14
-bingo_elastic-1.9.0rc3.dist-info/RECORD,,
+bingo_elastic-1.9.0rc4.dist-info/METADATA,sha256=o-dsCyikSq6WczDGnxu6W9FnuDF-lwRnRl9bXsvslE4,1925
+bingo_elastic-1.9.0rc4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bingo_elastic-1.9.0rc4.dist-info/top_level.txt,sha256=67ub73ySXViAI3OJN1CaNd94vwTh3zSuTZ9LHOBxoSg,14
+bingo_elastic-1.9.0rc4.dist-info/RECORD,,
```

