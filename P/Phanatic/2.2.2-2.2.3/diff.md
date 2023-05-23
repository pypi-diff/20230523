# Comparing `tmp/Phanatic-2.2.2.tar.gz` & `tmp/Phanatic-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phanatic-2.2.2.tar", last modified: Sat May 20 02:21:44 2023, max compression
+gzip compressed data, was "Phanatic-2.2.3.tar", last modified: Tue May 23 10:06:39 2023, max compression
```

## Comparing `Phanatic-2.2.2.tar` & `Phanatic-2.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-20 02:21:44.763568 Phanatic-2.2.2/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)    34523 2023-05-20 02:11:07.000000 Phanatic-2.2.2/LICENSE.md
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-20 02:21:44.763568 Phanatic-2.2.2/PKG-INFO
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-20 02:21:44.763568 Phanatic-2.2.2/Phanatic/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-20 02:14:40.000000 Phanatic-2.2.2/Phanatic/__init__.py
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     4116 2023-05-20 02:14:41.000000 Phanatic-2.2.2/Phanatic/main.py
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-20 02:21:44.763568 Phanatic-2.2.2/Phanatic.egg-info/
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-20 02:21:44.000000 Phanatic-2.2.2/Phanatic.egg-info/PKG-INFO
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      251 2023-05-20 02:21:44.000000 Phanatic-2.2.2/Phanatic.egg-info/SOURCES.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        1 2023-05-20 02:21:44.000000 Phanatic-2.2.2/Phanatic.egg-info/dependency_links.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       51 2023-05-20 02:21:44.000000 Phanatic-2.2.2/Phanatic.egg-info/entry_points.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        7 2023-05-20 02:21:44.000000 Phanatic-2.2.2/Phanatic.egg-info/requires.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        9 2023-05-20 02:21:44.000000 Phanatic-2.2.2/Phanatic.egg-info/top_level.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       38 2023-05-20 02:21:44.763568 Phanatic-2.2.2/setup.cfg
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     1008 2023-05-20 02:14:45.000000 Phanatic-2.2.2/setup.py
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-23 10:06:39.862907 Phanatic-2.2.3/
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)    34523 2023-05-20 02:23:00.000000 Phanatic-2.2.3/LICENSE.md
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-23 10:06:39.862907 Phanatic-2.2.3/PKG-INFO
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-23 10:06:39.862907 Phanatic-2.2.3/Phanatic/
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-20 02:23:00.000000 Phanatic-2.2.3/Phanatic/__init__.py
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     4116 2023-05-23 10:03:17.000000 Phanatic-2.2.3/Phanatic/main.py
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-23 10:06:39.862907 Phanatic-2.2.3/Phanatic.egg-info/
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/PKG-INFO
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      251 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        1 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       51 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/entry_points.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        7 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/requires.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        9 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/top_level.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       38 2023-05-23 10:06:39.862907 Phanatic-2.2.3/setup.cfg
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     1008 2023-05-23 10:03:27.000000 Phanatic-2.2.3/setup.py
```

### Comparing `Phanatic-2.2.2/LICENSE.md` & `Phanatic-2.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Phanatic-2.2.2/PKG-INFO` & `Phanatic-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phanatic
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python package to run de novo bacteriophage assembly container.
 Home-page: https://github.com/JoshuaIszatt/Phanatic
 Author: Joshua Iszatt
 Author-email: joshiszatt@gmail.com
 License: AGPL-3.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Phanatic-2.2.2/Phanatic/main.py` & `Phanatic-2.2.3/Phanatic/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 f"{file_path} is not a valid file path")
         if not os.access(file_path, os.R_OK):
             raise argparse.ArgumentTypeError(
                 f"{file_path} is not a readable file")
         return file_path
 
     # Parsing arguments
-    image = 'iszatt/phanatic:2.2.2'
+    image = 'iszatt/phanatic:2.2.3'
     parser = argparse.ArgumentParser(description=f"Easy short read assembly. Joshua J Iszatt: https://github.com/JoshuaIszatt")
 
     # Input/output options
     parser.add_argument('-i', '--input', type=valid_dir, help='Input reads files')
     parser.add_argument('-o', '--output', type=valid_dir, help='Direct output to this location')
     parser.add_argument('-r', '--reads', type=str, choices=['PE_illumina_150'], default='PE_illumina_150', help='Pipeline options')
     parser.add_argument('-c', '--config', type=valid_file, help='Use config file to customise assembly')
```

### Comparing `Phanatic-2.2.2/Phanatic.egg-info/PKG-INFO` & `Phanatic-2.2.3/Phanatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phanatic
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python package to run de novo bacteriophage assembly container.
 Home-page: https://github.com/JoshuaIszatt/Phanatic
 Author: Joshua Iszatt
 Author-email: joshiszatt@gmail.com
 License: AGPL-3.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Phanatic-2.2.2/setup.py` & `Phanatic-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Phanatic",
-    version="2.2.2",
+    version="2.2.3",
     description="Python package to run de novo bacteriophage assembly container.",
     url="https://github.com/JoshuaIszatt/Phanatic",
     author="Joshua Iszatt",
     author_email="joshiszatt@gmail.com",
     license="AGPL-3.0",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

