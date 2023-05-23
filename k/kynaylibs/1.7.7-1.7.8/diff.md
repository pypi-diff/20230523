# Comparing `tmp/kynaylibs-1.7.7.tar.gz` & `tmp/kynaylibs-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-1.7.7.tar", last modified: Mon May 22 01:05:35 2023, max compression
+gzip compressed data, was "kynaylibs-1.7.8.tar", last modified: Mon May 22 22:41:47 2023, max compression
```

## Comparing `kynaylibs-1.7.7.tar` & `kynaylibs-1.7.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.654610 kynaylibs-1.7.7/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1338 2023-05-21 22:32:43.000000 kynaylibs-1.7.7/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.658610 kynaylibs-1.7.7/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1737 2023-05-22 01:04:55.000000 kynaylibs-1.7.7/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-22 01:04:55.000000 kynaylibs-1.7.7/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    13329 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-22 01:04:55.000000 kynaylibs-1.7.7/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:05:35.658610 kynaylibs-1.7.7/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-22 01:05:35.000000 kynaylibs-1.7.7/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 01:05:35.662610 kynaylibs-1.7.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:41:47.676707 kynaylibs-1.7.8/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-22 22:41:47.676707 kynaylibs-1.7.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:41:47.668707 kynaylibs-1.7.8/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-21 22:32:43.000000 kynaylibs-1.7.8/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:41:47.672707 kynaylibs-1.7.8/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-22 01:04:55.000000 kynaylibs-1.7.8/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-22 01:04:55.000000 kynaylibs-1.7.8/kynaylibs/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:41:47.676707 kynaylibs-1.7.8/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:41:47.676707 kynaylibs-1.7.8/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    13389 2023-05-22 22:41:21.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-22 22:41:21.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-22 22:41:21.000000 kynaylibs-1.7.8/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:41:47.672707 kynaylibs-1.7.8/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-22 22:41:47.000000 kynaylibs-1.7.8/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-22 22:41:47.000000 kynaylibs-1.7.8/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 22:41:47.000000 kynaylibs-1.7.8/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-22 22:41:47.000000 kynaylibs-1.7.8/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-22 22:41:47.000000 kynaylibs-1.7.8/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 22:41:47.680708 kynaylibs-1.7.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.7.8/setup.py
```

### Comparing `kynaylibs-1.7.7/PKG-INFO` & `kynaylibs-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.7.7
+Version: 1.7.8
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.7.7/README.md` & `kynaylibs-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/__init__.py` & `kynaylibs-1.7.8/kynaylibs/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/__init__.py` & `kynaylibs-1.7.8/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/load.py` & `kynaylibs-1.7.8/kynaylibs/nan/load.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/log.py` & `kynaylibs-1.7.8/kynaylibs/nan/log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/ai.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/basic.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/constants.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,18 @@
 
 async def buat_log():
     botlog_chat_id = None
     for _bots in await get_userbots():
         bots_ = Ubot(**_bots)
     try:
         if bots_.is_connected:
-            await bots_.stop()
-        await bots_.start()
+            await bots_.disconnect()
+        else:
+            bots_.in_memory = False
+            await bots_.start()
         try:
             user = await bots_.get_me()
             user_id = user.id
             user_data = await usersdb.users.find_one({"user_id": user_id})
             botlog_chat_id = None
 
             if user_data:
```

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/function.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/get_id.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/http.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/inline.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/inline.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     callback_data="{}_module({},{})".format(
                         prefix, chat, x.__MODULE__.replace(" ", "_").lower()
                     ),
                 )
                 for x in module_dict.values()
             ]
         )
-    line = 5
+    line = 4
     pairs = list(zip(modules[::2], modules[1::2]))
     i = 0
     for m in pairs:
         for _ in m:
             i += 1
     if len(modules) - i == 1:
         pairs.append((modules[-1],))
```

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/interval.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/misc.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/parser.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/pilter.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/tools.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/unpack.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs/nan/utils/utility.py` & `kynaylibs-1.7.8/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-1.7.8/kynaylibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.7.7
+Version: 1.7.8
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.7.7/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-1.7.8/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.7.7/setup.py` & `kynaylibs-1.7.8/setup.py`

 * *Files identical despite different names*

