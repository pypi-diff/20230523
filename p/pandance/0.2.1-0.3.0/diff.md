# Comparing `tmp/pandance-0.2.1.tar.gz` & `tmp/pandance-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandance-0.2.1.tar", last modified: Fri Jan 20 14:31:01 2023, max compression
+gzip compressed data, was "pandance-0.3.0.tar", last modified: Tue May 23 09:38:19 2023, max compression
```

## Comparing `pandance-0.2.1.tar` & `pandance-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-01-20 14:31:01.886136 pandance-0.2.1/
--rw-r--r--   0 phil      (1000) phil      (1000)     1519 2022-05-13 20:04:24.000000 pandance-0.2.1/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     1756 2023-01-20 14:31:01.886136 pandance-0.2.1/PKG-INFO
--rw-r--r--   0 phil      (1000) phil      (1000)      978 2023-01-19 19:12:08.000000 pandance-0.2.1/README.md
-drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-01-20 14:31:01.882803 pandance-0.2.1/pandance/
--rw-r--r--   0 phil      (1000) phil      (1000)       47 2023-01-20 14:30:12.000000 pandance-0.2.1/pandance/__init__.py
--rw-rw-rw-   0 phil      (1000) phil      (1000)    21599 2023-01-20 10:39:01.000000 pandance-0.2.1/pandance/pandance.py
-drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-01-20 14:31:01.886136 pandance-0.2.1/pandance.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     1756 2023-01-20 14:31:01.000000 pandance-0.2.1/pandance.egg-info/PKG-INFO
--rw-r--r--   0 phil      (1000) phil      (1000)      259 2023-01-20 14:31:01.000000 pandance-0.2.1/pandance.egg-info/SOURCES.txt
--rw-r--r--   0 phil      (1000) phil      (1000)        1 2023-01-20 14:31:01.000000 pandance-0.2.1/pandance.egg-info/dependency_links.txt
--rw-r--r--   0 phil      (1000) phil      (1000)       63 2023-01-20 14:31:01.000000 pandance-0.2.1/pandance.egg-info/requires.txt
--rw-r--r--   0 phil      (1000) phil      (1000)        9 2023-01-20 14:31:01.000000 pandance-0.2.1/pandance.egg-info/top_level.txt
--rw-r--r--   0 phil      (1000) phil      (1000)      952 2023-01-20 14:30:24.000000 pandance-0.2.1/pyproject.toml
--rw-r--r--   0 phil      (1000) phil      (1000)       38 2023-01-20 14:31:01.886136 pandance-0.2.1/setup.cfg
--rw-r--r--   0 phil      (1000) phil      (1000)      259 2023-01-20 14:26:12.000000 pandance-0.2.1/setup.py
-drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-01-20 14:31:01.886136 pandance-0.2.1/test/
--rw-r--r--   0 phil      (1000) phil      (1000)    11084 2023-01-20 11:50:55.000000 pandance-0.2.1/test/test_ops.py
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 09:38:19.961364 pandance-0.3.0/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1519 2022-05-13 20:04:24.000000 pandance-0.3.0/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1795 2023-05-23 09:38:19.961364 pandance-0.3.0/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)     1017 2023-05-18 08:09:52.000000 pandance-0.3.0/README.md
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 09:38:19.958031 pandance-0.3.0/pandance/
+-rw-r--r--   0 phil      (1000) phil      (1000)       47 2023-05-16 10:22:57.000000 pandance-0.3.0/pandance/__init__.py
+-rw-r--r--   0 phil      (1000) phil      (1000)    38374 2023-05-22 19:32:21.000000 pandance-0.3.0/pandance/pandance.py
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 09:38:19.961364 pandance-0.3.0/pandance.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1795 2023-05-23 09:38:19.000000 pandance-0.3.0/pandance.egg-info/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)      259 2023-05-23 09:38:19.000000 pandance-0.3.0/pandance.egg-info/SOURCES.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)        1 2023-05-23 09:38:19.000000 pandance-0.3.0/pandance.egg-info/dependency_links.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)       63 2023-05-23 09:38:19.000000 pandance-0.3.0/pandance.egg-info/requires.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)        9 2023-05-23 09:38:19.000000 pandance-0.3.0/pandance.egg-info/top_level.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)      952 2023-05-16 10:22:15.000000 pandance-0.3.0/pyproject.toml
+-rw-r--r--   0 phil      (1000) phil      (1000)       38 2023-05-23 09:38:19.961364 pandance-0.3.0/setup.cfg
+-rw-r--r--   0 phil      (1000) phil      (1000)      259 2023-01-20 14:26:12.000000 pandance-0.3.0/setup.py
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 09:38:19.961364 pandance-0.3.0/test/
+-rw-r--r--   0 phil      (1000) phil      (1000)    17426 2023-05-22 19:36:59.000000 pandance-0.3.0/test/test_ops.py
```

### Comparing `pandance-0.2.1/LICENSE` & `pandance-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandance-0.2.1/PKG-INFO` & `pandance-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandance
-Version: 0.2.1
+Version: 0.3.0
 Summary: Advanced relational operations for pandas DataFrames
 Author: Filip Buric
 Maintainer: Filip Buric
 Project-URL: Homepage, https://pandance.readthedocs.io
 Project-URL: Documentation, https://pandance.readthedocs.io
 Project-URL: Source Code, https://github.com/fburic/pandance
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,16 @@
 enabling powerful and efficient joins (aka merges).
 
 ## Highlights
 
 Pandance extends the set of standard join operations in pandas
 (inner, outer, cross, left, right) with:
 
-- **fuzzy joins**: Match columns with a tolerance
+- **fuzzy joins**: Match columns with a tolerance. Supports numerical and datetime values.
+- **inequality join**: Match one column's values that are less / greater than the other column's values.
 - **[theta joins](https://en.wikipedia.org/wiki/Relational_algebra#%CE%B8-join_and_equijoin)**:
   Allows the user to specify arbitrary matching conditions on which to join
 
 Pandance is designed with performance in mind, aiming to provide fast implementations
 whenever possible.
 
 ## Installation
@@ -48,11 +49,7 @@
 ```shell
 pip install pandance
 ```
 
 ## Usage
 
 See the [documentation](https://pandance.readthedocs.io)
-
-## TODO
-
-- `[0.3.0]` inequality join: efficient implementation of non-equijoins using inequalities (<, >)
```

### Comparing `pandance-0.2.1/README.md` & `pandance-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 enabling powerful and efficient joins (aka merges).
 
 ## Highlights
 
 Pandance extends the set of standard join operations in pandas
 (inner, outer, cross, left, right) with:
 
-- **fuzzy joins**: Match columns with a tolerance
+- **fuzzy joins**: Match columns with a tolerance. Supports numerical and datetime values.
+- **inequality join**: Match one column's values that are less / greater than the other column's values.
 - **[theta joins](https://en.wikipedia.org/wiki/Relational_algebra#%CE%B8-join_and_equijoin)**:
   Allows the user to specify arbitrary matching conditions on which to join
 
 Pandance is designed with performance in mind, aiming to provide fast implementations
 whenever possible.
 
 ## Installation
@@ -27,11 +28,7 @@
 ```shell
 pip install pandance
 ```
 
 ## Usage
 
 See the [documentation](https://pandance.readthedocs.io)
-
-## TODO
-
-- `[0.3.0]` inequality join: efficient implementation of non-equijoins using inequalities (<, >)
```

### Comparing `pandance-0.2.1/pandance.egg-info/PKG-INFO` & `pandance-0.3.0/pandance.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandance
-Version: 0.2.1
+Version: 0.3.0
 Summary: Advanced relational operations for pandas DataFrames
 Author: Filip Buric
 Maintainer: Filip Buric
 Project-URL: Homepage, https://pandance.readthedocs.io
 Project-URL: Documentation, https://pandance.readthedocs.io
 Project-URL: Source Code, https://github.com/fburic/pandance
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,16 @@
 enabling powerful and efficient joins (aka merges).
 
 ## Highlights
 
 Pandance extends the set of standard join operations in pandas
 (inner, outer, cross, left, right) with:
 
-- **fuzzy joins**: Match columns with a tolerance
+- **fuzzy joins**: Match columns with a tolerance. Supports numerical and datetime values.
+- **inequality join**: Match one column's values that are less / greater than the other column's values.
 - **[theta joins](https://en.wikipedia.org/wiki/Relational_algebra#%CE%B8-join_and_equijoin)**:
   Allows the user to specify arbitrary matching conditions on which to join
 
 Pandance is designed with performance in mind, aiming to provide fast implementations
 whenever possible.
 
 ## Installation
@@ -48,11 +49,7 @@
 ```shell
 pip install pandance
 ```
 
 ## Usage
 
 See the [documentation](https://pandance.readthedocs.io)
-
-## TODO
-
-- `[0.3.0]` inequality join: efficient implementation of non-equijoins using inequalities (<, >)
```

### Comparing `pandance-0.2.1/pyproject.toml` & `pandance-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["pandance"]
 
 [project]
 name = "pandance"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="Filip Buric" }
 ]
 maintainers = [
   { name="Filip Buric" }
 ]
 description = "Advanced relational operations for pandas DataFrames"
```

