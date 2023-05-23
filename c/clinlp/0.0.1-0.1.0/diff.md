# Comparing `tmp/clinlp-0.0.1.tar.gz` & `tmp/clinlp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.0.1.tar", max compression
+gzip compressed data, was "clinlp-0.1.0.tar", max compression
```

## Comparing `clinlp-0.0.1.tar` & `clinlp-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-12-16 15:24:54.274547 clinlp-0.0.1/LICENSE
--rw-r--r--   0        0        0      143 2022-12-16 15:26:27.152314 clinlp-0.0.1/README.md
--rw-r--r--   0        0        0        0 2022-12-16 15:27:04.905960 clinlp-0.0.1/clinlp/__init__.py
--rw-r--r--   0        0        0       45 2022-12-16 15:28:18.569190 clinlp-0.0.1/clinlp/clinlp.py
--rw-r--r--   0        0        0      275 2022-12-16 15:26:43.960062 clinlp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 clinlp-0.0.1/setup.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 clinlp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-23 13:34:48.119725 clinlp-0.1.0/LICENSE
+-rw-r--r--   0        0        0     7783 2023-05-23 13:34:48.119725 clinlp-0.1.0/README.md
+-rw-r--r--   0        0        0       54 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/component/__init__.py
+-rw-r--r--   0        0        0    10789 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/component/qualifier.py
+-rw-r--r--   0        0        0     2308 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/component/sentencizer.py
+-rw-r--r--   0        0        0     7698 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/language.py
+-rw-r--r--   0        0        0    24443 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/resources/psynlp_context_rules.json
+-rw-r--r--   0        0        0      450 2023-05-23 13:34:48.119725 clinlp-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 clinlp-0.1.0/PKG-INFO
```

### Comparing `clinlp-0.0.1/LICENSE` & `clinlp-0.1.0/LICENSE`

 * *Files identical despite different names*

