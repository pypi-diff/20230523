# Comparing `tmp/oci_mlflow-1.0.0-py3-none-any.whl.zip` & `tmp/oci_mlflow-1.0b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 23365 bytes, number of entries: 17
--rw-r--r--  2.0 unx      938 b- defN 23-May-23 18:17 oci_mlflow/__init__.py
--rw-r--r--  2.0 unx    21498 b- defN 23-May-23 18:17 oci_mlflow/deployment.py
--rw-r--r--  2.0 unx     4235 b- defN 23-May-23 18:17 oci_mlflow/oci_object_storage.py
--rw-r--r--  2.0 unx    26088 b- defN 23-May-23 18:17 oci_mlflow/project.py
--rw-r--r--  2.0 unx     4448 b- defN 23-May-23 18:17 oci_mlflow/telemetry_logging.py
--rw-r--r--  2.0 unx     9236 b- defN 23-May-23 18:17 oci_mlflow/utils.py
--rwxrwxrwx  2.0 unx       25 b- defN 23-May-23 18:17 oci_mlflow/version.json
--rw-r--r--  2.0 unx        0 b- defN 23-May-23 18:17 oci_mlflow/templates/__init__.py
--rwxrwxrwx  2.0 unx     1200 b- defN 23-May-23 18:17 oci_mlflow/templates/project_description.jinja2
--rwxrwxrwx  2.0 unx      163 b- defN 23-May-23 18:17 oci_mlflow/templates/runtime.yaml.jinja2
--rwxrwxrwx  2.0 unx      422 b- defN 23-May-23 18:17 oci_mlflow/templates/score.py.jinja2
--rwxrwxrwx  2.0 unx     1860 b- defN 23-May-23 18:22 oci_mlflow-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2156 b- defN 23-May-23 18:22 oci_mlflow-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 18:22 oci_mlflow-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      243 b- defN 23-May-23 18:22 oci_mlflow-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-23 18:22 oci_mlflow-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1452 b- defN 23-May-23 18:22 oci_mlflow-1.0.0.dist-info/RECORD
-17 files, 74067 bytes uncompressed, 20955 bytes compressed:  71.7%
+Zip file size: 23367 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      938 b- defN 23-May-17 00:36 oci_mlflow/__init__.py
+-rw-r--r--  2.0 unx    21498 b- defN 23-May-17 00:36 oci_mlflow/deployment.py
+-rw-r--r--  2.0 unx     4235 b- defN 23-May-17 00:36 oci_mlflow/oci_object_storage.py
+-rw-r--r--  2.0 unx    26088 b- defN 23-May-17 00:36 oci_mlflow/project.py
+-rw-r--r--  2.0 unx     4448 b- defN 23-May-17 00:36 oci_mlflow/telemetry_logging.py
+-rw-r--r--  2.0 unx     9236 b- defN 23-May-17 00:36 oci_mlflow/utils.py
+-rwxrwxrwx  2.0 unx       25 b- defN 23-May-17 00:36 oci_mlflow/version.json
+-rw-r--r--  2.0 unx        0 b- defN 23-May-17 00:36 oci_mlflow/templates/__init__.py
+-rwxrwxrwx  2.0 unx     1200 b- defN 23-May-17 00:36 oci_mlflow/templates/project_description.jinja2
+-rwxrwxrwx  2.0 unx      163 b- defN 23-May-17 00:36 oci_mlflow/templates/runtime.yaml.jinja2
+-rwxrwxrwx  2.0 unx      422 b- defN 23-May-17 00:36 oci_mlflow/templates/score.py.jinja2
+-rwxrwxrwx  2.0 unx     1860 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2156 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      243 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1452 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/RECORD
+17 files, 74067 bytes uncompressed, 20957 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: oci_mlflow/templates/runtime.yaml.jinja2
 Comment: 
 
 Filename: oci_mlflow/templates/score.py.jinja2
 Comment: 
 
-Filename: oci_mlflow-1.0.0.dist-info/LICENSE.txt
+Filename: oci_mlflow-1.0b0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: oci_mlflow-1.0.0.dist-info/METADATA
+Filename: oci_mlflow-1.0b0.dist-info/METADATA
 Comment: 
 
-Filename: oci_mlflow-1.0.0.dist-info/WHEEL
+Filename: oci_mlflow-1.0b0.dist-info/WHEEL
 Comment: 
 
-Filename: oci_mlflow-1.0.0.dist-info/entry_points.txt
+Filename: oci_mlflow-1.0b0.dist-info/entry_points.txt
 Comment: 
 
-Filename: oci_mlflow-1.0.0.dist-info/top_level.txt
+Filename: oci_mlflow-1.0b0.dist-info/top_level.txt
 Comment: 
 
-Filename: oci_mlflow-1.0.0.dist-info/RECORD
+Filename: oci_mlflow-1.0b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oci_mlflow/version.json

### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'version'": "'1.0b0'"}*

```diff
@@ -1,3 +1,3 @@
 {
-    "version": "1.0.0"
+    "version": "1.0b0"
 }
```

## Comparing `oci_mlflow-1.0.0.dist-info/LICENSE.txt` & `oci_mlflow-1.0b0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `oci_mlflow-1.0.0.dist-info/METADATA` & `oci_mlflow-1.0b0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oci-mlflow
-Version: 1.0.0
+Version: 1.0b0
 Summary: OCI MLflow plugin to use OCI resources within MLflow
 Author: Oracle Cloud Infrastructure Data Science
 License: Universal Permissive License 1.0
 Keywords: Oracle Cloud Infrastructure,OCI,Object Storage,MLflow
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `oci_mlflow-1.0.0.dist-info/RECORD` & `oci_mlflow-1.0b0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 oci_mlflow/__init__.py,sha256=fObIqoSRHDbkSEBxLxH8j52vTOR5B4qzGJXpwhw2KNo,938
 oci_mlflow/deployment.py,sha256=XKxQU5hzefmMsKHL7D90sM0FMB-qQW3m27bIlHyb59o,21498
 oci_mlflow/oci_object_storage.py,sha256=T2WGInAx0MloieknoveVk8vOGQQ5lJM-cC6fXZ4dxh4,4235
 oci_mlflow/project.py,sha256=feqiOBTyCP6HQBenzjfwT90u_wiBNyw3bUniuievkHo,26088
 oci_mlflow/telemetry_logging.py,sha256=NWufc4Y7sFvSG9npPXRVudxO6gB1k5azCCZ9Yi_jbME,4448
 oci_mlflow/utils.py,sha256=Yc0mqf0-j_5VZuEWFKAPqlde9gSJLetODqCJX1mbtIQ,9236
-oci_mlflow/version.json,sha256=YEM13WltP5yALFW_oqGVhXqDnYFp9QYKJUHxZrIkX8s,25
+oci_mlflow/version.json,sha256=dIF7j8Kscg63L06DLzFI5t0nH4LWJOH1Byf99ECohNY,25
 oci_mlflow/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oci_mlflow/templates/project_description.jinja2,sha256=WPUhBUA8xs0AFpxs5aSCK7Rvd1YPIyjegxp_W1rMlxk,1200
 oci_mlflow/templates/runtime.yaml.jinja2,sha256=cBhdxsurzIw2kEZ0-HNpepytsQdGRugfyi50KUSvVdE,163
 oci_mlflow/templates/score.py.jinja2,sha256=-yynJDrIYTJD4-zCYaxRoQ0oPdVKhB1b1wjDzvoADCk,422
-oci_mlflow-1.0.0.dist-info/LICENSE.txt,sha256=0ggOnaxgPaQEBstfywBdLBJ-kO9cJ4shpvZplaXiSDo,1860
-oci_mlflow-1.0.0.dist-info/METADATA,sha256=yx_WBjaH-gJlbhURkfjdWACoSvrFvIDIbBw0RVpXDQI,2156
-oci_mlflow-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-oci_mlflow-1.0.0.dist-info/entry_points.txt,sha256=o3F_Wjg0uvEgMbYAAKC8dEmQJLd750Y1u14raQN77Uk,243
-oci_mlflow-1.0.0.dist-info/top_level.txt,sha256=_4zSAoTy-jMuG5boO5gwRB9cI9WuD5x4ReALJaKH9Q0,11
-oci_mlflow-1.0.0.dist-info/RECORD,,
+oci_mlflow-1.0b0.dist-info/LICENSE.txt,sha256=0ggOnaxgPaQEBstfywBdLBJ-kO9cJ4shpvZplaXiSDo,1860
+oci_mlflow-1.0b0.dist-info/METADATA,sha256=XcTltXCpt_X2Wwi-G1pA2twilqLeVagosQWNbGvHXgA,2156
+oci_mlflow-1.0b0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+oci_mlflow-1.0b0.dist-info/entry_points.txt,sha256=o3F_Wjg0uvEgMbYAAKC8dEmQJLd750Y1u14raQN77Uk,243
+oci_mlflow-1.0b0.dist-info/top_level.txt,sha256=_4zSAoTy-jMuG5boO5gwRB9cI9WuD5x4ReALJaKH9Q0,11
+oci_mlflow-1.0b0.dist-info/RECORD,,
```

