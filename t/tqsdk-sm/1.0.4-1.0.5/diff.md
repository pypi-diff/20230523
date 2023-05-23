# Comparing `tmp/tqsdk-sm-1.0.4.tar.gz` & `tmp/tqsdk-sm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tqsdk-sm-1.0.4.tar", last modified: Wed Apr 12 06:31:08 2023, max compression
+gzip compressed data, was "dist/tqsdk-sm-1.0.5.tar", last modified: Tue May 23 07:57:53 2023, max compression
```

## Comparing `tqsdk-sm-1.0.4.tar` & `tqsdk-sm-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/tqsdk_sm/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-12 06:30:57.000000 tqsdk-sm-1.0.4/tqsdk_sm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/tqsdk_sm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/tqsdk_sm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/tqsdk_sm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/tqsdk_sm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 06:31:08.000000 tqsdk-sm-1.0.4/tqsdk_sm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-12 06:30:57.000000 tqsdk-sm-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-05-23 07:57:43.000000 tqsdk-sm-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/tqsdk_sm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/tqsdk_sm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/tqsdk_sm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/tqsdk_sm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/tqsdk_sm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 07:57:53.000000 tqsdk-sm-1.0.5/tqsdk_sm/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-23 07:57:43.000000 tqsdk-sm-1.0.5/tqsdk_sm/__init__.py
```

### Comparing `tqsdk-sm-1.0.4/setup.py` & `tqsdk-sm-1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             python, abi = 'py3', 'none'
             return python, abi, plat
 except ImportError:
     bdist_wheel = None
 
 setuptools.setup(
     name='tqsdk-sm',
-    version="1.0.4",
+    version="1.0.5",
     description='TianQin SDK - sm lib',
     author='TianQin',
     author_email='tianqincn@gmail.com',
     url='https://www.shinnytech.com/tqsdk',
     packages=setuptools.find_packages(),
     python_requires='>=3',
     cmdclass={'bdist_wheel': bdist_wheel},
```

