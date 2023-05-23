# Comparing `tmp/revtongyi-0.0.0.1.tar.gz` & `tmp/revtongyi-0.0.0.2.tar.gz`

## Comparing `revtongyi-0.0.0.1.tar` & `revtongyi-0.0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 revtongyi-0.0.0.1/test.py
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 revtongyi-0.0.0.1/revTongYi/__init__.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 revtongyi-0.0.0.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.0.0.1/LICENSE
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 revtongyi-0.0.0.1/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 revtongyi-0.0.0.1/pyproject.toml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 revtongyi-0.0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/test.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/revTongYi/__init__.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/LICENSE
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/PKG-INFO
```

### Comparing `revtongyi-0.0.0.1/test.py` & `revtongyi-0.0.0.2/test.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.0.0.1/.gitignore` & `revtongyi-0.0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `revtongyi-0.0.0.1/LICENSE` & `revtongyi-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revtongyi-0.0.0.1/pyproject.toml` & `revtongyi-0.0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "revTongYi"
-version = "0.0.0.1"
+version = "0.0.0.2"
 authors = [
   { name="xw5xr6", email="xw5xr6@hotmail.com" },
 ]
 description = "阿里通义千问逆向工程API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

