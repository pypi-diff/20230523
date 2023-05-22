# Comparing `tmp/grpcio-status-1.55.0.tar.gz` & `tmp/grpcio-status-1.55.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-status-1.55.0.tar", last modified: Fri May 19 00:11:42 2023, max compression
+gzip compressed data, was "grpcio-status-1.55.0rc1.tar", last modified: Wed Apr 26 10:35:46 2023, max compression
```

## Comparing `grpcio-status-1.55.0.tar` & `grpcio-status-1.55.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 00:11:42.537476 grpcio-status-1.55.0/
--rw-r--r--   0 root         (0) root         (0)    29687 2023-05-19 00:11:42.000000 grpcio-status-1.55.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1136 2023-05-19 00:11:42.537476 grpcio-status-1.55.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 00:11:42.533475 grpcio-status-1.55.0/grpc_status/
--rw-r--r--   0 root         (0) root         (0)      580 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/grpc_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/grpc_status/_async.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/grpc_status/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 00:11:42.529475 grpcio-status-1.55.0/grpc_status/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 00:11:42.533475 grpcio-status-1.55.0/grpc_status/google/rpc/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-05-19 00:11:42.000000 grpcio-status-1.55.0/grpc_status/google/rpc/status.proto
--rw-r--r--   0 root         (0) root         (0)     3017 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/grpc_status/rpc_status.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 00:11:42.537476 grpcio-status-1.55.0/grpcio_status.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-05-19 00:11:42.000000 grpcio-status-1.55.0/grpcio_status.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-19 00:11:42.000000 grpcio-status-1.55.0/grpcio_status.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 00:11:42.000000 grpcio-status-1.55.0/grpcio_status.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-19 00:11:42.000000 grpcio-status-1.55.0/grpcio_status.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-19 00:11:42.000000 grpcio-status-1.55.0/grpcio_status.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 00:11:42.537476 grpcio-status-1.55.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3236 2023-05-19 00:03:20.000000 grpcio-status-1.55.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:46.872168 grpcio-status-1.55.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    29687 2023-04-26 10:35:46.000000 grpcio-status-1.55.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-26 10:35:46.872168 grpcio-status-1.55.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:46.868168 grpcio-status-1.55.0rc1/grpc_status/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/grpc_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/grpc_status/_async.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/grpc_status/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:46.860167 grpcio-status-1.55.0rc1/grpc_status/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:46.872168 grpcio-status-1.55.0rc1/grpc_status/google/rpc/
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-04-26 10:35:46.000000 grpcio-status-1.55.0rc1/grpc_status/google/rpc/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/grpc_status/rpc_status.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:46.872168 grpcio-status-1.55.0rc1/grpcio_status.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-26 10:35:46.000000 grpcio-status-1.55.0rc1/grpcio_status.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-26 10:35:46.000000 grpcio-status-1.55.0rc1/grpcio_status.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:35:46.000000 grpcio-status-1.55.0rc1/grpcio_status.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-26 10:35:46.000000 grpcio-status-1.55.0rc1/grpcio_status.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 10:35:46.000000 grpcio-status-1.55.0rc1/grpcio_status.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:35:46.872168 grpcio-status-1.55.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3236 2023-04-26 10:25:03.000000 grpcio-status-1.55.0rc1/setup.py
```

### Comparing `grpcio-status-1.55.0/LICENSE` & `grpcio-status-1.55.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.55.0/PKG-INFO` & `grpcio-status-1.55.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.55.0
+Version: 1.55.0rc1
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-status-1.55.0/grpc_status/__init__.py` & `grpcio-status-1.55.0rc1/grpc_status/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.55.0/grpc_status/_async.py` & `grpcio-status-1.55.0rc1/grpc_status/_async.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.55.0/grpc_status/_common.py` & `grpcio-status-1.55.0rc1/grpc_status/_common.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.55.0/grpc_status/google/rpc/status.proto` & `grpcio-status-1.55.0rc1/grpc_status/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.55.0/grpc_status/rpc_status.py` & `grpcio-status-1.55.0rc1/grpc_status/rpc_status.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.55.0/grpc_version.py` & `grpcio-status-1.55.0rc1/grpc_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_status/grpc_version.py.template`!!!
 
-VERSION = '1.55.0'
+VERSION = '1.55.0rc1'
```

### Comparing `grpcio-status-1.55.0/grpcio_status.egg-info/PKG-INFO` & `grpcio-status-1.55.0rc1/grpcio_status.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.55.0
+Version: 1.55.0rc1
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-status-1.55.0/setup.py` & `grpcio-status-1.55.0rc1/setup.py`

 * *Files identical despite different names*

