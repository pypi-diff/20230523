# Comparing `tmp/mystran_validation-0.8.0.tar.gz` & `tmp/mystran_validation-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystran_validation-0.8.0.tar", last modified: Tue Aug 24 07:51:52 2021, max compression
+gzip compressed data, was "mystran_validation-0.9.0.tar", last modified: Wed Sep  1 04:46:28 2021, max compression
```

## Comparing `mystran_validation-0.8.0.tar` & `mystran_validation-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-08-24 07:51:52.199432 mystran_validation-0.8.0/
--rw-r--r--   0 nic       (1001) nic       (1001)      172 2021-05-17 05:41:29.000000 mystran_validation-0.8.0/AUTHORS.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      221 2021-05-17 05:41:29.000000 mystran_validation-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       89 2021-05-17 05:41:29.000000 mystran_validation-0.8.0/HISTORY.rst
--rw-r--r--   0 nic       (1001) nic       (1001)     1074 2021-05-17 05:41:29.000000 mystran_validation-0.8.0/LICENSE
--rw-r--r--   0 nic       (1001) nic       (1001)      336 2021-08-15 10:38:23.000000 mystran_validation-0.8.0/MANIFEST.in
--rw-rw-r--   0 nic       (1001) nic       (1001)     8084 2021-08-24 07:51:52.199432 mystran_validation-0.8.0/PKG-INFO
--rw-r--r--   0 nic       (1001) nic       (1001)     5743 2021-08-16 11:21:00.000000 mystran_validation-0.8.0/README.md
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-08-24 07:51:52.195432 mystran_validation-0.8.0/docs/
--rw-r--r--   0 nic       (1001) nic       (1001)      619 2021-05-17 05:41:29.000000 mystran_validation-0.8.0/docs/Makefile
--rw-r--r--   0 nic       (1001) nic       (1001)       28 2021-05-17 05:41:30.000000 mystran_validation-0.8.0/docs/authors.rst
--rwxr-xr-x   0 nic       (1001) nic       (1001)     5043 2021-05-19 07:41:49.000000 mystran_validation-0.8.0/docs/conf.py
--rw-r--r--   0 nic       (1001) nic       (1001)       33 2021-05-17 05:41:30.000000 mystran_validation-0.8.0/docs/contributing.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       28 2021-05-17 05:41:30.000000 mystran_validation-0.8.0/docs/history.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      315 2021-05-17 05:41:30.000000 mystran_validation-0.8.0/docs/index.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      102 2021-05-17 05:41:30.000000 mystran_validation-0.8.0/docs/installation.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      780 2021-05-17 05:41:30.000000 mystran_validation-0.8.0/docs/make.bat
--rw-r--r--   0 nic       (1001) nic       (1001)       27 2021-05-17 05:41:30.000000 mystran_validation-0.8.0/docs/readme.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       91 2021-05-17 05:41:29.000000 mystran_validation-0.8.0/docs/usage.rst
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-08-24 07:51:52.195432 mystran_validation-0.8.0/mystran_validation/
--rw-r--r--   0 nic       (1001) nic       (1001)     4486 2021-08-24 07:51:43.000000 mystran_validation-0.8.0/mystran_validation/__init__.py
--rw-r--r--   0 nic       (1001) nic       (1001)    10032 2021-08-24 07:50:47.000000 mystran_validation-0.8.0/mystran_validation/cli.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    14181 2021-08-23 14:07:48.000000 mystran_validation-0.8.0/mystran_validation/conftest_ref.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-08-24 07:51:52.195432 mystran_validation-0.8.0/mystran_validation/data/
--rw-rw-r--   0 nic       (1001) nic       (1001)        0 2021-08-15 07:53:09.000000 mystran_validation-0.8.0/mystran_validation/data/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     6074 2021-05-17 20:48:53.000000 mystran_validation-0.8.0/mystran_validation/data/bulk_model.nas
--rw-rw-r--   0 nic       (1001) nic       (1001)     6074 2021-05-17 20:48:53.000000 mystran_validation-0.8.0/mystran_validation/data/bulk_model_2.dat
--rw-rw-r--   0 nic       (1001) nic       (1001)      582 2021-08-15 09:11:55.000000 mystran_validation-0.8.0/mystran_validation/data/test_bar.ini
--rw-rw-r--   0 nic       (1001) nic       (1001)    35016 2021-05-17 20:48:53.000000 mystran_validation-0.8.0/mystran_validation/data/test_case_03.op2
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-08-24 07:51:52.199432 mystran_validation-0.8.0/mystran_validation/parsers/
--rw-rw-r--   0 nic       (1001) nic       (1001)      769 2021-05-19 07:41:49.000000 mystran_validation-0.8.0/mystran_validation/parsers/__init__.py
--rw-r--r--   0 nic       (1001) nic       (1001)     2281 2021-05-25 07:11:13.000000 mystran_validation-0.8.0/mystran_validation/parsers/nastran_op2.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     2738 2021-08-15 09:13:23.000000 mystran_validation-0.8.0/mystran_validation/xml_junit2html.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-08-24 07:51:52.195432 mystran_validation-0.8.0/mystran_validation.egg-info/
--rw-rw-r--   0 nic       (1001) nic       (1001)     8084 2021-08-24 07:51:52.000000 mystran_validation-0.8.0/mystran_validation.egg-info/PKG-INFO
--rw-rw-r--   0 nic       (1001) nic       (1001)      971 2021-08-24 07:51:52.000000 mystran_validation-0.8.0/mystran_validation.egg-info/SOURCES.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2021-08-24 07:51:52.000000 mystran_validation-0.8.0/mystran_validation.egg-info/dependency_links.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)       61 2021-08-24 07:51:52.000000 mystran_validation-0.8.0/mystran_validation.egg-info/entry_points.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2021-08-24 07:51:52.000000 mystran_validation-0.8.0/mystran_validation.egg-info/not-zip-safe
--rw-rw-r--   0 nic       (1001) nic       (1001)      113 2021-08-24 07:51:52.000000 mystran_validation-0.8.0/mystran_validation.egg-info/requires.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)       19 2021-08-24 07:51:52.000000 mystran_validation-0.8.0/mystran_validation.egg-info/top_level.txt
--rw-r--r--   0 nic       (1001) nic       (1001)      460 2021-08-24 07:51:52.199432 mystran_validation-0.8.0/setup.cfg
--rw-r--r--   0 nic       (1001) nic       (1001)     1516 2021-08-24 07:51:43.000000 mystran_validation-0.8.0/setup.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-08-24 07:51:52.199432 mystran_validation-0.8.0/tests/
--rw-r--r--   0 nic       (1001) nic       (1001)       73 2021-05-17 10:04:45.000000 mystran_validation-0.8.0/tests/__init__.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-09-01 04:46:28.418400 mystran_validation-0.9.0/
+-rw-r--r--   0 nic       (1001) nic       (1001)      172 2021-05-17 05:41:29.000000 mystran_validation-0.9.0/AUTHORS.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      221 2021-05-17 05:41:29.000000 mystran_validation-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       89 2021-05-17 05:41:29.000000 mystran_validation-0.9.0/HISTORY.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)     1074 2021-05-17 05:41:29.000000 mystran_validation-0.9.0/LICENSE
+-rw-r--r--   0 nic       (1001) nic       (1001)      336 2021-08-15 10:38:23.000000 mystran_validation-0.9.0/MANIFEST.in
+-rw-rw-r--   0 nic       (1001) nic       (1001)     8084 2021-09-01 04:46:28.418400 mystran_validation-0.9.0/PKG-INFO
+-rw-r--r--   0 nic       (1001) nic       (1001)     5743 2021-08-16 11:21:00.000000 mystran_validation-0.9.0/README.md
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-09-01 04:46:28.414400 mystran_validation-0.9.0/docs/
+-rw-r--r--   0 nic       (1001) nic       (1001)      619 2021-05-17 05:41:29.000000 mystran_validation-0.9.0/docs/Makefile
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2021-05-17 05:41:30.000000 mystran_validation-0.9.0/docs/authors.rst
+-rwxr-xr-x   0 nic       (1001) nic       (1001)     5043 2021-05-19 07:41:49.000000 mystran_validation-0.9.0/docs/conf.py
+-rw-r--r--   0 nic       (1001) nic       (1001)       33 2021-05-17 05:41:30.000000 mystran_validation-0.9.0/docs/contributing.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2021-05-17 05:41:30.000000 mystran_validation-0.9.0/docs/history.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      315 2021-05-17 05:41:30.000000 mystran_validation-0.9.0/docs/index.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      102 2021-05-17 05:41:30.000000 mystran_validation-0.9.0/docs/installation.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      780 2021-05-17 05:41:30.000000 mystran_validation-0.9.0/docs/make.bat
+-rw-r--r--   0 nic       (1001) nic       (1001)       27 2021-05-17 05:41:30.000000 mystran_validation-0.9.0/docs/readme.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       91 2021-05-17 05:41:29.000000 mystran_validation-0.9.0/docs/usage.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-09-01 04:46:28.414400 mystran_validation-0.9.0/mystran_validation/
+-rw-r--r--   0 nic       (1001) nic       (1001)     4486 2021-09-01 04:46:20.000000 mystran_validation-0.9.0/mystran_validation/__init__.py
+-rw-r--r--   0 nic       (1001) nic       (1001)    10377 2021-09-01 04:45:36.000000 mystran_validation-0.9.0/mystran_validation/cli.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    14361 2021-09-01 04:44:25.000000 mystran_validation-0.9.0/mystran_validation/conftest_ref.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-09-01 04:46:28.414400 mystran_validation-0.9.0/mystran_validation/data/
+-rw-rw-r--   0 nic       (1001) nic       (1001)        0 2021-08-15 07:53:09.000000 mystran_validation-0.9.0/mystran_validation/data/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     6074 2021-05-17 20:48:53.000000 mystran_validation-0.9.0/mystran_validation/data/bulk_model.nas
+-rw-rw-r--   0 nic       (1001) nic       (1001)     6074 2021-05-17 20:48:53.000000 mystran_validation-0.9.0/mystran_validation/data/bulk_model_2.dat
+-rw-rw-r--   0 nic       (1001) nic       (1001)      582 2021-08-15 09:11:55.000000 mystran_validation-0.9.0/mystran_validation/data/test_bar.ini
+-rw-rw-r--   0 nic       (1001) nic       (1001)    35016 2021-05-17 20:48:53.000000 mystran_validation-0.9.0/mystran_validation/data/test_case_03.op2
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-09-01 04:46:28.414400 mystran_validation-0.9.0/mystran_validation/parsers/
+-rw-rw-r--   0 nic       (1001) nic       (1001)      769 2021-05-19 07:41:49.000000 mystran_validation-0.9.0/mystran_validation/parsers/__init__.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     2281 2021-05-25 07:11:13.000000 mystran_validation-0.9.0/mystran_validation/parsers/nastran_op2.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     6257 2021-09-01 04:45:36.000000 mystran_validation-0.9.0/mystran_validation/xml_junit2html.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-09-01 04:46:28.414400 mystran_validation-0.9.0/mystran_validation.egg-info/
+-rw-rw-r--   0 nic       (1001) nic       (1001)     8084 2021-09-01 04:46:28.000000 mystran_validation-0.9.0/mystran_validation.egg-info/PKG-INFO
+-rw-rw-r--   0 nic       (1001) nic       (1001)      971 2021-09-01 04:46:28.000000 mystran_validation-0.9.0/mystran_validation.egg-info/SOURCES.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2021-09-01 04:46:28.000000 mystran_validation-0.9.0/mystran_validation.egg-info/dependency_links.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)       61 2021-09-01 04:46:28.000000 mystran_validation-0.9.0/mystran_validation.egg-info/entry_points.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2021-09-01 04:46:28.000000 mystran_validation-0.9.0/mystran_validation.egg-info/not-zip-safe
+-rw-rw-r--   0 nic       (1001) nic       (1001)      113 2021-09-01 04:46:28.000000 mystran_validation-0.9.0/mystran_validation.egg-info/requires.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)       19 2021-09-01 04:46:28.000000 mystran_validation-0.9.0/mystran_validation.egg-info/top_level.txt
+-rw-r--r--   0 nic       (1001) nic       (1001)      460 2021-09-01 04:46:28.418400 mystran_validation-0.9.0/setup.cfg
+-rw-r--r--   0 nic       (1001) nic       (1001)     1516 2021-09-01 04:46:20.000000 mystran_validation-0.9.0/setup.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2021-09-01 04:46:28.418400 mystran_validation-0.9.0/tests/
+-rw-r--r--   0 nic       (1001) nic       (1001)       73 2021-05-17 10:04:45.000000 mystran_validation-0.9.0/tests/__init__.py
```

### Comparing `mystran_validation-0.8.0/LICENSE` & `mystran_validation-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/PKG-INFO` & `mystran_validation-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mystran_validation
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python framework for MYSTRAN validation
 Home-page: UNKNOWN
 Author: Nicolas Cordier
 Author-email: nicolas.cordier@numeric-gmbh.ch
 License: MIT license
 Description: MYSTRAN validation
         ==================
```

### Comparing `mystran_validation-0.8.0/README.md` & `mystran_validation-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/docs/Makefile` & `mystran_validation-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/docs/conf.py` & `mystran_validation-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/docs/make.bat` & `mystran_validation-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/mystran_validation/__init__.py` & `mystran_validation-0.9.0/mystran_validation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for MYSTRAN validation."""
 
 __author__ = """Nicolas Cordier"""
 __email__ = "nicolas.cordier@numeric-gmbh.ch"
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 import os
 import configparser
 from pathlib import Path
 import logging
 import shutil
 from functools import wraps
```

### Comparing `mystran_validation-0.8.0/mystran_validation/cli.py` & `mystran_validation-0.9.0/mystran_validation/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 import pkg_resources
 
 import click
 import pytest
 
 from mystran_validation import get_conf, get_profile, init_config
 
+HTML = "notown"
+
 
 def find(
     path,
     extensions,
     name="*",
     break_on_first=True,
     return_first=True,
@@ -253,23 +255,31 @@
     click.echo(click.style(f"  * rootdir={rootdir}", fg="green"))
     click.echo(click.style(f"  * {dump=}", fg="green"))
     click.echo("\n")
     args = list(pytest_args)
     if report:
         junit_file, junit_html_target = get_junit_files(rootdir)
         args += [f"--junitxml={junit_file}"]
+    args += ["--disable-pytest-warnings"]  # disable UnknownMarkWarning
     args.append(str(rootdir))
     pytest.main(args)
     if report:
-        python_bin = shutil.which("python")
-        subprocess.run(
-            shlex.split(
-                f"{python_bin} -m junit2htmlreport {junit_file} {junit_html_target}"
+        if HTML == "own":
+            from mystran_validation.xml_junit2html import xml2html
+
+            html = xml2html(junit_file)
+            with open(junit_html_target, "w") as fh:
+                fh.write(html)
+        else:
+            python_bin = shutil.which("python")
+            subprocess.run(
+                shlex.split(
+                    f"{python_bin} -m junit2htmlreport {junit_file} {junit_html_target}"
+                )
             )
-        )
     teardown(rootdir)
     if report and open_report:
         webbrowser.open(str(junit_html_target.resolve()))
     return 0
 
 
 @main.command(
```

### Comparing `mystran_validation-0.8.0/mystran_validation/conftest_ref.py` & `mystran_validation-0.9.0/mystran_validation/conftest_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,34 @@
 
 # =============================================================================
 # test collection
 # =============================================================================
 ROOTDIR = None
 
 
-# def pytest_collection_modifyitems(items):
-#     """add CARDs to marks"""
-#     for item in items:
-#         bulk_file = item.spec["bulk"]
-#         with open(bulk_file, "r") as fh:
-#             lines = fh.readlines()
-#         words = set(
-#             [
-#                 l.split(" ")[0].strip()
-#                 for l in lines
-#                 if not l.startswith("$") and not l.startswith("+")
-#             ]
-#         ) - set(["", " "])
-#         for tag in words:
-#             item.add_marker(getattr(pytest.mark, tag))
+def pytest_collection_modifyitems(items):
+    """add CARDs to marks"""
+    for item in items:
+        bulk_file = item.spec["bulk"]
+        with open(bulk_file, "r") as fh:
+            lines = fh.readlines()
+        words = set(
+            [
+                l.split(" ")[0].strip()
+                for l in lines
+                if not l.startswith("$") and not l.startswith("+")
+            ]
+        ) - set(["", " "])
+        for tag in words:
+            item.add_marker(getattr(pytest.mark, tag))
+        marks = item.spec.get("marks", ())
+        if marks:
+            marks = [m.strip() for m in marks.split(",")]
+            for mark in marks:
+                item.add_marker(getattr(pytest.mark, mark))
 
 
 def pytest_collect_file(parent, path):
     global ROOTDIR
     if ROOTDIR is None:  # set rootdir for centralized dumping
         ROOTDIR = Path(path.dirpath())
     _path = Path(path)
```

### Comparing `mystran_validation-0.8.0/mystran_validation/data/bulk_model.nas` & `mystran_validation-0.9.0/mystran_validation/data/bulk_model.nas`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/mystran_validation/data/bulk_model_2.dat` & `mystran_validation-0.9.0/mystran_validation/data/bulk_model_2.dat`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/mystran_validation/data/test_bar.ini` & `mystran_validation-0.9.0/mystran_validation/data/test_bar.ini`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/mystran_validation/data/test_case_03.op2` & `mystran_validation-0.9.0/mystran_validation/data/test_case_03.op2`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/mystran_validation/parsers/__init__.py` & `mystran_validation-0.9.0/mystran_validation/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/mystran_validation/parsers/nastran_op2.py` & `mystran_validation-0.9.0/mystran_validation/parsers/nastran_op2.py`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/mystran_validation.egg-info/PKG-INFO` & `mystran_validation-0.9.0/mystran_validation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mystran-validation
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python framework for MYSTRAN validation
 Home-page: UNKNOWN
 Author: Nicolas Cordier
 Author-email: nicolas.cordier@numeric-gmbh.ch
 License: MIT license
 Description: MYSTRAN validation
         ==================
```

### Comparing `mystran_validation-0.8.0/mystran_validation.egg-info/SOURCES.txt` & `mystran_validation-0.9.0/mystran_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mystran_validation-0.8.0/setup.py` & `mystran_validation-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     packages=find_packages(include=["mystran_validation", "mystran_validation.*"]),
     package_data={
         "data": ["*.op2", "*.OP2", "*.ini", "*.nas", "*.dat", "*.bdf"],
     },
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
-    version="0.8.0",
+    version="0.9.0",
     zip_safe=False,
 )
```

