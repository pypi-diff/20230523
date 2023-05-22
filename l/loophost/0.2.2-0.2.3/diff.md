# Comparing `tmp/loophost-0.2.2.tar.gz` & `tmp/loophost-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loophost-0.2.2.tar", max compression
+gzip compressed data, was "loophost-0.2.3.tar", max compression
```

## Comparing `loophost-0.2.2.tar` & `loophost-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.2/README.md
--rw-r--r--   0        0        0        5 2023-05-22 21:35:35.923087 loophost-0.2.2/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.2/build.py
--rw-r--r--   0        0        0      669 2023-05-22 21:35:41.188616 loophost-0.2.2/loophost/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-22 20:58:52.834903 loophost-0.2.2/loophost/flingroute.py
--rw-r--r--   0        0        0     1021 2023-05-22 20:58:58.330155 loophost-0.2.2/loophost/launchd_plist.py
--rwxr-xr-x   0        0        0  8301536 2023-05-22 21:35:10.810528 loophost-0.2.2/loophost/loopproxy
--rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.2/loophost/plist/hub.plist.template
--rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.2/loophost/plist/loophost.plist.template
--rw-r--r--   0        0        0     1251 2023-05-22 17:51:54.149105 loophost-0.2.2/loophost/plist/ssh.plist.template
--rw-r--r--   0        0        0     3528 2023-05-22 20:59:10.162069 loophost-0.2.2/loophost/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.2/loophost/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.2/loophost/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.2/loophost/static/logo-hc.txt
--rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.2/loophost/static/logo-square.png
--rw-r--r--   0        0        0     1759 2023-05-22 18:09:46.308757 loophost-0.2.2/loophost/templates/admin.html
--rw-r--r--   0        0        0     2667 2023-05-21 23:39:30.263833 loophost-0.2.2/loophost/templates/local.html
--rw-r--r--   0        0        0     1476 2023-05-22 19:26:55.811597 loophost-0.2.2/loophost/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.2/loophost/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1166 2023-05-22 21:35:32.912469 loophost-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.2/setup.py
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 loophost-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.3/README.md
+-rw-r--r--   0        0        0        5 2023-05-22 22:47:48.370045 loophost-0.2.3/VERSION
+-rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.3/build.py
+-rw-r--r--   0        0        0      669 2023-05-22 22:47:52.343228 loophost-0.2.3/loophost/__init__.py
+-rw-r--r--   0        0        0     3370 2023-05-22 20:58:52.834903 loophost-0.2.3/loophost/flingroute.py
+-rw-r--r--   0        0        0     1021 2023-05-22 20:58:58.330155 loophost-0.2.3/loophost/launchd_plist.py
+-rwxr-xr-x   0        0        0  8301536 2023-05-22 21:35:10.810528 loophost-0.2.3/loophost/loopproxy
+-rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.3/loophost/plist/hub.plist.template
+-rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.3/loophost/plist/loophost.plist.template
+-rw-r--r--   0        0        0     1249 2023-05-22 22:47:19.211207 loophost-0.2.3/loophost/plist/ssh.plist.template
+-rw-r--r--   0        0        0     3528 2023-05-22 20:59:10.162069 loophost-0.2.3/loophost/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.3/loophost/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.3/loophost/static/fling-logo-light.png
+-rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.3/loophost/static/logo-hc.txt
+-rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.3/loophost/static/logo-square.png
+-rw-r--r--   0        0        0     1759 2023-05-22 18:09:46.308757 loophost-0.2.3/loophost/templates/admin.html
+-rw-r--r--   0        0        0     2667 2023-05-21 23:39:30.263833 loophost-0.2.3/loophost/templates/local.html
+-rw-r--r--   0        0        0     1476 2023-05-22 19:26:55.811597 loophost-0.2.3/loophost/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.3/loophost/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1167 2023-05-22 22:47:46.075713 loophost-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.3/setup.py
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 loophost-0.2.3/PKG-INFO
```

### Comparing `loophost-0.2.2/build.py` & `loophost-0.2.3/build.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/__init__.py` & `loophost-0.2.3/loophost/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 import os
 import pathlib
 import sys
 
 
 LOOPHOST_DOMAIN = "loophost.dev"
```

### Comparing `loophost-0.2.2/loophost/flingroute.py` & `loophost-0.2.3/loophost/flingroute.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/launchd_plist.py` & `loophost-0.2.3/loophost/launchd_plist.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/loopproxy` & `loophost-0.2.3/loophost/loopproxy`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/plist/hub.plist.template` & `loophost-0.2.3/loophost/plist/hub.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/plist/loophost.plist.template` & `loophost-0.2.3/loophost/plist/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/plist/ssh.plist.template` & `loophost-0.2.3/loophost/plist/ssh.plist.template`

 * *Files 3% similar despite different names*

#### Comparing `loophost-0.2.2/loophost/plist/ssh.plist.template` & `loophost-0.2.3/loophost/plist/ssh.plist.template`

```diff
@@ -15,15 +15,15 @@
       <string>-o ExitOnForwardFailure=yes</string>
       <string>-o UserKnownHostsFile=/dev/null</string>
       <string>-o StrictHostKeyChecking=no</string>
       <string>-i</string>
       <string>/Users/${LOCAL_USER}/.ssh/id_rsa</string>
       <string>-p 2222</string>
       <string>-R ${PROJECT}:443:localhost:4433</string>
-      <string>${LOCAL_USER}@${TUNNEL_DOMAIN}</string>
+      <string>${USERNAME}@${TUNNEL_DOMAIN}</string>
     </array>
     <key>WorkingDirectory</key>
     <string>${CWD}</string>
     <key>UserName</key>
     <string>${LOCAL_USER}</string>
     <key>RunAtLoad</key>
     <true/>
```

### Comparing `loophost-0.2.2/loophost/postinstall.py` & `loophost-0.2.3/loophost/postinstall.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/static/fling-logo-dark.png` & `loophost-0.2.3/loophost/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/static/fling-logo-light.png` & `loophost-0.2.3/loophost/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/static/logo-hc.txt` & `loophost-0.2.3/loophost/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/static/logo-square.png` & `loophost-0.2.3/loophost/static/logo-square.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/templates/admin.html` & `loophost-0.2.3/loophost/templates/admin.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/templates/local.html` & `loophost-0.2.3/loophost/templates/local.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/loophost/templates/partials/apptable.html` & `loophost-0.2.3/loophost/templates/partials/apptable.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.2/pyproject.toml` & `loophost-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loophost"
-version = "0.2.2"
+version = "0.2.3"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 include = [{ path = "VERSION" }, 
@@ -31,12 +31,12 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 setuptools = "*"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fling-start = "^0.1.6"
+fling-start = "^0.1.13"
 fling-cli = "^0.1.5"
 certbot = "^2.6.0"
 flask = "^2.3.2"
 lastversion = "^2.4.15"
```

### Comparing `loophost-0.2.2/PKG-INFO` & `loophost-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 0.2.2
+Version: 0.2.3
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certbot (>=2.6.0,<3.0.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: fling-cli (>=0.1.5,<0.2.0)
-Requires-Dist: fling-start (>=0.1.6,<0.2.0)
+Requires-Dist: fling-start (>=0.1.13,<0.2.0)
 Requires-Dist: lastversion (>=2.4.15,<3.0.0)
 Project-URL: documentation, https://readthedocs.org/loophost
 Project-URL: homepage, https://loophost.dev
 Project-URL: repository, https://github.com/delving-co/loophost.git
 Description-Content-Type: text/markdown
 
 # Loophost
```

