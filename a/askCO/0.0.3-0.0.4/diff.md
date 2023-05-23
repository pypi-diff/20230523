# Comparing `tmp/askCO-0.0.3.tar.gz` & `tmp/askCO-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.3.tar", last modified: Mon May 22 02:24:03 2023, max compression
+gzip compressed data, was "askCO-0.0.4.tar", last modified: Tue May 23 00:10:45 2023, max compression
```

## Comparing `askCO-0.0.3.tar` & `askCO-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 02:24:03.554121 askCO-0.0.3/
--rw-rw-rw-   0        0        0     3769 2023-05-22 02:24:03.554121 askCO-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3199 2023-05-22 02:18:06.000000 askCO-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 02:24:03.554121 askCO-0.0.3/askCO.egg-info/
--rw-rw-rw-   0        0        0     3769 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 02:24:03.554121 askCO-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      806 2023-05-22 02:23:00.000000 askCO-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 00:10:45.952313 askCO-0.0.4/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 00:10:45.952313 askCO-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 00:10:45.952313 askCO-0.0.4/askCO.egg-info/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 00:10:45.952313 askCO-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-05-23 00:09:42.000000 askCO-0.0.4/setup.py
```

### Comparing `askCO-0.0.3/PKG-INFO` & `askCO-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python interface for Te Papa's collections API
 Home-page: https://github.com/lucyschrader/askCO
 Author: Lucy Schrader
 Author-email: lucy@schrader.nz
 License: MIT License
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
@@ -60,7 +60,12 @@
 - `endpoint`
 
 It also takes an `irn` parameter, the specific number for that record within the endpoint. Make sure you've set the correct endpoint - /object/123456 isn't the same as /agent/123456.
 
 The record's data is stored as a dictionary in the `response_text` attribute of the request object.
 
 HTTP status is stored as an integer in the `status_code` attribute.
+
+Get related records by adding the following parameters:
+- `related` (set to True)
+- `size` (the number of related records to return)
+- `types` (a comma separated list of `type` values, eg `Object,Specimen` or `Person`)
```

### Comparing `askCO-0.0.3/README.md` & `askCO-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,8 +42,13 @@
 - `attempts`
 - `endpoint`
 
 It also takes an `irn` parameter, the specific number for that record within the endpoint. Make sure you've set the correct endpoint - /object/123456 isn't the same as /agent/123456.
 
 The record's data is stored as a dictionary in the `response_text` attribute of the request object.
 
-HTTP status is stored as an integer in the `status_code` attribute.
+HTTP status is stored as an integer in the `status_code` attribute.
+
+Get related records by adding the following parameters:
+- `related` (set to True)
+- `size` (the number of related records to return)
+- `types` (a comma separated list of `type` values, eg `Object,Specimen` or `Person`)
```

### Comparing `askCO-0.0.3/askCO.egg-info/PKG-INFO` & `askCO-0.0.4/askCO.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python interface for Te Papa's collections API
 Home-page: https://github.com/lucyschrader/askCO
 Author: Lucy Schrader
 Author-email: lucy@schrader.nz
 License: MIT License
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
@@ -60,7 +60,12 @@
 - `endpoint`
 
 It also takes an `irn` parameter, the specific number for that record within the endpoint. Make sure you've set the correct endpoint - /object/123456 isn't the same as /agent/123456.
 
 The record's data is stored as a dictionary in the `response_text` attribute of the request object.
 
 HTTP status is stored as an integer in the `status_code` attribute.
+
+Get related records by adding the following parameters:
+- `related` (set to True)
+- `size` (the number of related records to return)
+- `types` (a comma separated list of `type` values, eg `Object,Specimen` or `Person`)
```

### Comparing `askCO-0.0.3/setup.py` & `askCO-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setup(
 	name="askCO",
-	version="0.0.3",
+	version="0.0.4",
 	author="Lucy Schrader",
 	author_email="lucy@schrader.nz",
 	license="MIT License",
 	description="Python interface for Te Papa's collections API",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/lucyschrader/askCO",
```

