# Comparing `tmp/rudderclient-1.1.1.tar.gz` & `tmp/rudderclient-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.1.1.tar", last modified: Tue May 23 06:16:06 2023, max compression
+gzip compressed data, was "rudderclient-1.2.0.tar", last modified: Tue May 23 08:15:59 2023, max compression
```

## Comparing `rudderclient-1.1.1.tar` & `rudderclient-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 06:16:06.393255 rudderclient-1.1.1/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1069 2023-05-17 06:37:36.000000 rudderclient-1.1.1/LICENSE
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1934 2023-05-23 06:16:06.393255 rudderclient-1.1.1/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      224 2023-05-22 12:05:46.000000 rudderclient-1.1.1/README.md
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 06:16:06.393255 rudderclient-1.1.1/gcp/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-22 12:05:46.000000 rudderclient-1.1.1/gcp/__init__.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      847 2023-05-22 12:24:42.000000 rudderclient-1.1.1/gcp/auth.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      338 2023-05-22 12:24:42.000000 rudderclient-1.1.1/gcp/http_requests.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      636 2023-05-23 06:15:55.000000 rudderclient-1.1.1/pyproject.toml
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 06:16:06.393255 rudderclient-1.1.1/rudderclient.egg-info/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1934 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      260 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/SOURCES.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        1 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/dependency_links.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       28 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/requires.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        4 2023-05-23 06:16:06.000000 rudderclient-1.1.1/rudderclient.egg-info/top_level.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       38 2023-05-23 06:16:06.393255 rudderclient-1.1.1/setup.cfg
+drwxrwxr-x   0 inigo     (1001) inigo     (1001)        0 2023-05-23 08:15:59.906770 rudderclient-1.2.0/
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)     1069 2023-05-22 11:58:38.000000 rudderclient-1.2.0/LICENSE
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)     1968 2023-05-23 08:15:59.906770 rudderclient-1.2.0/PKG-INFO
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)      224 2023-05-22 12:07:13.000000 rudderclient-1.2.0/README.md
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)      681 2023-05-23 07:32:21.000000 rudderclient-1.2.0/pyproject.toml
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)       38 2023-05-23 08:15:59.906770 rudderclient-1.2.0/setup.cfg
+drwxrwxr-x   0 inigo     (1001) inigo     (1001)        0 2023-05-23 08:15:59.902770 rudderclient-1.2.0/src/
+drwxrwxr-x   0 inigo     (1001) inigo     (1001)        0 2023-05-23 08:15:59.902770 rudderclient-1.2.0/src/rudderclient/
+drwxrwxr-x   0 inigo     (1001) inigo     (1001)        0 2023-05-23 08:15:59.902770 rudderclient-1.2.0/src/rudderclient/gcp/
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)        0 2023-05-22 12:07:13.000000 rudderclient-1.2.0/src/rudderclient/gcp/__init__.py
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)      847 2023-05-23 07:28:36.000000 rudderclient-1.2.0/src/rudderclient/gcp/auth.py
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)      338 2023-05-23 07:28:36.000000 rudderclient-1.2.0/src/rudderclient/gcp/http_requests.py
+drwxrwxr-x   0 inigo     (1001) inigo     (1001)        0 2023-05-23 08:15:59.906770 rudderclient-1.2.0/src/rudderclient/tools/
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)     5118 2023-05-23 07:17:27.000000 rudderclient-1.2.0/src/rudderclient/tools/send_account_email.py
+drwxrwxr-x   0 inigo     (1001) inigo     (1001)        0 2023-05-23 08:15:59.902770 rudderclient-1.2.0/src/rudderclient.egg-info/
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)     1968 2023-05-23 08:15:59.000000 rudderclient-1.2.0/src/rudderclient.egg-info/PKG-INFO
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)      376 2023-05-23 08:15:59.000000 rudderclient-1.2.0/src/rudderclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)        1 2023-05-23 08:15:59.000000 rudderclient-1.2.0/src/rudderclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)       28 2023-05-23 08:15:59.000000 rudderclient-1.2.0/src/rudderclient.egg-info/requires.txt
+-rw-rw-r--   0 inigo     (1001) inigo     (1001)       13 2023-05-23 08:15:59.000000 rudderclient-1.2.0/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.1.1/LICENSE` & `rudderclient-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.1.1/PKG-INFO` & `rudderclient-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.1.1
+Version: 1.2.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,17 +22,18 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/realnautops/rudder-client
+Keywords: rudder,client,helper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rudder client
 
 The official library for Realnaut Rudder tool. Realnaut Rudder tool backend consist of multiple Cloud Runs and this library contains the necessary code for these services to communicate with different APIs.
```

### Comparing `rudderclient-1.1.1/gcp/auth.py` & `rudderclient-1.2.0/src/rudderclient/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.1.1/pyproject.toml` & `rudderclient-1.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.1.1"
+version = "1.2.0"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 authors = [{ name = "Rudder Team", email = "rudder@realnaut.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
 ]
+keywords = ["rudder", "client", "helper"]
 dependencies = [
     "google-cloud-secret-manager"
 ]
 requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://github.com/realnautops/rudder-client"
```

### Comparing `rudderclient-1.1.1/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.2.0/src/rudderclient.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.1.1
+Version: 1.2.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,17 +22,18 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/realnautops/rudder-client
+Keywords: rudder,client,helper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rudder client
 
 The official library for Realnaut Rudder tool. Realnaut Rudder tool backend consist of multiple Cloud Runs and this library contains the necessary code for these services to communicate with different APIs.
```

