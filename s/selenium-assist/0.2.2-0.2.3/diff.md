# Comparing `tmp/selenium_assist-0.2.2.tar.gz` & `tmp/selenium_assist-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_assist-0.2.2.tar", last modified: Wed May 17 21:18:52 2023, max compression
+gzip compressed data, was "selenium_assist-0.2.3.tar", last modified: Tue May 23 13:23:54 2023, max compression
```

## Comparing `selenium_assist-0.2.2.tar` & `selenium_assist-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/
--rw-rw-r--   0 mich      (1000) mich      (1000)     1071 2023-04-05 22:02:25.000000 selenium_assist-0.2.2/LICENSE
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)       71 2023-05-12 23:13:38.000000 selenium_assist-0.2.2/README.md
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-17 21:18:52.576188 selenium_assist-0.2.2/selenium_assist/
--rw-rw-r--   0 mich      (1000) mich      (1000)      458 2023-05-12 23:13:37.000000 selenium_assist-0.2.2/selenium_assist/__init__.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     1048 2023-04-05 22:44:18.000000 selenium_assist-0.2.2/selenium_assist/helpers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     1125 2023-05-17 20:55:52.000000 selenium_assist-0.2.2/selenium_assist/managers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     3847 2023-05-12 23:13:37.000000 selenium_assist-0.2.2/selenium_assist/wrappers.py
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/selenium_assist.egg-info/
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)      341 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/SOURCES.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)        1 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/dependency_links.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       39 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/requires.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       16 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/top_level.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       79 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/setup.cfg
--rw-rw-r--   0 mich      (1000) mich      (1000)     1097 2023-05-17 20:55:52.000000 selenium_assist-0.2.2/setup.py
+drwxrwxr-x   0 mich      (1001) mich      (1001)        0 2023-05-23 13:23:54.804198 selenium_assist-0.2.3/
+-rw-rw-r--   0 mich      (1001) mich      (1001)     1071 2023-05-23 12:38:43.000000 selenium_assist-0.2.3/LICENSE
+-rw-rw-r--   0 mich      (1001) mich      (1001)      831 2023-05-23 13:23:54.804198 selenium_assist-0.2.3/PKG-INFO
+-rw-rw-r--   0 mich      (1001) mich      (1001)       71 2023-05-23 12:38:43.000000 selenium_assist-0.2.3/README.md
+drwxrwxr-x   0 mich      (1001) mich      (1001)        0 2023-05-23 13:23:54.804198 selenium_assist-0.2.3/selenium_assist/
+-rw-rw-r--   0 mich      (1001) mich      (1001)      458 2023-05-23 12:38:43.000000 selenium_assist-0.2.3/selenium_assist/__init__.py
+-rw-rw-r--   0 mich      (1001) mich      (1001)     1183 2023-05-23 12:47:31.000000 selenium_assist-0.2.3/selenium_assist/helpers.py
+-rw-rw-r--   0 mich      (1001) mich      (1001)     1125 2023-05-23 12:38:43.000000 selenium_assist-0.2.3/selenium_assist/managers.py
+-rw-rw-r--   0 mich      (1001) mich      (1001)     3847 2023-05-23 12:38:43.000000 selenium_assist-0.2.3/selenium_assist/wrappers.py
+drwxrwxr-x   0 mich      (1001) mich      (1001)        0 2023-05-23 13:23:54.804198 selenium_assist-0.2.3/selenium_assist.egg-info/
+-rw-rw-r--   0 mich      (1001) mich      (1001)      831 2023-05-23 13:23:54.000000 selenium_assist-0.2.3/selenium_assist.egg-info/PKG-INFO
+-rw-rw-r--   0 mich      (1001) mich      (1001)      341 2023-05-23 13:23:54.000000 selenium_assist-0.2.3/selenium_assist.egg-info/SOURCES.txt
+-rw-rw-r--   0 mich      (1001) mich      (1001)        1 2023-05-23 13:23:54.000000 selenium_assist-0.2.3/selenium_assist.egg-info/dependency_links.txt
+-rw-rw-r--   0 mich      (1001) mich      (1001)       39 2023-05-23 13:23:54.000000 selenium_assist-0.2.3/selenium_assist.egg-info/requires.txt
+-rw-rw-r--   0 mich      (1001) mich      (1001)       16 2023-05-23 13:23:54.000000 selenium_assist-0.2.3/selenium_assist.egg-info/top_level.txt
+-rw-rw-r--   0 mich      (1001) mich      (1001)       79 2023-05-23 13:23:54.804198 selenium_assist-0.2.3/setup.cfg
+-rw-rw-r--   0 mich      (1001) mich      (1001)     1097 2023-05-23 12:47:31.000000 selenium_assist-0.2.3/setup.py
```

### Comparing `selenium_assist-0.2.2/LICENSE` & `selenium_assist-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.2/PKG-INFO` & `selenium_assist-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium_assist
-Version: 0.2.2
+Version: 0.2.3
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.2.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.3.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.2/selenium_assist/helpers.py` & `selenium_assist-0.2.3/selenium_assist/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+import sys
 import os
 import logging
 import time
 import datetime
 from pathlib import Path
 
 
 def cleanup():
     logging.debug("Cleaning up ...")
     pass
     return
 
 
 def save_screenshot(filename, driver):
-    fn = os.path.join(os.path.dirname(os.path.realpath(__file__)), filename)
+    try:
+        main_file = str(sys.modules['__main__'].__file__)
+    except AttributeError:
+        main_file = __file__
+    fn = os.path.join(os.path.dirname(os.path.realpath(main_file)), filename)
     logging.info(f"Saving screenshot {fn} ...")
     if os.path.exists(fn):
         os.remove(fn)
     driver.save_screenshot(fn)
     return
```

### Comparing `selenium_assist-0.2.2/selenium_assist/managers.py` & `selenium_assist-0.2.3/selenium_assist/managers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.2/selenium_assist/wrappers.py` & `selenium_assist-0.2.3/selenium_assist/wrappers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.2/selenium_assist.egg-info/PKG-INFO` & `selenium_assist-0.2.3/selenium_assist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium-assist
-Version: 0.2.2
+Version: 0.2.3
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.2.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.3.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.2/setup.py` & `selenium_assist-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium_assist",
-    version="0.2.2",
+    version="0.2.3",
     author="Ivan Mičetić",
     author_email="ivan.micetic@gmail.com",
     description="Helper functions for selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ivanmicetic/selenium-assist",
     project_urls={
@@ -22,9 +22,9 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
-    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.2.tar.gz"
+    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.3.tar.gz"
 )
```

