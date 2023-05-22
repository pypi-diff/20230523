# Comparing `tmp/determined_cli-0.22.2rc0-py3-none-any.whl.zip` & `tmp/determined_cli-0.22.2rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1765 bytes, number of entries: 6
--rw-r--r--  2.0 unx      226 b- defN 23-May-17 23:33 determined_cli/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-May-17 23:33 determined_cli/__version__.py
--rw-r--r--  2.0 unx      414 b- defN 23-May-17 23:33 determined_cli-0.22.2rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 23:33 determined_cli-0.22.2rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-17 23:33 determined_cli-0.22.2rc0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      507 b- defN 23-May-17 23:33 determined_cli-0.22.2rc0.dist-info/RECORD
-6 files, 1281 bytes uncompressed, 833 bytes compressed:  35.0%
+Zip file size: 1768 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      226 b- defN 23-May-22 23:17 determined_cli/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-May-22 23:17 determined_cli/__version__.py
+-rw-r--r--  2.0 unx      414 b- defN 23-May-22 23:17 determined_cli-0.22.2rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 23:17 determined_cli-0.22.2rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-22 23:17 determined_cli-0.22.2rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      507 b- defN 23-May-22 23:17 determined_cli-0.22.2rc1.dist-info/RECORD
+6 files, 1281 bytes uncompressed, 836 bytes compressed:  34.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_cli/__init__.py
 Comment: 
 
 Filename: determined_cli/__version__.py
 Comment: 
 
-Filename: determined_cli-0.22.2rc0.dist-info/METADATA
+Filename: determined_cli-0.22.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: determined_cli-0.22.2rc0.dist-info/WHEEL
+Filename: determined_cli-0.22.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: determined_cli-0.22.2rc0.dist-info/top_level.txt
+Filename: determined_cli-0.22.2rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_cli-0.22.2rc0.dist-info/RECORD
+Filename: determined_cli-0.22.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_cli/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.22.2-rc0"
+__version__ = "0.22.2-rc1"
```

