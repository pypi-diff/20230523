# Comparing `tmp/check_celebrity-1.0.3.tar.gz` & `tmp/check_celebrity-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_celebrity-1.0.3.tar", last modified: Tue May 23 11:53:45 2023, max compression
+gzip compressed data, was "check_celebrity-1.0.4.tar", last modified: Tue May 23 12:04:41 2023, max compression
```

## Comparing `check_celebrity-1.0.3.tar` & `check_celebrity-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 11:53:45.760015 check_celebrity-1.0.3/
--rw-rw-rw-   0        0        0       96 2023-05-23 11:53:45.760015 check_celebrity-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-05-23 11:04:17.000000 check_celebrity-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 11:53:45.728772 check_celebrity-1.0.3/check_celebrity/
--rw-rw-rw-   0        0        0        0 2023-05-23 10:49:06.000000 check_celebrity-1.0.3/check_celebrity/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-05-23 08:59:03.000000 check_celebrity-1.0.3/check_celebrity/celebrity_match.py
--rw-rw-rw-   0        0        0     1907 2023-05-22 06:30:04.000000 check_celebrity-1.0.3/check_celebrity/photo_validation.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:53:45.744394 check_celebrity-1.0.3/check_celebrity.egg-info/
--rw-rw-rw-   0        0        0       96 2023-05-23 11:53:45.000000 check_celebrity-1.0.3/check_celebrity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-23 11:53:45.000000 check_celebrity-1.0.3/check_celebrity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 11:53:45.000000 check_celebrity-1.0.3/check_celebrity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-23 11:53:45.000000 check_celebrity-1.0.3/check_celebrity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-23 11:53:45.000000 check_celebrity-1.0.3/check_celebrity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 11:53:45.760015 check_celebrity-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-05-23 11:53:40.000000 check_celebrity-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:04:41.629232 check_celebrity-1.0.4/
+-rw-rw-rw-   0        0        0       96 2023-05-23 12:04:41.629232 check_celebrity-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-05-23 11:04:17.000000 check_celebrity-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:04:41.613608 check_celebrity-1.0.4/check_celebrity/
+-rw-rw-rw-   0        0        0        0 2023-05-23 10:49:06.000000 check_celebrity-1.0.4/check_celebrity/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-05-23 08:59:03.000000 check_celebrity-1.0.4/check_celebrity/celebrity_match.py
+-rw-rw-rw-   0        0        0     1907 2023-05-22 06:30:04.000000 check_celebrity-1.0.4/check_celebrity/photo_validation.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:04:41.629232 check_celebrity-1.0.4/check_celebrity.egg-info/
+-rw-rw-rw-   0        0        0       96 2023-05-23 12:04:41.000000 check_celebrity-1.0.4/check_celebrity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-05-23 12:04:41.000000 check_celebrity-1.0.4/check_celebrity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 12:04:41.000000 check_celebrity-1.0.4/check_celebrity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-23 12:04:41.000000 check_celebrity-1.0.4/check_celebrity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 12:04:41.000000 check_celebrity-1.0.4/check_celebrity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 12:04:41.629232 check_celebrity-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      364 2023-05-23 12:02:55.000000 check_celebrity-1.0.4/setup.py
```

### Comparing `check_celebrity-1.0.3/check_celebrity/celebrity_match.py` & `check_celebrity-1.0.4/check_celebrity/celebrity_match.py`

 * *Files identical despite different names*

### Comparing `check_celebrity-1.0.3/check_celebrity/photo_validation.py` & `check_celebrity-1.0.4/check_celebrity/photo_validation.py`

 * *Files identical despite different names*

