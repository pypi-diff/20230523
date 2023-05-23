# Comparing `tmp/freetar-0.1.1.tar.gz` & `tmp/freetar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freetar-0.1.1.tar", max compression
+gzip compressed data, was "freetar-0.1.2.tar", max compression
```

## Comparing `freetar-0.1.1.tar` & `freetar-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-01 10:41:21.268315 freetar-0.1.1/README.md
--rw-r--r--   0        0        0     1049 2023-05-23 18:11:27.344236 freetar-0.1.1/freetar/backend.py
--rw-r--r--   0        0        0     1669 2023-05-23 17:55:05.049736 freetar-0.1.1/freetar/templates/base.html
--rw-r--r--   0        0        0     5083 2023-05-23 18:02:54.775254 freetar-0.1.1/freetar/templates/index.html
--rw-r--r--   0        0        0     3969 2023-05-23 17:46:58.807515 freetar-0.1.1/freetar/ug.py
--rw-r--r--   0        0        0      461 2023-05-23 18:12:49.654603 freetar-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 freetar-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-01 10:41:21.268315 freetar-0.1.2/README.md
+-rw-r--r--   0        0        0     1049 2023-05-23 18:11:27.344236 freetar-0.1.2/freetar/backend.py
+-rw-r--r--   0        0        0     1669 2023-05-23 17:55:05.049736 freetar-0.1.2/freetar/templates/base.html
+-rw-r--r--   0        0        0     5083 2023-05-23 18:02:54.775254 freetar-0.1.2/freetar/templates/index.html
+-rw-r--r--   0        0        0     3969 2023-05-23 17:46:58.807515 freetar-0.1.2/freetar/ug.py
+-rw-r--r--   0        0        0      557 2023-05-23 18:26:16.318177 freetar-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 freetar-0.1.2/PKG-INFO
```

### Comparing `freetar-0.1.1/LICENSE` & `freetar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freetar-0.1.1/freetar/backend.py` & `freetar-0.1.2/freetar/backend.py`

 * *Files identical despite different names*

### Comparing `freetar-0.1.1/freetar/templates/base.html` & `freetar-0.1.2/freetar/templates/base.html`

 * *Files identical despite different names*

### Comparing `freetar-0.1.1/freetar/templates/index.html` & `freetar-0.1.2/freetar/templates/index.html`

 * *Files identical despite different names*

### Comparing `freetar-0.1.1/freetar/ug.py` & `freetar-0.1.2/freetar/ug.py`

 * *Files identical despite different names*

