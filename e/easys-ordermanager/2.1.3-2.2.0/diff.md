# Comparing `tmp/easys-ordermanager-2.1.3.tar.gz` & `tmp/easys-ordermanager-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easys-ordermanager-2.1.3.tar", last modified: Wed May  3 10:19:48 2023, max compression
+gzip compressed data, was "easys-ordermanager-2.2.0.tar", last modified: Tue May 23 10:02:07 2023, max compression
```

## Comparing `easys-ordermanager-2.1.3.tar` & `easys-ordermanager-2.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/
--rw-r--r--   0 root         (0) root         (0)    12228 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     9435 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/CHANGELOG_SERIALIZER.md
--rw-r--r--   0 root         (0) root         (0)    34940 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22442 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/dev/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/dev/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/management/commands/i18n.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v1/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v2/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v3/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      519 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      829 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/easys_ordermanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/easys_ordermanager/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    13139 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93490 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v1/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93587 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v2/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94724 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v3/serializer.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22442 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1249 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)    12390 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     9435 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/CHANGELOG_SERIALIZER.md
+-rw-r--r--   0 root         (0) root         (0)    34940 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22569 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/dev/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/dev/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/dev/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/management/commands/i18n.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/dev/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/dev/tests/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/tests/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/tests/v1/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/dev/tests/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/tests/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/tests/v2/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/dev/tests/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/tests/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      826 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/dev/tests/v3/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/easys_ordermanager/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/easys_ordermanager/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-23 10:02:07.000000 easys-ordermanager-2.2.0/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.611917 easys-ordermanager-2.2.0/easys_ordermanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.611917 easys-ordermanager-2.2.0/easys_ordermanager/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/easys_ordermanager/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    13139 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/easys_ordermanager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93490 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/v1/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/easys_ordermanager/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93587 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/v2/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/easys_ordermanager/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94724 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/v3/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/easys_ordermanager/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:02:07.615918 easys-ordermanager-2.2.0/easys_ordermanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22569 2023-05-23 10:02:07.000000 easys-ordermanager-2.2.0/easys_ordermanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-23 10:02:07.000000 easys-ordermanager-2.2.0/easys_ordermanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 10:02:07.000000 easys-ordermanager-2.2.0/easys_ordermanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-23 10:02:07.000000 easys-ordermanager-2.2.0/easys_ordermanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 10:02:07.000000 easys-ordermanager-2.2.0/easys_ordermanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-23 10:02:07.619917 easys-ordermanager-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-23 10:00:57.000000 easys-ordermanager-2.2.0/setup.py
```

### Comparing `easys-ordermanager-2.1.3/CHANGELOG.md` & `easys-ordermanager-2.2.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 2.2.0 (2023-05-23)
+* Remove support for Django < 4.1
+* Remove support for djangorestframework < 3.14
+* Updated minimum required versions of related libraries
+
 ## 2.1.3 (2023-05-03)
 * Updates to Serializer v2 & v3, see serializer changelog
 
 ## 2.1.2 (2023-04-12)
 * Updates to Serializer v3, see serializer changelog
 * Fixed missing development dependency
```

### Comparing `easys-ordermanager-2.1.3/CHANGELOG_SERIALIZER.md` & `easys-ordermanager-2.2.0/CHANGELOG_SERIALIZER.md`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/LICENSE.md` & `easys-ordermanager-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/PKG-INFO` & `easys-ordermanager-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.1.3
+Version: 2.2.0
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -15,29 +15,30 @@
 
 # EasyS order manager API
 
 ## Compatibility matrix
 
 Python 3.8, 3.9 and 3.10 
 
-### Django 3.2
-
-DRF 3.11 or newer
-
-### Django 4.0
+### Django 4.1
 
-DRF 3.13 or newer
+DRF 3.14 or newer
 
-### Django 4.1
+### Django 4.2
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.2.0 (2023-05-23)
+* Remove support for Django < 4.1
+* Remove support for djangorestframework < 3.14
+* Updated minimum required versions of related libraries
+
 ## 2.1.3 (2023-05-03)
 * Updates to Serializer v2 & v3, see serializer changelog
 
 ## 2.1.2 (2023-04-12)
 * Updates to Serializer v3, see serializer changelog
 * Fixed missing development dependency
```

### Comparing `easys-ordermanager-2.1.3/dev/management/commands/i18n.py` & `easys-ordermanager-2.2.0/dev/management/commands/i18n.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/dev/tests/v3/test_serializer.py` & `easys-ordermanager-2.2.0/dev/tests/v3/test_serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager/__pycache__/__init__.cpython-311.pyc` & `easys-ordermanager-2.2.0/easys_ordermanager/__pycache__/__init__.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x562d5264 (Wed May  3 09:45:58 2023 UTC)
+moddate:  0xd98e6c64 (Tue May 23 10:00:57 2023 UTC)
 files sz: 300
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 1
    flags     : 0
    code
@@ -13,15 +13,15 @@
    
      1           2 LOAD_CONST               0 ('easys-ordermanager')
                  4 STORE_NAME               0 (__title__)
    
      2           6 LOAD_CONST               1 ('API definition of RH order manager for EasyS')
                  8 STORE_NAME               1 (__description__)
    
-     3          10 LOAD_CONST               2 ('2.1.3')
+     3          10 LOAD_CONST               2 ('2.2.0')
                 12 STORE_NAME               2 (__version__)
    
      4          14 LOAD_CONST               3 ('https://gitlab.herocentral.de/development/easys-ordermanager')
                 16 STORE_NAME               3 (__url__)
    
      5          18 LOAD_CONST               4 ('RegioHelden developers')
                 20 STORE_NAME               4 (__author__)
@@ -32,15 +32,15 @@
      7          26 LOAD_CONST               6 ('GPL 3')
                 28 STORE_NAME               6 (__license__)
                 30 LOAD_CONST               7 (None)
                 32 RETURN_VALUE
    consts
       'easys-ordermanager'
       'API definition of RH order manager for EasyS'
-      '2.1.3'
+      '2.2.0'
       'https://gitlab.herocentral.de/development/easys-ordermanager'
       'RegioHelden developers'
       'opensource@regiohelden.de'
       'GPL 3'
       None
    names      ('__title__', '__description__', '__version__', '__url__', '__author__', '__author_email__', '__license__')
    varnames   ()
```

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager/fields.py` & `easys-ordermanager-2.2.0/easys_ordermanager/fields.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager/locale/de/LC_MESSAGES/django.po` & `easys-ordermanager-2.2.0/easys_ordermanager/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager/v1/serializer.py` & `easys-ordermanager-2.2.0/easys_ordermanager/v1/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager/v2/serializer.py` & `easys-ordermanager-2.2.0/easys_ordermanager/v2/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager/v3/serializer.py` & `easys-ordermanager-2.2.0/easys_ordermanager/v3/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager/validators.py` & `easys-ordermanager-2.2.0/easys_ordermanager/validators.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager.egg-info/PKG-INFO` & `easys-ordermanager-2.2.0/easys_ordermanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.1.3
+Version: 2.2.0
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -15,29 +15,30 @@
 
 # EasyS order manager API
 
 ## Compatibility matrix
 
 Python 3.8, 3.9 and 3.10 
 
-### Django 3.2
-
-DRF 3.11 or newer
-
-### Django 4.0
+### Django 4.1
 
-DRF 3.13 or newer
+DRF 3.14 or newer
 
-### Django 4.1
+### Django 4.2
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.2.0 (2023-05-23)
+* Remove support for Django < 4.1
+* Remove support for djangorestframework < 3.14
+* Updated minimum required versions of related libraries
+
 ## 2.1.3 (2023-05-03)
 * Updates to Serializer v2 & v3, see serializer changelog
 
 ## 2.1.2 (2023-04-12)
 * Updates to Serializer v3, see serializer changelog
 * Fixed missing development dependency
```

### Comparing `easys-ordermanager-2.1.3/easys_ordermanager.egg-info/SOURCES.txt` & `easys-ordermanager-2.2.0/easys_ordermanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.3/setup.py` & `easys-ordermanager-2.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         + "\n\n"
         + read_file("CHANGELOG.md")
         + "\n\n"
         + read_file("CHANGELOG_SERIALIZER.md")
     ),
     long_description_content_type='text/markdown',
     install_requires=[
-        'django>=3.2,<4.2',
-        'django-countries>=6.0,<8.0',
-        'django-internationalflavor>=0.4.0,<0.5.0',
-        'django-model-utils>=3.1.2,<5.0.0',
-        'django-phonenumber-field>=3.0.1,<8.0',
-        'djangorestframework>=3.11,<3.15',
-        'phonenumbers>=7.0.6,<8.14.0',
+        'django>=4.1,<4.3',
+        'django-countries>=7.0,<8.0',
+        'django-internationalflavor>=0.4.3,<0.5.0',
+        'django-model-utils>=4.2.0,<5.0.0',
+        'django-phonenumber-field>=4.0.0,<8.0',
+        'djangorestframework>=3.14,<3.15',
+        'phonenumbers>=8.12.50,<8.14.0',
     ],
     license=easys_ordermanager.__license__,
     url=easys_ordermanager.__url__,
     download_url='',
     keywords=[],
     include_package_data=True,
     classifiers=[],
```

