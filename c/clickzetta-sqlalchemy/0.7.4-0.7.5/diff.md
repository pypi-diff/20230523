# Comparing `tmp/clickzetta-sqlalchemy-0.7.4.tar.gz` & `tmp/clickzetta-sqlalchemy-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-sqlalchemy-0.7.4.tar", last modified: Tue May 23 06:35:03 2023, max compression
+gzip compressed data, was "clickzetta-sqlalchemy-0.7.5.tar", last modified: Tue May 23 07:08:14 2023, max compression
```

## Comparing `clickzetta-sqlalchemy-0.7.4.tar` & `clickzetta-sqlalchemy-0.7.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:35:03.738375 clickzetta-sqlalchemy-0.7.4/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      416 2023-05-23 06:35:03.738245 clickzetta-sqlalchemy-0.7.4/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:35:03.736616 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      416 2023-05-23 06:35:03.000000 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-05-23 06:35:03.000000 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:35:03.000000 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-23 06:35:03.000000 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:35:03.000000 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      633 2023-05-23 06:35:03.000000 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-05-23 06:35:03.000000 clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-23 06:35:03.738416 clickzetta-sqlalchemy-0.7.4/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-23 06:34:43.000000 clickzetta-sqlalchemy-0.7.4/setup.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:35:03.738098 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1123 2023-05-18 07:25:29.000000 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/_types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20451 2023-05-19 07:33:35.000000 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/base.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1244 2023-05-18 07:25:29.000000 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/parse_url.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/requirements.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-23 06:34:43.000000 clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 07:08:14.567939 clickzetta-sqlalchemy-0.7.5/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      416 2023-05-23 07:08:14.567822 clickzetta-sqlalchemy-0.7.5/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 07:08:14.566122 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      416 2023-05-23 07:08:14.000000 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-05-23 07:08:14.000000 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 07:08:14.000000 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-23 07:08:14.000000 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 07:08:14.000000 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      633 2023-05-23 07:08:14.000000 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-05-23 07:08:14.000000 clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-23 07:08:14.567978 clickzetta-sqlalchemy-0.7.5/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-23 07:07:56.000000 clickzetta-sqlalchemy-0.7.5/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 07:08:14.567655 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1123 2023-05-18 07:25:29.000000 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/_types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20451 2023-05-19 07:33:35.000000 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/base.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1244 2023-05-18 07:25:29.000000 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/parse_url.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/requirements.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-23 07:07:56.000000 clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/version.py
```

### Comparing `clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/SOURCES.txt` & `clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.7.4/clickzetta_sqlalchemy.egg-info/requires.txt` & `clickzetta-sqlalchemy-0.7.5/clickzetta_sqlalchemy.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 proto-plus<2.0.0dev,>=1.22.0
 packaging<24.0.0dev,>=14.3
 protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 python-dateutil<3.0dev,>=2.7.2
 requests<3.0.0dev,>=2.21.0
 sqlalchemy==2.0.6
 future
-clickzetta-connector==0.7.4
+clickzetta-connector==0.7.5
 
 [all]
 pandas>=1.0.0
 db-dtypes<2.0.0dev,>=0.3.0
 ipywidgets==7.7.1
 geopandas<1.0dev,>=0.9.0
 Shapely<2.0dev,>=1.6.0
```

### Comparing `clickzetta-sqlalchemy-0.7.4/setup.py` & `clickzetta-sqlalchemy-0.7.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "proto-plus >= 1.22.0, <2.0.0dev",
     "packaging >= 14.3, <24.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "python-dateutil >= 2.7.2, <3.0dev",
     "requests >= 2.21.0, < 3.0.0dev",
     "sqlalchemy==2.0.6",
     "future",
-    'clickzetta-connector==0.7.4',
+    'clickzetta-connector==0.7.5',
 ]
 extras = {
     "pandas": ["pandas>=1.0.0", "db-dtypes>=0.3.0,<2.0.0dev"],
     "ipywidgets": ["ipywidgets==7.7.1"],
     "geopandas": ["geopandas>=0.9.0, <1.0dev", "Shapely>=1.6.0, <2.0dev"],
     "ipython": ["ipython>=7.0.1,!=8.1.0"],
     "tqdm": ["tqdm >= 4.7.4, <5.0.0dev"],
```

### Comparing `clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/_helpers.py` & `clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/_types.py` & `clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/_types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/base.py` & `clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/parse_url.py` & `clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/parse_url.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.7.4/sqlalchemy_clickzetta/requirements.py` & `clickzetta-sqlalchemy-0.7.5/sqlalchemy_clickzetta/requirements.py`

 * *Files identical despite different names*

