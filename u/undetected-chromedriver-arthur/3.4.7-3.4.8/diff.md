# Comparing `tmp/undetected-chromedriver-arthur-3.4.7.tar.gz` & `tmp/undetected-chromedriver-arthur-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undetected-chromedriver-arthur-3.4.7.tar", last modified: Mon May 22 11:26:19 2023, max compression
+gzip compressed data, was "undetected-chromedriver-arthur-3.4.8.tar", last modified: Tue May 23 07:32:42 2023, max compression
```

## Comparing `undetected-chromedriver-arthur-3.4.7.tar` & `undetected-chromedriver-arthur-3.4.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 11:26:19.650235 undetected-chromedriver-arthur-3.4.7/
--rw-rw-rw-   0        0        0    35823 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/LICENSE
--rw-rw-rw-   0        0        0    76728 2023-05-22 11:26:19.648236 undetected-chromedriver-arthur-3.4.7/PKG-INFO
--rw-rw-rw-   0        0        0    75683 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 11:26:19.650235 undetected-chromedriver-arthur-3.4.7/setup.cfg
--rw-rw-rw-   0        0        0     2699 2023-05-22 11:26:04.000000 undetected-chromedriver-arthur-3.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 11:26:19.625233 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/
--rw-rw-rw-   0        0        0    33698 2023-05-22 06:50:55.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/__init__.py
--rw-rw-rw-   0        0        0     3386 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/cdp.py
--rw-rw-rw-   0        0        0     5747 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/devtool.py
--rw-rw-rw-   0        0        0     1763 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/dprocess.py
--rw-rw-rw-   0        0        0     2666 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/options.py
--rw-rw-rw-   0        0        0    11434 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/patcher.py
--rw-rw-rw-   0        0        0     2966 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/reactor.py
--rw-rw-rw-   0        0        0     2814 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/webelement.py
-drwxrwxrwx   0        0        0        0 2023-05-22 11:26:19.644236 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/
--rw-rw-rw-   0        0        0    76728 2023-05-22 11:26:19.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-05-22 11:26:19.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 11:26:19.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-22 11:26:19.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-22 11:26:19.000000 undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 07:32:42.946093 undetected-chromedriver-arthur-3.4.8/
+-rw-rw-rw-   0        0        0    35823 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/LICENSE
+-rw-rw-rw-   0        0        0    76622 2023-05-23 07:32:42.945094 undetected-chromedriver-arthur-3.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0    75683 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:32:42.946093 undetected-chromedriver-arthur-3.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     2598 2023-05-22 11:38:23.000000 undetected-chromedriver-arthur-3.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:32:42.922094 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/
+-rw-rw-rw-   0        0        0    33721 2023-05-23 07:31:02.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/__init__.py
+-rw-rw-rw-   0        0        0     3386 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/cdp.py
+-rw-rw-rw-   0        0        0     5747 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/devtool.py
+-rw-rw-rw-   0        0        0     1763 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/dprocess.py
+-rw-rw-rw-   0        0        0     2666 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/options.py
+-rw-rw-rw-   0        0        0    11434 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/patcher.py
+-rw-rw-rw-   0        0        0     2966 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/reactor.py
+-rw-rw-rw-   0        0        0     2814 2023-05-22 06:47:58.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/webelement.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:32:42.941094 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/
+-rw-rw-rw-   0        0        0    76622 2023-05-23 07:32:42.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-05-23 07:32:42.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:32:42.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-23 07:32:42.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-23 07:32:42.000000 undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/top_level.txt
```

### Comparing `undetected-chromedriver-arthur-3.4.7/LICENSE` & `undetected-chromedriver-arthur-3.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/PKG-INFO` & `undetected-chromedriver-arthur-3.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver-arthur
-Version: 3.4.7
-Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
+Version: 3.4.8
+Summary: ('(just an impatient fix for headless bug as: https://github.com/ultrafunkamsterdam/undetected-chromedriver/issues/1252#issuecomment-1544900464),can remove anytime once the main stream updated',)
 Home-page: https://github.com/ppLorins/undetected-chromedriver/tree/fix-headless-version-issue
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `undetected-chromedriver-arthur-3.4.7/README.md` & `undetected-chromedriver-arthur-3.4.8/README.md`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/setup.py` & `undetected-chromedriver-arthur-3.4.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 ) as fp:
     try:
         version = re.findall(r"^__version__ = ['\"]([^'\"]*)['\"]", fp.read(), re.M)[0]
     except Exception:
         raise RuntimeError("unable to determine version")
 
 description = (
-    "Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.",
-    "Not triggered by CloudFlare/Imperva/hCaptcha and such.",
-    "NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.",
+    "(just an impatient fix for headless bug as: "
+    "https://github.com/ultrafunkamsterdam/undetected-chromedriver/issues/1252#issuecomment-1544900464)"
+    ",can remove anytime once the main stream updated",
 )
 
 setup(
     name="undetected-chromedriver-arthur",
     version=version,
     packages=["undetected_chromedriver"],
     install_requires=[
```

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/__init__.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 by UltrafunkAmsterdam (https://github.com/ultrafunkamsterdam)
 
 """
 from __future__ import annotations
 
 
-__version__ = "3.4.7"
+__version__ = "3.4.8"
 
 import json
 import logging
 import os
 import re
 import shutil
 import subprocess
@@ -384,14 +384,15 @@
 
         # if headless or options.headless:
         #     if self.patcher.version_main < 108:
         #         options.add_argument("--headless=chrome")
         #     elif self.patcher.version_main >= 108:
         #         options.add_argument("--headless=new")
 
+        version = None
         if headless or options.headless:
             version = self.patcher.version_main
         if version and version < 108:
             options.add_argument("--headless=chrome")
         else:
             options.add_argument("--headless=new")
```

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/cdp.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/cdp.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/devtool.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/devtool.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/dprocess.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/dprocess.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/options.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/options.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/patcher.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/patcher.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/reactor.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/reactor.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver/webelement.py` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver/webelement.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/PKG-INFO` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver-arthur
-Version: 3.4.7
-Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
+Version: 3.4.8
+Summary: ('(just an impatient fix for headless bug as: https://github.com/ultrafunkamsterdam/undetected-chromedriver/issues/1252#issuecomment-1544900464),can remove anytime once the main stream updated',)
 Home-page: https://github.com/ppLorins/undetected-chromedriver/tree/fix-headless-version-issue
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `undetected-chromedriver-arthur-3.4.7/undetected_chromedriver_arthur.egg-info/SOURCES.txt` & `undetected-chromedriver-arthur-3.4.8/undetected_chromedriver_arthur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

