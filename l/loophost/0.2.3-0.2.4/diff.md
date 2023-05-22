# Comparing `tmp/loophost-0.2.3.tar.gz` & `tmp/loophost-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loophost-0.2.3.tar", max compression
+gzip compressed data, was "loophost-0.2.4.tar", max compression
```

## Comparing `loophost-0.2.3.tar` & `loophost-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.3/README.md
--rw-r--r--   0        0        0        5 2023-05-22 22:47:48.370045 loophost-0.2.3/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.3/build.py
--rw-r--r--   0        0        0      669 2023-05-22 22:47:52.343228 loophost-0.2.3/loophost/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-22 20:58:52.834903 loophost-0.2.3/loophost/flingroute.py
--rw-r--r--   0        0        0     1021 2023-05-22 20:58:58.330155 loophost-0.2.3/loophost/launchd_plist.py
--rwxr-xr-x   0        0        0  8301536 2023-05-22 21:35:10.810528 loophost-0.2.3/loophost/loopproxy
--rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.3/loophost/plist/hub.plist.template
--rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.3/loophost/plist/loophost.plist.template
--rw-r--r--   0        0        0     1249 2023-05-22 22:47:19.211207 loophost-0.2.3/loophost/plist/ssh.plist.template
--rw-r--r--   0        0        0     3528 2023-05-22 20:59:10.162069 loophost-0.2.3/loophost/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.3/loophost/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.3/loophost/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.3/loophost/static/logo-hc.txt
--rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.3/loophost/static/logo-square.png
--rw-r--r--   0        0        0     1759 2023-05-22 18:09:46.308757 loophost-0.2.3/loophost/templates/admin.html
--rw-r--r--   0        0        0     2667 2023-05-21 23:39:30.263833 loophost-0.2.3/loophost/templates/local.html
--rw-r--r--   0        0        0     1476 2023-05-22 19:26:55.811597 loophost-0.2.3/loophost/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.3/loophost/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1167 2023-05-22 22:47:46.075713 loophost-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.3/setup.py
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 loophost-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.4/README.md
+-rw-r--r--   0        0        0        5 2023-05-22 23:04:39.071533 loophost-0.2.4/VERSION
+-rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.4/build.py
+-rw-r--r--   0        0        0      669 2023-05-22 23:04:47.713954 loophost-0.2.4/loophost/__init__.py
+-rw-r--r--   0        0        0     3370 2023-05-22 20:58:52.834903 loophost-0.2.4/loophost/flingroute.py
+-rw-r--r--   0        0        0     1021 2023-05-22 20:58:58.330155 loophost-0.2.4/loophost/launchd_plist.py
+-rwxr-xr-x   0        0        0  8301536 2023-05-22 21:35:10.810528 loophost-0.2.4/loophost/loopproxy
+-rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.4/loophost/plist/hub.plist.template
+-rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.4/loophost/plist/loophost.plist.template
+-rw-r--r--   0        0        0     1249 2023-05-22 22:47:19.211207 loophost-0.2.4/loophost/plist/ssh.plist.template
+-rw-r--r--   0        0        0     3532 2023-05-22 23:04:25.023331 loophost-0.2.4/loophost/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.4/loophost/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.4/loophost/static/fling-logo-light.png
+-rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.4/loophost/static/logo-hc.txt
+-rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.4/loophost/static/logo-square.png
+-rw-r--r--   0        0        0     1759 2023-05-22 18:09:46.308757 loophost-0.2.4/loophost/templates/admin.html
+-rw-r--r--   0        0        0     2667 2023-05-21 23:39:30.263833 loophost-0.2.4/loophost/templates/local.html
+-rw-r--r--   0        0        0     1476 2023-05-22 19:26:55.811597 loophost-0.2.4/loophost/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.4/loophost/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1167 2023-05-22 23:04:43.283435 loophost-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.4/setup.py
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 loophost-0.2.4/PKG-INFO
```

### Comparing `loophost-0.2.3/build.py` & `loophost-0.2.4/build.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/__init__.py` & `loophost-0.2.4/loophost/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 import os
 import pathlib
 import sys
 
 
 LOOPHOST_DOMAIN = "loophost.dev"
```

### Comparing `loophost-0.2.3/loophost/flingroute.py` & `loophost-0.2.4/loophost/flingroute.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/launchd_plist.py` & `loophost-0.2.4/loophost/launchd_plist.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/loopproxy` & `loophost-0.2.4/loophost/loopproxy`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/plist/hub.plist.template` & `loophost-0.2.4/loophost/plist/hub.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/plist/loophost.plist.template` & `loophost-0.2.4/loophost/plist/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/plist/ssh.plist.template` & `loophost-0.2.4/loophost/plist/ssh.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/postinstall.py` & `loophost-0.2.4/loophost/postinstall.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def post_install_one():
     print("Installing LoopHost...")
     os.makedirs(pathlib.Path(TARGET_DIR, "certs"), exist_ok=True)
     os.chdir(TARGET_DIR)
     with open("localuser.txt", "w+") as userfile:
-        userfile.write(os.getlogin())
+        userfile.write(os.getenv("USER"))
     authenticate_with_fling()
     issue_certs()
     create_update_loophost_json()
     register_tunnel(
         "flinghub",
         pathlib.Path(HUBDIR, "plist", "loophost.plist.template"),
         pathlib.Path(
```

### Comparing `loophost-0.2.3/loophost/static/fling-logo-dark.png` & `loophost-0.2.4/loophost/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/static/fling-logo-light.png` & `loophost-0.2.4/loophost/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/static/logo-hc.txt` & `loophost-0.2.4/loophost/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/static/logo-square.png` & `loophost-0.2.4/loophost/static/logo-square.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/templates/admin.html` & `loophost-0.2.4/loophost/templates/admin.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/templates/local.html` & `loophost-0.2.4/loophost/templates/local.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/loophost/templates/partials/apptable.html` & `loophost-0.2.4/loophost/templates/partials/apptable.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.3/pyproject.toml` & `loophost-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loophost"
-version = "0.2.3"
+version = "0.2.4"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 include = [{ path = "VERSION" },
```

### Comparing `loophost-0.2.3/PKG-INFO` & `loophost-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 0.2.3
+Version: 0.2.4
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

