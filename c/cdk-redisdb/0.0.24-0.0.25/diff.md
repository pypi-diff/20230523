# Comparing `tmp/cdk-redisdb-0.0.24.tar.gz` & `tmp/cdk-redisdb-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.24.tar", last modified: Mon May 22 02:21:18 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.25.tar", last modified: Tue May 23 01:53:14 2023, max compression
```

## Comparing `cdk-redisdb-0.0.24.tar` & `cdk-redisdb-0.0.25.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.224521 cdk-redisdb-0.0.24/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.24.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:14.951907 cdk-redisdb-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-23 01:53:14.951907 cdk-redisdb-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:53:14.951907 cdk-redisdb-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:14.947907 cdk-redisdb-0.0.25/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:14.947907 cdk-redisdb-0.0.25/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:14.951907 cdk-redisdb-0.0.25/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25934 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.25.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:53:03.000000 cdk-redisdb-0.0.25/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:14.951907 cdk-redisdb-0.0.25/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-23 01:53:14.000000 cdk-redisdb-0.0.25/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 01:53:14.000000 cdk-redisdb-0.0.25/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:53:14.000000 cdk-redisdb-0.0.25/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 01:53:14.000000 cdk-redisdb-0.0.25/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 01:53:14.000000 cdk-redisdb-0.0.25/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.24/LICENSE` & `cdk-redisdb-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.24/PKG-INFO` & `cdk-redisdb-0.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.24
+Version: 0.0.25
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.24/README.md` & `cdk-redisdb-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.24/setup.py` & `cdk-redisdb-0.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.24",
+    "version": "0.0.25",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.24.jsii.tgz"
+            "cdk-redisdb@0.0.25.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.76.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-redisdb-0.0.24/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.25/src/cdk_redisdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.25/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.24
+Version: 0.0.25
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

