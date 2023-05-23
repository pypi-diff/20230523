# Comparing `tmp/mysmallutils-2.0.2.tar.gz` & `tmp/mysmallutils-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysmallutils-2.0.2.tar", last modified: Tue Feb 14 12:11:36 2023, max compression
+gzip compressed data, was "mysmallutils-2.0.3.tar", last modified: Tue May 23 11:14:47 2023, max compression
```

## Comparing `mysmallutils-2.0.2.tar` & `mysmallutils-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 12:11:36.355822 mysmallutils-2.0.2/
--rw-rw-rw-   0        0        0    57504 2023-02-14 12:11:36.353983 mysmallutils-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    57022 2023-02-14 12:08:15.000000 mysmallutils-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-14 12:11:36.263277 mysmallutils-2.0.2/mysmallutils.egg-info/
--rw-rw-rw-   0        0        0    57504 2023-02-14 12:11:35.000000 mysmallutils-2.0.2/mysmallutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-02-14 12:11:36.000000 mysmallutils-2.0.2/mysmallutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 12:11:35.000000 mysmallutils-2.0.2/mysmallutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-14 12:11:35.000000 mysmallutils-2.0.2/mysmallutils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-14 12:11:36.348395 mysmallutils-2.0.2/mysutils/
--rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/__init__.py
--rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.2/mysutils/collections.py
--rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/command.py
--rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/config.py
--rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/fastapi.py
--rw-rw-rw-   0        0        0    25877 2023-02-13 14:44:23.000000 mysmallutils-2.0.2/mysutils/file.py
--rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/logging.py
--rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/method.py
--rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/misc.py
--rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/request.py
--rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/service.py
--rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.2/mysutils/tar.py
--rw-rw-rw-   0        0        0     7759 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/text.py
--rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.2/mysutils/tmp.py
--rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/unittest.py
--rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.2/mysutils/web.py
--rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.2/mysutils/yaml.py
--rw-rw-rw-   0        0        0       42 2023-02-14 12:11:36.355822 mysmallutils-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-02-14 11:45:36.000000 mysmallutils-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:14:47.331429 mysmallutils-2.0.3/
+-rw-rw-rw-   0        0        0    57504 2023-05-23 11:14:47.331429 mysmallutils-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    57022 2023-02-14 12:08:15.000000 mysmallutils-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 11:14:47.295476 mysmallutils-2.0.3/mysmallutils.egg-info/
+-rw-rw-rw-   0        0        0    57504 2023-05-23 11:14:47.000000 mysmallutils-2.0.3/mysmallutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-23 11:14:47.000000 mysmallutils-2.0.3/mysmallutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:14:47.000000 mysmallutils-2.0.3/mysmallutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 11:14:47.000000 mysmallutils-2.0.3/mysmallutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 11:14:47.327935 mysmallutils-2.0.3/mysutils/
+-rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/__init__.py
+-rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.3/mysutils/collections.py
+-rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/command.py
+-rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/config.py
+-rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/fastapi.py
+-rw-rw-rw-   0        0        0    25877 2023-02-13 14:44:23.000000 mysmallutils-2.0.3/mysutils/file.py
+-rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/logging.py
+-rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/method.py
+-rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/misc.py
+-rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/request.py
+-rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/service.py
+-rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.3/mysutils/tar.py
+-rw-rw-rw-   0        0        0     8671 2023-05-23 11:05:38.000000 mysmallutils-2.0.3/mysutils/text.py
+-rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.3/mysutils/tmp.py
+-rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/unittest.py
+-rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.3/mysutils/web.py
+-rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.3/mysutils/yaml.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 11:14:47.331429 mysmallutils-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1711 2023-05-23 11:06:53.000000 mysmallutils-2.0.3/setup.py
```

### Comparing `mysmallutils-2.0.2/PKG-INFO` & `mysmallutils-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.2
+Version: 2.0.3
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysmallutils-2.0.2/README.md` & `mysmallutils-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysmallutils.egg-info/PKG-INFO` & `mysmallutils-2.0.3/mysmallutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.2
+Version: 2.0.3
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysmallutils-2.0.2/mysutils/collections.py` & `mysmallutils-2.0.3/mysutils/collections.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/command.py` & `mysmallutils-2.0.3/mysutils/command.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/config.py` & `mysmallutils-2.0.3/mysutils/config.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/fastapi.py` & `mysmallutils-2.0.3/mysutils/fastapi.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/file.py` & `mysmallutils-2.0.3/mysutils/file.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/logging.py` & `mysmallutils-2.0.3/mysutils/logging.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/method.py` & `mysmallutils-2.0.3/mysutils/method.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/request.py` & `mysmallutils-2.0.3/mysutils/request.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/service.py` & `mysmallutils-2.0.3/mysutils/service.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/tar.py` & `mysmallutils-2.0.3/mysutils/tar.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/text.py` & `mysmallutils-2.0.3/mysutils/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,59 @@
 import re
 from enum import Enum, unique
-from typing import Union
+from re import Match
+from typing import Union, Iterator, List
 
 URL_PATTERN = r'[A-Za-z0-9]+://[A-Za-z0-9%-_]+(/[A-Za-z0-9%-_])*(#|\\?)[A-Za-z0-9%-_&=]*'
 
 
+def find_urls(text: str, end_with: str = '') -> Iterator[Match[str]]:
+    """ Find all the urls in the text.
+    :param text: The text to search in.
+    :param end_with: If set, only remove the URLs that finish with that regular expression.
+        By default, all the URLs are matched.
+    :return: An iterator over the url matches.
+    """
+    return re.finditer(URL_PATTERN + end_with, text)
+
+
+def get_urls(text: str, end_with: str = '') -> List[str]:
+    """ Get all the urls in the text.
+    :param text: The text to search in.
+    :param end_with: If set, only remove the URLs that finish with that regular expression.
+        By default, all the URLs are returned.
+    """
+    urls = []
+    for match in find_urls(text, end_with):
+        start, end = match.span()[0], match.span()[1]
+        urls.append(text[start:end])
+    return urls
+
+
 def remove_urls(text: str, end_with: str = '') -> str:
     """ Remove any url in the text.
 
     :param text: The text to remove urls.
     :param end_with: If set, only remove the URLs that finish with that regular expression.
-        By default, all the URLs are remvoed.
+        By default, all the URLs are removed.
     :return: The same text but without urls.
     """
     return replace_urls(text, '', end_with)
 
 
 def replace_urls(text: str, replace: str, end_with: str = '') -> str:
     """ Replace all the URLs with path by a text.
 
     :param text: The text to replace.
     :param replace: The text to replace with.
-    :param end_with: A regular expression which the URL has to finish with.
-         By default, replace all the URLs.
+    :param end_with: If set, only remove the URLs that finish with that regular expression.
+        By default, all the URLs are replaced.
     :return: The replaced text.
     """
-    matches = list(re.finditer(URL_PATTERN + end_with, text))
+    matches = list(find_urls(text, end_with))
     matches.reverse()
     for match in matches:
         start, end = match.span()[0], match.span()[1]
         text = text[:start] + replace + text[end:]
     return text
```

### Comparing `mysmallutils-2.0.2/mysutils/tmp.py` & `mysmallutils-2.0.3/mysutils/tmp.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/unittest.py` & `mysmallutils-2.0.3/mysutils/unittest.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/web.py` & `mysmallutils-2.0.3/mysutils/web.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/mysutils/yaml.py` & `mysmallutils-2.0.3/mysutils/yaml.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.2/setup.py` & `mysmallutils-2.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import glob
 import os
-from os.path import exists
 from shutil import rmtree
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
@@ -43,15 +42,15 @@
 
 setuptools.setup(
     cmdclass={
         'clean': CleanCommand,
         'prepublish': PrepublishCommand,
     },
     name='mysmallutils',
-    version='2.0.2',
+    version='2.0.3',
     url='https://github.com/jmgomezsoriano/mysmallutils',
     license='LGPL2',
     author='José Manuel Gómez Soriano',
     author_email='jmgomez.soriano@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='Small Python utils to do life easier.',
```

