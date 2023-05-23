# Comparing `tmp/psychopy-usbToBNC-0.0.3.tar.gz` & `tmp/psychopy-usbToBNC-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psychopy-usbToBNC-0.0.3.tar", last modified: Tue May 23 15:17:19 2023, max compression
+gzip compressed data, was "dist\psychopy-usbToBNC-0.0.4.tar", last modified: Tue May 23 15:21:54 2023, max compression
```

## Comparing `psychopy-usbToBNC-0.0.3.tar` & `psychopy-usbToBNC-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.929342 psychopy-usbToBNC-0.0.3/
--rw-rw-rw-   0        0        0      608 2023-05-23 15:17:19.929342 psychopy-usbToBNC-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.910337 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/
--rw-rw-rw-   0        0        0      389 2023-05-20 01:52:07.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.928342 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/usbToBNC/
--rw-rw-rw-   0        0        0    11487 2023-05-20 01:52:53.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/usbToBNC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:17:19.927346 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/
--rw-rw-rw-   0        0        0      608 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-23 15:17:19.000000 psychopy-usbToBNC-0.0.3/psychopy_usbToBNC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 15:17:19.929342 psychopy-usbToBNC-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      989 2023-05-23 15:17:16.000000 psychopy-usbToBNC-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.144055 psychopy-usbToBNC-0.0.4/
+-rw-rw-rw-   0        0        0     1049 2023-05-23 15:21:54.143056 psychopy-usbToBNC-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.128141 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/
+-rw-rw-rw-   0        0        0      389 2023-05-20 01:52:07.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.143056 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/usbToBNC/
+-rw-rw-rw-   0        0        0    11487 2023-05-20 01:52:53.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/usbToBNC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:21:54.142056 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/
+-rw-rw-rw-   0        0        0     1049 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-23 15:21:54.000000 psychopy-usbToBNC-0.0.4/psychopy_usbToBNC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 15:21:54.144055 psychopy-usbToBNC-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2023-05-23 15:20:53.000000 psychopy-usbToBNC-0.0.4/setup.py
```

### Comparing `psychopy-usbToBNC-0.0.3/psychopy_usbToBNC/usbToBNC/__init__.py` & `psychopy-usbToBNC-0.0.4/psychopy_usbToBNC/usbToBNC/__init__.py`

 * *Files identical despite different names*

