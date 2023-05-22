# Comparing `tmp/kynaylibs-1.7.6.tar.gz` & `tmp/kynaylibs-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-1.7.6.tar", last modified: Sun May 21 22:39:07 2023, max compression
+gzip compressed data, was "kynaylibs-1.7.7.tar", last modified: Mon May 22 01:05:35 2023, max compression
```

## Comparing `kynaylibs-1.7.6.tar` & `kynaylibs-1.7.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:39:07.772211 kynaylibs-1.7.6/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-21 22:39:07.772211 kynaylibs-1.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:39:07.768211 kynaylibs-1.7.6/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1338 2023-05-21 22:32:43.000000 kynaylibs-1.7.6/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:39:07.768211 kynaylibs-1.7.6/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1802 2023-05-21 22:32:43.000000 kynaylibs-1.7.6/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-05-21 22:38:52.000000 kynaylibs-1.7.6/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:39:07.772211 kynaylibs-1.7.6/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:39:07.772211 kynaylibs-1.7.6/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    13329 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-21 22:38:52.000000 kynaylibs-1.7.6/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:39:07.768211 kynaylibs-1.7.6/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-21 22:39:07.000000 kynaylibs-1.7.6/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-21 22:39:07.000000 kynaylibs-1.7.6/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 22:39:07.000000 kynaylibs-1.7.6/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-21 22:39:07.000000 kynaylibs-1.7.6/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-21 22:39:07.000000 kynaylibs-1.7.6/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 22:39:07.772211 kynaylibs-1.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.654610 kynaylibs-1.7.7/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-21 22:32:43.000000 kynaylibs-1.7.7/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.658610 kynaylibs-1.7.7/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-22 01:04:55.000000 kynaylibs-1.7.7/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-22 01:04:55.000000 kynaylibs-1.7.7/kynaylibs/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    13329 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-22 01:04:55.000000 kynaylibs-1.7.7/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.658610 kynaylibs-1.7.7/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/setup.py
```

### Comparing `kynaylibs-1.7.6/PKG-INFO` & `kynaylibs-1.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.7.6
+Version: 1.7.7
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.7.6/README.md` & `kynaylibs-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/__init__.py` & `kynaylibs-1.7.7/kynaylibs/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/__init__.py` & `kynaylibs-1.7.7/kynaylibs/nan/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,8 +61,7 @@
         if self not in self._bots:
             self._bots.append(self)
 
     async def stop(self, *args):
         await super().stop()
         if self not in self._bots:
             self._bots.append(self)
-        self.LOGGER(__name__).info("Naya-Premium stopped. Bye.")
```

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/load.py` & `kynaylibs-1.7.7/kynaylibs/nan/load.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from importlib import import_module
 from platform import python_version
 
 from naya import *
+from naya.config import *
 from naya.modules import loadModule
 from pyrogram import __version__
 from pyrogram.types import InlineKeyboardButton, InlineKeyboardMarkup
-from naya.config import *
+
 from kynaylibs.nan.utils.db import *
 
 
 async def loadprem():
     modules = loadModule()
     for mod in modules:
         imported_module = import_module(f"naya.modules.{mod}")
```

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/log.py` & `kynaylibs-1.7.7/kynaylibs/nan/log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/ai.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/basic.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/constants.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/function.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/get_id.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/http.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/inline.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/interval.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/misc.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/parser.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/pilter.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/tools.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/unpack.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs/nan/utils/utility.py` & `kynaylibs-1.7.7/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-1.7.7/kynaylibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.7.6
+Version: 1.7.7
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.7.6/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-1.7.7/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.6/setup.py` & `kynaylibs-1.7.7/setup.py`

 * *Files identical despite different names*

