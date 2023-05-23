# Comparing `tmp/prusaLink-0.1.1.tar.gz` & `tmp/prusaLink-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusaLink-0.1.1.tar", last modified: Tue May 16 20:33:10 2023, max compression
+gzip compressed data, was "prusaLink-1.0.0.tar", last modified: Tue May 23 20:00:53 2023, max compression
```

## Comparing `prusaLink-0.1.1.tar` & `prusaLink-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:33:10.668107 prusaLink-0.1.1/
--rw-rw-rw-   0        0        0     1075 2023-05-15 15:07:17.000000 prusaLink-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     9228 2023-05-16 20:33:10.668107 prusaLink-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7310 2023-05-16 20:32:05.000000 prusaLink-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 20:33:10.644395 prusaLink-0.1.1/prusaLink/
--rw-rw-rw-   0        0        0     4429 2023-05-16 20:30:11.000000 prusaLink-0.1.1/prusaLink/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:33:10.668107 prusaLink-0.1.1/prusaLink.egg-info/
--rw-rw-rw-   0        0        0     9228 2023-05-16 20:33:10.000000 prusaLink-0.1.1/prusaLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-16 20:33:10.000000 prusaLink-0.1.1/prusaLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:33:10.000000 prusaLink-0.1.1/prusaLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 20:33:10.000000 prusaLink-0.1.1/prusaLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      683 2023-05-16 20:32:32.000000 prusaLink-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 20:33:10.668107 prusaLink-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      197 2023-05-16 13:25:26.000000 prusaLink-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:33:10.668107 prusaLink-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusaLink-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusaLink-0.1.1/tests/test_prusaLink.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:00:53.400783 prusaLink-1.0.0/
+-rw-rw-rw-   0        0        0     1075 2023-05-23 19:57:05.000000 prusaLink-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2125 2023-05-23 20:00:53.400783 prusaLink-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-05-23 19:58:50.000000 prusaLink-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 20:00:53.384266 prusaLink-1.0.0/prusaLink/
+-rw-rw-rw-   0        0        0      255 2023-05-23 19:59:50.000000 prusaLink-1.0.0/prusaLink/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:00:53.384266 prusaLink-1.0.0/prusaLink.egg-info/
+-rw-rw-rw-   0        0        0     2125 2023-05-23 20:00:53.000000 prusaLink-1.0.0/prusaLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-23 20:00:53.000000 prusaLink-1.0.0/prusaLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 20:00:53.000000 prusaLink-1.0.0/prusaLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 20:00:53.000000 prusaLink-1.0.0/prusaLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      683 2023-05-23 20:00:22.000000 prusaLink-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 20:00:53.400783 prusaLink-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      197 2023-05-23 20:00:05.000000 prusaLink-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:00:53.400783 prusaLink-1.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:57:05.000000 prusaLink-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:57:05.000000 prusaLink-1.0.0/tests/test_prusaLink.py
```

### Comparing `prusaLink-0.1.1/LICENSE` & `prusaLink-1.0.0/LICENSE`

 * *Files identical despite different names*

