# Comparing `tmp/slash3-1.1.0-py3-none-any.whl.zip` & `tmp/slash3-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8572 bytes, number of entries: 11
--rw-r--r--  2.0 unx        6 b- defN 23-May-11 16:52 slash3/VERSION
--rw-r--r--  2.0 unx     3975 b- defN 23-May-11 16:51 slash3/__init__.py
--rw-r--r--  2.0 unx     5800 b- defN 23-May-11 16:51 slash3/key.py
--rw-r--r--  2.0 unx       60 b- defN 23-May-11 16:51 slash3/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-11 16:51 slash3/py.typed
--rw-r--r--  2.0 unx     3938 b- defN 23-May-11 16:51 slash3/uri.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4567 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      804 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/RECORD
-11 files, 20322 bytes uncompressed, 7226 bytes compressed:  64.4%
+Zip file size: 8570 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        6 b- defN 23-May-23 10:23 slash3/VERSION
+-rw-r--r--  2.0 unx     3975 b- defN 23-May-23 10:23 slash3/__init__.py
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-23 10:23 slash3/key.py
+-rw-r--r--  2.0 unx       60 b- defN 23-May-23 10:23 slash3/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 10:23 slash3/py.typed
+-rw-r--r--  2.0 unx     3938 b- defN 23-May-23 10:23 slash3/uri.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-23 10:23 slash3-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4567 b- defN 23-May-23 10:23 slash3-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 10:23 slash3-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-23 10:23 slash3-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      804 b- defN 23-May-23 10:23 slash3-1.1.1.dist-info/RECORD
+11 files, 20322 bytes uncompressed, 7224 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: slash3/py.typed
 Comment: 
 
 Filename: slash3/uri.py
 Comment: 
 
-Filename: slash3-1.1.0.dist-info/LICENSE
+Filename: slash3-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: slash3-1.1.0.dist-info/METADATA
+Filename: slash3-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: slash3-1.1.0.dist-info/WHEEL
+Filename: slash3-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: slash3-1.1.0.dist-info/top_level.txt
+Filename: slash3-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: slash3-1.1.0.dist-info/RECORD
+Filename: slash3-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## slash3/VERSION

```diff
@@ -1 +1 @@
-1.1.0
+1.1.1
```

## Comparing `slash3-1.1.0.dist-info/LICENSE` & `slash3-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `slash3-1.1.0.dist-info/METADATA` & `slash3-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slash3
-Version: 1.1.0
+Version: 1.1.1
 Summary: Builds and navigates Amazon Web Services S3 URIs
 Author: Cariad Eccleston
 Author-email: cariad@cariad.earth
 License: MIT
 Project-URL: Documentation, https://cariad.github.io/slash3/slash3.html
 Project-URL: Source, https://github.com/cariad/slash3
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `slash3-1.1.0.dist-info/RECORD` & `slash3-1.1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-slash3/VERSION,sha256=FXXhr0qV8S9wtO5qatzoFglT2T6hfcJhG5CIPMw607g,6
+slash3/VERSION,sha256=zFL2eISLgUNzdXtGA4O_YZYOSUPCA3Na3eCjULPlCYk,6
 slash3/__init__.py,sha256=zKr4B7stHuwKLK3fXR4kKnDntinmDLemppziz2S5dBE,3975
 slash3/key.py,sha256=2tiP33qV6hSHoq2_t3lXRYcbGiYqz7y8ky2rx9jtiyg,5800
 slash3/logging.py,sha256=oT1TNNMM_bJcH0BSN-VQeNmP-n061zL4_CRN-Elfh5w,60
 slash3/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 slash3/uri.py,sha256=X0xYHbUw0WJcDAHoQ7C8VDLck24BqAtT_XW1z2MfDCQ,3938
-slash3-1.1.0.dist-info/LICENSE,sha256=jXz8xZq3cMjXXQ2Hb9sj6RNKFigwHmut-OnbWc-uHOU,1073
-slash3-1.1.0.dist-info/METADATA,sha256=zh0SkiaXSXMoTDJSfQWJ4Qb38r4YyVdED_1AD4I2gic,4567
-slash3-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-slash3-1.1.0.dist-info/top_level.txt,sha256=38t2bff0V6fN3YUDFFjlVn2u4K_F_8TV7g-Ao3ydX_E,7
-slash3-1.1.0.dist-info/RECORD,,
+slash3-1.1.1.dist-info/LICENSE,sha256=jXz8xZq3cMjXXQ2Hb9sj6RNKFigwHmut-OnbWc-uHOU,1073
+slash3-1.1.1.dist-info/METADATA,sha256=YvyfMQR7QkpI55RUWH0nTVEZPTuiVB4n-ZV_jdZQpxE,4567
+slash3-1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+slash3-1.1.1.dist-info/top_level.txt,sha256=38t2bff0V6fN3YUDFFjlVn2u4K_F_8TV7g-Ao3ydX_E,7
+slash3-1.1.1.dist-info/RECORD,,
```

