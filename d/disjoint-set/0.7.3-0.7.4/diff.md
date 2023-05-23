# Comparing `tmp/disjoint_set-0.7.3.tar.gz` & `tmp/disjoint_set-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/disjoint_set-0.7.3.tar", last modified: Tue Nov  2 18:53:02 2021, max compression
+gzip compressed data, was "disjoint_set-0.7.4.tar", last modified: Tue May 23 12:32:02 2023, max compression
```

## Comparing `disjoint_set-0.7.3.tar` & `disjoint_set-0.7.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 mrapacz    (501) staff       (20)        0 2021-11-02 18:53:02.000000 disjoint_set-0.7.3/
--rw-r--r--   0 mrapacz    (501) staff       (20)     2521 2021-11-02 18:53:02.000000 disjoint_set-0.7.3/PKG-INFO
--rw-r--r--   0 mrapacz    (501) staff       (20)     1451 2021-11-02 18:52:30.000000 disjoint_set-0.7.3/README.md
-drwxr-xr-x   0 mrapacz    (501) staff       (20)        0 2021-11-02 18:53:02.000000 disjoint_set-0.7.3/disjoint_set/
--rw-r--r--   0 mrapacz    (501) staff       (20)      176 2021-11-02 18:52:30.000000 disjoint_set-0.7.3/disjoint_set/__init__.py
--rw-r--r--   0 mrapacz    (501) staff       (20)     4453 2021-11-02 18:49:46.000000 disjoint_set-0.7.3/disjoint_set/main.py
--rw-r--r--   0 mrapacz    (501) staff       (20)       58 2020-06-15 16:51:39.000000 disjoint_set-0.7.3/disjoint_set/py.typed
--rw-r--r--   0 mrapacz    (501) staff       (20)      376 2020-11-09 21:51:37.000000 disjoint_set-0.7.3/disjoint_set/utils.py
-drwxr-xr-x   0 mrapacz    (501) staff       (20)        0 2021-11-02 18:53:02.000000 disjoint_set-0.7.3/disjoint_set.egg-info/
--rw-r--r--   0 mrapacz    (501) staff       (20)     2521 2021-11-02 18:53:01.000000 disjoint_set-0.7.3/disjoint_set.egg-info/PKG-INFO
--rw-r--r--   0 mrapacz    (501) staff       (20)      267 2021-11-02 18:53:01.000000 disjoint_set-0.7.3/disjoint_set.egg-info/SOURCES.txt
--rw-r--r--   0 mrapacz    (501) staff       (20)        1 2021-11-02 18:53:01.000000 disjoint_set-0.7.3/disjoint_set.egg-info/dependency_links.txt
--rw-r--r--   0 mrapacz    (501) staff       (20)       13 2021-11-02 18:53:01.000000 disjoint_set-0.7.3/disjoint_set.egg-info/top_level.txt
--rw-r--r--   0 mrapacz    (501) staff       (20)      504 2021-11-02 18:52:30.000000 disjoint_set-0.7.3/pyproject.toml
--rw-r--r--   0 mrapacz    (501) staff       (20)       38 2021-11-02 18:53:02.000000 disjoint_set-0.7.3/setup.cfg
--rw-r--r--   0 mrapacz    (501) staff       (20)      688 2020-11-09 21:51:37.000000 disjoint_set-0.7.3/setup.py
+drwxr-xr-x   0 mrapacz    (501) staff       (20)        0 2023-05-23 12:32:02.353394 disjoint_set-0.7.4/
+-rw-r--r--   0 mrapacz    (501) staff       (20)     1070 2023-05-23 12:02:01.000000 disjoint_set-0.7.4/LICENSE
+-rw-r--r--   0 mrapacz    (501) staff       (20)     1907 2023-05-23 12:32:02.352963 disjoint_set-0.7.4/PKG-INFO
+-rw-r--r--   0 mrapacz    (501) staff       (20)     1455 2023-05-23 12:27:47.000000 disjoint_set-0.7.4/README.md
+drwxr-xr-x   0 mrapacz    (501) staff       (20)        0 2023-05-23 12:32:02.349288 disjoint_set-0.7.4/disjoint_set/
+-rw-r--r--   0 mrapacz    (501) staff       (20)      176 2023-05-23 12:28:13.000000 disjoint_set-0.7.4/disjoint_set/__init__.py
+-rw-r--r--   0 mrapacz    (501) staff       (20)     4453 2023-05-23 12:02:01.000000 disjoint_set-0.7.4/disjoint_set/main.py
+-rw-r--r--   0 mrapacz    (501) staff       (20)       58 2023-05-23 12:02:01.000000 disjoint_set-0.7.4/disjoint_set/py.typed
+-rw-r--r--   0 mrapacz    (501) staff       (20)      376 2023-05-23 12:02:01.000000 disjoint_set-0.7.4/disjoint_set/utils.py
+drwxr-xr-x   0 mrapacz    (501) staff       (20)        0 2023-05-23 12:32:02.351585 disjoint_set-0.7.4/disjoint_set.egg-info/
+-rw-r--r--   0 mrapacz    (501) staff       (20)     1907 2023-05-23 12:32:02.000000 disjoint_set-0.7.4/disjoint_set.egg-info/PKG-INFO
+-rw-r--r--   0 mrapacz    (501) staff       (20)      302 2023-05-23 12:32:02.000000 disjoint_set-0.7.4/disjoint_set.egg-info/SOURCES.txt
+-rw-r--r--   0 mrapacz    (501) staff       (20)        1 2023-05-23 12:32:02.000000 disjoint_set-0.7.4/disjoint_set.egg-info/dependency_links.txt
+-rw-r--r--   0 mrapacz    (501) staff       (20)       13 2023-05-23 12:32:02.000000 disjoint_set-0.7.4/disjoint_set.egg-info/top_level.txt
+-rw-r--r--   0 mrapacz    (501) staff       (20)      492 2023-05-23 12:19:58.000000 disjoint_set-0.7.4/pyproject.toml
+-rw-r--r--   0 mrapacz    (501) staff       (20)       38 2023-05-23 12:32:02.353530 disjoint_set-0.7.4/setup.cfg
+-rw-r--r--   0 mrapacz    (501) staff       (20)      720 2023-05-23 12:31:00.000000 disjoint_set-0.7.4/setup.py
+drwxr-xr-x   0 mrapacz    (501) staff       (20)        0 2023-05-23 12:32:02.352019 disjoint_set-0.7.4/tests/
+-rw-r--r--   0 mrapacz    (501) staff       (20)     2184 2023-05-23 12:02:01.000000 disjoint_set-0.7.4/tests/test_disjoint_set.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `disjoint_set-0.7.3/README.md` & `disjoint_set-0.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 ![Coveralls](https://img.shields.io/coveralls/github/mrapacz/disjoint-set/master.svg)
 ![PyPI - License](https://img.shields.io/pypi/l/disjoint_set.svg)
 
 [DisjointSet](https://en.wikipedia.org/wiki/Disjoint-set_data_structure) (a.k.a. union–find data structure or merge–find set) implementation for Python.
 
 ## Prerequisites
 
-The only requirement is having Python 3 installed, you can verify this by running:
+The only requirement is having Python 3.8+ installed, you can verify this by running:
 ```bash
 $ python --version
-Python 3.7.2
+Python 3.8.16
 ```
 
 ## Installation
 ```
 pip install disjoint-set
 ```
 
 You can verify you're running the latest package version by running:
 ```python
 >>> import disjoint_set
 >>> disjoint_set.__version__
-'0.7.3'
+'0.7.4'
 
 ```
 
 ## Usage
 
 ```python
 >>> from disjoint_set import DisjointSet
```

### Comparing `disjoint_set-0.7.3/disjoint_set/main.py` & `disjoint_set-0.7.4/disjoint_set/main.py`

 * *Files identical despite different names*

### Comparing `disjoint_set-0.7.3/setup.py` & `disjoint_set-0.7.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setuptools.setup(
     name="disjoint_set",
     version=disjoint_set.__version__,
     packages=setuptools.find_packages(),
     package_data={"disjoint_set": ["py.typed"]},
     description="Disjoint set data structure implementation for Python",
     url="https://github.com/mrapacz/disjoint_set",
+    license_files=("LICENSE",),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     maintainer="Maciej Rapacz",
     maintainer_email="python.disjointset@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

