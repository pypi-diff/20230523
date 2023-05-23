# Comparing `tmp/iotics-grpc-client-3.0.0.tar.gz` & `tmp/iotics-grpc-client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotics-grpc-client-3.0.0.tar", last modified: Tue Jan 31 17:31:50 2023, max compression
+gzip compressed data, was "iotics-grpc-client-3.0.1.tar", last modified: Tue May 23 12:09:12 2023, max compression
```

## Comparing `iotics-grpc-client-3.0.0.tar` & `iotics-grpc-client-3.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:31:50.035401 iotics-grpc-client-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-01-31 17:31:50.035401 iotics-grpc-client-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-31 17:31:50.035401 iotics-grpc-client-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:31:50.031401 iotics-grpc-client-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:31:50.031401 iotics-grpc-client-3.0.0/src/iotics/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:31:50.035401 iotics-grpc-client-3.0.0/src/iotics/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/feed_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/feed_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/host_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/host_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/input_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/input_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/interest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/interest_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/meta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/meta_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/search_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/twin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/api/twin_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:31:50.035401 iotics-grpc-client-3.0.0/src/iotics/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:31:50.035401 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/interest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/iotics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-01-31 17:31:45.000000 iotics-grpc-client-3.0.0/src/iotics/lib/grpc/twins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 17:31:50.035401 iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-01-31 17:31:49.000000 iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-01-31 17:31:50.000000 iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 17:31:49.000000 iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-31 17:31:49.000000 iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-31 17:31:49.000000 iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 17:31:49.000000 iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:09:12.398499 iotics-grpc-client-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-05-23 12:09:12.398499 iotics-grpc-client-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-23 12:09:12.398499 iotics-grpc-client-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:09:12.390500 iotics-grpc-client-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:09:12.390500 iotics-grpc-client-3.0.1/src/iotics/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:09:12.394499 iotics-grpc-client-3.0.1/src/iotics/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/feed_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/feed_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/host_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/host_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/input_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/input_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/interest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/interest_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/meta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/meta_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/twin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/api/twin_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:09:12.394499 iotics-grpc-client-3.0.1/src/iotics/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:09:12.398499 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/interest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/iotics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-23 12:09:07.000000 iotics-grpc-client-3.0.1/src/iotics/lib/grpc/twins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:09:12.398499 iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-05-23 12:09:12.000000 iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-23 12:09:12.000000 iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:09:12.000000 iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 12:09:12.000000 iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 12:09:12.000000 iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:09:12.000000 iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/zip-safe
```

### Comparing `iotics-grpc-client-3.0.0/LICENSE` & `iotics-grpc-client-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/PKG-INFO` & `iotics-grpc-client-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotics-grpc-client
-Version: 3.0.0
+Version: 3.0.1
 Summary: Iotics gRPC client library
 Home-page: https://github.com/Iotic-Labs/iotics-grpc-client-py
 Author: Iotics
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Iotic-Labs/iotics-grpc-client-py/issues
 Project-URL: Changelog, https://github.com/Iotic-Labs/iotics-grpc-client-py/releases
 Description: # Iotics gRPC Python Client
```

### Comparing `iotics-grpc-client-3.0.0/README.md` & `iotics-grpc-client-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/setup.cfg` & `iotics-grpc-client-3.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iotics-grpc-client
-version = 3.0.0
+version = 3.0.1
 description = Iotics gRPC client library
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Iotics
 platform = any
 url = https://github.com/Iotic-Labs/iotics-grpc-client-py
 keywords = iotics, grpc, digital twin
@@ -31,15 +31,15 @@
 	googleapis-common-protos>=1.56.3
 	grpcio>=1.50.0
 
 [options.extras_require]
 dev = 
 	mypy-protobuf>=3.2.0
 	python-dotenv>=0.20.0
-	iotics-identity>=1.0.2
+	iotics-identity>=1.0.4
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `iotics-grpc-client-3.0.0/src/iotics/__init__.py` & `iotics-grpc-client-3.0.1/src/iotics/__init__.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/common_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/common_pb2.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/feed_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/feed_pb2.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/feed_pb2_grpc.py` & `iotics-grpc-client-3.0.1/src/iotics/api/feed_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/host_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/host_pb2.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/host_pb2_grpc.py` & `iotics-grpc-client-3.0.1/src/iotics/api/host_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/input_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/input_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from iotics.api import common_pb2 as iotics_dot_api_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16iotics/api/input.proto\x12\niotics.api\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17iotics/api/common.proto\"I\n\x07InputID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x16\n\x06twinId\x18\x02 \x01(\tR\x06twinId\x12\x16\n\x06hostId\x18\x03 \x01(\tR\x06hostId\"\xbd\x01\n\x12\x44\x65leteInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12<\n\x04\x61rgs\x18\x02 \x01(\x0b\x32(.iotics.api.DeleteInputRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x13\x44\x65leteInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.DeleteInputResponse.PayloadR\x07payload\x1a\x38\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x14\x44\x65scribeInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12>\n\x04\x61rgs\x18\x02 \x01(\x0b\x32*.iotics.api.DescribeInputRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xfa\x02\n\x15\x44\x65scribeInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x43\n\x07payload\x18\x02 \x01(\x0b\x32).iotics.api.DescribeInputResponse.PayloadR\x07payload\x1am\n\nMetaResult\x12)\n\x06values\x18\x01 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x34\n\nproperties\x18\x02 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\x1a~\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\x12\x44\n\x06result\x18\x02 \x01(\x0b\x32,.iotics.api.DescribeInputResponse.MetaResultR\x06result\"\x86\x01\n\x13UpsertInputWithMeta\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12)\n\x06values\x18\x02 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x34\n\nproperties\x18\x03 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\"r\n\x0cInputMessage\x12:\n\noccurredAt\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x12\n\x04mime\x18\x02 \x01(\tR\x04mime\x12\x12\n\x04\x64\x61ta\x18\x03 \x01(\x0cR\x04\x64\x61ta\"\xcd\x01\n\x1aReceiveInputMessageRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x44\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x30.iotics.api.ReceiveInputMessageRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\x85\x02\n\x1bReceiveInputMessageResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12I\n\x07payload\x18\x02 \x01(\x0b\x32/.iotics.api.ReceiveInputMessageResponse.PayloadR\x07payload\x1al\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\x12\x32\n\x07message\x18\x02 \x01(\x0b\x32\x18.iotics.api.InputMessageR\x07message2\xa1\x02\n\x08InputAPI\x12P\n\x0b\x44\x65leteInput\x12\x1e.iotics.api.DeleteInputRequest\x1a\x1f.iotics.api.DeleteInputResponse\"\x00\x12V\n\rDescribeInput\x12 .iotics.api.DescribeInputRequest\x1a!.iotics.api.DescribeInputResponse\"\x00\x12k\n\x14ReceiveInputMessages\x12&.iotics.api.ReceiveInputMessageRequest\x1a\'.iotics.api.ReceiveInputMessageResponse\"\x00\x30\x01\x42~\n\x0e\x63om.iotics.apiB\nInputProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16iotics/api/input.proto\x12\niotics.api\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17iotics/api/common.proto\"I\n\x07InputID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x16\n\x06twinId\x18\x02 \x01(\tR\x06twinId\x12\x16\n\x06hostId\x18\x03 \x01(\tR\x06hostId\"\xbd\x01\n\x12\x44\x65leteInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12<\n\x04\x61rgs\x18\x02 \x01(\x0b\x32(.iotics.api.DeleteInputRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x13\x44\x65leteInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.DeleteInputResponse.PayloadR\x07payload\x1a\x38\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\x97\x02\n\x12\x43reateInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12<\n\x04\x61rgs\x18\x02 \x01(\x0b\x32(.iotics.api.CreateInputRequest.ArgumentsR\x04\x61rgs\x12@\n\x07payload\x18\x03 \x01(\x0b\x32&.iotics.api.CreateInputRequest.PayloadR\x07payload\x1a\x19\n\x07Payload\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x1a\x37\n\tArguments\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\xc1\x01\n\x13\x43reateInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.CreateInputResponse.PayloadR\x07payload\x1a\x38\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xf2\x02\n\x12UpdateInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12<\n\x04\x61rgs\x18\x02 \x01(\x0b\x32(.iotics.api.UpdateInputRequest.ArgumentsR\x04\x61rgs\x12@\n\x07payload\x18\x03 \x01(\x0b\x32&.iotics.api.UpdateInputRequest.PayloadR\x07payload\x1aq\n\x07Payload\x12*\n\x06values\x18\x01 \x01(\x0b\x32\x12.iotics.api.ValuesR\x06values\x12:\n\nproperties\x18\x02 \x01(\x0b\x32\x1a.iotics.api.PropertyUpdateR\nproperties\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x13UpdateInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.UpdateInputResponse.PayloadR\x07payload\x1a\x38\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x14\x44\x65scribeInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12>\n\x04\x61rgs\x18\x02 \x01(\x0b\x32*.iotics.api.DescribeInputRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xfa\x02\n\x15\x44\x65scribeInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x43\n\x07payload\x18\x02 \x01(\x0b\x32).iotics.api.DescribeInputResponse.PayloadR\x07payload\x1am\n\nMetaResult\x12)\n\x06values\x18\x01 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x34\n\nproperties\x18\x02 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\x1a~\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\x12\x44\n\x06result\x18\x02 \x01(\x0b\x32,.iotics.api.DescribeInputResponse.MetaResultR\x06result\"\x86\x01\n\x13UpsertInputWithMeta\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12)\n\x06values\x18\x02 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x34\n\nproperties\x18\x03 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\"r\n\x0cInputMessage\x12:\n\noccurredAt\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x12\n\x04mime\x18\x02 \x01(\tR\x04mime\x12\x12\n\x04\x64\x61ta\x18\x03 \x01(\x0cR\x04\x64\x61ta\"\xcd\x01\n\x1aReceiveInputMessageRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x44\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x30.iotics.api.ReceiveInputMessageRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\x85\x02\n\x1bReceiveInputMessageResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12I\n\x07payload\x18\x02 \x01(\x0b\x32/.iotics.api.ReceiveInputMessageResponse.PayloadR\x07payload\x1al\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\x12\x32\n\x07message\x18\x02 \x01(\x0b\x32\x18.iotics.api.InputMessageR\x07message2\xc5\x03\n\x08InputAPI\x12P\n\x0b\x44\x65leteInput\x12\x1e.iotics.api.DeleteInputRequest\x1a\x1f.iotics.api.DeleteInputResponse\"\x00\x12V\n\rDescribeInput\x12 .iotics.api.DescribeInputRequest\x1a!.iotics.api.DescribeInputResponse\"\x00\x12k\n\x14ReceiveInputMessages\x12&.iotics.api.ReceiveInputMessageRequest\x1a\'.iotics.api.ReceiveInputMessageResponse\"\x00\x30\x01\x12P\n\x0b\x43reateInput\x12\x1e.iotics.api.CreateInputRequest\x1a\x1f.iotics.api.CreateInputResponse\"\x00\x12P\n\x0bUpdateInput\x12\x1e.iotics.api.UpdateInputRequest\x1a\x1f.iotics.api.UpdateInputResponse\"\x00\x42~\n\x0e\x63om.iotics.apiB\nInputProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.input_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.iotics.apiB\nInputProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
@@ -29,32 +29,52 @@
   _DELETEINPUTREQUEST._serialized_end=361
   _DELETEINPUTREQUEST_ARGUMENTS._serialized_start=303
   _DELETEINPUTREQUEST_ARGUMENTS._serialized_end=361
   _DELETEINPUTRESPONSE._serialized_start=364
   _DELETEINPUTRESPONSE._serialized_end=557
   _DELETEINPUTRESPONSE_PAYLOAD._serialized_start=501
   _DELETEINPUTRESPONSE_PAYLOAD._serialized_end=557
-  _DESCRIBEINPUTREQUEST._serialized_start=560
-  _DESCRIBEINPUTREQUEST._serialized_end=753
+  _CREATEINPUTREQUEST._serialized_start=560
+  _CREATEINPUTREQUEST._serialized_end=839
+  _CREATEINPUTREQUEST_PAYLOAD._serialized_start=757
+  _CREATEINPUTREQUEST_PAYLOAD._serialized_end=782
+  _CREATEINPUTREQUEST_ARGUMENTS._serialized_start=784
+  _CREATEINPUTREQUEST_ARGUMENTS._serialized_end=839
+  _CREATEINPUTRESPONSE._serialized_start=842
+  _CREATEINPUTRESPONSE._serialized_end=1035
+  _CREATEINPUTRESPONSE_PAYLOAD._serialized_start=501
+  _CREATEINPUTRESPONSE_PAYLOAD._serialized_end=557
+  _UPDATEINPUTREQUEST._serialized_start=1038
+  _UPDATEINPUTREQUEST._serialized_end=1408
+  _UPDATEINPUTREQUEST_PAYLOAD._serialized_start=1235
+  _UPDATEINPUTREQUEST_PAYLOAD._serialized_end=1348
+  _UPDATEINPUTREQUEST_ARGUMENTS._serialized_start=303
+  _UPDATEINPUTREQUEST_ARGUMENTS._serialized_end=361
+  _UPDATEINPUTRESPONSE._serialized_start=1411
+  _UPDATEINPUTRESPONSE._serialized_end=1604
+  _UPDATEINPUTRESPONSE_PAYLOAD._serialized_start=501
+  _UPDATEINPUTRESPONSE_PAYLOAD._serialized_end=557
+  _DESCRIBEINPUTREQUEST._serialized_start=1607
+  _DESCRIBEINPUTREQUEST._serialized_end=1800
   _DESCRIBEINPUTREQUEST_ARGUMENTS._serialized_start=303
   _DESCRIBEINPUTREQUEST_ARGUMENTS._serialized_end=361
-  _DESCRIBEINPUTRESPONSE._serialized_start=756
-  _DESCRIBEINPUTRESPONSE._serialized_end=1134
-  _DESCRIBEINPUTRESPONSE_METARESULT._serialized_start=897
-  _DESCRIBEINPUTRESPONSE_METARESULT._serialized_end=1006
-  _DESCRIBEINPUTRESPONSE_PAYLOAD._serialized_start=1008
-  _DESCRIBEINPUTRESPONSE_PAYLOAD._serialized_end=1134
-  _UPSERTINPUTWITHMETA._serialized_start=1137
-  _UPSERTINPUTWITHMETA._serialized_end=1271
-  _INPUTMESSAGE._serialized_start=1273
-  _INPUTMESSAGE._serialized_end=1387
-  _RECEIVEINPUTMESSAGEREQUEST._serialized_start=1390
-  _RECEIVEINPUTMESSAGEREQUEST._serialized_end=1595
+  _DESCRIBEINPUTRESPONSE._serialized_start=1803
+  _DESCRIBEINPUTRESPONSE._serialized_end=2181
+  _DESCRIBEINPUTRESPONSE_METARESULT._serialized_start=1944
+  _DESCRIBEINPUTRESPONSE_METARESULT._serialized_end=2053
+  _DESCRIBEINPUTRESPONSE_PAYLOAD._serialized_start=2055
+  _DESCRIBEINPUTRESPONSE_PAYLOAD._serialized_end=2181
+  _UPSERTINPUTWITHMETA._serialized_start=2184
+  _UPSERTINPUTWITHMETA._serialized_end=2318
+  _INPUTMESSAGE._serialized_start=2320
+  _INPUTMESSAGE._serialized_end=2434
+  _RECEIVEINPUTMESSAGEREQUEST._serialized_start=2437
+  _RECEIVEINPUTMESSAGEREQUEST._serialized_end=2642
   _RECEIVEINPUTMESSAGEREQUEST_ARGUMENTS._serialized_start=303
   _RECEIVEINPUTMESSAGEREQUEST_ARGUMENTS._serialized_end=361
-  _RECEIVEINPUTMESSAGERESPONSE._serialized_start=1598
-  _RECEIVEINPUTMESSAGERESPONSE._serialized_end=1859
-  _RECEIVEINPUTMESSAGERESPONSE_PAYLOAD._serialized_start=1751
-  _RECEIVEINPUTMESSAGERESPONSE_PAYLOAD._serialized_end=1859
-  _INPUTAPI._serialized_start=1862
-  _INPUTAPI._serialized_end=2151
+  _RECEIVEINPUTMESSAGERESPONSE._serialized_start=2645
+  _RECEIVEINPUTMESSAGERESPONSE._serialized_end=2906
+  _RECEIVEINPUTMESSAGERESPONSE_PAYLOAD._serialized_start=2798
+  _RECEIVEINPUTMESSAGERESPONSE_PAYLOAD._serialized_end=2906
+  _INPUTAPI._serialized_start=2909
+  _INPUTAPI._serialized_end=3362
 # @@protoc_insertion_point(module_scope)
```

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/input_pb2_grpc.py` & `iotics-grpc-client-3.0.1/src/iotics/api/input_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,24 @@
                 response_deserializer=iotics_dot_api_dot_input__pb2.DescribeInputResponse.FromString,
                 )
         self.ReceiveInputMessages = channel.unary_stream(
                 '/iotics.api.InputAPI/ReceiveInputMessages',
                 request_serializer=iotics_dot_api_dot_input__pb2.ReceiveInputMessageRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_input__pb2.ReceiveInputMessageResponse.FromString,
                 )
+        self.CreateInput = channel.unary_unary(
+                '/iotics.api.InputAPI/CreateInput',
+                request_serializer=iotics_dot_api_dot_input__pb2.CreateInputRequest.SerializeToString,
+                response_deserializer=iotics_dot_api_dot_input__pb2.CreateInputResponse.FromString,
+                )
+        self.UpdateInput = channel.unary_unary(
+                '/iotics.api.InputAPI/UpdateInput',
+                request_serializer=iotics_dot_api_dot_input__pb2.UpdateInputRequest.SerializeToString,
+                response_deserializer=iotics_dot_api_dot_input__pb2.UpdateInputResponse.FromString,
+                )
 
 
 class InputAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     Input API groups all the actions link to a twin input.
     Services only affect local resources, unless stated otherwise.
@@ -59,14 +69,28 @@
     def ReceiveInputMessages(self, request, context):
         """Receives input messages for a specific input.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def CreateInput(self, request, context):
+        """Creates an input owned by a twin. (Idempotent)
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UpdateInput(self, request, context):
+        """Updates attributes of an input, including its metadata.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_InputAPIServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'DeleteInput': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteInput,
                     request_deserializer=iotics_dot_api_dot_input__pb2.DeleteInputRequest.FromString,
                     response_serializer=iotics_dot_api_dot_input__pb2.DeleteInputResponse.SerializeToString,
@@ -77,14 +101,24 @@
                     response_serializer=iotics_dot_api_dot_input__pb2.DescribeInputResponse.SerializeToString,
             ),
             'ReceiveInputMessages': grpc.unary_stream_rpc_method_handler(
                     servicer.ReceiveInputMessages,
                     request_deserializer=iotics_dot_api_dot_input__pb2.ReceiveInputMessageRequest.FromString,
                     response_serializer=iotics_dot_api_dot_input__pb2.ReceiveInputMessageResponse.SerializeToString,
             ),
+            'CreateInput': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateInput,
+                    request_deserializer=iotics_dot_api_dot_input__pb2.CreateInputRequest.FromString,
+                    response_serializer=iotics_dot_api_dot_input__pb2.CreateInputResponse.SerializeToString,
+            ),
+            'UpdateInput': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateInput,
+                    request_deserializer=iotics_dot_api_dot_input__pb2.UpdateInputRequest.FromString,
+                    response_serializer=iotics_dot_api_dot_input__pb2.UpdateInputResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.InputAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -141,7 +175,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/iotics.api.InputAPI/ReceiveInputMessages',
             iotics_dot_api_dot_input__pb2.ReceiveInputMessageRequest.SerializeToString,
             iotics_dot_api_dot_input__pb2.ReceiveInputMessageResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateInput(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iotics.api.InputAPI/CreateInput',
+            iotics_dot_api_dot_input__pb2.CreateInputRequest.SerializeToString,
+            iotics_dot_api_dot_input__pb2.CreateInputResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UpdateInput(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iotics.api.InputAPI/UpdateInput',
+            iotics_dot_api_dot_input__pb2.UpdateInputRequest.SerializeToString,
+            iotics_dot_api_dot_input__pb2.UpdateInputResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/interest_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/interest_pb2.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/interest_pb2_grpc.py` & `iotics-grpc-client-3.0.1/src/iotics/api/interest_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/meta_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/meta_pb2_grpc.py` & `iotics-grpc-client-3.0.1/src/iotics/api/meta_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/search_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/search_pb2.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/search_pb2_grpc.py` & `iotics-grpc-client-3.0.1/src/iotics/api/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/twin_pb2.py` & `iotics-grpc-client-3.0.1/src/iotics/api/twin_pb2.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/api/twin_pb2_grpc.py` & `iotics-grpc-client-3.0.1/src/iotics/api/twin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/__init__.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/__init__.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from iotics.api.interest_pb2 import FetchInterestResponse
 from iotics.api.search_pb2 import SearchRequest, SearchResponse
 from iotics.api.meta_pb2 import SparqlQueryResponse, SparqlResultType, SparqlUpdateResponse
 from iotics.api.twin_pb2 import CreateTwinResponse, DeleteTwinResponse, DescribeTwinResponse, ListAllTwinsResponse, \
     UpdateTwinResponse, UpsertTwinResponse
 from iotics.lib.grpc.iotics_api import IoticsApi
 from iotics.lib.grpc.feeds import FeedApi
+from iotics.lib.grpc.input import InputApi
 from iotics.lib.grpc.interest import InterestApi
 from iotics.lib.grpc.search import SearchApi
 from iotics.lib.grpc.sparql import SparqlApi
 from iotics.lib.grpc.twins import TwinApi
 from iotics.lib.grpc.helpers import *
 
 del globals()['get_channel']
```

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/auth.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/auth.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/base.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/base.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/feeds.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/feeds.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/helpers.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/helpers.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/host.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/host.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/interest.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/interest.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/iotics_api.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/iotics_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,16 @@
         self.update_feed = self.feed_api.update_feed
         self.share_feed_data = self.feed_api.share_feed_data
         self.list_all_feeds = self.feed_api.list_all_feeds
         self.describe_feed = self.feed_api.describe_feed
 
     def _initialise_input_api(self):
         self._input_api = InputApi(self._auth, self._channel)
+        self.create_input = self.input_api.create_input
+        self.update_input = self.input_api.update_input
         self.describe_input = self.input_api.describe_input
         self.delete_input = self.input_api.delete_input
         self.receive_input_messages = self.input_api.receive_input_messages
 
     def _initialise_interest_api(self):
         self._interest_api = InterestApi(self._auth, self._channel)
         self.send_input_message = self.interest_api.send_input_message
```

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/search.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/search.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/sparql.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/sparql.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics/lib/grpc/twins.py` & `iotics-grpc-client-3.0.1/src/iotics/lib/grpc/twins.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/PKG-INFO` & `iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotics-grpc-client
-Version: 3.0.0
+Version: 3.0.1
 Summary: Iotics gRPC client library
 Home-page: https://github.com/Iotic-Labs/iotics-grpc-client-py
 Author: Iotics
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Iotic-Labs/iotics-grpc-client-py/issues
 Project-URL: Changelog, https://github.com/Iotic-Labs/iotics-grpc-client-py/releases
 Description: # Iotics gRPC Python Client
```

### Comparing `iotics-grpc-client-3.0.0/src/iotics_grpc_client.egg-info/SOURCES.txt` & `iotics-grpc-client-3.0.1/src/iotics_grpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

