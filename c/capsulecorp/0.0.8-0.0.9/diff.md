# Comparing `tmp/capsulecorp-0.0.8.tar.gz` & `tmp/capsulecorp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.0.8.tar", last modified: Fri Feb 17 19:53:55 2023, max compression
+gzip compressed data, was "capsulecorp-0.0.9.tar", last modified: Mon Feb 20 19:07:30 2023, max compression
```

## Comparing `capsulecorp-0.0.8.tar` & `capsulecorp-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-17 19:53:55.898771 capsulecorp-0.0.8/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.0.8/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      416 2023-02-17 19:53:55.898398 capsulecorp-0.0.8/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.0.8/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-17 19:53:55.895378 capsulecorp-0.0.8/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.0.8/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7014 2023-02-17 19:52:02.000000 capsulecorp-0.0.8/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-02-17 19:50:49.000000 capsulecorp-0.0.8/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-17 19:53:55.897898 capsulecorp-0.0.8/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      416 2023-02-17 19:53:55.000000 capsulecorp-0.0.8/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      283 2023-02-17 19:53:55.000000 capsulecorp-0.0.8/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-02-17 19:53:55.000000 capsulecorp-0.0.8/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)       41 2023-02-17 19:53:55.000000 capsulecorp-0.0.8/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-02-17 19:53:55.000000 capsulecorp-0.0.8/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.0.8/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-02-17 19:53:55.898904 capsulecorp-0.0.8/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6468 2023-02-16 19:41:24.000000 capsulecorp-0.0.8/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-20 19:07:30.561112 capsulecorp-0.0.9/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.0.9/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      416 2023-02-20 19:07:30.560795 capsulecorp-0.0.9/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.0.9/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-20 19:07:30.558177 capsulecorp-0.0.9/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.0.9/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)    11476 2023-02-20 19:02:38.000000 capsulecorp-0.0.9/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-02-20 18:55:49.000000 capsulecorp-0.0.9/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-20 19:07:30.560406 capsulecorp-0.0.9/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      416 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      283 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       55 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.0.9/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-02-20 19:07:30.561224 capsulecorp-0.0.9/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6493 2023-02-20 18:55:51.000000 capsulecorp-0.0.9/setup.py
```

### Comparing `capsulecorp-0.0.8/LICENSE` & `capsulecorp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.0.8/setup.py` & `capsulecorp-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,12 +54,13 @@
         'Programming Language :: Python :: 3.9',
     ],
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     python_requires='>=3.9',
     # Dependencies
     install_requires=[
         'PyYAML>=5.3',
+        'numpy>=1.20.3',
         'pandas>=1.3.4',
         'boto3==1.24.75'
     ],
     include_package_data=True
 )
```

