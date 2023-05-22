# Comparing `tmp/cardamom_ai-0.0.1.tar.gz` & `tmp/cardamom_ai-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardamom_ai-0.0.1.tar", last modified: Mon May 22 23:46:16 2023, max compression
+gzip compressed data, was "cardamom_ai-0.1.tar", last modified: Mon May 22 23:17:57 2023, max compression
```

## Comparing `cardamom_ai-0.0.1.tar` & `cardamom_ai-0.1.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-22 23:46:16.079602 cardamom_ai-0.0.1/
--rw-r--r--   0 nmh        (501) staff       (20)    34523 2023-05-21 21:37:45.000000 cardamom_ai-0.0.1/LICENSE
--rw-r--r--   0 nmh        (501) staff       (20)      279 2023-05-22 23:46:16.079641 cardamom_ai-0.0.1/PKG-INFO
--rw-r--r--   0 nmh        (501) staff       (20)        0 2023-05-22 22:37:46.000000 cardamom_ai-0.0.1/README.md
-drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-22 23:46:16.079188 cardamom_ai-0.0.1/cardamom_ai.egg-info/
--rw-r--r--   0 nmh        (501) staff       (20)      279 2023-05-22 23:46:16.000000 cardamom_ai-0.0.1/cardamom_ai.egg-info/PKG-INFO
--rw-r--r--   0 nmh        (501) staff       (20)      271 2023-05-22 23:46:16.000000 cardamom_ai-0.0.1/cardamom_ai.egg-info/SOURCES.txt
--rw-r--r--   0 nmh        (501) staff       (20)        1 2023-05-22 23:46:16.000000 cardamom_ai-0.0.1/cardamom_ai.egg-info/dependency_links.txt
--rw-r--r--   0 nmh        (501) staff       (20)       52 2023-05-22 23:46:16.000000 cardamom_ai-0.0.1/cardamom_ai.egg-info/requires.txt
--rw-r--r--   0 nmh        (501) staff       (20)        4 2023-05-22 23:46:16.000000 cardamom_ai-0.0.1/cardamom_ai.egg-info/top_level.txt
--rw-r--r--   0 nmh        (501) staff       (20)      122 2023-05-22 23:42:19.000000 cardamom_ai-0.0.1/pyproject.toml
--rw-r--r--   0 nmh        (501) staff       (20)      524 2023-05-22 23:46:16.079859 cardamom_ai-0.0.1/setup.cfg
-drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-22 23:46:16.079497 cardamom_ai-0.0.1/src/
--rw-r--r--   0 nmh        (501) staff       (20)       33 2023-05-22 23:00:56.000000 cardamom_ai-0.0.1/src/__init__.py
--rw-r--r--   0 nmh        (501) staff       (20)     1903 2023-05-22 23:00:00.000000 cardamom_ai-0.0.1/src/deploy.py
--rw-r--r--   0 nmh        (501) staff       (20)     6782 2023-05-21 22:39:27.000000 cardamom_ai-0.0.1/src/serialize_sklearn.py
+drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-22 23:17:57.059160 cardamom_ai-0.1/
+-rw-r--r--   0 nmh        (501) staff       (20)    34523 2023-05-21 21:37:45.000000 cardamom_ai-0.1/LICENSE
+-rw-r--r--   0 nmh        (501) staff       (20)      174 2023-05-22 23:17:57.059218 cardamom_ai-0.1/PKG-INFO
+-rw-r--r--   0 nmh        (501) staff       (20)        0 2023-05-22 22:37:46.000000 cardamom_ai-0.1/README.md
+-rw-r--r--   0 nmh        (501) staff       (20)      103 2023-05-22 23:17:57.059388 cardamom_ai-0.1/setup.cfg
+-rw-r--r--   0 nmh        (501) staff       (20)      377 2023-05-22 23:17:54.000000 cardamom_ai-0.1/setup.py
+drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-22 23:17:57.057802 cardamom_ai-0.1/src/
+drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-22 23:17:57.059056 cardamom_ai-0.1/src/cardamom_ai.egg-info/
+-rw-r--r--   0 nmh        (501) staff       (20)      174 2023-05-22 23:17:57.000000 cardamom_ai-0.1/src/cardamom_ai.egg-info/PKG-INFO
+-rw-r--r--   0 nmh        (501) staff       (20)      230 2023-05-22 23:17:57.000000 cardamom_ai-0.1/src/cardamom_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 nmh        (501) staff       (20)        1 2023-05-22 23:17:57.000000 cardamom_ai-0.1/src/cardamom_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 nmh        (501) staff       (20)       28 2023-05-22 23:17:57.000000 cardamom_ai-0.1/src/cardamom_ai.egg-info/requires.txt
+-rw-r--r--   0 nmh        (501) staff       (20)        1 2023-05-22 23:17:57.000000 cardamom_ai-0.1/src/cardamom_ai.egg-info/top_level.txt
```

### Comparing `cardamom_ai-0.0.1/LICENSE` & `cardamom_ai-0.1/LICENSE`

 * *Files identical despite different names*

