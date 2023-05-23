# Comparing `tmp/flaw-0.0.1.tar.gz` & `tmp/flaw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaw-0.0.1.tar", last modified: Tue May 23 19:25:33 2023, max compression
+gzip compressed data, was "flaw-0.0.2.tar", last modified: Tue May 23 19:35:48 2023, max compression
```

## Comparing `flaw-0.0.1.tar` & `flaw-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 19:25:33.576882 flaw-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-22 20:21:15.000000 flaw-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1179 2023-05-23 19:25:33.573886 flaw-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      808 2023-05-22 20:37:34.000000 flaw-0.0.1/README.md
--rw-rw-rw-   0        0        0      444 2023-05-23 19:23:37.000000 flaw-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 19:25:33.577883 flaw-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 19:25:33.314298 flaw-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 19:25:33.394170 flaw-0.0.1/src/flaw/
--rw-rw-rw-   0        0        0       20 2023-05-22 22:25:13.000000 flaw-0.0.1/src/flaw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:25:33.564904 flaw-0.0.1/src/flaw/utils/
--rw-rw-rw-   0        0        0       46 2023-05-22 20:08:26.000000 flaw-0.0.1/src/flaw/utils/__init__.py
--rw-rw-rw-   0        0        0     6319 2023-05-23 01:53:10.000000 flaw-0.0.1/src/flaw/utils/embed.py
--rw-rw-rw-   0        0        0      788 2023-05-22 20:09:04.000000 flaw-0.0.1/src/flaw/utils/shortener.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:25:33.526962 flaw-0.0.1/src/flaw.egg-info/
--rw-rw-rw-   0        0        0     1179 2023-05-23 19:25:33.000000 flaw-0.0.1/src/flaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-23 19:25:33.000000 flaw-0.0.1/src/flaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 19:25:33.000000 flaw-0.0.1/src/flaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-23 19:25:33.000000 flaw-0.0.1/src/flaw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 19:35:48.200839 flaw-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-22 20:21:15.000000 flaw-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1179 2023-05-23 19:35:48.194845 flaw-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2023-05-22 20:37:34.000000 flaw-0.0.2/README.md
+-rw-rw-rw-   0        0        0      444 2023-05-23 19:34:22.000000 flaw-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 19:35:48.201836 flaw-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 19:35:48.062237 flaw-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 19:35:48.102177 flaw-0.0.2/src/flaw/
+-rw-rw-rw-   0        0        0       20 2023-05-22 22:25:13.000000 flaw-0.0.2/src/flaw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:35:48.187228 flaw-0.0.2/src/flaw/utils/
+-rw-rw-rw-   0        0        0       46 2023-05-22 20:08:26.000000 flaw-0.0.2/src/flaw/utils/__init__.py
+-rw-rw-rw-   0        0        0    17055 2023-05-23 19:30:30.000000 flaw-0.0.2/src/flaw/utils/embed.py
+-rw-rw-rw-   0        0        0      788 2023-05-22 20:09:04.000000 flaw-0.0.2/src/flaw/utils/shortener.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:35:48.165076 flaw-0.0.2/src/flaw.egg-info/
+-rw-rw-rw-   0        0        0     1179 2023-05-23 19:35:47.000000 flaw-0.0.2/src/flaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-23 19:35:48.000000 flaw-0.0.2/src/flaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:35:47.000000 flaw-0.0.2/src/flaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 19:35:47.000000 flaw-0.0.2/src/flaw.egg-info/top_level.txt
```

### Comparing `flaw-0.0.1/LICENSE` & `flaw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flaw-0.0.1/PKG-INFO` & `flaw-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaw
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that makes python easier to understand
 Author-email: hue janis <null@fuckoff.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flaw-0.0.1/README.md` & `flaw-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flaw-0.0.1/src/flaw/utils/shortener.py` & `flaw-0.0.2/src/flaw/utils/shortener.py`

 * *Files identical despite different names*

### Comparing `flaw-0.0.1/src/flaw.egg-info/PKG-INFO` & `flaw-0.0.2/src/flaw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaw
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that makes python easier to understand
 Author-email: hue janis <null@fuckoff.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

