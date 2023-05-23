# Comparing `tmp/migdalor-0.0.2.dev9.tar.gz` & `tmp/migdalor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migdalor-0.0.2.dev9.tar", last modified: Sun May 21 14:09:54 2023, max compression
+gzip compressed data, was "migdalor-0.0.3.tar", last modified: Tue May 23 19:08:29 2023, max compression
```

## Comparing `migdalor-0.0.2.dev9.tar` & `migdalor-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev9/README.md
--rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev9/migdalor/__init__.py
--rw-r--r--   0        0        0     4328 2023-05-21 14:08:58.439808 migdalor-0.0.2.dev9/migdalor/cluster.py
--rw-r--r--   0        0        0     1319 2023-05-21 13:47:46.833402 migdalor-0.0.2.dev9/migdalor/discovery.py
--rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev9/migdalor/logger.py
--rw-r--r--   0        0        0      641 2023-05-21 14:09:54.807198 migdalor-0.0.2.dev9/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-23 18:48:51.128883 migdalor-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1710 2023-05-21 17:36:55.719860 migdalor-0.0.3/README.md
+-rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.3/migdalor/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-23 18:56:16.607825 migdalor-0.0.3/migdalor/__version__.py
+-rw-r--r--   0        0        0     4328 2023-05-21 17:34:06.476439 migdalor-0.0.3/migdalor/cluster.py
+-rw-r--r--   0        0        0     1319 2023-05-21 13:47:46.833402 migdalor-0.0.3/migdalor/discovery.py
+-rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.3/migdalor/logger.py
+-rw-r--r--   0        0        0        0 2023-05-21 14:32:36.534671 migdalor-0.0.3/migdalor/py.typed
+-rw-r--r--   0        0        0     1418 2023-05-23 19:08:29.533504 migdalor-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 migdalor-0.0.3/PKG-INFO
```

### Comparing `migdalor-0.0.2.dev9/migdalor/cluster.py` & `migdalor-0.0.3/migdalor/cluster.py`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev9/migdalor/discovery.py` & `migdalor-0.0.3/migdalor/discovery.py`

 * *Files identical despite different names*

