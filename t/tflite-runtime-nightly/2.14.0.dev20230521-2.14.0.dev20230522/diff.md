# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230521-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230522-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 2396295 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-May-22 04:51 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6814248 b- defN 23-May-22 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-May-22 04:51 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-May-22 04:51 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-May-22 04:51 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-May-22 04:53 tflite_runtime_nightly-2.14.0.dev20230521.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-May-22 04:53 tflite_runtime_nightly-2.14.0.dev20230521.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-May-22 04:53 tflite_runtime_nightly-2.14.0.dev20230521.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-May-22 04:53 tflite_runtime_nightly-2.14.0.dev20230521.dist-info/RECORD
+-rw-rw-r--  2.0 unx       80 b- defN 23-May-23 04:59 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6814248 b- defN 23-May-23 05:01 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-May-23 04:59 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-May-23 04:59 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-May-23 04:59 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-May-23 05:01 tflite_runtime_nightly-2.14.0.dev20230522.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-May-23 05:01 tflite_runtime_nightly-2.14.0.dev20230522.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-23 05:01 tflite_runtime_nightly-2.14.0.dev20230522.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-May-23 05:01 tflite_runtime_nightly-2.14.0.dev20230522.dist-info/RECORD
 9 files, 6859137 bytes uncompressed, 2394749 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230521.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230522.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230521.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230522.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230521.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230522.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230521.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230522.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230521'
-__git_version__ = '0.6.0-148128-g388d952114e'
+__version__ = '2.14.0dev20230522'
+__git_version__ = '0.6.0-148194-g9b2e41eca2d'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230521.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230522.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230521
+Version: 2.14.0.dev20230522
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230521.dist-info/RECORD` & `tflite_runtime_nightly-2.14.0.dev20230522.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=6hljTy18lY9PbaNQq5kVJwD6QioMq668Ws9I-Osub0Q,80
+tflite_runtime/__init__.py,sha256=NWt7wtRVEi9moFAWGGV5Dp1NBVlAkd4Qr7jdVQfMwcg,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=hLggXAxAEkFER6hntwmCxZYKJPOv4cYrw8Zg2vVfR_g,6814248
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.14.0.dev20230521.dist-info/METADATA,sha256=1Tu3TycY3lLImRR_v9oRVSJzz2FCcEAoLHUv65Mno04,1440
-tflite_runtime_nightly-2.14.0.dev20230521.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
-tflite_runtime_nightly-2.14.0.dev20230521.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.14.0.dev20230521.dist-info/RECORD,,
+tflite_runtime_nightly-2.14.0.dev20230522.dist-info/METADATA,sha256=k2LV3RuTu3Bdr52Uwgjgd2afWGnU9aw5OBSqOEexFlQ,1440
+tflite_runtime_nightly-2.14.0.dev20230522.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
+tflite_runtime_nightly-2.14.0.dev20230522.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.14.0.dev20230522.dist-info/RECORD,,
```

