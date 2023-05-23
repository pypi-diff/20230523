# Comparing `tmp/quickstart-vdk-0.2.874128920.dev10670.tar.gz` & `tmp/quickstart-vdk-0.2.874667213.dev10687.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.874128920.dev10670.tar", last modified: Mon May 22 04:23:28 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.874667213.dev10687.tar", last modified: Mon May 22 12:58:39 2023, max compression
```

## Comparing `quickstart-vdk-0.2.874128920.dev10670.tar` & `quickstart-vdk-0.2.874667213.dev10687.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:23:28.264664 quickstart-vdk-0.2.874128920.dev10670/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 04:23:28.264664 quickstart-vdk-0.2.874128920.dev10670/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-22 04:20:41.000000 quickstart-vdk-0.2.874128920.dev10670/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:23:28.264664 quickstart-vdk-0.2.874128920.dev10670/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 04:23:28.000000 quickstart-vdk-0.2.874128920.dev10670/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-22 04:23:28.000000 quickstart-vdk-0.2.874128920.dev10670/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 04:23:28.000000 quickstart-vdk-0.2.874128920.dev10670/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 04:23:28.000000 quickstart-vdk-0.2.874128920.dev10670/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-22 04:23:28.000000 quickstart-vdk-0.2.874128920.dev10670/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 04:23:28.264664 quickstart-vdk-0.2.874128920.dev10670/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-22 04:23:16.000000 quickstart-vdk-0.2.874128920.dev10670/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:23:28.264664 quickstart-vdk-0.2.874128920.dev10670/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-22 04:20:41.000000 quickstart-vdk-0.2.874128920.dev10670/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-22 12:58:19.000000 quickstart-vdk-0.2.874667213.dev10687/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-22 12:58:29.000000 quickstart-vdk-0.2.874667213.dev10687/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-22 12:58:19.000000 quickstart-vdk-0.2.874667213.dev10687/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.874128920.dev10670/PKG-INFO` & `quickstart-vdk-0.2.874667213.dev10687/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.874128920.dev10670
+Version: 0.2.874667213.dev10687
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.874128920.dev10670/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.874128920.dev10670
+Version: 0.2.874667213.dev10687
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.874128920.dev10670/setup.py` & `quickstart-vdk-0.2.874667213.dev10687/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.874128920.dev10670"
+__version__ = "0.2.874667213.dev10687"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

