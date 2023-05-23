# Comparing `tmp/fetchify-1.0.3.tar.gz` & `tmp/fetchify-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchify-1.0.3.tar", last modified: Sat May 20 09:37:03 2023, max compression
+gzip compressed data, was "fetchify-1.0.4.tar", last modified: Mon May 22 14:00:01 2023, max compression
```

## Comparing `fetchify-1.0.3.tar` & `fetchify-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 09:37:03.095903 fetchify-1.0.3/
--rw-rw-rw-   0        0        0      594 2023-05-20 09:37:03.095903 fetchify-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 09:37:03.093902 fetchify-1.0.3/fetchify.egg-info/
--rw-rw-rw-   0        0        0      594 2023-05-20 09:37:02.000000 fetchify-1.0.3/fetchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-20 09:37:02.000000 fetchify-1.0.3/fetchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 09:37:02.000000 fetchify-1.0.3/fetchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 09:37:02.000000 fetchify-1.0.3/fetchify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 09:37:02.000000 fetchify-1.0.3/fetchify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1208 2023-05-19 11:55:57.000000 fetchify-1.0.3/fetchify.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 09:37:03.096900 fetchify-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-20 09:36:31.000000 fetchify-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:00:01.603223 fetchify-1.0.4/
+-rw-rw-rw-   0        0        0      594 2023-05-22 14:00:01.602221 fetchify-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 14:00:01.599730 fetchify-1.0.4/fetchify.egg-info/
+-rw-rw-rw-   0        0        0      594 2023-05-22 14:00:01.000000 fetchify-1.0.4/fetchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-22 14:00:01.000000 fetchify-1.0.4/fetchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:00:01.000000 fetchify-1.0.4/fetchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 14:00:01.000000 fetchify-1.0.4/fetchify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 14:00:01.000000 fetchify-1.0.4/fetchify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1332 2023-05-22 13:42:24.000000 fetchify-1.0.4/fetchify.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 14:00:01.604226 fetchify-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-05-22 13:59:39.000000 fetchify-1.0.4/setup.py
```

### Comparing `fetchify-1.0.3/PKG-INFO` & `fetchify-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.0.3/fetchify.egg-info/PKG-INFO` & `fetchify-1.0.4/fetchify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.0.3/fetchify.py` & `fetchify-1.0.4/fetchify.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,7 +28,11 @@
     page = requests.get(url4 + filename)
     return page.text
 
 def secure(filename):
     """To access files from the Repository 'SecuriPy'"""
     page = request.get(url + filename)
     return page.text
+
+def save(file, name):
+    with open(f"{name}", "w", encoding = "utf-8", newline = "") as f:
+        f.writelines(file)
```

### Comparing `fetchify-1.0.3/setup.py` & `fetchify-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fetchify",
-    version="1.0.3",
+    version="1.0.4",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library to access Code Files from Cloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
```

