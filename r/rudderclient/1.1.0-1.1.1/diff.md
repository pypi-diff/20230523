# Comparing `tmp/rudderclient-1.1.0.tar.gz` & `tmp/rudderclient-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.1.0.tar", last modified: Mon May 22 12:31:46 2023, max compression
+gzip compressed data, was "rudderclient-1.1.1.tar", last modified: Tue May 23 06:16:06 2023, max compression
```

## Comparing `rudderclient-1.1.0.tar` & `rudderclient-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-22 12:31:46.515979 rudderclient-1.1.0/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1069 2023-05-17 06:37:36.000000 rudderclient-1.1.0/LICENSE
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1934 2023-05-22 12:31:46.515979 rudderclient-1.1.0/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      224 2023-05-22 12:05:46.000000 rudderclient-1.1.0/README.md
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-22 12:31:46.515979 rudderclient-1.1.0/gcp/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-22 12:05:46.000000 rudderclient-1.1.0/gcp/__init__.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      847 2023-05-22 12:24:42.000000 rudderclient-1.1.0/gcp/auth.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      338 2023-05-22 12:24:42.000000 rudderclient-1.1.0/gcp/http-requests.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      636 2023-05-22 12:31:02.000000 rudderclient-1.1.0/pyproject.toml
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-22 12:31:46.515979 rudderclient-1.1.0/rudderclient.egg-info/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1934 2023-05-22 12:31:46.000000 rudderclient-1.1.0/rudderclient.egg-info/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      260 2023-05-22 12:31:46.000000 rudderclient-1.1.0/rudderclient.egg-info/SOURCES.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        1 2023-05-22 12:31:46.000000 rudderclient-1.1.0/rudderclient.egg-info/dependency_links.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       28 2023-05-22 12:31:46.000000 rudderclient-1.1.0/rudderclient.egg-info/requires.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        4 2023-05-22 12:31:46.000000 rudderclient-1.1.0/rudderclient.egg-info/top_level.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       38 2023-05-22 12:31:46.515979 rudderclient-1.1.0/setup.cfg
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 06:16:06.393255 rudderclient-1.1.1/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1069 2023-05-17 06:37:36.000000 rudderclient-1.1.1/LICENSE
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1934 2023-05-23 06:16:06.393255 rudderclient-1.1.1/PKG-INFO
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      224 2023-05-22 12:05:46.000000 rudderclient-1.1.1/README.md
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 06:16:06.393255 rudderclient-1.1.1/gcp/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-22 12:05:46.000000 rudderclient-1.1.1/gcp/__init__.py
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      847 2023-05-22 12:24:42.000000 rudderclient-1.1.1/gcp/auth.py
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      338 2023-05-22 12:24:42.000000 rudderclient-1.1.1/gcp/http_requests.py
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      636 2023-05-23 06:15:55.000000 rudderclient-1.1.1/pyproject.toml
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 06:16:06.393255 rudderclient-1.1.1/rudderclient.egg-info/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1934 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/PKG-INFO
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      260 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        1 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       28 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/requires.txt
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        4 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/top_level.txt
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       38 2023-05-23 06:16:06.393255 rudderclient-1.1.1/setup.cfg
```

### Comparing `rudderclient-1.1.0/LICENSE` & `rudderclient-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.1.0/PKG-INFO` & `rudderclient-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.1.0/gcp/auth.py` & `rudderclient-1.1.1/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.1.0/pyproject.toml` & `rudderclient-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.1.0"
+version = "1.1.1"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 authors = [{ name = "Rudder Team", email = "rudder@realnaut.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rudderclient-1.1.0/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.1.1/rudderclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

