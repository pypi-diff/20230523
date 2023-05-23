# Comparing `tmp/pytest-goldie-0.1.0.tar.gz` & `tmp/pytest-goldie-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-goldie-0.1.0.tar", last modified: Wed Apr 12 14:55:42 2023, max compression
+gzip compressed data, was "pytest-goldie-0.1.1.tar", last modified: Tue May 23 00:48:53 2023, max compression
```

## Comparing `pytest-goldie-0.1.0.tar` & `pytest-goldie-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-04-12 14:55:42.896037 pytest-goldie-0.1.0/
--rw-r--r--   0 nkartashov   (501) staff       (20)     1084 2023-03-28 22:22:38.000000 pytest-goldie-0.1.0/LICENSE
--rw-r--r--   0 nkartashov   (501) staff       (20)       97 2023-03-28 22:22:38.000000 pytest-goldie-0.1.0/MANIFEST.in
--rw-r--r--   0 nkartashov   (501) staff       (20)     3137 2023-04-12 14:55:42.895845 pytest-goldie-0.1.0/PKG-INFO
--rw-r--r--   0 nkartashov   (501) staff       (20)     2021 2023-03-28 22:22:38.000000 pytest-goldie-0.1.0/README.rst
--rw-r--r--   0 nkartashov   (501) staff       (20)      105 2023-04-12 14:50:25.000000 pytest-goldie-0.1.0/pyproject.toml
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-04-12 14:55:42.889712 pytest-goldie-0.1.0/pytest_goldie/
--rw-r--r--   0 nkartashov   (501) staff       (20)     2558 2023-04-12 12:52:47.000000 pytest-goldie-0.1.0/pytest_goldie/plugin.py
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-04-12 14:55:42.894927 pytest-goldie-0.1.0/pytest_goldie.egg-info/
--rw-r--r--   0 nkartashov   (501) staff       (20)     3137 2023-04-12 14:55:42.000000 pytest-goldie-0.1.0/pytest_goldie.egg-info/PKG-INFO
--rw-r--r--   0 nkartashov   (501) staff       (20)      345 2023-04-12 14:55:42.000000 pytest-goldie-0.1.0/pytest_goldie.egg-info/SOURCES.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)        1 2023-04-12 14:55:42.000000 pytest-goldie-0.1.0/pytest_goldie.egg-info/dependency_links.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       41 2023-04-12 14:55:42.000000 pytest-goldie-0.1.0/pytest_goldie.egg-info/entry_points.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-04-12 14:55:42.000000 pytest-goldie-0.1.0/pytest_goldie.egg-info/requires.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-04-12 14:55:42.000000 pytest-goldie-0.1.0/pytest_goldie.egg-info/top_level.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       38 2023-04-12 14:55:42.896081 pytest-goldie-0.1.0/setup.cfg
--rw-r--r--   0 nkartashov   (501) staff       (20)     1617 2023-03-28 22:22:38.000000 pytest-goldie-0.1.0/setup.py
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-04-12 14:55:42.895576 pytest-goldie-0.1.0/tests/
--rw-r--r--   0 nkartashov   (501) staff       (20)      586 2023-04-12 12:21:32.000000 pytest-goldie-0.1.0/tests/test_goldens.py
--rw-r--r--   0 nkartashov   (501) staff       (20)      320 2023-03-28 22:22:38.000000 pytest-goldie-0.1.0/tests/test_goldie.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 00:48:53.775361 pytest-goldie-0.1.1/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1084 2023-03-28 22:22:38.000000 pytest-goldie-0.1.1/LICENSE
+-rw-r--r--   0 nkartashov   (501) staff       (20)       97 2023-03-28 22:22:38.000000 pytest-goldie-0.1.1/MANIFEST.in
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2937 2023-05-23 00:48:53.775214 pytest-goldie-0.1.1/PKG-INFO
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1794 2023-05-23 00:46:08.000000 pytest-goldie-0.1.1/README.rst
+-rw-r--r--   0 nkartashov   (501) staff       (20)      105 2023-04-12 14:50:25.000000 pytest-goldie-0.1.1/pyproject.toml
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 00:48:53.774058 pytest-goldie-0.1.1/pytest_goldie/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2694 2023-04-24 20:31:20.000000 pytest-goldie-0.1.1/pytest_goldie/plugin.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 00:48:53.774791 pytest-goldie-0.1.1/pytest_goldie.egg-info/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2937 2023-05-23 00:48:53.000000 pytest-goldie-0.1.1/pytest_goldie.egg-info/PKG-INFO
+-rw-r--r--   0 nkartashov   (501) staff       (20)      345 2023-05-23 00:48:53.000000 pytest-goldie-0.1.1/pytest_goldie.egg-info/SOURCES.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)        1 2023-05-23 00:48:53.000000 pytest-goldie-0.1.1/pytest_goldie.egg-info/dependency_links.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       41 2023-05-23 00:48:53.000000 pytest-goldie-0.1.1/pytest_goldie.egg-info/entry_points.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 00:48:53.000000 pytest-goldie-0.1.1/pytest_goldie.egg-info/requires.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 00:48:53.000000 pytest-goldie-0.1.1/pytest_goldie.egg-info/top_level.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       38 2023-05-23 00:48:53.775407 pytest-goldie-0.1.1/setup.cfg
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1709 2023-05-23 00:48:24.000000 pytest-goldie-0.1.1/setup.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 00:48:53.775052 pytest-goldie-0.1.1/tests/
+-rw-r--r--   0 nkartashov   (501) staff       (20)      586 2023-04-12 12:21:32.000000 pytest-goldie-0.1.1/tests/test_goldens.py
+-rw-r--r--   0 nkartashov   (501) staff       (20)      320 2023-03-28 22:22:38.000000 pytest-goldie-0.1.1/tests/test_goldie.py
```

### Comparing `pytest-goldie-0.1.0/LICENSE` & `pytest-goldie-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-goldie-0.1.0/pytest_goldie/plugin.py` & `pytest-goldie-0.1.1/pytest_goldie/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         return self.test_file_path.name + "-" + self.test_name
 
     @property
     def _golden_path(self) -> Path:
         return self._golden_dir / self._golden_filename
 
     def test(self, output):
+        """Compare the given test output to the saved one. If the fixture has `update_goldens` set, updates the saved data instead."""
+
         if isinstance(output, bytes):
             return self._test(output, is_binary=True)
 
         if isinstance(output, str):
             return self._test(output, is_binary=False)
 
         return self._test(json.dumps(output, sort_keys=True, indent=2), is_binary=False)
```

### Comparing `pytest-goldie-0.1.0/setup.py` & `pytest-goldie-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-goldie",
-    version="0.1.0",
-    author="Nikita Kartashov",
+    version="0.1.1",
+    author="Nick Kartashov",
     author_email="snailandmail@gmail.com",
-    maintainer="Nikita Kartashov",
+    maintainer="Nick Kartashov",
     maintainer_email="snailandmail@gmail.com",
     license="MIT",
-    url="https://github.com/nkartashov/pytest-goldie",
+    url="https://github.com/nkartashov/goldie",
+    repository="https://github.com/nkartashov/goldie",
     description="A plugin to support golden tests with pytest.",
     long_description=read("README.rst"),
+    long_description_content_type="text/x-rst",
     py_modules=["pytest_goldie.plugin"],
     python_requires=">=3.5",
     install_requires=["pytest>=3.5.0"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
```

### Comparing `pytest-goldie-0.1.0/tests/test_goldens.py` & `pytest-goldie-0.1.1/tests/test_goldens.py`

 * *Files identical despite different names*

