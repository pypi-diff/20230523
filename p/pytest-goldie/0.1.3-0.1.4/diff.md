# Comparing `tmp/pytest-goldie-0.1.3.tar.gz` & `tmp/pytest-goldie-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-goldie-0.1.3.tar", last modified: Tue May 23 01:05:00 2023, max compression
+gzip compressed data, was "pytest-goldie-0.1.4.tar", last modified: Tue May 23 01:06:14 2023, max compression
```

## Comparing `pytest-goldie-0.1.3.tar` & `pytest-goldie-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:05:00.316139 pytest-goldie-0.1.3/
--rw-r--r--   0 nkartashov   (501) staff       (20)     1084 2023-03-28 22:22:38.000000 pytest-goldie-0.1.3/LICENSE
--rw-r--r--   0 nkartashov   (501) staff       (20)       97 2023-03-28 22:22:38.000000 pytest-goldie-0.1.3/MANIFEST.in
--rw-r--r--   0 nkartashov   (501) staff       (20)     2919 2023-05-23 01:05:00.316006 pytest-goldie-0.1.3/PKG-INFO
--rw-r--r--   0 nkartashov   (501) staff       (20)     1776 2023-05-23 01:04:32.000000 pytest-goldie-0.1.3/README.rst
--rw-r--r--   0 nkartashov   (501) staff       (20)      105 2023-04-12 14:50:25.000000 pytest-goldie-0.1.3/pyproject.toml
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:05:00.314978 pytest-goldie-0.1.3/pytest_goldie/
--rw-r--r--   0 nkartashov   (501) staff       (20)     2694 2023-04-24 20:31:20.000000 pytest-goldie-0.1.3/pytest_goldie/plugin.py
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:05:00.315649 pytest-goldie-0.1.3/pytest_goldie.egg-info/
--rw-r--r--   0 nkartashov   (501) staff       (20)     2919 2023-05-23 01:05:00.000000 pytest-goldie-0.1.3/pytest_goldie.egg-info/PKG-INFO
--rw-r--r--   0 nkartashov   (501) staff       (20)      345 2023-05-23 01:05:00.000000 pytest-goldie-0.1.3/pytest_goldie.egg-info/SOURCES.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)        1 2023-05-23 01:05:00.000000 pytest-goldie-0.1.3/pytest_goldie.egg-info/dependency_links.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       41 2023-05-23 01:05:00.000000 pytest-goldie-0.1.3/pytest_goldie.egg-info/entry_points.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 01:05:00.000000 pytest-goldie-0.1.3/pytest_goldie.egg-info/requires.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 01:05:00.000000 pytest-goldie-0.1.3/pytest_goldie.egg-info/top_level.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       38 2023-05-23 01:05:00.316179 pytest-goldie-0.1.3/setup.cfg
--rw-r--r--   0 nkartashov   (501) staff       (20)     1709 2023-05-23 01:04:54.000000 pytest-goldie-0.1.3/setup.py
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:05:00.315865 pytest-goldie-0.1.3/tests/
--rw-r--r--   0 nkartashov   (501) staff       (20)      586 2023-04-12 12:21:32.000000 pytest-goldie-0.1.3/tests/test_goldens.py
--rw-r--r--   0 nkartashov   (501) staff       (20)      320 2023-03-28 22:22:38.000000 pytest-goldie-0.1.3/tests/test_goldie.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.146624 pytest-goldie-0.1.4/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1084 2023-03-28 22:22:38.000000 pytest-goldie-0.1.4/LICENSE
+-rw-r--r--   0 nkartashov   (501) staff       (20)       97 2023-03-28 22:22:38.000000 pytest-goldie-0.1.4/MANIFEST.in
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2920 2023-05-23 01:06:14.146474 pytest-goldie-0.1.4/PKG-INFO
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1777 2023-05-23 01:05:57.000000 pytest-goldie-0.1.4/README.rst
+-rw-r--r--   0 nkartashov   (501) staff       (20)      105 2023-04-12 14:50:25.000000 pytest-goldie-0.1.4/pyproject.toml
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.145429 pytest-goldie-0.1.4/pytest_goldie/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2694 2023-04-24 20:31:20.000000 pytest-goldie-0.1.4/pytest_goldie/plugin.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.146076 pytest-goldie-0.1.4/pytest_goldie.egg-info/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2920 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/PKG-INFO
+-rw-r--r--   0 nkartashov   (501) staff       (20)      345 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/SOURCES.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)        1 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/dependency_links.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       41 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/entry_points.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/requires.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/top_level.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       38 2023-05-23 01:06:14.146665 pytest-goldie-0.1.4/setup.cfg
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1709 2023-05-23 01:06:09.000000 pytest-goldie-0.1.4/setup.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.146298 pytest-goldie-0.1.4/tests/
+-rw-r--r--   0 nkartashov   (501) staff       (20)      586 2023-04-12 12:21:32.000000 pytest-goldie-0.1.4/tests/test_goldens.py
+-rw-r--r--   0 nkartashov   (501) staff       (20)      320 2023-03-28 22:22:38.000000 pytest-goldie-0.1.4/tests/test_goldie.py
```

### Comparing `pytest-goldie-0.1.3/LICENSE` & `pytest-goldie-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-goldie-0.1.3/PKG-INFO` & `pytest-goldie-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-goldie
-Version: 0.1.3
+Version: 0.1.4
 Summary: A plugin to support golden tests with pytest.
 Home-page: https://github.com/nkartashov/goldie
 Author: Nick Kartashov
 Author-email: snailandmail@gmail.com
 Maintainer: Nick Kartashov
 Maintainer-email: snailandmail@gmail.com
 License: MIT
@@ -58,14 +58,15 @@
     def test_my_function(golden):
         output = my_function()
         golden.test(output)
 
 The `golden.test` method takes the output of your function and compares it to the saved output of a previous run. If the `update_goldens` flag is set, pytest-goldie will update the saved output with the new output.
 
 To run the tests and update goldens, use the following command:
+
 .. code-block:: bash
 
     $ pytest --update_goldens
 
 By default, the golden files are stored in a folder named 'goldens'. You can change the folder name with --goldens_folder flag:
 
 .. code-block:: bash
```

### Comparing `pytest-goldie-0.1.3/README.rst` & `pytest-goldie-0.1.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     def test_my_function(golden):
         output = my_function()
         golden.test(output)
 
 The `golden.test` method takes the output of your function and compares it to the saved output of a previous run. If the `update_goldens` flag is set, pytest-goldie will update the saved output with the new output.
 
 To run the tests and update goldens, use the following command:
+
 .. code-block:: bash
 
     $ pytest --update_goldens
 
 By default, the golden files are stored in a folder named 'goldens'. You can change the folder name with --goldens_folder flag:
 
 .. code-block:: bash
```

### Comparing `pytest-goldie-0.1.3/pytest_goldie/plugin.py` & `pytest-goldie-0.1.4/pytest_goldie/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-goldie-0.1.3/pytest_goldie.egg-info/PKG-INFO` & `pytest-goldie-0.1.4/pytest_goldie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-goldie
-Version: 0.1.3
+Version: 0.1.4
 Summary: A plugin to support golden tests with pytest.
 Home-page: https://github.com/nkartashov/goldie
 Author: Nick Kartashov
 Author-email: snailandmail@gmail.com
 Maintainer: Nick Kartashov
 Maintainer-email: snailandmail@gmail.com
 License: MIT
@@ -58,14 +58,15 @@
     def test_my_function(golden):
         output = my_function()
         golden.test(output)
 
 The `golden.test` method takes the output of your function and compares it to the saved output of a previous run. If the `update_goldens` flag is set, pytest-goldie will update the saved output with the new output.
 
 To run the tests and update goldens, use the following command:
+
 .. code-block:: bash
 
     $ pytest --update_goldens
 
 By default, the golden files are stored in a folder named 'goldens'. You can change the folder name with --goldens_folder flag:
 
 .. code-block:: bash
```

### Comparing `pytest-goldie-0.1.3/setup.py` & `pytest-goldie-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-goldie",
-    version="0.1.3",
+    version="0.1.4",
     author="Nick Kartashov",
     author_email="snailandmail@gmail.com",
     maintainer="Nick Kartashov",
     maintainer_email="snailandmail@gmail.com",
     license="MIT",
     url="https://github.com/nkartashov/goldie",
     repository="https://github.com/nkartashov/goldie",
```

### Comparing `pytest-goldie-0.1.3/tests/test_goldens.py` & `pytest-goldie-0.1.4/tests/test_goldens.py`

 * *Files identical despite different names*

