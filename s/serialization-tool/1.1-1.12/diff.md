# Comparing `tmp/serialization_tool-1.1.tar.gz` & `tmp/serialization_tool-1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialization_tool-1.1.tar", last modified: Thu May 18 09:51:29 2023, max compression
+gzip compressed data, was "serialization_tool-1.12.tar", last modified: Tue May 23 18:31:16 2023, max compression
```

## Comparing `serialization_tool-1.1.tar` & `serialization_tool-1.12.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.443299 serialization_tool-1.1/
--rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      313 2023-05-18 09:51:29.443299 serialization_tool-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-1.1/README.md
--rw-rw-rw-   0        0        0      115 2023-05-18 09:51:29.452837 serialization_tool-1.1/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-05-18 09:51:25.000000 serialization_tool-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.368292 serialization_tool-1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.389348 serialization_tool-1.1/src/serialization_tool/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.1/src/serialization_tool/__init__.py
--rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-1.1/src/serialization_tool/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.420296 serialization_tool-1.1/src/serialization_tool/serialization/
--rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-1.1/src/serialization_tool/serialization/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-05-03 17:44:51.000000 serialization_tool-1.1/src/serialization_tool/serialization/constants.py
--rw-rw-rw-   0        0        0     9770 2023-05-18 08:09:13.000000 serialization_tool-1.1/src/serialization_tool/serialization/serializer.py
--rw-rw-rw-   0        0        0      725 2023-05-18 09:47:32.000000 serialization_tool-1.1/src/serialization_tool/serialization_factory.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.424292 serialization_tool-1.1/src/serialization_tool/types/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.1/src/serialization_tool/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.432292 serialization_tool-1.1/src/serialization_tool/types/json/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.1/src/serialization_tool/types/json/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-28 13:23:00.000000 serialization_tool-1.1/src/serialization_tool/types/json/constants.py
--rw-rw-rw-   0        0        0      578 2023-05-17 19:50:20.000000 serialization_tool-1.1/src/serialization_tool/types/json/json.py
--rw-rw-rw-   0        0        0     6666 2023-05-18 09:38:10.000000 serialization_tool-1.1/src/serialization_tool/types/json/utilities.py
--rw-rw-rw-   0        0        0     1012 2023-05-18 09:50:41.000000 serialization_tool-1.1/src/serialization_tool/types/serialization.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.441302 serialization_tool-1.1/src/serialization_tool/types/xml/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.1/src/serialization_tool/types/xml/__init__.py
--rw-rw-rw-   0        0        0      132 2023-05-11 08:00:16.000000 serialization_tool-1.1/src/serialization_tool/types/xml/constants.py
--rw-rw-rw-   0        0        0     2246 2023-05-18 09:36:12.000000 serialization_tool-1.1/src/serialization_tool/types/xml/utilities.py
--rw-rw-rw-   0        0        0      857 2023-05-18 09:35:59.000000 serialization_tool-1.1/src/serialization_tool/types/xml/xml.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:51:29.414337 serialization_tool-1.1/src/serialization_tool.egg-info/
--rw-rw-rw-   0        0        0      313 2023-05-18 09:51:29.000000 serialization_tool-1.1/src/serialization_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-05-18 09:51:29.000000 serialization_tool-1.1/src/serialization_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 09:51:29.000000 serialization_tool-1.1/src/serialization_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-18 09:51:29.000000 serialization_tool-1.1/src/serialization_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.851911 serialization_tool-1.12/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-1.12/LICENSE.txt
+-rw-rw-rw-   0        0        0      314 2023-05-23 18:31:16.852913 serialization_tool-1.12/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-1.12/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-23 18:31:16.853912 serialization_tool-1.12/setup.cfg
+-rw-rw-rw-   0        0        0      427 2023-05-23 18:31:11.000000 serialization_tool-1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.773697 serialization_tool-1.12/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.787784 serialization_tool-1.12/src/serialization_tool/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-1.12/src/serialization_tool/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.837423 serialization_tool-1.12/src/serialization_tool/serialization/
+-rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-1.12/src/serialization_tool/serialization/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-05-03 17:44:51.000000 serialization_tool-1.12/src/serialization_tool/serialization/constants.py
+-rw-rw-rw-   0        0        0     9770 2023-05-22 16:21:59.000000 serialization_tool-1.12/src/serialization_tool/serialization/serializer.py
+-rw-rw-rw-   0        0        0      725 2023-05-18 09:47:32.000000 serialization_tool-1.12/src/serialization_tool/serialization_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.840434 serialization_tool-1.12/src/serialization_tool/types/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.845432 serialization_tool-1.12/src/serialization_tool/types/json/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/types/json/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-28 13:23:00.000000 serialization_tool-1.12/src/serialization_tool/types/json/constants.py
+-rw-rw-rw-   0        0        0      578 2023-05-17 19:50:20.000000 serialization_tool-1.12/src/serialization_tool/types/json/json.py
+-rw-rw-rw-   0        0        0     6666 2023-05-22 16:21:59.000000 serialization_tool-1.12/src/serialization_tool/types/json/utilities.py
+-rw-rw-rw-   0        0        0     1012 2023-05-18 09:50:41.000000 serialization_tool-1.12/src/serialization_tool/types/serialization.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.850914 serialization_tool-1.12/src/serialization_tool/types/xml/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/types/xml/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-05-11 08:00:16.000000 serialization_tool-1.12/src/serialization_tool/types/xml/constants.py
+-rw-rw-rw-   0        0        0     2246 2023-05-18 09:36:12.000000 serialization_tool-1.12/src/serialization_tool/types/xml/utilities.py
+-rw-rw-rw-   0        0        0      857 2023-05-18 09:35:59.000000 serialization_tool-1.12/src/serialization_tool/types/xml/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.832908 serialization_tool-1.12/src/serialization_tool.egg-info/
+-rw-rw-rw-   0        0        0      314 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/top_level.txt
```

### Comparing `serialization_tool-1.1/LICENSE.txt` & `serialization_tool-1.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/serialization/constants.py` & `serialization_tool-1.12/src/serialization_tool/serialization/constants.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/serialization/serializer.py` & `serialization_tool-1.12/src/serialization_tool/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/serialization_factory.py` & `serialization_tool-1.12/src/serialization_tool/serialization_factory.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/types/json/json.py` & `serialization_tool-1.12/src/serialization_tool/types/json/json.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/types/json/utilities.py` & `serialization_tool-1.12/src/serialization_tool/types/json/utilities.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/types/serialization.py` & `serialization_tool-1.12/src/serialization_tool/types/serialization.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/types/xml/utilities.py` & `serialization_tool-1.12/src/serialization_tool/types/xml/utilities.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool/types/xml/xml.py` & `serialization_tool-1.12/src/serialization_tool/types/xml/xml.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.1/src/serialization_tool.egg-info/SOURCES.txt` & `serialization_tool-1.12/src/serialization_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

