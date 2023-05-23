# Comparing `tmp/cloudmesh-vpn-4.3.5.tar.gz` & `tmp/cloudmesh-vpn-4.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmesh-vpn-4.3.5.tar", last modified: Tue May 23 12:37:56 2023, max compression
+gzip compressed data, was "cloudmesh-vpn-4.3.6.tar", last modified: Tue May 23 17:04:25 2023, max compression
```

## Comparing `cloudmesh-vpn-4.3.5.tar` & `cloudmesh-vpn-4.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.674718 cloudmesh-vpn-4.3.5/
--rw-r--r--   0 grey       (502) staff       (20)      769 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/LICENSE
--rw-r--r--   0 grey       (502) staff       (20)       99 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/MANIFEST.in
--rw-r--r--   0 grey       (502) staff       (20)     3405 2023-05-23 12:37:56.674785 cloudmesh-vpn-4.3.5/PKG-INFO
--rw-r--r--   0 grey       (502) staff       (20)     2654 2023-05-23 11:59:09.000000 cloudmesh-vpn-4.3.5/README.md
--rw-r--r--   0 grey       (502) staff       (20)        5 2023-05-23 12:37:39.000000 cloudmesh-vpn-4.3.5/VERSION
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.673004 cloudmesh-vpn-4.3.5/cloudmesh/
--rw-r--r--   0 grey       (502) staff       (20)       63 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/cloudmesh/__init__.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.673382 cloudmesh-vpn-4.3.5/cloudmesh/vpn/
--rw-r--r--   0 grey       (502) staff       (20)       22 2023-05-23 12:37:39.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/__init__.py
--rw-r--r--   0 grey       (502) staff       (20)       18 2023-05-23 12:37:39.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/__version__.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.673601 cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/
--rw-r--r--   0 grey       (502) staff       (20)        0 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/__init__.py
--rw-r--r--   0 grey       (502) staff       (20)     2640 2023-05-23 12:37:21.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/vpn.py
--rw-r--r--   0 grey       (502) staff       (20)     8776 2023-05-23 12:31:19.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/vpn.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.674591 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/
--rw-r--r--   0 grey       (502) staff       (20)     3405 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/PKG-INFO
--rw-r--r--   0 grey       (502) staff       (20)      521 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/SOURCES.txt
--rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/dependency_links.txt
--rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/namespace_packages.txt
--rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/not-zip-safe
--rw-r--r--   0 grey       (502) staff       (20)       90 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/requires.txt
--rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/top_level.txt
--rw-r--r--   0 grey       (502) staff       (20)       29 2022-07-19 23:33:31.000000 cloudmesh-vpn-4.3.5/requirements-dev.txt
--rw-r--r--   0 grey       (502) staff       (20)      714 2023-03-23 13:24:20.000000 cloudmesh-vpn-4.3.5/requirements.txt
--rw-r--r--   0 grey       (502) staff       (20)       67 2023-05-23 12:37:56.675212 cloudmesh-vpn-4.3.5/setup.cfg
--rw-r--r--   0 grey       (502) staff       (20)     2815 2022-07-18 14:53:05.000000 cloudmesh-vpn-4.3.5/setup.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:25.071796 cloudmesh-vpn-4.3.6/
+-rw-r--r--   0 grey       (502) staff       (20)      769 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.6/LICENSE
+-rw-r--r--   0 grey       (502) staff       (20)       99 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.6/MANIFEST.in
+-rw-r--r--   0 grey       (502) staff       (20)     3405 2023-05-23 17:04:25.071855 cloudmesh-vpn-4.3.6/PKG-INFO
+-rw-r--r--   0 grey       (502) staff       (20)     2654 2023-05-23 11:59:09.000000 cloudmesh-vpn-4.3.6/README.md
+-rw-r--r--   0 grey       (502) staff       (20)        5 2023-05-23 17:04:13.000000 cloudmesh-vpn-4.3.6/VERSION
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:25.070281 cloudmesh-vpn-4.3.6/cloudmesh/
+-rw-r--r--   0 grey       (502) staff       (20)       63 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.6/cloudmesh/__init__.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:25.070615 cloudmesh-vpn-4.3.6/cloudmesh/vpn/
+-rw-r--r--   0 grey       (502) staff       (20)       22 2023-05-23 17:04:13.000000 cloudmesh-vpn-4.3.6/cloudmesh/vpn/__init__.py
+-rw-r--r--   0 grey       (502) staff       (20)       18 2023-05-23 17:04:13.000000 cloudmesh-vpn-4.3.6/cloudmesh/vpn/__version__.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:25.070829 cloudmesh-vpn-4.3.6/cloudmesh/vpn/command/
+-rw-r--r--   0 grey       (502) staff       (20)        0 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.6/cloudmesh/vpn/command/__init__.py
+-rw-r--r--   0 grey       (502) staff       (20)     2640 2023-05-23 12:37:21.000000 cloudmesh-vpn-4.3.6/cloudmesh/vpn/command/vpn.py
+-rw-r--r--   0 grey       (502) staff       (20)     8825 2023-05-23 17:03:12.000000 cloudmesh-vpn-4.3.6/cloudmesh/vpn/vpn.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:25.071691 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/
+-rw-r--r--   0 grey       (502) staff       (20)     3405 2023-05-23 17:04:25.000000 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/PKG-INFO
+-rw-r--r--   0 grey       (502) staff       (20)      521 2023-05-23 17:04:25.000000 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/SOURCES.txt
+-rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 17:04:25.000000 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/dependency_links.txt
+-rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 17:04:25.000000 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/namespace_packages.txt
+-rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 17:04:25.000000 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/not-zip-safe
+-rw-r--r--   0 grey       (502) staff       (20)       90 2023-05-23 17:04:25.000000 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/requires.txt
+-rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 17:04:25.000000 cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/top_level.txt
+-rw-r--r--   0 grey       (502) staff       (20)       29 2022-07-19 23:33:31.000000 cloudmesh-vpn-4.3.6/requirements-dev.txt
+-rw-r--r--   0 grey       (502) staff       (20)      714 2023-03-23 13:24:20.000000 cloudmesh-vpn-4.3.6/requirements.txt
+-rw-r--r--   0 grey       (502) staff       (20)       67 2023-05-23 17:04:25.072036 cloudmesh-vpn-4.3.6/setup.cfg
+-rw-r--r--   0 grey       (502) staff       (20)     2815 2022-07-18 14:53:05.000000 cloudmesh-vpn-4.3.6/setup.py
```

### Comparing `cloudmesh-vpn-4.3.5/LICENSE` & `cloudmesh-vpn-4.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.5/PKG-INFO` & `cloudmesh-vpn-4.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-vpn
-Version: 4.3.5
+Version: 4.3.6
 Summary: A command called vpn and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-vpn
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `cloudmesh-vpn-4.3.5/README.md` & `cloudmesh-vpn-4.3.6/README.md`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/vpn.py` & `cloudmesh-vpn-4.3.6/cloudmesh/vpn/command/vpn.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.5/cloudmesh/vpn/vpn.py` & `cloudmesh-vpn-4.3.6/cloudmesh/vpn/vpn.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     def __init__(self,
                  service=None,
                  timeout=None,
                  debug=False):
 
         if timeout is None:
             self.timeout = 60
+        else:
+            self.timeout = timeout
 
         if os_is_windows():
             self.anyconnect = r'C:\Program Files (x86)\Cisco\Cisco Secure Client\vpncli.exe'
         elif os_is_mac():
             self.anyconnect = None
             for command in ["/opt/cisco/anyconnect/bin/vpn",
                             "/opt/cisco/secureclient/bin/vpn"]:
```

### Comparing `cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/PKG-INFO` & `cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-vpn
-Version: 4.3.5
+Version: 4.3.6
 Summary: A command called vpn and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-vpn
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/SOURCES.txt` & `cloudmesh-vpn-4.3.6/cloudmesh_vpn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.5/requirements.txt` & `cloudmesh-vpn-4.3.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.5/setup.py` & `cloudmesh-vpn-4.3.6/setup.py`

 * *Files identical despite different names*

