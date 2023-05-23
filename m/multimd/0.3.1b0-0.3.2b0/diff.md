# Comparing `tmp/multimd-0.3.1b0.tar.gz` & `tmp/multimd-0.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimd-0.3.1b0.tar", max compression
+gzip compressed data, was "multimd-0.3.2b0.tar", max compression
```

## Comparing `multimd-0.3.1b0.tar` & `multimd-0.3.2b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2774 2023-05-14 20:08:40.340143 multimd-0.3.1b0/README.md
--rw-r--r--   0        0        0    35121 2023-05-15 16:56:51.757748 multimd-0.3.1b0/multimd/LICENSE.txt
--rw-r--r--   0        0        0     2774 2023-05-15 16:57:34.231747 multimd-0.3.1b0/multimd/README.md
--rw-r--r--   0        0        0       88 2023-05-15 16:56:51.756184 multimd-0.3.1b0/multimd/__init__.py
--rw-r--r--   0        0        0      126 2023-05-15 16:56:51.758378 multimd-0.3.1b0/multimd/__main__.py
--rw-r--r--   0        0        0     1859 2023-05-15 16:56:51.754576 multimd-0.3.1b0/multimd/build.py
--rw-r--r--   0        0        0     1955 2023-05-15 16:56:51.756772 multimd-0.3.1b0/multimd/cli.py
--rw-r--r--   0        0        0     5045 2023-05-15 16:56:51.755513 multimd-0.3.1b0/multimd/toc.py
--rw-r--r--   0        0        0      703 2023-05-14 21:07:43.771016 multimd-0.3.1b0/pyproject.toml
--rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 multimd-0.3.1b0/PKG-INFO
+-rw-r--r--   0        0        0     2774 2023-05-14 20:08:40.340143 multimd-0.3.2b0/README.md
+-rw-r--r--   0        0        0    35121 2023-05-15 16:56:51.757748 multimd-0.3.2b0/multimd/LICENSE.txt
+-rw-r--r--   0        0        0     2774 2023-05-15 16:57:34.231747 multimd-0.3.2b0/multimd/README.md
+-rw-r--r--   0        0        0       88 2023-05-15 16:56:51.756184 multimd-0.3.2b0/multimd/__init__.py
+-rw-r--r--   0        0        0      126 2023-05-15 16:56:51.758378 multimd-0.3.2b0/multimd/__main__.py
+-rw-r--r--   0        0        0     1859 2023-05-15 16:56:51.754576 multimd-0.3.2b0/multimd/build.py
+-rw-r--r--   0        0        0     1964 2023-05-23 21:00:01.539125 multimd-0.3.2b0/multimd/cli.py
+-rw-r--r--   0        0        0     5045 2023-05-15 16:56:51.755513 multimd-0.3.2b0/multimd/toc.py
+-rw-r--r--   0        0        0      703 2023-05-23 20:51:45.644845 multimd-0.3.2b0/pyproject.toml
+-rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 multimd-0.3.2b0/PKG-INFO
```

### Comparing `multimd-0.3.1b0/README.md` & `multimd-0.3.2b0/README.md`

 * *Files identical despite different names*

### Comparing `multimd-0.3.1b0/multimd/LICENSE.txt` & `multimd-0.3.2b0/multimd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multimd-0.3.1b0/multimd/README.md` & `multimd-0.3.2b0/multimd/README.md`

 * *Files identical despite different names*

### Comparing `multimd-0.3.1b0/multimd/build.py` & `multimd-0.3.2b0/multimd/build.py`

 * *Files identical despite different names*

### Comparing `multimd-0.3.1b0/multimd/cli.py` & `multimd-0.3.2b0/multimd/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 from typing import Tuple
 
 import                        typer
 from typing_extensions import Annotated
 
-from .build import Builder
+from .build import Builder, Path
 
 
 # --------- #
 # -- CLI -- #
 # --------- #
 
 CLI = typer.Typer()
@@ -39,15 +39,15 @@
     src_dest: Annotated[
         Tuple[Path,Path],
         typer.Argument(
             help = "Path of the source directory with "
                    "the MD chunks to be merged, followed "
                    "by the path of the final MD file to build."
     )],
-    erase: Annotated[
+    erase   : Annotated[
         bool,
         typer.Option(
             '--erase', '-e',
             help = "Erase an existing final MD file before "
                    "building the new one."
     )] = False,
 ) -> None:
```

### Comparing `multimd-0.3.1b0/multimd/toc.py` & `multimd-0.3.2b0/multimd/toc.py`

 * *Files identical despite different names*

### Comparing `multimd-0.3.1b0/pyproject.toml` & `multimd-0.3.2b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name         = "multimd"
-version      = "0.3.1-beta"
+version      = "0.3.2-beta"
 description  = 'This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single final `MD` file.'
 readme       = "README.md"
 authors      = ["Christophe BAL"]
 maintainers  = ["Christophe BAL"]
 license      = "GNU License Version 3"
 repository   = "https://github.com/bc-tools/for-dev/tree/main/multimd"
```

### Comparing `multimd-0.3.1b0/PKG-INFO` & `multimd-0.3.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimd
-Version: 0.3.1b0
+Version: 0.3.2b0
 Summary: This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single final `MD` file.
 Home-page: https://github.com/bc-tools/for-dev/tree/main/multimd
 License: GNU License Version 3
 Author: Christophe BAL
 Maintainer: Christophe BAL
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

