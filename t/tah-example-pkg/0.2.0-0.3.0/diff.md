# Comparing `tmp/tah_example_pkg-0.2.0.tar.gz` & `tmp/tah_example_pkg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tah_example_pkg-0.2.0.tar", max compression
+gzip compressed data, was "tah_example_pkg-0.3.0.tar", max compression
```

## Comparing `tah_example_pkg-0.2.0.tar` & `tah_example_pkg-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 tah_example_pkg-0.2.0/README.md
--rw-r--r--   0        0        0      604 2023-05-23 19:50:19.176873 tah_example_pkg-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-05-23 19:18:29.148038 tah_example_pkg-0.2.0/src/model/__init__.py
--rwxr-xr-x   0        0        0     1907 2023-05-15 14:40:02.436185 tah_example_pkg-0.2.0/src/model/evaluate.py
--rw-r--r--   0        0        0     3994 2023-05-23 19:28:36.280423 tah_example_pkg-0.2.0/src/model/helpers.py
--rw-r--r--   0        0        0     1630 2023-05-23 19:29:35.621312 tah_example_pkg-0.2.0/src/model/model_class.py
--rwxr-xr-x   0        0        0     4709 2023-05-20 12:10:53.785322 tah_example_pkg-0.2.0/src/model/onnx_base.py
--rwxr-xr-x   0        0        0     1797 2023-05-23 18:46:58.183819 tah_example_pkg-0.2.0/src/model/predict.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 tah_example_pkg-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 tah_example_pkg-0.3.0/README.md
+-rw-r--r--   0        0        0      604 2023-05-23 20:00:02.831783 tah_example_pkg-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-05-23 19:18:29.148038 tah_example_pkg-0.3.0/src/model/__init__.py
+-rwxr-xr-x   0        0        0     1907 2023-05-15 14:40:02.436185 tah_example_pkg-0.3.0/src/model/evaluate.py
+-rw-r--r--   0        0        0     3994 2023-05-23 19:28:36.280423 tah_example_pkg-0.3.0/src/model/helpers.py
+-rw-r--r--   0        0        0     1630 2023-05-23 19:29:35.621312 tah_example_pkg-0.3.0/src/model/model_class.py
+-rwxr-xr-x   0        0        0     4709 2023-05-20 12:10:53.785322 tah_example_pkg-0.3.0/src/model/onnx_base.py
+-rwxr-xr-x   0        0        0     1797 2023-05-23 18:46:58.183819 tah_example_pkg-0.3.0/src/model/predict.py
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 tah_example_pkg-0.3.0/PKG-INFO
```

### Comparing `tah_example_pkg-0.2.0/README.md` & `tah_example_pkg-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.2.0/pyproject.toml` & `tah_example_pkg-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "tah-example-pkg"
-version = "0.2.0"
+name = "tah_example_pkg"
+version = "0.3.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "src/model"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `tah_example_pkg-0.2.0/src/model/evaluate.py` & `tah_example_pkg-0.3.0/src/model/evaluate.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.2.0/src/model/helpers.py` & `tah_example_pkg-0.3.0/src/model/helpers.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.2.0/src/model/model_class.py` & `tah_example_pkg-0.3.0/src/model/model_class.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.2.0/src/model/onnx_base.py` & `tah_example_pkg-0.3.0/src/model/onnx_base.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.2.0/src/model/predict.py` & `tah_example_pkg-0.3.0/src/model/predict.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.2.0/PKG-INFO` & `tah_example_pkg-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tah-example-pkg
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

