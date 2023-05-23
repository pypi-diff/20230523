# Comparing `tmp/yowasp_runtime-1.6-py3-none-any.whl.zip` & `tmp/yowasp_runtime-1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3820 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2689 b- defN 23-Feb-06 20:32 yowasp_runtime/__init__.py
--rw-r--r--  2.0 unx      763 b- defN 23-Feb-06 20:32 yowasp_runtime-1.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1870 b- defN 23-Feb-06 20:32 yowasp_runtime-1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-06 20:32 yowasp_runtime-1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-06 20:32 yowasp_runtime-1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      497 b- defN 23-Feb-06 20:32 yowasp_runtime-1.6.dist-info/RECORD
-6 files, 5926 bytes uncompressed, 2914 bytes compressed:  50.8%
+Zip file size: 3822 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2689 b- defN 23-Feb-07 02:03 yowasp_runtime/__init__.py
+-rw-r--r--  2.0 unx      763 b- defN 23-Feb-07 02:03 yowasp_runtime-1.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1870 b- defN 23-Feb-07 02:03 yowasp_runtime-1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-07 02:03 yowasp_runtime-1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Feb-07 02:03 yowasp_runtime-1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      497 b- defN 23-Feb-07 02:03 yowasp_runtime-1.7.dist-info/RECORD
+6 files, 5926 bytes uncompressed, 2916 bytes compressed:  50.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: yowasp_runtime/__init__.py
 Comment: 
 
-Filename: yowasp_runtime-1.6.dist-info/LICENSE.txt
+Filename: yowasp_runtime-1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: yowasp_runtime-1.6.dist-info/METADATA
+Filename: yowasp_runtime-1.7.dist-info/METADATA
 Comment: 
 
-Filename: yowasp_runtime-1.6.dist-info/WHEEL
+Filename: yowasp_runtime-1.7.dist-info/WHEEL
 Comment: 
 
-Filename: yowasp_runtime-1.6.dist-info/top_level.txt
+Filename: yowasp_runtime-1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: yowasp_runtime-1.6.dist-info/RECORD
+Filename: yowasp_runtime-1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `yowasp_runtime-1.6.dist-info/LICENSE.txt` & `yowasp_runtime-1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `yowasp_runtime-1.6.dist-info/METADATA` & `yowasp_runtime-1.7.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yowasp-runtime
-Version: 1.6
+Version: 1.7
 Summary: Common runtime for YoWASP packages
 Author-email: Catherine <whitequark@whitequark.org>
 License: ISC License
         
         Copyright (C) Catherine <whitequark@whitequark.org>
         
         Permission to use, copy, modify, and/or distribute this software for any
@@ -22,15 +22,15 @@
 Project-URL: Homepage, https://yowasp.org/
 Project-URL: Source Code, https://github.com/YoWASP/runtime
 Project-URL: Bug Tracker, https://github.com/YoWASP/runtime/issues
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: appdirs (~=1.4)
-Requires-Dist: wasmtime (<2,>=1.0)
+Requires-Dist: wasmtime (<6,>=1.0)
 Requires-Dist: importlib-resources ; python_version < "3.9"
 
 YoWASP runtime
 ==============
 
 This package is an internal support package for the [YoWASP project][yowasp]. It handles interfacing with the [WebAssembly][] runtime and the supported operating systems. Do not depend on this package in your own code.
```

