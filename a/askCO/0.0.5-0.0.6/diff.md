# Comparing `tmp/askCO-0.0.5.tar.gz` & `tmp/askCO-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.5.tar", last modified: Tue May 23 04:29:46 2023, max compression
+gzip compressed data, was "askCO-0.0.6.tar", last modified: Tue May 23 04:35:07 2023, max compression
```

## Comparing `askCO-0.0.5.tar` & `askCO-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 04:29:46.338913 askCO-0.0.5/
--rw-rw-rw-   0        0        0     3994 2023-05-23 04:29:46.338913 askCO-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.5/README.md
--rw-rw-rw-   0        0        0      676 2023-05-23 04:29:06.000000 askCO-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 04:29:46.338913 askCO-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 04:29:46.323310 askCO-0.0.5/src/
--rw-rw-rw-   0        0        0     9765 2023-05-23 03:56:27.000000 askCO-0.0.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 04:29:46.338913 askCO-0.0.5/src/askCO.egg-info/
--rw-rw-rw-   0        0        0     3994 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-23 04:29:46.000000 askCO-0.0.5/src/askCO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2296 2023-05-18 02:08:58.000000 askCO-0.0.5/src/tryCO.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.189811 askCO-0.0.6/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 04:35:07.189811 askCO-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.6/README.md
+-rw-rw-rw-   0        0        0      676 2023-05-23 04:34:15.000000 askCO-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 04:35:07.189811 askCO-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.158586 askCO-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.158586 askCO-0.0.6/src/askCO/
+-rw-rw-rw-   0        0        0     9765 2023-05-23 03:56:27.000000 askCO-0.0.6/src/askCO/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-05-18 02:08:58.000000 askCO-0.0.6/src/askCO/tryCO.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.189811 askCO-0.0.6/src/askCO.egg-info/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/top_level.txt
```

### Comparing `askCO-0.0.5/PKG-INFO` & `askCO-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.0.5/README.md` & `askCO-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `askCO-0.0.5/pyproject.toml` & `askCO-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "askCO"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
 	{name = "Lucy Schrader", email = "lucy@schrader.nz"},
 ]
 description = "Python interface for Te Papa's collections API"
 readme = "README.md"
 keywords = ["python", "museum", "api"]
 requires-python = ">=3.7"
```

### Comparing `askCO-0.0.5/src/__init__.py` & `askCO-0.0.6/src/askCO/__init__.py`

 * *Files identical despite different names*

### Comparing `askCO-0.0.5/src/askCO.egg-info/PKG-INFO` & `askCO-0.0.6/src/askCO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.0.5/src/tryCO.py` & `askCO-0.0.6/src/askCO/tryCO.py`

 * *Files identical despite different names*

