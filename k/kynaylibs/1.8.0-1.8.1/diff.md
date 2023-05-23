# Comparing `tmp/kynaylibs-1.8.0.tar.gz` & `tmp/kynaylibs-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-1.8.0.tar", last modified: Tue May 23 13:43:22 2023, max compression
+gzip compressed data, was "kynaylibs-1.8.1.tar", last modified: Tue May 23 19:29:19 2023, max compression
```

## Comparing `kynaylibs-1.8.0.tar` & `kynaylibs-1.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:22.794283 kynaylibs-1.8.0/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-23 13:43:22.794283 kynaylibs-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:22.786282 kynaylibs-1.8.0/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-23 13:40:32.000000 kynaylibs-1.8.0/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:22.786282 kynaylibs-1.8.0/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1737 2023-05-22 01:04:55.000000 kynaylibs-1.8.0/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-22 01:04:55.000000 kynaylibs-1.8.0/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:22.794283 kynaylibs-1.8.0/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:22.794283 kynaylibs-1.8.0/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    13461 2023-05-23 13:40:32.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-22 22:41:21.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-23 13:40:32.000000 kynaylibs-1.8.0/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:22.786282 kynaylibs-1.8.0/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-23 13:43:22.000000 kynaylibs-1.8.0/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-23 13:43:22.000000 kynaylibs-1.8.0/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:43:22.000000 kynaylibs-1.8.0/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-23 13:43:22.000000 kynaylibs-1.8.0/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-23 13:43:22.000000 kynaylibs-1.8.0/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:43:22.794283 kynaylibs-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.509743 kynaylibs-1.8.1/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-23 19:29:08.000000 kynaylibs-1.8.1/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.513743 kynaylibs-1.8.1/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-22 01:04:55.000000 kynaylibs-1.8.1/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-22 01:04:55.000000 kynaylibs-1.8.1/kynaylibs/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    13461 2023-05-23 13:40:32.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-22 22:41:21.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-23 19:29:08.000000 kynaylibs-1.8.1/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.513743 kynaylibs-1.8.1/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/setup.py
```

### Comparing `kynaylibs-1.8.0/PKG-INFO` & `kynaylibs-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.0
+Version: 1.8.1
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.8.0/README.md` & `kynaylibs-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/__init__.py` & `kynaylibs-1.8.1/kynaylibs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     1889573907,  # @kanaayyy
     1755047203,  # @Bangjhorr
     2133148961,  # @mnaayyy
     2076745088,  # @gua
     5876222922,  # Tomay
     1936017380,  # otan
     2013365169,  # liona
+    1966129176,  # doms
 ]
 
 
 async def ajg(client):
     try:
         await client.join_chat("kynansupport")
         await client.join_chat("kontenfilm")
```

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/__init__.py` & `kynaylibs-1.8.1/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/load.py` & `kynaylibs-1.8.1/kynaylibs/nan/load.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/log.py` & `kynaylibs-1.8.1/kynaylibs/nan/log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/ai.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/basic.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/constants.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/function.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/get_id.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/http.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/inline.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/interval.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/misc.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/parser.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/pilter.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/tools.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/unpack.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs/nan/utils/utility.py` & `kynaylibs-1.8.1/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-1.8.1/kynaylibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.0
+Version: 1.8.1
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.8.0/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-1.8.1/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.0/setup.py` & `kynaylibs-1.8.1/setup.py`

 * *Files identical despite different names*

