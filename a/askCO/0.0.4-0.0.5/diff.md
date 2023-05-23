# Comparing `tmp/askCO-0.0.4.tar.gz` & `tmp/askCO-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.4.tar", last modified: Tue May 23 00:10:45 2023, max compression
+gzip compressed data, was "askCO-0.0.5.tar", last modified: Tue May 23 04:29:46 2023, max compression
```

## Comparing `askCO-0.0.4.tar` & `askCO-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 00:10:45.952313 askCO-0.0.4/
--rw-rw-rw-   0        0        0     3994 2023-05-23 00:10:45.952313 askCO-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 00:10:45.952313 askCO-0.0.4/askCO.egg-info/
--rw-rw-rw-   0        0        0     3994 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 00:10:45.000000 askCO-0.0.4/askCO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 00:10:45.952313 askCO-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      806 2023-05-23 00:09:42.000000 askCO-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:29:46.338913 askCO-0.0.5/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 04:29:46.338913 askCO-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.5/README.md
+-rw-rw-rw-   0        0        0      676 2023-05-23 04:29:06.000000 askCO-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 04:29:46.338913 askCO-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 04:29:46.323310 askCO-0.0.5/src/
+-rw-rw-rw-   0        0        0     9765 2023-05-23 03:56:27.000000 askCO-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:29:46.338913 askCO-0.0.5/src/askCO.egg-info/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2296 2023-05-18 02:08:58.000000 askCO-0.0.5/src/tryCO.py
```

### Comparing `askCO-0.0.4/PKG-INFO` & `askCO-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python interface for Te Papa's collections API
-Home-page: https://github.com/lucyschrader/askCO
-Author: Lucy Schrader
-Author-email: lucy@schrader.nz
+Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
+Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
@@ -17,15 +16,15 @@
 
 # askCO: search and query records from Te Papa's collections API
 
 This script provides an interface for getting data from the Museum of New Zealand Te Papa Tongarewa. With it, you can run searches and request individual records, which are returned as python objects.
 
 See the [API documentation](https://data.tepapa.govt.nz/docs/) for what's available and how to construct searches.
 
-Te Papa's API requires a registration key in the headers of each request â€“ go to https://data.tepapa.govt.nz/docs/register.html to register. I recommend adding the API key to an environment variable called 'TE-PAPA-KEY', and then calling that from your script to pass to askCO.
+Te Papa's API requires a registration key in the headers of each request – go to https://data.tepapa.govt.nz/docs/register.html to register. I recommend adding the API key to an environment variable called 'TE-PAPA-KEY', and then calling that from your script to pass to askCO.
 
 ## Installation
 Install using pip: `pip install askCO`
 
 askCO requires the `requests` module.
 
 ## Run a search query
```

### Comparing `askCO-0.0.4/README.md` & `askCO-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `askCO-0.0.4/askCO.egg-info/PKG-INFO` & `askCO-0.0.5/src/askCO.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python interface for Te Papa's collections API
-Home-page: https://github.com/lucyschrader/askCO
-Author: Lucy Schrader
-Author-email: lucy@schrader.nz
+Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
+Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
@@ -17,15 +16,15 @@
 
 # askCO: search and query records from Te Papa's collections API
 
 This script provides an interface for getting data from the Museum of New Zealand Te Papa Tongarewa. With it, you can run searches and request individual records, which are returned as python objects.
 
 See the [API documentation](https://data.tepapa.govt.nz/docs/) for what's available and how to construct searches.
 
-Te Papa's API requires a registration key in the headers of each request â€“ go to https://data.tepapa.govt.nz/docs/register.html to register. I recommend adding the API key to an environment variable called 'TE-PAPA-KEY', and then calling that from your script to pass to askCO.
+Te Papa's API requires a registration key in the headers of each request – go to https://data.tepapa.govt.nz/docs/register.html to register. I recommend adding the API key to an environment variable called 'TE-PAPA-KEY', and then calling that from your script to pass to askCO.
 
 ## Installation
 Install using pip: `pip install askCO`
 
 askCO requires the `requests` module.
 
 ## Run a search query
```

