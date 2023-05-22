# Comparing `tmp/isolate_proto-0.0.8.tar.gz` & `tmp/isolate_proto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isolate_proto-0.0.8.tar", max compression
+gzip compressed data, was "isolate_proto-0.0.9.tar", max compression
```

## Comparing `isolate_proto-0.0.8.tar` & `isolate_proto-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      140 2022-12-09 06:39:04.479421 isolate_proto-0.0.8/README.md
--rw-r--r--   0        0        0      408 2022-12-09 06:39:04.479421 isolate_proto-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      575 2022-12-09 06:39:04.479421 isolate_proto-0.0.8/src/isolate_proto/__init__.py
--rw-r--r--   0        0        0     4449 2022-12-09 06:39:04.479421 isolate_proto-0.0.8/src/isolate_proto/controller.proto
--rw-r--r--   0        0        0     6003 2022-12-09 06:39:04.479421 isolate_proto-0.0.8/src/isolate_proto/controller_pb2.py
--rw-r--r--   0        0        0    16700 2022-12-09 06:39:04.479421 isolate_proto-0.0.8/src/isolate_proto/controller_pb2.pyi
--rw-r--r--   0        0        0    12717 2022-12-09 06:39:04.479421 isolate_proto-0.0.8/src/isolate_proto/controller_pb2_grpc.py
--rw-r--r--   0        0        0      873 2022-12-09 06:39:18.118603 isolate_proto-0.0.8/setup.py
--rw-r--r--   0        0        0      719 2022-12-09 06:39:18.118945 isolate_proto-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      140 2022-12-09 06:42:06.325994 isolate_proto-0.0.9/README.md
+-rw-r--r--   0        0        0      408 2022-12-09 06:42:06.329994 isolate_proto-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      575 2022-12-09 06:42:06.329994 isolate_proto-0.0.9/src/isolate_proto/__init__.py
+-rw-r--r--   0        0        0     4449 2022-12-09 06:42:06.329994 isolate_proto-0.0.9/src/isolate_proto/controller.proto
+-rw-r--r--   0        0        0     6003 2022-12-09 06:42:06.329994 isolate_proto-0.0.9/src/isolate_proto/controller_pb2.py
+-rw-r--r--   0        0        0    16700 2022-12-09 06:42:06.329994 isolate_proto-0.0.9/src/isolate_proto/controller_pb2.pyi
+-rw-r--r--   0        0        0    12717 2022-12-09 06:42:06.329994 isolate_proto-0.0.9/src/isolate_proto/controller_pb2_grpc.py
+-rw-r--r--   0        0        0      873 2022-12-09 06:42:18.579863 isolate_proto-0.0.9/setup.py
+-rw-r--r--   0        0        0      719 2022-12-09 06:42:18.580205 isolate_proto-0.0.9/PKG-INFO
```

### Comparing `isolate_proto-0.0.8/src/isolate_proto/__init__.py` & `isolate_proto-0.0.9/src/isolate_proto/__init__.py`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.0.8/src/isolate_proto/controller.proto` & `isolate_proto-0.0.9/src/isolate_proto/controller.proto`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.0.8/src/isolate_proto/controller_pb2.py` & `isolate_proto-0.0.9/src/isolate_proto/controller_pb2.py`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.0.8/src/isolate_proto/controller_pb2.pyi` & `isolate_proto-0.0.9/src/isolate_proto/controller_pb2.pyi`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.0.8/src/isolate_proto/controller_pb2_grpc.py` & `isolate_proto-0.0.9/src/isolate_proto/controller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.0.8/setup.py` & `isolate_proto-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['grpcio>=1.49', 'isolate[grpc]>=0.7,<0.8', 'protobuf']
 
 setup_kwargs = {
     'name': 'isolate-proto',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '(internal) gRPC definitions for Isolate Cloud',
     'long_description': '# gRPC definitions\n\nFor regenerating definitions\n\n```\n$ python tools/regen_grpc.py src/isolate_proto/controller.proto <isolate version>\n```\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `isolate_proto-0.0.8/PKG-INFO` & `isolate_proto-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isolate-proto
-Version: 0.0.8
+Version: 0.0.9
 Summary: (internal) gRPC definitions for Isolate Cloud
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

