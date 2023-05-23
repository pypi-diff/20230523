# Comparing `tmp/pytest-goldie-0.1.4.tar.gz` & `tmp/pytest-goldie-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-goldie-0.1.4.tar", last modified: Tue May 23 01:06:14 2023, max compression
+gzip compressed data, was "pytest-goldie-0.1.5.tar", last modified: Tue May 23 10:43:58 2023, max compression
```

## Comparing `pytest-goldie-0.1.4.tar` & `pytest-goldie-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.146624 pytest-goldie-0.1.4/
--rw-r--r--   0 nkartashov   (501) staff       (20)     1084 2023-03-28 22:22:38.000000 pytest-goldie-0.1.4/LICENSE
--rw-r--r--   0 nkartashov   (501) staff       (20)       97 2023-03-28 22:22:38.000000 pytest-goldie-0.1.4/MANIFEST.in
--rw-r--r--   0 nkartashov   (501) staff       (20)     2920 2023-05-23 01:06:14.146474 pytest-goldie-0.1.4/PKG-INFO
--rw-r--r--   0 nkartashov   (501) staff       (20)     1777 2023-05-23 01:05:57.000000 pytest-goldie-0.1.4/README.rst
--rw-r--r--   0 nkartashov   (501) staff       (20)      105 2023-04-12 14:50:25.000000 pytest-goldie-0.1.4/pyproject.toml
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.145429 pytest-goldie-0.1.4/pytest_goldie/
--rw-r--r--   0 nkartashov   (501) staff       (20)     2694 2023-04-24 20:31:20.000000 pytest-goldie-0.1.4/pytest_goldie/plugin.py
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.146076 pytest-goldie-0.1.4/pytest_goldie.egg-info/
--rw-r--r--   0 nkartashov   (501) staff       (20)     2920 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/PKG-INFO
--rw-r--r--   0 nkartashov   (501) staff       (20)      345 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/SOURCES.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)        1 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/dependency_links.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       41 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/entry_points.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/requires.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 01:06:14.000000 pytest-goldie-0.1.4/pytest_goldie.egg-info/top_level.txt
--rw-r--r--   0 nkartashov   (501) staff       (20)       38 2023-05-23 01:06:14.146665 pytest-goldie-0.1.4/setup.cfg
--rw-r--r--   0 nkartashov   (501) staff       (20)     1709 2023-05-23 01:06:09.000000 pytest-goldie-0.1.4/setup.py
-drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 01:06:14.146298 pytest-goldie-0.1.4/tests/
--rw-r--r--   0 nkartashov   (501) staff       (20)      586 2023-04-12 12:21:32.000000 pytest-goldie-0.1.4/tests/test_goldens.py
--rw-r--r--   0 nkartashov   (501) staff       (20)      320 2023-03-28 22:22:38.000000 pytest-goldie-0.1.4/tests/test_goldie.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 10:43:58.824122 pytest-goldie-0.1.5/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1084 2023-03-28 22:22:38.000000 pytest-goldie-0.1.5/LICENSE
+-rw-r--r--   0 nkartashov   (501) staff       (20)       97 2023-03-28 22:22:38.000000 pytest-goldie-0.1.5/MANIFEST.in
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2920 2023-05-23 10:43:58.823988 pytest-goldie-0.1.5/PKG-INFO
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1777 2023-05-23 01:05:57.000000 pytest-goldie-0.1.5/README.rst
+-rw-r--r--   0 nkartashov   (501) staff       (20)      105 2023-04-12 14:50:25.000000 pytest-goldie-0.1.5/pyproject.toml
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 10:43:58.822939 pytest-goldie-0.1.5/pytest_goldie/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2664 2023-05-23 10:43:33.000000 pytest-goldie-0.1.5/pytest_goldie/plugin.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 10:43:58.823589 pytest-goldie-0.1.5/pytest_goldie.egg-info/
+-rw-r--r--   0 nkartashov   (501) staff       (20)     2920 2023-05-23 10:43:58.000000 pytest-goldie-0.1.5/pytest_goldie.egg-info/PKG-INFO
+-rw-r--r--   0 nkartashov   (501) staff       (20)      345 2023-05-23 10:43:58.000000 pytest-goldie-0.1.5/pytest_goldie.egg-info/SOURCES.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)        1 2023-05-23 10:43:58.000000 pytest-goldie-0.1.5/pytest_goldie.egg-info/dependency_links.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       41 2023-05-23 10:43:58.000000 pytest-goldie-0.1.5/pytest_goldie.egg-info/entry_points.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 10:43:58.000000 pytest-goldie-0.1.5/pytest_goldie.egg-info/requires.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       14 2023-05-23 10:43:58.000000 pytest-goldie-0.1.5/pytest_goldie.egg-info/top_level.txt
+-rw-r--r--   0 nkartashov   (501) staff       (20)       38 2023-05-23 10:43:58.824159 pytest-goldie-0.1.5/setup.cfg
+-rw-r--r--   0 nkartashov   (501) staff       (20)     1709 2023-05-23 10:43:48.000000 pytest-goldie-0.1.5/setup.py
+drwxr-xr-x   0 nkartashov   (501) staff       (20)        0 2023-05-23 10:43:58.823831 pytest-goldie-0.1.5/tests/
+-rw-r--r--   0 nkartashov   (501) staff       (20)      586 2023-04-12 12:21:32.000000 pytest-goldie-0.1.5/tests/test_goldens.py
+-rw-r--r--   0 nkartashov   (501) staff       (20)      320 2023-03-28 22:22:38.000000 pytest-goldie-0.1.5/tests/test_goldie.py
```

### Comparing `pytest-goldie-0.1.4/LICENSE` & `pytest-goldie-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-goldie-0.1.4/PKG-INFO` & `pytest-goldie-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-goldie
-Version: 0.1.4
+Version: 0.1.5
 Summary: A plugin to support golden tests with pytest.
 Home-page: https://github.com/nkartashov/goldie
 Author: Nick Kartashov
 Author-email: snailandmail@gmail.com
 Maintainer: Nick Kartashov
 Maintainer-email: snailandmail@gmail.com
 License: MIT
```

### Comparing `pytest-goldie-0.1.4/README.rst` & `pytest-goldie-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-goldie-0.1.4/pytest_goldie/plugin.py` & `pytest-goldie-0.1.5/pytest_goldie/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,31 @@
         "--update_goldens",
         action="store_true",
         dest="update_goldens",
         default=False,
         help="Update golden files.",
     )
     group.addoption(
-        "--goldens_folder_name",
-        dest="goldens_folder_name",
+        "--goldens_folder",
+        dest="goldens_folder",
         default="goldens",
         help="Goldens folder name.",
     )
 
 
 @dataclasses.dataclass
 class GoldieFixture:
     update_goldens: bool
-    goldens_folder_name: str
+    goldens_folder: str
     test_file_path: Path
     test_name: str
 
     @property
     def _golden_dir(self) -> Path:
-        return self.test_file_path.parent / self.goldens_folder_name
+        return self.test_file_path.parent / self.goldens_folder
 
     @property
     def _golden_filename(self) -> str:
         return self.test_file_path.name + "-" + self.test_name
 
     @property
     def _golden_path(self) -> Path:
@@ -80,11 +80,11 @@
             )
 
 
 @pytest.fixture(scope="function")
 def golden(request):
     yield GoldieFixture(
         update_goldens=request.config.getoption("update_goldens"),
-        goldens_folder_name=request.config.getoption("goldens_folder_name"),
+        goldens_folder=request.config.getoption("goldens_folder"),
         test_file_path=Path(request.node.fspath),
         test_name=request.node.name,
     )
```

### Comparing `pytest-goldie-0.1.4/pytest_goldie.egg-info/PKG-INFO` & `pytest-goldie-0.1.5/pytest_goldie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-goldie
-Version: 0.1.4
+Version: 0.1.5
 Summary: A plugin to support golden tests with pytest.
 Home-page: https://github.com/nkartashov/goldie
 Author: Nick Kartashov
 Author-email: snailandmail@gmail.com
 Maintainer: Nick Kartashov
 Maintainer-email: snailandmail@gmail.com
 License: MIT
```

### Comparing `pytest-goldie-0.1.4/setup.py` & `pytest-goldie-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-goldie",
-    version="0.1.4",
+    version="0.1.5",
     author="Nick Kartashov",
     author_email="snailandmail@gmail.com",
     maintainer="Nick Kartashov",
     maintainer_email="snailandmail@gmail.com",
     license="MIT",
     url="https://github.com/nkartashov/goldie",
     repository="https://github.com/nkartashov/goldie",
```

### Comparing `pytest-goldie-0.1.4/tests/test_goldens.py` & `pytest-goldie-0.1.5/tests/test_goldens.py`

 * *Files identical despite different names*

