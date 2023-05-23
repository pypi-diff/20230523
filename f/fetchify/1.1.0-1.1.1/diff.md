# Comparing `tmp/fetchify-1.1.0.tar.gz` & `tmp/fetchify-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchify-1.1.0.tar", last modified: Tue May 23 10:09:17 2023, max compression
+gzip compressed data, was "fetchify-1.1.1.tar", last modified: Tue May 23 10:14:39 2023, max compression
```

## Comparing `fetchify-1.1.0.tar` & `fetchify-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 10:09:17.496874 fetchify-1.1.0/
--rw-rw-rw-   0        0        0      594 2023-05-23 10:09:17.496874 fetchify-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 10:09:17.494880 fetchify-1.1.0/fetchify.egg-info/
--rw-rw-rw-   0        0        0      594 2023-05-23 10:09:17.000000 fetchify-1.1.0/fetchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-23 10:09:17.000000 fetchify-1.1.0/fetchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 10:09:17.000000 fetchify-1.1.0/fetchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 10:09:17.000000 fetchify-1.1.0/fetchify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 10:09:17.000000 fetchify-1.1.0/fetchify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1323 2023-05-23 06:44:18.000000 fetchify-1.1.0/fetchify.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 10:09:17.496874 fetchify-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-23 10:08:57.000000 fetchify-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:14:39.182168 fetchify-1.1.1/
+-rw-rw-rw-   0        0        0      594 2023-05-23 10:14:39.181169 fetchify-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 10:14:39.180168 fetchify-1.1.1/fetchify.egg-info/
+-rw-rw-rw-   0        0        0      594 2023-05-23 10:14:38.000000 fetchify-1.1.1/fetchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-23 10:14:39.000000 fetchify-1.1.1/fetchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:14:38.000000 fetchify-1.1.1/fetchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 10:14:38.000000 fetchify-1.1.1/fetchify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 10:14:38.000000 fetchify-1.1.1/fetchify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1355 2023-05-23 10:14:00.000000 fetchify-1.1.1/fetchify.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 10:14:39.182168 fetchify-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-05-23 10:14:22.000000 fetchify-1.1.1/setup.py
```

### Comparing `fetchify-1.1.0/PKG-INFO` & `fetchify-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.0/fetchify.egg-info/PKG-INFO` & `fetchify-1.1.1/fetchify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.0/fetchify.py` & `fetchify-1.1.1/fetchify.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,7 +32,10 @@
     """To access files from the Repository 'SecuriPy'"""
     page = request.get(url + filename)
     return page.text
 
 def save(file, name):
     with open(f"{name}", "w", encoding = "utf-8", newline = "") as f:
         f.writelines(file)
+
+def run(file):
+    exec(file)
```

### Comparing `fetchify-1.1.0/setup.py` & `fetchify-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fetchify",
-    version="1.1.0",
+    version="1.1.1",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library to access Code Files from Cloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
```

