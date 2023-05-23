# Comparing `tmp/bgstools-0.1.3.tar.gz` & `tmp/bgstools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgstools-0.1.3.tar", max compression
+gzip compressed data, was "bgstools-0.1.4.tar", max compression
```

## Comparing `bgstools-0.1.3.tar` & `bgstools-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.3/bgstools/__init__.py
--rw-r--r--   0        0        0       64 2023-05-22 20:01:20.000000 bgstools-0.1.3/bgstools/datastorage/__init__.py
--rw-r--r--   0        0        0     5014 2023-05-22 20:29:18.000000 bgstools-0.1.3/bgstools/datastorage/datastorage.py
--rw-r--r--   0        0        0       50 2023-05-22 20:28:44.000000 bgstools-0.1.3/bgstools/io/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-22 17:37:56.000000 bgstools-0.1.3/bgstools/io/io.py
--rw-r--r--   0        0        0      122 2023-05-22 20:28:18.000000 bgstools-0.1.3/bgstools/spatial/__init__.py
--rw-r--r--   0        0        0     2654 2023-05-22 17:37:56.000000 bgstools-0.1.3/bgstools/spatial/spatial.py
--rw-r--r--   0        0        0       39 2023-05-22 20:27:28.000000 bgstools-0.1.3/bgstools/stt/__init__.py
--rw-r--r--   0        0        0     2176 2023-05-22 20:27:34.000000 bgstools-0.1.3/bgstools/stt/stt.py
--rw-r--r--   0        0        0       99 2023-05-22 20:25:04.000000 bgstools-0.1.3/bgstools/utils/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-22 20:24:36.000000 bgstools-0.1.3/bgstools/utils/utils.py
--rw-r--r--   0        0        0      373 2023-05-22 20:50:44.761986 bgstools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bgstools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.4/bgstools/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-22 20:01:20.000000 bgstools-0.1.4/bgstools/datastorage/__init__.py
+-rw-r--r--   0        0        0     5014 2023-05-22 20:29:18.000000 bgstools-0.1.4/bgstools/datastorage/datastorage.py
+-rw-r--r--   0        0        0      165 2023-05-23 09:24:52.850097 bgstools-0.1.4/bgstools/io/__init__.py
+-rw-r--r--   0        0        0     3990 2023-05-23 08:59:13.676273 bgstools-0.1.4/bgstools/io/io.py
+-rw-r--r--   0        0        0     4820 2023-05-23 13:42:54.752929 bgstools-0.1.4/bgstools/io/media.py
+-rw-r--r--   0        0        0      122 2023-05-22 20:28:18.000000 bgstools-0.1.4/bgstools/spatial/__init__.py
+-rw-r--r--   0        0        0     2654 2023-05-22 17:37:56.000000 bgstools-0.1.4/bgstools/spatial/spatial.py
+-rw-r--r--   0        0        0       39 2023-05-22 20:27:28.000000 bgstools-0.1.4/bgstools/stt/__init__.py
+-rw-r--r--   0        0        0     2171 2023-05-23 06:03:13.166243 bgstools-0.1.4/bgstools/stt/stt.py
+-rw-r--r--   0        0        0       99 2023-05-22 20:25:04.000000 bgstools-0.1.4/bgstools/utils/__init__.py
+-rw-r--r--   0        0        0     2971 2023-05-22 20:24:36.000000 bgstools-0.1.4/bgstools/utils/utils.py
+-rw-r--r--   0        0        0      418 2023-05-23 13:51:00.277544 bgstools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 bgstools-0.1.4/PKG-INFO
```

### Comparing `bgstools-0.1.3/bgstools/datastorage/datastorage.py` & `bgstools-0.1.4/bgstools/datastorage/datastorage.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.3/bgstools/spatial/spatial.py` & `bgstools-0.1.4/bgstools/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.3/bgstools/stt/stt.py` & `bgstools-0.1.4/bgstools/stt/stt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # streamlit tools (stt)
 from collections import OrderedDict
-from typing import Optional, Tuple, Any
+from typing import Optional, Tuple
 from ..utils import script_as_module
 import streamlit as st
 
 
 def build_activities_menu(
     activities_dict: OrderedDict[str, dict], 
     label: str,
```

### Comparing `bgstools-0.1.3/bgstools/utils/utils.py` & `bgstools-0.1.4/bgstools/utils/utils.py`

 * *Files identical despite different names*

