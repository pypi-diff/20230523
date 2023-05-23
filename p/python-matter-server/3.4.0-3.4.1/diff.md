# Comparing `tmp/python-matter-server-3.4.0.tar.gz` & `tmp/python-matter-server-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.4.0.tar", last modified: Mon May 22 13:05:25 2023, max compression
+gzip compressed data, was "python-matter-server-3.4.1.tar", last modified: Tue May 23 13:16:02 2023, max compression
```

## Comparing `python-matter-server-3.4.0.tar` & `python-matter-server-3.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:05:23.000000 python-matter-server-3.4.0/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:16:00.000000 python-matter-server-3.4.1/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/setup.cfg
```

### Comparing `python-matter-server-3.4.0/LICENSE` & `python-matter-server-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/PKG-INFO` & `python-matter-server-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.4.0
+Version: 3.4.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,30 +15,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: server
 Provides-Extra: test
 License-File: LICENSE
 
 # Python Matter Server
 
-This project implements a Matter Controller Server over WebSockets using the [official CHIP SDK](https://github.com/project-chip/connectedhomeip) as a base and provides both a server and client implementation.
+This project implements a Matter Controller Server over WebSockets using the [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip) as a base and provides both a server and client implementation.
 
 The goal of this project is primary to have Matter support in Home Assistant but its universal approach makes it suitable to be used in other projects too.
 
 This repository is for development only (so not for enduser support). For enabling Matter support within Home Assistant, please refer to the [Home Assistant documentation](https://www.home-assistant.io/integrations/matter/).
 
 NOTE: Both Matter and this implementation are in early (v1) state and features are probably missing or could be improved. See our [development notes](#development) how you can help out, with development and/or testing.
 
 ## Trying it out
 
 `For enabling Matter support within Home Assistant, please refer to the Home Assistant documentation. These instructions are for development/advanced scenarios only!`
 
 To install the server (including client): `pip install python-matter-server[server]`
 To only install the client part: `pip install python-matter-server`
 
-The client library has a dependency on the chip clusters package which contains all (Cluster) models and this package is os/platform independent. The server library depends on the CHIP Core SDK which is architecture and OS specific. We build (and publish) wheels for Linux (amd64 and aarch64) to pypi but for other platforms (like Macos) you will need to build those wheels yourself using the exact same version of the SDK as we use for the clusters package. Take a look at our build script for directions: https://github.com/home-assistant-libs/chip-wheels/blob/main/.github/workflows/build.yaml
+The client library has a dependency on the chip/matter clusters package which contains all (Cluster) models and this package is os/platform independent. The server library depends on the Matter Core SDK (still named CHIP) which is architecture and OS specific. We build (and publish) wheels for Linux (amd64 and aarch64) to pypi but for other platforms (like Macos) you will need to build those wheels yourself using the exact same version of the SDK as we use for the clusters package. Take a look at our build script for directions: https://github.com/home-assistant-libs/chip-wheels/blob/main/.github/workflows/build.yaml
 
 Once you have the wheels installed, you can check out the example script in the scripts folder for generic directions to run the client and server. To just run the server, you can run:
 
 ```
 python -m matter_server.server
 
 Optional arguments:
```

### Comparing `python-matter-server-3.4.0/README.md` & `python-matter-server-3.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Python Matter Server
 
-This project implements a Matter Controller Server over WebSockets using the [official CHIP SDK](https://github.com/project-chip/connectedhomeip) as a base and provides both a server and client implementation.
+This project implements a Matter Controller Server over WebSockets using the [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip) as a base and provides both a server and client implementation.
 
 The goal of this project is primary to have Matter support in Home Assistant but its universal approach makes it suitable to be used in other projects too.
 
 This repository is for development only (so not for enduser support). For enabling Matter support within Home Assistant, please refer to the [Home Assistant documentation](https://www.home-assistant.io/integrations/matter/).
 
 NOTE: Both Matter and this implementation are in early (v1) state and features are probably missing or could be improved. See our [development notes](#development) how you can help out, with development and/or testing.
 
 ## Trying it out
 
 `For enabling Matter support within Home Assistant, please refer to the Home Assistant documentation. These instructions are for development/advanced scenarios only!`
 
 To install the server (including client): `pip install python-matter-server[server]`
 To only install the client part: `pip install python-matter-server`
 
-The client library has a dependency on the chip clusters package which contains all (Cluster) models and this package is os/platform independent. The server library depends on the CHIP Core SDK which is architecture and OS specific. We build (and publish) wheels for Linux (amd64 and aarch64) to pypi but for other platforms (like Macos) you will need to build those wheels yourself using the exact same version of the SDK as we use for the clusters package. Take a look at our build script for directions: https://github.com/home-assistant-libs/chip-wheels/blob/main/.github/workflows/build.yaml
+The client library has a dependency on the chip/matter clusters package which contains all (Cluster) models and this package is os/platform independent. The server library depends on the Matter Core SDK (still named CHIP) which is architecture and OS specific. We build (and publish) wheels for Linux (amd64 and aarch64) to pypi but for other platforms (like Macos) you will need to build those wheels yourself using the exact same version of the SDK as we use for the clusters package. Take a look at our build script for directions: https://github.com/home-assistant-libs/chip-wheels/blob/main/.github/workflows/build.yaml
 
 Once you have the wheels installed, you can check out the example script in the scripts folder for generic directions to run the client and server. To just run the server, you can run:
 
 ```
 python -m matter_server.server
 
 Optional arguments:
```

### Comparing `python-matter-server-3.4.0/matter_server/client/client.py` & `python-matter-server-3.4.1/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/client/connection.py` & `python-matter-server-3.4.1/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/client/exceptions.py` & `python-matter-server-3.4.1/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/client/models/device_types.py` & `python-matter-server-3.4.1/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/client/models/node.py` & `python-matter-server-3.4.1/matter_server/client/models/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,22 +193,21 @@
 
     def update(self, attributes_data: dict[str, Any]) -> None:
         """Update MatterEndpoint from (endpoint-specific) raw Attributes data."""
         # unwrap cluster and clusterattributes from raw node data attributes
         for attribute_path, attribute_value in attributes_data.items():
             self.set_attribute_value(attribute_path, attribute_value)
         # extract device types from Descriptor Cluster
-        cluster = self.get_cluster(Clusters.Descriptor)
-        assert cluster is not None
-        for dev_info in cluster.deviceTypeList:  # type: ignore[unreachable]
-            device_type = DEVICE_TYPES.get(dev_info.deviceType)
-            if device_type is None:
-                LOGGER.debug("Found unknown device type %s", dev_info)
-                continue
-            self.device_types.add(device_type)
+        if cluster := self.get_cluster(Clusters.Descriptor):
+            for dev_info in cluster.deviceTypeList:  # type: ignore[unreachable]
+                device_type = DEVICE_TYPES.get(dev_info.deviceType)
+                if device_type is None:
+                    LOGGER.debug("Found unknown device type %s", dev_info)
+                    continue
+                self.device_types.add(device_type)
 
     def __repr__(self) -> str:
         """Return the representation."""
         return f"<MatterEndoint {self.endpoint_id} (node {self.node.node_id})>"
 
 
 class MatterNode:
@@ -322,15 +321,21 @@
                 # ignore root endpoint
                 continue
             if Aggregator in endpoint.device_types:
                 # ignore Bridge endpoint
                 # (as that will also use partsList to indicate its child's)
                 continue
             descriptor = endpoint.get_cluster(Clusters.Descriptor)
-            assert descriptor is not None
+            if descriptor is None:
+                LOGGER.warning(
+                    "Found endpoint without a Descriptor: Node %s, endpoint %s",
+                    self.node_id,
+                    endpoint.endpoint_id,
+                )
+                continue
             if descriptor.partsList:  # type: ignore[unreachable]
                 for endpoint_id in descriptor.partsList:
                     self._composed_endpoints[endpoint_id] = endpoint.endpoint_id
 
     def update_attribute(self, attribute_path: str, new_value: Any) -> None:
         """Handle Attribute value update."""
         endpoint_id = int(attribute_path.split("/")[0])
```

### Comparing `python-matter-server-3.4.0/matter_server/common/errors.py` & `python-matter-server-3.4.1/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/common/helpers/api.py` & `python-matter-server-3.4.1/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/common/helpers/json.py` & `python-matter-server-3.4.1/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/common/helpers/util.py` & `python-matter-server-3.4.1/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/common/models.py` & `python-matter-server-3.4.1/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/__main__.py` & `python-matter-server-3.4.1/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/client_handler.py` & `python-matter-server-3.4.1/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/const.py` & `python-matter-server-3.4.1/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/device_controller.py` & `python-matter-server-3.4.1/matter_server/server/device_controller.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.4.1/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/server.py` & `python-matter-server-3.4.1/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/stack.py` & `python-matter-server-3.4.1/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/storage.py` & `python-matter-server-3.4.1/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/matter_server/server/vendor_info.py` & `python-matter-server-3.4.1/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.0/pyproject.toml` & `python-matter-server-3.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.4.0"
+version = "3.4.1"
 license     = {text = "Apache-2.0"}
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
@@ -22,20 +22,20 @@
 ]
 dependencies = [
   "aiohttp",
   "aiorun",
   "coloredlogs",
   "dacite",
   "orjson",
-  "home-assistant-chip-clusters==2023.5.1"
+  "home-assistant-chip-clusters==2023.5.2"
 ]
 
 [project.optional-dependencies]
 server = [
-  "home-assistant-chip-core==2023.5.1",
+  "home-assistant-chip-core==2023.5.2",
   "cryptography==40.0.2"
 ]
 test = [
   "black==23.3.0",
   "flake8==6.0.0",
   "flake8-docstrings==1.7.0",
   "isort==5.12.0",
```

### Comparing `python-matter-server-3.4.0/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.4.1/python_matter_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.4.0
+Version: 3.4.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,30 +15,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: server
 Provides-Extra: test
 License-File: LICENSE
 
 # Python Matter Server
 
-This project implements a Matter Controller Server over WebSockets using the [official CHIP SDK](https://github.com/project-chip/connectedhomeip) as a base and provides both a server and client implementation.
+This project implements a Matter Controller Server over WebSockets using the [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip) as a base and provides both a server and client implementation.
 
 The goal of this project is primary to have Matter support in Home Assistant but its universal approach makes it suitable to be used in other projects too.
 
 This repository is for development only (so not for enduser support). For enabling Matter support within Home Assistant, please refer to the [Home Assistant documentation](https://www.home-assistant.io/integrations/matter/).
 
 NOTE: Both Matter and this implementation are in early (v1) state and features are probably missing or could be improved. See our [development notes](#development) how you can help out, with development and/or testing.
 
 ## Trying it out
 
 `For enabling Matter support within Home Assistant, please refer to the Home Assistant documentation. These instructions are for development/advanced scenarios only!`
 
 To install the server (including client): `pip install python-matter-server[server]`
 To only install the client part: `pip install python-matter-server`
 
-The client library has a dependency on the chip clusters package which contains all (Cluster) models and this package is os/platform independent. The server library depends on the CHIP Core SDK which is architecture and OS specific. We build (and publish) wheels for Linux (amd64 and aarch64) to pypi but for other platforms (like Macos) you will need to build those wheels yourself using the exact same version of the SDK as we use for the clusters package. Take a look at our build script for directions: https://github.com/home-assistant-libs/chip-wheels/blob/main/.github/workflows/build.yaml
+The client library has a dependency on the chip/matter clusters package which contains all (Cluster) models and this package is os/platform independent. The server library depends on the Matter Core SDK (still named CHIP) which is architecture and OS specific. We build (and publish) wheels for Linux (amd64 and aarch64) to pypi but for other platforms (like Macos) you will need to build those wheels yourself using the exact same version of the SDK as we use for the clusters package. Take a look at our build script for directions: https://github.com/home-assistant-libs/chip-wheels/blob/main/.github/workflows/build.yaml
 
 Once you have the wheels installed, you can check out the example script in the scripts folder for generic directions to run the client and server. To just run the server, you can run:
 
 ```
 python -m matter_server.server
 
 Optional arguments:
```

### Comparing `python-matter-server-3.4.0/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.4.1/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

