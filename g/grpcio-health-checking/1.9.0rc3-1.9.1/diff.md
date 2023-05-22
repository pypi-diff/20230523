# Comparing `tmp/grpcio-health-checking-1.9.0rc3.tar.gz` & `tmp/grpcio-health-checking-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grpcio-health-checking-1.9.0rc3.tar", last modified: Mon Jan 29 23:57:01 2018, max compression
+gzip compressed data, was "dist/grpcio-health-checking-1.9.1.tar", last modified: Mon Feb  5 23:35:12 2018, max compression
```

## Comparing `grpcio-health-checking-1.9.0rc3.tar` & `grpcio-health-checking-1.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/
--rw-r--r--   0 root         (0) root         (0)       39 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      770 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      564 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       80 2018-01-29 23:45:42.000000 grpcio-health-checking-1.9.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2910 2018-01-29 23:45:42.000000 grpcio-health-checking-1.9.0rc3/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpc_health/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpc_health/v1/
--rw-r--r--   0 root         (0) root         (0)     5223 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpc_health/v1/health_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1550 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/grpc_health/v1/health_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1726 2018-01-29 23:45:42.000000 grpcio-health-checking-1.9.0rc3/grpc_health/v1/health.py
--rw-r--r--   0 root         (0) root         (0)      577 2018-01-29 23:45:42.000000 grpcio-health-checking-1.9.0rc3/grpc_health/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      577 2018-01-29 23:45:42.000000 grpcio-health-checking-1.9.0rc3/grpc_health/__init__.py
--rw-r--r--   0 root         (0) root         (0)      770 2018-01-29 23:57:01.000000 grpcio-health-checking-1.9.0rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      707 2018-01-29 23:45:42.000000 grpcio-health-checking-1.9.0rc3/grpc_version.py
--rw-r--r--   0 root         (0) root         (0)      215 2018-01-29 23:45:42.000000 grpcio-health-checking-1.9.0rc3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       36 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      767 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2018-02-05 23:23:48.000000 grpcio-health-checking-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2910 2018-02-05 23:23:48.000000 grpcio-health-checking-1.9.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpc_health/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpc_health/v1/
+-rw-r--r--   0 root         (0) root         (0)     5223 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpc_health/v1/health_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/grpc_health/v1/health_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2018-02-05 23:23:48.000000 grpcio-health-checking-1.9.1/grpc_health/v1/health.py
+-rw-r--r--   0 root         (0) root         (0)      577 2018-02-05 23:23:48.000000 grpcio-health-checking-1.9.1/grpc_health/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      577 2018-02-05 23:23:48.000000 grpcio-health-checking-1.9.1/grpc_health/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      767 2018-02-05 23:35:12.000000 grpcio-health-checking-1.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2018-02-05 23:23:48.000000 grpcio-health-checking-1.9.1/grpc_version.py
+-rw-r--r--   0 root         (0) root         (0)      215 2018-02-05 23:23:48.000000 grpcio-health-checking-1.9.1/README.rst
```

### Comparing `grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/PKG-INFO` & `grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: grpcio-health-checking
-Version: 1.9.0rc3
+Version: 1.9.1
 Summary: Standard Health Checking Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `grpcio-health-checking-1.9.0rc3/grpcio_health_checking.egg-info/SOURCES.txt` & `grpcio-health-checking-1.9.1/grpcio_health_checking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-health-checking-1.9.0rc3/setup.py` & `grpcio-health-checking-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `grpcio-health-checking-1.9.0rc3/grpc_health/v1/health_pb2.py` & `grpcio-health-checking-1.9.1/grpc_health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `grpcio-health-checking-1.9.0rc3/grpc_health/v1/health_pb2_grpc.py` & `grpcio-health-checking-1.9.1/grpc_health/v1/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-health-checking-1.9.0rc3/grpc_health/v1/health.py` & `grpcio-health-checking-1.9.1/grpc_health/v1/health.py`

 * *Files identical despite different names*

### Comparing `grpcio-health-checking-1.9.0rc3/grpc_health/v1/__init__.py` & `grpcio-health-checking-1.9.1/grpc_health/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-health-checking-1.9.0rc3/grpc_health/__init__.py` & `grpcio-health-checking-1.9.1/grpc_health/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-health-checking-1.9.0rc3/PKG-INFO` & `grpcio-health-checking-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: grpcio-health-checking
-Version: 1.9.0rc3
+Version: 1.9.1
 Summary: Standard Health Checking Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `grpcio-health-checking-1.9.0rc3/grpc_version.py` & `grpcio-health-checking-1.9.1/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_health_checking/grpc_version.py.template`!!!
 
-VERSION = '1.9.0rc3'
+VERSION = '1.9.1'
```

