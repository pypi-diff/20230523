# Comparing `tmp/grpcio-reflection-1.9.0rc3.tar.gz` & `tmp/grpcio-reflection-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grpcio-reflection-1.9.0rc3.tar", last modified: Mon Jan 29 23:57:02 2018, max compression
+gzip compressed data, was "dist/grpcio-reflection-1.9.1.tar", last modified: Mon Feb  5 23:35:13 2018, max compression
```

## Comparing `grpcio-reflection-1.9.0rc3.tar` & `grpcio-reflection-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/
--rw-r--r--   0 root         (0) root         (0)       84 2018-01-29 23:45:42.000000 grpcio-reflection-1.9.0rc3/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/
--rw-r--r--   0 root         (0) root         (0)       39 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      769 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpc_reflection/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/
--rw-r--r--   0 root         (0) root         (0)    22345 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/reflection_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5947 2018-01-29 23:45:42.000000 grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/reflection.py
--rw-r--r--   0 root         (0) root         (0)     1869 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/reflection_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      577 2018-01-29 23:45:42.000000 grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)      577 2018-01-29 23:45:42.000000 grpcio-reflection-1.9.0rc3/grpc_reflection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2931 2018-01-29 23:45:42.000000 grpcio-reflection-1.9.0rc3/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      769 2018-01-29 23:57:02.000000 grpcio-reflection-1.9.0rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      702 2018-01-29 23:45:42.000000 grpcio-reflection-1.9.0rc3/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/
+-rw-r--r--   0 root         (0) root         (0)       84 2018-02-05 23:23:48.000000 grpcio-reflection-1.9.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpcio_reflection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       36 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpcio_reflection.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpcio_reflection.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpcio_reflection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      766 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpcio_reflection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpcio_reflection.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpc_reflection/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpc_reflection/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)    22345 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpc_reflection/v1alpha/reflection_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5947 2018-02-05 23:23:48.000000 grpcio-reflection-1.9.1/grpc_reflection/v1alpha/reflection.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/grpc_reflection/v1alpha/reflection_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      577 2018-02-05 23:23:48.000000 grpcio-reflection-1.9.1/grpc_reflection/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      577 2018-02-05 23:23:48.000000 grpcio-reflection-1.9.1/grpc_reflection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2931 2018-02-05 23:23:48.000000 grpcio-reflection-1.9.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      766 2018-02-05 23:35:13.000000 grpcio-reflection-1.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      699 2018-02-05 23:23:48.000000 grpcio-reflection-1.9.1/grpc_version.py
```

### Comparing `grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/PKG-INFO` & `grpcio-reflection-1.9.1/grpcio_reflection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: grpcio-reflection
-Version: 1.9.0rc3
+Version: 1.9.1
 Summary: Standard Protobuf Reflection Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `grpcio-reflection-1.9.0rc3/grpcio_reflection.egg-info/SOURCES.txt` & `grpcio-reflection-1.9.1/grpcio_reflection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/reflection_pb2.py` & `grpcio-reflection-1.9.1/grpc_reflection/v1alpha/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/reflection.py` & `grpcio-reflection-1.9.1/grpc_reflection/v1alpha/reflection.py`

 * *Files identical despite different names*

### Comparing `grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/reflection_pb2_grpc.py` & `grpcio-reflection-1.9.1/grpc_reflection/v1alpha/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-reflection-1.9.0rc3/grpc_reflection/v1alpha/__init__.py` & `grpcio-reflection-1.9.1/grpc_reflection/v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-reflection-1.9.0rc3/grpc_reflection/__init__.py` & `grpcio-reflection-1.9.1/grpc_reflection/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-reflection-1.9.0rc3/setup.py` & `grpcio-reflection-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `grpcio-reflection-1.9.0rc3/PKG-INFO` & `grpcio-reflection-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: grpcio-reflection
-Version: 1.9.0rc3
+Version: 1.9.1
 Summary: Standard Protobuf Reflection Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `grpcio-reflection-1.9.0rc3/grpc_version.py` & `grpcio-reflection-1.9.1/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_reflection/grpc_version.py.template`!!!
 
-VERSION = '1.9.0rc3'
+VERSION = '1.9.1'
```

