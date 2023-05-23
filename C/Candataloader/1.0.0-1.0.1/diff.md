# Comparing `tmp/Candataloader-1.0.0.tar.gz` & `tmp/Candataloader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Candataloader-1.0.0.tar", last modified: Tue May 23 16:38:13 2023, max compression
+gzip compressed data, was "dist/Candataloader-1.0.1.tar", last modified: Tue May 23 17:27:34 2023, max compression
```

## Comparing `Candataloader-1.0.0.tar` & `Candataloader-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 16:38:13.000000 Candataloader-1.0.0/
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 16:38:13.000000 Candataloader-1.0.0/download_dataset/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.0.0/download_dataset/__init__.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1045 2023-05-23 03:48:22.000000 Candataloader-1.0.0/download_dataset/download.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:35:39.000000 Candataloader-1.0.0/README.md
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-05-23 16:38:13.000000 Candataloader-1.0.0/setup.cfg
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 16:38:13.000000 Candataloader-1.0.0/Candataloader.egg-info/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       20 2023-05-23 16:38:13.000000 Candataloader-1.0.0/Candataloader.egg-info/requires.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-05-23 16:38:13.000000 Candataloader-1.0.0/Candataloader.egg-info/dependency_links.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      260 2023-05-23 16:38:13.000000 Candataloader-1.0.0/Candataloader.egg-info/SOURCES.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       17 2023-05-23 16:38:13.000000 Candataloader-1.0.0/Candataloader.egg-info/top_level.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      231 2023-05-23 16:38:13.000000 Candataloader-1.0.0/Candataloader.egg-info/PKG-INFO
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      316 2023-05-23 05:04:14.000000 Candataloader-1.0.0/setup.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      231 2023-05-23 16:38:13.000000 Candataloader-1.0.0/PKG-INFO
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 17:27:34.000000 Candataloader-1.0.1/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:35:39.000000 Candataloader-1.0.1/README.md
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 17:27:34.000000 Candataloader-1.0.1/Candataloader/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.0.1/Candataloader/__init__.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1045 2023-05-23 03:48:22.000000 Candataloader-1.0.1/Candataloader/download.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-05-23 17:27:34.000000 Candataloader-1.0.1/setup.cfg
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 17:27:34.000000 Candataloader-1.0.1/Candataloader.egg-info/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       20 2023-05-23 17:27:34.000000 Candataloader-1.0.1/Candataloader.egg-info/requires.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-05-23 17:27:34.000000 Candataloader-1.0.1/Candataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      254 2023-05-23 17:27:34.000000 Candataloader-1.0.1/Candataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       14 2023-05-23 17:27:34.000000 Candataloader-1.0.1/Candataloader.egg-info/top_level.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      254 2023-05-23 17:27:34.000000 Candataloader-1.0.1/Candataloader.egg-info/PKG-INFO
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      342 2023-05-23 17:22:30.000000 Candataloader-1.0.1/setup.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      254 2023-05-23 17:27:34.000000 Candataloader-1.0.1/PKG-INFO
```

### Comparing `Candataloader-1.0.0/download_dataset/download.py` & `Candataloader-1.0.1/Candataloader/download.py`

 * *Files identical despite different names*

