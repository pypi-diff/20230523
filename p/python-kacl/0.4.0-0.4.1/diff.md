# Comparing `tmp/python-kacl-0.4.0.tar.gz` & `tmp/python-kacl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kacl-0.4.0.tar", last modified: Sun May 21 18:15:03 2023, max compression
+gzip compressed data, was "python-kacl-0.4.1.tar", last modified: Sun May 21 18:27:45 2023, max compression
```

## Comparing `python-kacl-0.4.0.tar` & `python-kacl-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.269774 python-kacl-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-21 18:14:53.000000 python-kacl-0.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-21 18:14:53.000000 python-kacl-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:15:03.269774 python-kacl-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17249 2023-05-21 18:14:53.000000 python-kacl-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.267774 python-kacl-0.4.0/kacl/
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/changes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.267774 python-kacl-0.4.0/kacl/config/
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/config/kacl-default.yml
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/config.py
--rw-rw-rw-   0 root         (0) root         (0)    23133 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/document.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/element.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/exception.py
--rwxrwxrwx   0 root         (0) root         (0)    14244 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/kacl_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/link_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.268774 python-kacl-0.4.0/python_kacl.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 18:15:03.269774 python-kacl-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-21 18:14:53.000000 python-kacl-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.269774 python-kacl-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/snapshot_directory.py
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11806 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/test_kacl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.474114 python-kacl-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-21 18:27:36.000000 python-kacl-0.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-21 18:27:36.000000 python-kacl-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:27:45.474114 python-kacl-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    17249 2023-05-21 18:27:36.000000 python-kacl-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.472114 python-kacl-0.4.1/kacl/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/changes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.472114 python-kacl-0.4.1/kacl/config/
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/config/kacl-default.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    23133 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/element.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)    14244 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/kacl_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/link_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.473114 python-kacl-0.4.1/python_kacl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 18:27:45.475114 python-kacl-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-21 18:27:36.000000 python-kacl-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.474114 python-kacl-0.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/snapshot_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11806 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/test_kacl.py
```

### Comparing `python-kacl-0.4.0/LICENSE` & `python-kacl-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/PKG-INFO` & `python-kacl-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-kacl-0.4.0/README.md` & `python-kacl-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/__init__.py` & `python-kacl-0.4.1/kacl/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the python-kacl package
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 from kacl.document import KACLDocument
 from kacl.serializer import KACLMarkdownSerializer
 
 
 def load(file):
     """
```

### Comparing `python-kacl-0.4.0/kacl/changes.py` & `python-kacl-0.4.1/kacl/changes.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/config/kacl-default.yml` & `python-kacl-0.4.1/kacl/config/kacl-default.yml`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/config.py` & `python-kacl-0.4.1/kacl/config.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/document.py` & `python-kacl-0.4.1/kacl/document.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/kacl_cli.py` & `python-kacl-0.4.1/kacl/kacl_cli.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/link_provider.py` & `python-kacl-0.4.1/kacl/link_provider.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/parser.py` & `python-kacl-0.4.1/kacl/parser.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/serializer.py` & `python-kacl-0.4.1/kacl/serializer.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/validation.py` & `python-kacl-0.4.1/kacl/validation.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/kacl/version.py` & `python-kacl-0.4.1/kacl/version.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/python_kacl.egg-info/PKG-INFO` & `python-kacl-0.4.1/python_kacl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-kacl-0.4.0/python_kacl.egg-info/SOURCES.txt` & `python-kacl-0.4.1/python_kacl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/setup.py` & `python-kacl-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.4.0"
+version = "0.4.1"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [
```

### Comparing `python-kacl-0.4.0/tests/snapshot_directory.py` & `python-kacl-0.4.1/tests/snapshot_directory.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/tests/test_cli.py` & `python-kacl-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.0/tests/test_kacl.py` & `python-kacl-0.4.1/tests/test_kacl.py`

 * *Files identical despite different names*

