# Comparing `tmp/quantbox-0.0.8-py3-none-any.whl.zip` & `tmp/quantbox-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3876 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       84 b- defN 23-May-22 02:45 quantbox/__init__.py
+Zip file size: 3951 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       82 b- defN 23-May-22 02:54 quantbox/__init__.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 quantbox/quantbox.py
--rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 quantbox/witapi.py
+-rw-rw-r--  2.0 unx     3360 b- defN 23-May-22 03:02 quantbox/witapi.py
 -rw-rw-r--  2.0 unx       66 b- defN 23-May-22 02:39 witapi/__init__.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 witapi/quantbox.py
--rw-rw-r--  2.0 unx      650 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      675 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/RECORD
-9 files, 11287 bytes uncompressed, 2718 bytes compressed:  75.9%
+-rw-rw-r--  2.0 unx      650 b- defN 23-May-22 03:02 quantbox-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 03:02 quantbox-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-22 03:02 quantbox-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      675 b- defN 23-May-22 03:02 quantbox-0.0.9.dist-info/RECORD
+9 files, 11408 bytes uncompressed, 2793 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: witapi/__init__.py
 Comment: 
 
 Filename: witapi/quantbox.py
 Comment: 
 
-Filename: quantbox-0.0.8.dist-info/METADATA
+Filename: quantbox-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: quantbox-0.0.8.dist-info/WHEEL
+Filename: quantbox-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: quantbox-0.0.8.dist-info/top_level.txt
+Filename: quantbox-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: quantbox-0.0.8.dist-info/RECORD
+Filename: quantbox-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quantbox/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .witapi import user_id, password, get_wit, get_shared_wit
+from .witapi import set_credentials, get_wit, get_shared_wit
 __version__ = '0.0.1'
```

## quantbox/witapi.py

```diff
@@ -3,15 +3,21 @@
 from motoo import wit_util as wu
 import requests
 import orjson
 
 user_id = ''
 password = ''
 
+def set_credentials(id, pw):
+    global user_id, password
+    user_id = id
+    password = pw
+
 def get_wit(wit_id, from_date=None, to_date=None, stock_codes=[]):
+    global user_id, password
     if user_id is None or user_id == '' or password is None or password == '':
         return ''
 
     data = dict(
         user_id=user_id,
         password=password,
         wit_id=wit_id,
```

## Comparing `quantbox-0.0.8.dist-info/METADATA` & `quantbox-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: quantbox wit api
 Home-page: UNKNOWN
 Author: ffolio
 Author-email: service@ffolio.co.kr
 License: UNKNOWN
 Keywords: pypi deploy
 Platform: UNKNOWN
```

