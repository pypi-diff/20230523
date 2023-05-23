# Comparing `tmp/wisdomweaver-0.1.0.tar.gz` & `tmp/wisdomweaver-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisdomweaver-0.1.0.tar", last modified: Tue May 23 16:36:28 2023, max compression
+gzip compressed data, was "wisdomweaver-0.3.0.tar", last modified: Tue May 23 21:49:20 2023, max compression
```

## Comparing `wisdomweaver-0.1.0.tar` & `wisdomweaver-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 16:36:27.997627 wisdomweaver-0.1.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)      588 2023-05-23 16:20:38.000000 wisdomweaver-0.1.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     7456 2023-05-23 16:36:27.997627 wisdomweaver-0.1.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     6234 2023-05-07 21:12:44.000000 wisdomweaver-0.1.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      817 2023-05-23 16:36:19.000000 wisdomweaver-0.1.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-23 16:36:28.001627 wisdomweaver-0.1.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      336 2023-05-23 16:15:03.000000 wisdomweaver-0.1.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 16:36:27.997627 wisdomweaver-0.1.0/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1238 2023-05-13 10:37:32.000000 wisdomweaver-0.1.0/tests/test_database.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1114 2023-05-13 10:35:01.000000 wisdomweaver-0.1.0/tests/test_document.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)       64 2023-05-23 16:28:44.000000 wisdomweaver-0.1.0/wisdom
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 16:36:27.997627 wisdomweaver-0.1.0/wisdomweaver/
--rw-rw-r--   0 martin    (1000) martin    (1000)      135 2023-05-23 16:26:55.000000 wisdomweaver-0.1.0/wisdomweaver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      103 2023-05-23 16:29:20.000000 wisdomweaver-0.1.0/wisdomweaver/__main__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 16:36:27.997627 wisdomweaver-0.1.0/wisdomweaver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7456 2023-05-23 16:36:27.000000 wisdomweaver-0.1.0/wisdomweaver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      362 2023-05-23 16:36:27.000000 wisdomweaver-0.1.0/wisdomweaver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-23 16:36:27.000000 wisdomweaver-0.1.0/wisdomweaver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-23 16:36:27.000000 wisdomweaver-0.1.0/wisdomweaver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-23 16:36:27.000000 wisdomweaver-0.1.0/wisdomweaver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-23 16:36:27.000000 wisdomweaver-0.1.0/wisdomweaver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      588 2023-05-23 16:20:38.000000 wisdomweaver-0.3.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1998 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      776 2023-05-23 21:34:57.000000 wisdomweaver-0.3.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1180 2023-05-23 21:48:09.000000 wisdomweaver-0.3.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      337 2023-05-23 20:03:42.000000 wisdomweaver-0.3.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.492689 wisdomweaver-0.3.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1238 2023-05-13 10:37:32.000000 wisdomweaver-0.3.0/tests/test_database.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1114 2023-05-13 10:35:01.000000 wisdomweaver-0.3.0/tests/test_document.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)     4334 2023-05-23 21:28:31.000000 wisdomweaver-0.3.0/wisdom
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/wisdomweaver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      241 2023-05-23 21:48:09.000000 wisdomweaver-0.3.0/wisdomweaver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       93 2023-05-23 20:05:48.000000 wisdomweaver-0.3.0/wisdomweaver/__main__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1984 2023-05-23 18:49:00.000000 wisdomweaver-0.3.0/wisdomweaver/database.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4581 2023-05-23 20:14:26.000000 wisdomweaver-0.3.0/wisdomweaver/document.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      108 2023-05-13 09:19:34.000000 wisdomweaver-0.3.0/wisdomweaver/models.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      987 2023-05-13 10:35:01.000000 wisdomweaver-0.3.0/wisdomweaver/postprocessor.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/wisdomweaver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1998 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      465 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/top_level.txt
```

### Comparing `wisdomweaver-0.1.0/LICENSE` & `wisdomweaver-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wisdomweaver-0.1.0/tests/test_database.py` & `wisdomweaver-0.3.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `wisdomweaver-0.1.0/tests/test_document.py` & `wisdomweaver-0.3.0/tests/test_document.py`

 * *Files identical despite different names*

