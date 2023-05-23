# Comparing `tmp/things-cli-0.2.0.tar.gz` & `tmp/things-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "things-cli-0.2.0.tar", last modified: Mon May 22 20:06:31 2023, max compression
+gzip compressed data, was "things-cli-0.2.1.tar", last modified: Tue May 23 06:01:16 2023, max compression
```

## Comparing `things-cli-0.2.0.tar` & `things-cli-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-22 20:06:31.228853 things-cli-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-22 20:06:11.000000 things-cli-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 20:06:31.228853 things-cli-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-22 20:06:11.000000 things-cli-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:11.000000 things-cli-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-22 20:06:11.000000 things-cli-0.2.0/tests/test_things_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/things_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 20:06:11.000000 things-cli-0.2.0/things_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17258 2023-05-22 20:06:11.000000 things-cli-0.2.0/things_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/things_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:01:16.437304 things-cli-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-23 06:01:16.437304 things-cli-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-23 06:01:05.000000 things-cli-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-23 06:01:16.437304 things-cli-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-23 06:01:05.000000 things-cli-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:01:16.433304 things-cli-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:01:05.000000 things-cli-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-23 06:01:05.000000 things-cli-0.2.1/tests/test_things_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:01:16.437304 things-cli-0.2.1/things_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-23 06:01:05.000000 things-cli-0.2.1/things_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17258 2023-05-23 06:01:05.000000 things-cli-0.2.1/things_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:01:16.437304 things-cli-0.2.1/things_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-23 06:01:16.000000 things-cli-0.2.1/things_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-23 06:01:16.000000 things-cli-0.2.1/things_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:01:16.000000 things-cli-0.2.1/things_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 06:01:16.000000 things-cli-0.2.1/things_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 06:01:16.000000 things-cli-0.2.1/things_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 06:01:16.000000 things-cli-0.2.1/things_cli.egg-info/top_level.txt
```

### Comparing `things-cli-0.2.0/PKG-INFO` & `things-cli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: things-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple Python 3 CLI to read your Things app data.
 Home-page: https://github.com/thingsapi/things-cli
 Author: Alexander Willner
 Author-email: alex@willner.ws
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `things-cli-0.2.0/README.md` & `things-cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `things-cli-0.2.0/setup.py` & `things-cli-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,9 +52,9 @@
     options={"py2app": OPTIONS},
     setup_requires=["py2app"],
     entry_points={
         "console_scripts": [
             "things-cli = things_cli.cli:main",
         ]
     },
-    install_requires=["things.py", "argcomplete"],
+    install_requires=["things.py>=0.0.15", "argcomplete>=3.0.0"],
 )
```

### Comparing `things-cli-0.2.0/tests/test_things_cli.py` & `things-cli-0.2.1/tests/test_things_cli.py`

 * *Files identical despite different names*

### Comparing `things-cli-0.2.0/things_cli/cli.py` & `things-cli-0.2.1/things_cli/cli.py`

 * *Files identical despite different names*

### Comparing `things-cli-0.2.0/things_cli.egg-info/PKG-INFO` & `things-cli-0.2.1/things_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: things-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple Python 3 CLI to read your Things app data.
 Home-page: https://github.com/thingsapi/things-cli
 Author: Alexander Willner
 Author-email: alex@willner.ws
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

