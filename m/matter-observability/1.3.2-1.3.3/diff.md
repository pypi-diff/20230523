# Comparing `tmp/matter_observability-1.3.2-py3-none-any.whl.zip` & `tmp/matter_observability-1.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11242 bytes, number of entries: 21
+Zip file size: 11239 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_observability/__about__.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 matter_observability/__init__.py
 -rw-r--r--  2.0 unx      286 b- defN 20-Feb-02 00:00 matter_observability/config.py
 -rw-r--r--  2.0 unx      132 b- defN 20-Feb-02 00:00 matter_observability/exceptions.py
 -rw-r--r--  2.0 unx      133 b- defN 20-Feb-02 00:00 matter_observability/fastapi/__init__.py
 -rw-r--r--  2.0 unx      641 b- defN 20-Feb-02 00:00 matter_observability/fastapi/request_id.py
 -rw-r--r--  2.0 unx      817 b- defN 20-Feb-02 00:00 matter_observability/fastapi/utils.py
@@ -12,12 +12,12 @@
 -rw-r--r--  2.0 unx      761 b- defN 20-Feb-02 00:00 matter_observability/metrics/custom_metrics.py
 -rw-r--r--  2.0 unx     2428 b- defN 20-Feb-02 00:00 matter_observability/metrics/decorators.py
 -rw-r--r--  2.0 unx      473 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_counter.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge.py
 -rw-r--r--  2.0 unx      708 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge_duration.py
 -rw-r--r--  2.0 unx      421 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_metric.py
 -rw-r--r--  2.0 unx      903 b- defN 20-Feb-02 00:00 matter_observability/metrics/utils.py
-?rw-r--r--  2.0 unx     5852 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/RECORD
-21 files, 19504 bytes uncompressed, 7876 bytes compressed:  59.6%
+?rw-r--r--  2.0 unx     5852 b- defN 20-Feb-02 00:00 matter_observability-1.3.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-1.3.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-1.3.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-1.3.3.dist-info/RECORD
+21 files, 19504 bytes uncompressed, 7873 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: matter_observability/metrics/labeled_metric.py
 Comment: 
 
 Filename: matter_observability/metrics/utils.py
 Comment: 
 
-Filename: matter_observability-1.3.2.dist-info/METADATA
+Filename: matter_observability-1.3.3.dist-info/METADATA
 Comment: 
 
-Filename: matter_observability-1.3.2.dist-info/WHEEL
+Filename: matter_observability-1.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: matter_observability-1.3.2.dist-info/licenses/LICENSE
+Filename: matter_observability-1.3.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_observability-1.3.2.dist-info/RECORD
+Filename: matter_observability-1.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_observability/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.3.2"
+__version__ = "1.3.3"
```

## Comparing `matter_observability-1.3.2.dist-info/METADATA` & `matter_observability-1.3.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: matter-observability
-Version: 1.3.2
+Version: 1.3.3
 Summary: A template for Matter's observability library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-observability#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-observability/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-observability
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: matter-exceptions==1.1.*
+Requires-Dist: matter-exceptions>=1.1.0
 Requires-Dist: starlette-exporter==0.15.1
 Description-Content-Type: text/markdown
 
 # matter-observability
 
 **Table of Contents**
```

## Comparing `matter_observability-1.3.2.dist-info/licenses/LICENSE` & `matter_observability-1.3.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

