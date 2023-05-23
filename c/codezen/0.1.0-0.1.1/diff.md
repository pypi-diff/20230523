# Comparing `tmp/codezen-0.1.0.tar.gz` & `tmp/codezen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codezen-0.1.0.tar", max compression
+gzip compressed data, was "codezen-0.1.1.tar", max compression
```

## Comparing `codezen-0.1.0.tar` & `codezen-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029587 codezen-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.1.0/codezen/__init__.py
--rw-r--r--   0        0        0       30 2023-05-23 13:08:17.312100 codezen-0.1.0/codezen/__main__.py
--rw-r--r--   0        0        0     4080 2023-05-23 13:21:39.848044 codezen-0.1.0/codezen/app.py
--rw-r--r--   0        0        0      399 2023-05-23 13:24:56.166419 codezen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      409 1970-01-01 00:00:00.000000 codezen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 14:43:11.360293 codezen-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1991 2023-05-23 15:08:53.787807 codezen-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.1.1/codezen/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-23 13:08:17.312100 codezen-0.1.1/codezen/__main__.py
+-rw-r--r--   0        0        0     4080 2023-05-23 13:21:39.848044 codezen-0.1.1/codezen/app.py
+-rw-r--r--   0        0        0      498 2023-05-23 16:01:39.044776 codezen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 codezen-0.1.1/PKG-INFO
```

### Comparing `codezen-0.1.0/codezen/app.py` & `codezen-0.1.1/codezen/app.py`

 * *Files identical despite different names*

