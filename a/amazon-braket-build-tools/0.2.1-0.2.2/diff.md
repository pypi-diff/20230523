# Comparing `tmp/amazon-braket-build-tools-0.2.1.tar.gz` & `tmp/amazon-braket-build-tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-build-tools-0.2.1.tar", last modified: Thu May 18 16:04:56 2023, max compression
+gzip compressed data, was "amazon-braket-build-tools-0.2.2.tar", last modified: Tue May 23 16:06:24 2023, max compression
```

## Comparing `amazon-braket-build-tools-0.2.1.tar` & `amazon-braket-build-tools-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/braket/_build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/src/braket/_build_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/braket/flake8_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/src/braket/flake8_plugins/braket_checkstyle_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.759700 amazon-braket-build-tools-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-23 16:06:24.759700 amazon-braket-build-tools-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 16:06:24.759700 amazon-braket-build-tools-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/braket/_build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/src/braket/_build_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/braket/flake8_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/src/braket/flake8_plugins/braket_checkstyle_plugin.py
```

### Comparing `amazon-braket-build-tools-0.2.1/LICENSE` & `amazon-braket-build-tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.1/PKG-INFO` & `amazon-braket-build-tools-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.1/README.md` & `amazon-braket-build-tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.1/setup.cfg` & `amazon-braket-build-tools-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.1/setup.py` & `amazon-braket-build-tools-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/PKG-INFO` & `amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.1/src/braket/_build_tools/_version.py` & `amazon-braket-build-tools-0.2.2/src/braket/_build_tools/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # language governing permissions and limitations under the License.
 
 """Version information.
 
 Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `amazon-braket-build-tools-0.2.1/src/braket/flake8_plugins/braket_checkstyle_plugin.py` & `amazon-braket-build-tools-0.2.2/src/braket/flake8_plugins/braket_checkstyle_plugin.py`

 * *Files identical despite different names*

