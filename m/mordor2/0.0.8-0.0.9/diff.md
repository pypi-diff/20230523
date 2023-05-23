# Comparing `tmp/mordor2-0.0.8.tar.gz` & `tmp/mordor2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mordor2-0.0.8.tar", last modified: Sat Mar 23 07:33:02 2019, max compression
+gzip compressed data, was "dist/mordor2-0.0.9.tar", last modified: Sat Mar 23 07:49:17 2019, max compression
```

## Comparing `mordor2-0.0.8.tar` & `mordor2-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:33:02.000000 mordor2-0.0.8/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2019-03-23 07:33:02.000000 mordor2-0.0.8/setup.cfg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor2.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        7 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor2.egg-info/top_level.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       47 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor2.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor2.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      372 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor2.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     7534 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor2.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5914 2019-03-22 03:03:08.000000 mordor2-0.0.8/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      982 2019-03-23 06:27:22.000000 mordor2-0.0.8/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor/
--rwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)    12466 2019-03-23 07:26:12.000000 mordor2-0.0.8/mordor/mordor.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-05 12:08:23.000000 mordor2-0.0.8/mordor/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:33:02.000000 mordor2-0.0.8/mordor/bin/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      242 2019-03-23 06:58:37.000000 mordor2-0.0.8/mordor/bin/run_app_py.sh
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      179 2019-03-23 06:08:09.000000 mordor2-0.0.8/mordor/bin/run_app.sh
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      300 2019-03-05 12:02:27.000000 mordor2-0.0.8/mordor/bin/get_app_status.sh
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      183 2019-03-05 12:03:17.000000 mordor2-0.0.8/mordor/bin/install_packages.sh
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       78 2019-03-05 12:03:17.000000 mordor2-0.0.8/mordor/bin/kill_app.sh
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1087 2019-03-23 07:22:10.000000 mordor2-0.0.8/mordor/app_env.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     7534 2019-03-23 07:33:02.000000 mordor2-0.0.8/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       49 2019-03-05 12:53:13.000000 mordor2-0.0.8/MANIFEST.in
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:49:17.000000 mordor2-0.0.9/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2019-03-23 07:49:17.000000 mordor2-0.0.9/setup.cfg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor2.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        7 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor2.egg-info/top_level.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       47 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor2.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor2.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      372 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor2.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     7534 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor2.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5914 2019-03-22 03:03:08.000000 mordor2-0.0.9/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      982 2019-03-23 07:39:32.000000 mordor2-0.0.9/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor/
+-rwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)    12466 2019-03-23 07:26:12.000000 mordor2-0.0.9/mordor/mordor.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       28 2019-03-23 07:43:54.000000 mordor2-0.0.9/mordor/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2019-03-23 07:49:17.000000 mordor2-0.0.9/mordor/bin/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      242 2019-03-23 06:58:37.000000 mordor2-0.0.9/mordor/bin/run_app_py.sh
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      179 2019-03-23 06:08:09.000000 mordor2-0.0.9/mordor/bin/run_app.sh
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      300 2019-03-05 12:02:27.000000 mordor2-0.0.9/mordor/bin/get_app_status.sh
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      183 2019-03-05 12:03:17.000000 mordor2-0.0.9/mordor/bin/install_packages.sh
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       78 2019-03-05 12:03:17.000000 mordor2-0.0.9/mordor/bin/kill_app.sh
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1087 2019-03-23 07:22:10.000000 mordor2-0.0.9/mordor/app_env.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     7534 2019-03-23 07:49:17.000000 mordor2-0.0.9/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       49 2019-03-05 12:53:13.000000 mordor2-0.0.9/MANIFEST.in
```

### Comparing `mordor2-0.0.8/mordor2.egg-info/PKG-INFO` & `mordor2-0.0.9/mordor2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mordor2
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Deployment Tool
 Home-page: https://github.com/stonezhong/mordor
 Author: Stone Zhong
 Author-email: stonezhong@hotmail.com
 License: MIT
 Description: # Purpose
```

### Comparing `mordor2-0.0.8/README.md` & `mordor2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mordor2-0.0.8/setup.py` & `mordor2-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="mordor2",
-    version="0.0.8",
+    version="0.0.9",
     description="Python Deployment Tool",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/mordor",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `mordor2-0.0.8/mordor/mordor.py` & `mordor2-0.0.9/mordor/mordor.py`

 * *Files identical despite different names*

### Comparing `mordor2-0.0.8/mordor/app_env.py` & `mordor2-0.0.9/mordor/app_env.py`

 * *Files identical despite different names*

### Comparing `mordor2-0.0.8/PKG-INFO` & `mordor2-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mordor2
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Deployment Tool
 Home-page: https://github.com/stonezhong/mordor
 Author: Stone Zhong
 Author-email: stonezhong@hotmail.com
 License: MIT
 Description: # Purpose
```

