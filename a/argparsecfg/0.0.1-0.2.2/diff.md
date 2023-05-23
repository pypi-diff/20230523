# Comparing `tmp/argparsecfg-0.0.1.tar.gz` & `tmp/argparsecfg-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparsecfg-0.0.1.tar", last modified: Wed Mar  1 13:35:49 2023, max compression
+gzip compressed data, was "argparsecfg-0.2.2.tar", last modified: Tue May 23 08:06:28 2023, max compression
```

## Comparing `argparsecfg-0.0.1.tar` & `argparsecfg-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-03-01 13:35:49.314869 argparsecfg-0.0.1/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-03-01 13:23:52.000000 argparsecfg-0.0.1/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)      510 2023-03-01 13:35:49.314869 argparsecfg-0.0.1/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)       39 2023-03-01 13:28:51.000000 argparsecfg-0.0.1/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      603 2023-03-01 13:35:49.318868 argparsecfg-0.0.1/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-03-01 13:26:27.000000 argparsecfg-0.0.1/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-03-01 13:35:49.314869 argparsecfg-0.0.1/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-03-01 13:35:49.314869 argparsecfg-0.0.1/src/argparsecfg/
--rw-rw-r--   0 aya       (1000) aya       (1000)        0 2023-03-01 13:27:16.000000 argparsecfg-0.0.1/src/argparsecfg/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-03-01 13:27:48.000000 argparsecfg-0.0.1/src/argparsecfg/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-03-01 13:35:49.314869 argparsecfg-0.0.1/src/argparsecfg.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)      510 2023-03-01 13:35:49.000000 argparsecfg-0.0.1/src/argparsecfg.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      285 2023-03-01 13:35:49.000000 argparsecfg-0.0.1/src/argparsecfg.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-03-01 13:35:49.000000 argparsecfg-0.0.1/src/argparsecfg.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       62 2023-03-01 13:35:49.000000 argparsecfg-0.0.1/src/argparsecfg.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       12 2023-03-01 13:35:49.000000 argparsecfg-0.0.1/src/argparsecfg.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-03-01 13:23:52.000000 argparsecfg-0.2.2/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)      510 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)       39 2023-03-01 13:28:51.000000 argparsecfg-0.2.2/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      635 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-03-01 13:26:27.000000 argparsecfg-0.2.2/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.766917 argparsecfg-0.2.2/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.770917 argparsecfg-0.2.2/src/argparsecfg/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      168 2023-05-16 08:07:33.000000 argparsecfg-0.2.2/src/argparsecfg/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11856 2023-05-23 08:03:10.000000 argparsecfg-0.2.2/src/argparsecfg/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-05-17 17:59:38.000000 argparsecfg-0.2.2/src/argparsecfg/test_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-05-23 08:03:10.000000 argparsecfg-0.2.2/src/argparsecfg/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.770917 argparsecfg-0.2.2/src/argparsecfg.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      510 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      560 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       48 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       12 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5664 2023-05-17 12:03:24.000000 argparsecfg-0.2.2/tests/test_add_argument_field.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4103 2023-05-23 08:03:10.000000 argparsecfg-0.2.2/tests/test_add_argument_field_errors.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4307 2023-05-11 15:13:36.000000 argparsecfg-0.2.2/tests/test_add_argument_metadata.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2055 2023-05-11 15:13:36.000000 argparsecfg-0.2.2/tests/test_add_argument_simple.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1184 2023-05-06 09:44:14.000000 argparsecfg-0.2.2/tests/test_create_parser.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      517 2023-04-28 14:29:56.000000 argparsecfg-0.2.2/tests/test_parse_args.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3942 2023-05-15 08:47:52.000000 argparsecfg-0.2.2/tests/test_test_tools.py
```

### Comparing `argparsecfg-0.0.1/LICENSE` & `argparsecfg-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.0.1/setup.cfg` & `argparsecfg-0.2.2/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.7
 
 [options.packages.find]
 where = src
+exclude = 
+	tests*
+	Nbs*
+	docs*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `argparsecfg-0.0.1/setup.py` & `argparsecfg-0.2.2/setup.py`

 * *Files identical despite different names*

