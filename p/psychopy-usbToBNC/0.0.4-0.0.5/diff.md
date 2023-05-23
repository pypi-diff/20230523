# Comparing `tmp/psychopy-usbToBNC-0.0.4.tar.gz` & `tmp/psychopy-usbToBNC-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psychopy-usbToBNC-0.0.4.tar", last modified: Tue May 23 15:21:54 2023, max compression
+gzip compressed data, was "C:\Users\chris\Desktop\psychopy-usbToBNC\dist\.tmp-c8tqwj8c\psychopy-usbToBNC-0.0.5.tar", last modified: Tue May 23 15:36:32 2023, max compression
```

## Comparing `psychopy-usbToBNC-0.0.4.tar` & `psychopy-usbToBNC-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.144055 psychopy-usbToBNC-0.0.4/
--rw-rw-rw-   0        0        0     1049 2023-05-23 15:21:54.143056 psychopy-usbToBNC-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.128141 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/
--rw-rw-rw-   0        0        0      389 2023-05-20 01:52:07.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.143056 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/usbToBNC/
--rw-rw-rw-   0        0        0    11487 2023-05-20 01:52:53.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/usbToBNC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.142056 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/
--rw-rw-rw-   0        0        0     1049 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 15:21:54.144055 psychopy-usbToBNC-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1422 2023-05-23 15:20:53.000000 psychopy-usbToBNC-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:36:32.971007 psychopy-usbToBNC-0.0.5/
+-rw-rw-rw-   0        0        0    35823 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1372 2023-05-23 15:36:32.970006 psychopy-usbToBNC-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 15:36:32.942011 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/
+-rw-rw-rw-   0        0        0      389 2023-05-20 01:52:07.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:36:32.964015 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/
+-rw-rw-rw-   0        0        0    11487 2023-05-20 01:52:53.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:36:32.966007 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/classic/
+-rw-rw-rw-   0        0        0     1187 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/classic/eau.png
+-rw-rw-rw-   0        0        0     1890 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/classic/reward.png
+-rw-rw-rw-   0        0        0     4456 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/classic/reward@2x.png
+drwxrwxrwx   0        0        0        0 2023-05-23 15:36:32.968012 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/dark/
+-rw-rw-rw-   0        0        0     1187 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/dark/eau.png
+-rw-rw-rw-   0        0        0     1706 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/dark/reward.png
+-rw-rw-rw-   0        0        0     2991 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/dark/reward@2x.png
+drwxrwxrwx   0        0        0        0 2023-05-23 15:36:32.970006 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/light/
+-rw-rw-rw-   0        0        0     1187 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/light/eau.png
+-rw-rw-rw-   0        0        0     1695 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/light/reward.png
+-rw-rw-rw-   0        0        0     3042 1970-01-01 00:00:00.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/light/reward@2x.png
+drwxrwxrwx   0        0        0        0 2023-05-23 15:36:32.964015 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/
+-rw-rw-rw-   0        0        0     1372 2023-05-23 15:36:32.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2023-05-23 15:36:32.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 15:36:32.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-05-23 15:36:32.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 15:36:32.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-23 15:36:32.000000 psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-05-23 15:33:26.000000 psychopy-usbToBNC-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 15:36:32.971007 psychopy-usbToBNC-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2023-05-23 15:20:53.000000 psychopy-usbToBNC-0.0.5/setup.py
```

### Comparing `psychopy-usbToBNC-0.0.4/PKG-INFO` & `psychopy-usbToBNC-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: psychopy-usbToBNC
-Version: 0.0.4
-Summary: Coming soon
-Home-page: UNKNOWN
+Version: 0.0.5
+Summary: Extension to add support for labeotech devices such as usbToBNC and water pump systems for mice.
 Author: Labeo Technologies(Christophe Cloutier-Tremblay)
-Author-email: <Christophe@labeotech.com>
-License: UNKNOWN
-Description: todo
+Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>, Christophe Cloutier-Tremblay <christophe@labeotech.com>
+License: GNU General Public License v3 (GPLv3)
+Project-URL: homepage, https://github.com/psychopy/psychopy-usbToBNC
+Project-URL: changelog, https://github.com/psychopy/psychopy-usbToBNC/blob/main/CHANGELOG.txt
+Project-URL: documentation, https://pages.github.com/psychopy/psychopy-usbToBNC
+Project-URL: repository, https://github.com/psychopy/psychopy-usbToBNC
 Keywords: python
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/usbToBNC/__init__.py` & `psychopy-usbToBNC-0.0.5/psychopy_usbToBNC/usbToBNC/__init__.py`

 * *Files identical despite different names*

### Comparing `psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/PKG-INFO` & `psychopy-usbToBNC-0.0.5/psychopy_usbToBNC.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: psychopy-usbToBNC
-Version: 0.0.4
-Summary: Coming soon
-Home-page: UNKNOWN
+Version: 0.0.5
+Summary: Extension to add support for labeotech devices such as usbToBNC and water pump systems for mice.
 Author: Labeo Technologies(Christophe Cloutier-Tremblay)
-Author-email: <Christophe@labeotech.com>
-License: UNKNOWN
-Description: todo
+Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>, Christophe Cloutier-Tremblay <christophe@labeotech.com>
+License: GNU General Public License v3 (GPLv3)
+Project-URL: homepage, https://github.com/psychopy/psychopy-usbToBNC
+Project-URL: changelog, https://github.com/psychopy/psychopy-usbToBNC/blob/main/CHANGELOG.txt
+Project-URL: documentation, https://pages.github.com/psychopy/psychopy-usbToBNC
+Project-URL: repository, https://github.com/psychopy/psychopy-usbToBNC
 Keywords: python
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `psychopy-usbToBNC-0.0.4/setup.py` & `psychopy-usbToBNC-0.0.5/setup.py`

 * *Files identical despite different names*

