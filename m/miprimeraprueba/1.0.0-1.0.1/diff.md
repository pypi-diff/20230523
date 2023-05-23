# Comparing `tmp/miprimeraprueba-1.0.0.tar.gz` & `tmp/miprimeraprueba-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miprimeraprueba-1.0.0.tar", last modified: Mon May 22 16:16:58 2023, max compression
+gzip compressed data, was "miprimeraprueba-1.0.1.tar", last modified: Tue May 23 14:59:19 2023, max compression
```

## Comparing `miprimeraprueba-1.0.0.tar` & `miprimeraprueba-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:16:58.015452 miprimeraprueba-1.0.0/
--rw-rw-rw-   0        0        0      166 2023-05-22 16:16:58.015452 miprimeraprueba-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 16:16:57.993368 miprimeraprueba-1.0.0/miprimeraprueba/
--rw-rw-rw-   0        0        0       44 2023-05-22 16:05:51.000000 miprimeraprueba-1.0.0/miprimeraprueba/hello.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:16:58.015452 miprimeraprueba-1.0.0/miprimeraprueba.egg-info/
--rw-rw-rw-   0        0        0      166 2023-05-22 16:16:57.000000 miprimeraprueba-1.0.0/miprimeraprueba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-05-22 16:16:57.000000 miprimeraprueba-1.0.0/miprimeraprueba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:16:57.000000 miprimeraprueba-1.0.0/miprimeraprueba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-22 16:16:57.000000 miprimeraprueba-1.0.0/miprimeraprueba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:16:58.015452 miprimeraprueba-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-05-22 16:16:41.000000 miprimeraprueba-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:59:19.740920 miprimeraprueba-1.0.1/
+-rw-rw-rw-   0        0        0      166 2023-05-23 14:59:19.740920 miprimeraprueba-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 14:59:19.709659 miprimeraprueba-1.0.1/miprimeraprueba/
+-rw-rw-rw-   0        0        0       44 2023-05-22 16:05:51.000000 miprimeraprueba-1.0.1/miprimeraprueba/hello.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:59:19.740920 miprimeraprueba-1.0.1/miprimeraprueba.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-05-23 14:59:19.000000 miprimeraprueba-1.0.1/miprimeraprueba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-23 14:59:19.000000 miprimeraprueba-1.0.1/miprimeraprueba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 14:59:19.000000 miprimeraprueba-1.0.1/miprimeraprueba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 14:59:19.000000 miprimeraprueba-1.0.1/miprimeraprueba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 14:59:19.740920 miprimeraprueba-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      245 2023-05-23 14:57:04.000000 miprimeraprueba-1.0.1/setup.py
```

