# Comparing `tmp/relativedate-0.1.2.tar.gz` & `tmp/relativedate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-0.1.2.tar", last modified: Mon May 22 16:57:32 2023, max compression
+gzip compressed data, was "relativedate-1.0.0.tar", last modified: Tue May 23 10:48:49 2023, max compression
```

## Comparing `relativedate-0.1.2.tar` & `relativedate-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:57:32.157441 relativedate-0.1.2/
--rw-rw-rw-   0        0        0     1353 2023-05-22 16:57:32.155445 relativedate-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-05-22 16:36:21.000000 relativedate-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 16:57:32.136496 relativedate-0.1.2/relativedate/
--rw-rw-rw-   0        0        0     1115 2023-05-22 15:26:47.000000 relativedate-0.1.2/relativedate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:57:32.154450 relativedate-0.1.2/relativedate.egg-info/
--rw-rw-rw-   0        0        0     1353 2023-05-22 16:57:31.000000 relativedate-0.1.2/relativedate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-05-22 16:57:32.000000 relativedate-0.1.2/relativedate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:57:31.000000 relativedate-0.1.2/relativedate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-22 16:57:31.000000 relativedate-0.1.2/relativedate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:57:32.158443 relativedate-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-22 16:57:26.000000 relativedate-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:48:49.625829 relativedate-1.0.0/
+-rw-rw-rw-   0        0        0     2310 2023-05-23 10:48:49.624844 relativedate-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2150 2023-05-23 10:47:11.000000 relativedate-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 10:48:49.604887 relativedate-1.0.0/relativedate/
+-rw-rw-rw-   0        0        0      813 2023-05-23 10:33:01.000000 relativedate-1.0.0/relativedate/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-05-23 10:32:01.000000 relativedate-1.0.0/relativedate/dtmath.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:48:49.623834 relativedate-1.0.0/relativedate.egg-info/
+-rw-rw-rw-   0        0        0     2310 2023-05-23 10:48:49.000000 relativedate-1.0.0/relativedate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-23 10:48:49.000000 relativedate-1.0.0/relativedate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:48:49.000000 relativedate-1.0.0/relativedate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 10:48:49.000000 relativedate-1.0.0/relativedate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 10:48:49.625829 relativedate-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-05-23 10:48:41.000000 relativedate-1.0.0/setup.py
```

