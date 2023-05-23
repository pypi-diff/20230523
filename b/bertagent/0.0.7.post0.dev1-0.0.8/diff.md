# Comparing `tmp/bertagent-0.0.7.post0.dev1-py3-none-any.whl.zip` & `tmp/bertagent-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 16671 bytes, number of entries: 7
+Zip file size: 16539 bytes, number of entries: 7
 -rw-------  2.0 unx     6139 b- defN 22-Dec-07 14:22 bertagent/__init__.py
--rw-------  2.0 unx      508 b- defN 22-Dec-07 14:34 bertagent/_version.py
--rw-------  2.0 unx    35149 b- defN 22-Dec-07 14:34 bertagent-0.0.7.post0.dev1.dist-info/LICENSE
--rw-------  2.0 unx     1426 b- defN 22-Dec-07 14:34 bertagent-0.0.7.post0.dev1.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 22-Dec-07 14:34 bertagent-0.0.7.post0.dev1.dist-info/WHEEL
--rw-------  2.0 unx       10 b- defN 22-Dec-07 14:34 bertagent-0.0.7.post0.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      607 b- defN 22-Dec-07 14:34 bertagent-0.0.7.post0.dev1.dist-info/RECORD
-7 files, 43931 bytes uncompressed, 15585 bytes compressed:  64.5%
+-rw-------  2.0 unx      497 b- defN 22-Dec-07 14:35 bertagent/_version.py
+-rw-------  2.0 unx    35149 b- defN 22-Dec-07 14:35 bertagent-0.0.8.dist-info/LICENSE
+-rw-------  2.0 unx     1415 b- defN 22-Dec-07 14:35 bertagent-0.0.8.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 22-Dec-07 14:35 bertagent-0.0.8.dist-info/WHEEL
+-rw-------  2.0 unx       10 b- defN 22-Dec-07 14:35 bertagent-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      552 b- defN 22-Dec-07 14:35 bertagent-0.0.8.dist-info/RECORD
+7 files, 43854 bytes uncompressed, 15563 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: bertagent/__init__.py
 Comment: 
 
 Filename: bertagent/_version.py
 Comment: 
 
-Filename: bertagent-0.0.7.post0.dev1.dist-info/LICENSE
+Filename: bertagent-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: bertagent-0.0.7.post0.dev1.dist-info/METADATA
+Filename: bertagent-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: bertagent-0.0.7.post0.dev1.dist-info/WHEEL
+Filename: bertagent-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: bertagent-0.0.7.post0.dev1.dist-info/top_level.txt
+Filename: bertagent-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: bertagent-0.0.7.post0.dev1.dist-info/RECORD
+Filename: bertagent-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bertagent/_version.py

```diff
@@ -8,14 +8,14 @@
 
 version_json = '''
 {
  "date": "2022-12-07T15:33:55+0100",
  "dirty": false,
  "error": null,
  "full-revisionid": "ac9996018b2c6866d195a1a9d9a66460aaf49bfc",
- "version": "0.0.7.post0.dev1"
+ "version": "0.0.8"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `bertagent-0.0.7.post0.dev1.dist-info/LICENSE` & `bertagent-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bertagent-0.0.7.post0.dev1.dist-info/METADATA` & `bertagent-0.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bertagent
-Version: 0.0.7.post0.dev1
+Version: 0.0.8
 Summary: bertagent helpers
 Home-page: https://github.com/bertagent/bertagent
 Author: The Bertagent Development Team
 Author-email: enchanted.stardust@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Bug Tracker, https://github.com/bertagent/bertagent/issues
 Project-URL: Documentation, https://github.com/bertagent/bertagent/docs
```

## Comparing `bertagent-0.0.7.post0.dev1.dist-info/RECORD` & `bertagent-0.0.8.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 bertagent/__init__.py,sha256=CfqKDh1FgP5OLtfBk8UV803CL1rMOVw94gl5OpLJa1Y,6139
-bertagent/_version.py,sha256=4gIVKexOK3XU9BGk3cG5NGlusle8EWV73bNP7F-dMKk,508
-bertagent-0.0.7.post0.dev1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-bertagent-0.0.7.post0.dev1.dist-info/METADATA,sha256=uQXc3Kkmad0HvTY7O3wpGHCKZfYJvk_kYJWuPssWB68,1426
-bertagent-0.0.7.post0.dev1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bertagent-0.0.7.post0.dev1.dist-info/top_level.txt,sha256=fyN_IoTGsa5NjmeogsRQ_OeZXY8T8-gFTg8JWFUUlVU,10
-bertagent-0.0.7.post0.dev1.dist-info/RECORD,,
+bertagent/_version.py,sha256=Ji9_bHN0iik2rEuhI6QqtKhASArHNYwEzDcfjNV5nB4,497
+bertagent-0.0.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+bertagent-0.0.8.dist-info/METADATA,sha256=BgldUF5l_Sp9IyHI75GYwzbY7eh6xpflAPCG-9fbOwc,1415
+bertagent-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bertagent-0.0.8.dist-info/top_level.txt,sha256=fyN_IoTGsa5NjmeogsRQ_OeZXY8T8-gFTg8JWFUUlVU,10
+bertagent-0.0.8.dist-info/RECORD,,
```

