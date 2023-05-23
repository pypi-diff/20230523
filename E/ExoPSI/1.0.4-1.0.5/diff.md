# Comparing `tmp/ExoPSI-1.0.4.tar.gz` & `tmp/ExoPSI-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExoPSI-1.0.4.tar", last modified: Mon Apr 17 18:50:26 2023, max compression
+gzip compressed data, was "ExoPSI-1.0.5.tar", last modified: Tue May 23 07:43:29 2023, max compression
```

## Comparing `ExoPSI-1.0.4.tar` & `ExoPSI-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 18:50:26.301625 ExoPSI-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-04-17 18:50:26.210859 ExoPSI-1.0.4/ExoPSI/
--rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.4/ExoPSI/__init__.py
--rw-rw-rw-   0        0        0     8371 2023-04-17 18:45:19.000000 ExoPSI-1.0.4/ExoPSI/exopsi.py
--rw-rw-rw-   0        0        0     1916 2023-04-17 18:43:49.000000 ExoPSI-1.0.4/ExoPSI/subfunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:50:26.295998 ExoPSI-1.0.4/ExoPSI.egg-info/
--rw-rw-rw-   0        0        0     6734 2023-04-17 18:50:25.000000 ExoPSI-1.0.4/ExoPSI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-17 18:50:26.000000 ExoPSI-1.0.4/ExoPSI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 18:50:25.000000 ExoPSI-1.0.4/ExoPSI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 18:50:25.000000 ExoPSI-1.0.4/ExoPSI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 18:50:25.000000 ExoPSI-1.0.4/ExoPSI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     6734 2023-04-17 18:50:26.300615 ExoPSI-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-04-13 17:19:38.000000 ExoPSI-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 18:50:26.301625 ExoPSI-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1417 2023-04-17 18:47:58.000000 ExoPSI-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:43:29.813613 ExoPSI-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-23 07:43:29.791101 ExoPSI-1.0.5/ExoPSI/
+-rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.5/ExoPSI/__init__.py
+-rw-rw-rw-   0        0        0     8371 2023-04-17 18:45:19.000000 ExoPSI-1.0.5/ExoPSI/exopsi.py
+-rw-rw-rw-   0        0        0     1916 2023-04-17 18:43:49.000000 ExoPSI-1.0.5/ExoPSI/subfunctions.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:43:29.805632 ExoPSI-1.0.5/ExoPSI.egg-info/
+-rw-rw-rw-   0        0        0     6754 2023-05-23 07:43:29.000000 ExoPSI-1.0.5/ExoPSI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-23 07:43:29.000000 ExoPSI-1.0.5/ExoPSI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:43:29.000000 ExoPSI-1.0.5/ExoPSI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-23 07:43:29.000000 ExoPSI-1.0.5/ExoPSI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 07:43:29.000000 ExoPSI-1.0.5/ExoPSI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     6754 2023-05-23 07:43:29.813613 ExoPSI-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-04-13 17:19:38.000000 ExoPSI-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:43:29.813613 ExoPSI-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1436 2023-05-23 07:40:08.000000 ExoPSI-1.0.5/setup.py
```

### Comparing `ExoPSI-1.0.4/ExoPSI/exopsi.py` & `ExoPSI-1.0.5/ExoPSI/exopsi.py`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.4/ExoPSI/subfunctions.py` & `ExoPSI-1.0.5/ExoPSI/subfunctions.py`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.4/ExoPSI.egg-info/PKG-INFO` & `ExoPSI-1.0.5/ExoPSI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ExoPSI
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to calculate Planet Similarity Indexes
 Home-page: https://github.com/ExoPSI/ExoPSI
-Author: ['Aditya Rai', 'Vaibhav Garg']
+Author: ['Aditya Rai', 'Vaibhav Garg', 'Divya Srinivasan']
 Author-email: rai.aditya01@gmail.com
 License: GNU GPL v3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ExoPSI-1.0.4/LICENSE` & `ExoPSI-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.4/PKG-INFO` & `ExoPSI-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ExoPSI
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to calculate Planet Similarity Indexes
 Home-page: https://github.com/ExoPSI/ExoPSI
-Author: ['Aditya Rai', 'Vaibhav Garg']
+Author: ['Aditya Rai', 'Vaibhav Garg', 'Divya Srinivasan']
 Author-email: rai.aditya01@gmail.com
 License: GNU GPL v3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ExoPSI-1.0.4/README.md` & `ExoPSI-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.4/setup.py` & `ExoPSI-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ExoPSI",
-    version="1.0.4",
+    version="1.0.5",
     description="Library to calculate Planet Similarity Indexes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ExoPSI/ExoPSI",
-    author=["Aditya Rai","Vaibhav Garg"],
+    author=["Aditya Rai","Vaibhav Garg","Divya Srinivasan"],
     author_email="rai.aditya01@gmail.com",
     license="GNU GPL v3.0", 
     classifiers=[
         "Intended Audience :: Developers",  
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

