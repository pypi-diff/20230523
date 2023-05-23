# Comparing `tmp/nefila-0.0.4.dev0.tar.gz` & `tmp/nefila-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nefila-0.0.4.dev0.tar", last modified: Thu Sep 10 20:42:22 2020, max compression
+gzip compressed data, was "dist/nefila-0.0.5.tar", last modified: Tue May 23 14:33:25 2023, max compression
```

## Comparing `nefila-0.0.4.dev0.tar` & `nefila-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/nefila.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      639 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/nefila.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/nefila.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/nefila.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      541 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/nefila.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/nefila.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      639 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1651 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/nefila/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5906 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/fortiswitch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4764 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/fortiManagerAnalyzerCore.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2398 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/fortimanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6046 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/modelmeta.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5162 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/fortianalyzer.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15597 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/fortigate.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3136 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6273 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/fortitester.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1597 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/nefila/forticare.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      800 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-10 20:42:22.000000 nefila-0.0.4.dev0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3669 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/tests/test_fortiswitch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1421 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/tests/test_fortimanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4581 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/tests/test_fortigate.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1537 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/tests/test_utils.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3344 2020-09-10 20:41:29.000000 nefila-0.0.4.dev0/tests/test_fortianalyzer.py
+drwxr-xr-x   0 mbarbosa   (501) staff       (20)        0 2023-05-23 14:33:25.000000 nefila-0.0.5/
+-rw-r--r--   0 mbarbosa   (501) staff       (20)    35149 2019-09-24 02:59:43.000000 nefila-0.0.5/LICENSE
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     2309 2023-05-23 14:33:25.000000 nefila-0.0.5/PKG-INFO
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     1651 2023-05-23 13:01:30.000000 nefila-0.0.5/README.md
+drwxr-xr-x   0 mbarbosa   (501) staff       (20)        0 2023-05-23 14:33:25.000000 nefila-0.0.5/nefila/
+-rw-r--r--   0 mbarbosa   (501) staff       (20)      187 2019-11-14 15:27:52.000000 nefila-0.0.5/nefila/__init__.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     4764 2019-12-17 14:35:54.000000 nefila-0.0.5/nefila/fortiManagerAnalyzerCore.py
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)     5162 2019-11-07 22:46:23.000000 nefila-0.0.5/nefila/fortianalyzer.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     1597 2023-05-23 13:01:30.000000 nefila-0.0.5/nefila/forticare.py
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)    15660 2023-05-23 13:01:30.000000 nefila-0.0.5/nefila/fortigate.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     2398 2019-12-17 14:35:54.000000 nefila-0.0.5/nefila/fortimanager.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     5906 2020-01-14 16:53:09.000000 nefila-0.0.5/nefila/fortiswitch.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     6273 2023-05-23 13:01:30.000000 nefila-0.0.5/nefila/fortitester.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     6046 2023-05-23 13:01:30.000000 nefila-0.0.5/nefila/modelmeta.py
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)     3136 2019-12-17 14:35:54.000000 nefila-0.0.5/nefila/utils.py
+drwxr-xr-x   0 mbarbosa   (501) staff       (20)        0 2023-05-23 14:33:25.000000 nefila-0.0.5/nefila.egg-info/
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)     2309 2023-05-23 14:33:25.000000 nefila-0.0.5/nefila.egg-info/PKG-INFO
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)      549 2023-05-23 14:33:25.000000 nefila-0.0.5/nefila.egg-info/SOURCES.txt
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)        1 2023-05-23 14:33:25.000000 nefila-0.0.5/nefila.egg-info/dependency_links.txt
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)       28 2023-05-23 14:33:25.000000 nefila-0.0.5/nefila.egg-info/requires.txt
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)       13 2023-05-23 14:33:25.000000 nefila-0.0.5/nefila.egg-info/top_level.txt
+-rw-r--r--   0 mbarbosa   (501) staff       (20)       79 2023-05-23 14:33:25.000000 nefila-0.0.5/setup.cfg
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     1052 2023-05-23 14:28:19.000000 nefila-0.0.5/setup.py
+drwxr-xr-x   0 mbarbosa   (501) staff       (20)        0 2023-05-23 14:33:25.000000 nefila-0.0.5/tests/
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)        0 2023-05-23 13:01:30.000000 nefila-0.0.5/tests/__init__.py
+-rwxr-xr-x   0 mbarbosa   (501) staff       (20)     3344 2019-11-08 18:40:32.000000 nefila-0.0.5/tests/test_fortianalyzer.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     4581 2019-12-17 14:35:54.000000 nefila-0.0.5/tests/test_fortigate.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     1421 2019-12-17 14:35:54.000000 nefila-0.0.5/tests/test_fortimanager.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     3669 2020-01-14 16:53:09.000000 nefila-0.0.5/tests/test_fortiswitch.py
+-rw-r--r--   0 mbarbosa   (501) staff       (20)     1537 2019-11-07 22:11:24.000000 nefila-0.0.5/tests/test_utils.py
```

### Comparing `nefila-0.0.4.dev0/nefila.egg-info/SOURCES.txt` & `nefila-0.0.5/nefila.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 nefila/__init__.py
 nefila/fortiManagerAnalyzerCore.py
 nefila/fortianalyzer.py
 nefila/forticare.py
```

### Comparing `nefila-0.0.4.dev0/README.md` & `nefila-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/fortiswitch.py` & `nefila-0.0.5/nefila/fortiswitch.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/fortiManagerAnalyzerCore.py` & `nefila-0.0.5/nefila/fortiManagerAnalyzerCore.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/fortimanager.py` & `nefila-0.0.5/nefila/fortimanager.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/modelmeta.py` & `nefila-0.0.5/nefila/modelmeta.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/fortianalyzer.py` & `nefila-0.0.5/nefila/fortianalyzer.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/fortigate.py` & `nefila-0.0.5/nefila/fortigate.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,18 @@
         url_login = f'https://{self.hostname}/logincheck'
 
         if not token:
             self.session.post(url=url_login,
                             data=f'username={username}&secretkey={password}',
                             timeout = self.timeout,
             )
-            csrftoken = self.session.cookies['ccsrftoken']
-            csrftoken = csrftoken[1:-1]
-            self.session.headers.update({'X-CSRFTOKEN': csrftoken})
+            for cookie in self.session.cookies:
+                if "ccsrftoken" in cookie.name:
+                    csrftoken = cookie.value[1:-1]
+                    self.session.headers.update({'X-CSRFTOKEN': csrftoken})       
 
         else:
             self.session.headers.update({'Authorization': f'Bearer {token}'})
             self.token = True
         
         # Call to license status during login to auto set device details
         r = self.license_status()
```

### Comparing `nefila-0.0.4.dev0/nefila/utils.py` & `nefila-0.0.5/nefila/utils.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/fortitester.py` & `nefila-0.0.5/nefila/fortitester.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/nefila/forticare.py` & `nefila-0.0.5/nefila/forticare.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/setup.py` & `nefila-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from setuptools import setup, find_packages
 
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
     name="nefila",
     packages=find_packages(),
-    version="0.0.4.dev0",
+    version="0.0.5",
     license="GPL-3",
     description="Nefila is an elegant and simple Fortinet Security Fabric library for Python.",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author="Michel Barbosa",
     author_email="nefila@deadpackets.io",
     url="https://github.com/mbdraks/nefila",
     download_url="https://github.com/mbdraks/nefila/archive/v0.0.4.tar.gz",
     keywords=["fortinet", "fortigate", "security fabric"],
     install_requires=["requests", "requests[security]"],
     classifiers=[
```

### Comparing `nefila-0.0.4.dev0/tests/test_fortiswitch.py` & `nefila-0.0.5/tests/test_fortiswitch.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/tests/test_fortimanager.py` & `nefila-0.0.5/tests/test_fortimanager.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/tests/test_fortigate.py` & `nefila-0.0.5/tests/test_fortigate.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/tests/test_utils.py` & `nefila-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nefila-0.0.4.dev0/tests/test_fortianalyzer.py` & `nefila-0.0.5/tests/test_fortianalyzer.py`

 * *Files identical despite different names*

