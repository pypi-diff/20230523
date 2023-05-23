# Comparing `tmp/cloudmesh-rivanna-4.3.7.tar.gz` & `tmp/cloudmesh-rivanna-4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmesh-rivanna-4.3.7.tar", last modified: Tue May 23 16:47:02 2023, max compression
+gzip compressed data, was "cloudmesh-rivanna-4.3.8.tar", last modified: Tue May 23 17:04:53 2023, max compression
```

## Comparing `cloudmesh-rivanna-4.3.7.tar` & `cloudmesh-rivanna-4.3.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 16:47:02.044824 cloudmesh-rivanna-4.3.7/
--rw-r--r--   0 grey       (502) staff       (20)      769 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/LICENSE
--rw-r--r--   0 grey       (502) staff       (20)       99 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/MANIFEST.in
--rw-r--r--   0 grey       (502) staff       (20)     1384 2023-05-23 16:47:02.044884 cloudmesh-rivanna-4.3.7/PKG-INFO
--rw-r--r--   0 grey       (502) staff       (20)      621 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/README.md
--rw-r--r--   0 grey       (502) staff       (20)        5 2023-05-23 16:46:48.000000 cloudmesh-rivanna-4.3.7/VERSION
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 16:47:02.043374 cloudmesh-rivanna-4.3.7/cloudmesh/
--rw-r--r--   0 grey       (502) staff       (20)       63 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/cloudmesh/__init__.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 16:47:02.043721 cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/
--rw-r--r--   0 grey       (502) staff       (20)       22 2023-05-23 16:46:48.000000 cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/__init__.py
--rw-r--r--   0 grey       (502) staff       (20)       18 2023-05-23 16:46:48.000000 cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/__version__.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 16:47:02.043930 cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/command/
--rw-r--r--   0 grey       (502) staff       (20)        0 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/command/__init__.py
--rw-r--r--   0 grey       (502) staff       (20)     3814 2023-05-23 16:44:28.000000 cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/command/rivanna.py
--rw-r--r--   0 grey       (502) staff       (20)     1362 2023-05-23 16:33:49.000000 cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/rivanna.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 16:47:02.044722 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/
--rw-r--r--   0 grey       (502) staff       (20)     1384 2023-05-23 16:47:02.000000 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/PKG-INFO
--rw-r--r--   0 grey       (502) staff       (20)      577 2023-05-23 16:47:02.000000 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/SOURCES.txt
--rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 16:47:02.000000 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/dependency_links.txt
--rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 16:47:02.000000 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/namespace_packages.txt
--rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 16:47:02.000000 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/not-zip-safe
--rw-r--r--   0 grey       (502) staff       (20)       73 2023-05-23 16:47:02.000000 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/requires.txt
--rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 16:47:02.000000 cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/top_level.txt
--rw-r--r--   0 grey       (502) staff       (20)       23 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/requirements-dev.txt
--rw-r--r--   0 grey       (502) staff       (20)      167 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/requirements.txt
--rw-r--r--   0 grey       (502) staff       (20)       67 2023-05-23 16:47:02.045055 cloudmesh-rivanna-4.3.7/setup.cfg
--rw-r--r--   0 grey       (502) staff       (20)     2811 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.7/setup.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:53.800734 cloudmesh-rivanna-4.3.8/
+-rw-r--r--   0 grey       (502) staff       (20)      769 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.8/LICENSE
+-rw-r--r--   0 grey       (502) staff       (20)       99 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.8/MANIFEST.in
+-rw-r--r--   0 grey       (502) staff       (20)     1384 2023-05-23 17:04:53.800799 cloudmesh-rivanna-4.3.8/PKG-INFO
+-rw-r--r--   0 grey       (502) staff       (20)      621 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.8/README.md
+-rw-r--r--   0 grey       (502) staff       (20)        5 2023-05-23 17:04:40.000000 cloudmesh-rivanna-4.3.8/VERSION
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:53.798967 cloudmesh-rivanna-4.3.8/cloudmesh/
+-rw-r--r--   0 grey       (502) staff       (20)       63 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.8/cloudmesh/__init__.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:53.799347 cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/
+-rw-r--r--   0 grey       (502) staff       (20)       22 2023-05-23 17:04:40.000000 cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/__init__.py
+-rw-r--r--   0 grey       (502) staff       (20)       18 2023-05-23 17:04:40.000000 cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/__version__.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:53.799701 cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/command/
+-rw-r--r--   0 grey       (502) staff       (20)        0 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/command/__init__.py
+-rw-r--r--   0 grey       (502) staff       (20)     4843 2023-05-23 17:00:52.000000 cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/command/rivanna.py
+-rw-r--r--   0 grey       (502) staff       (20)     1362 2023-05-23 16:33:49.000000 cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/rivanna.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 17:04:53.800610 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/
+-rw-r--r--   0 grey       (502) staff       (20)     1384 2023-05-23 17:04:53.000000 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/PKG-INFO
+-rw-r--r--   0 grey       (502) staff       (20)      577 2023-05-23 17:04:53.000000 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/SOURCES.txt
+-rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 17:04:53.000000 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/dependency_links.txt
+-rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 17:04:53.000000 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/namespace_packages.txt
+-rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 17:04:53.000000 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/not-zip-safe
+-rw-r--r--   0 grey       (502) staff       (20)       73 2023-05-23 17:04:53.000000 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/requires.txt
+-rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 17:04:53.000000 cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/top_level.txt
+-rw-r--r--   0 grey       (502) staff       (20)       23 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.8/requirements-dev.txt
+-rw-r--r--   0 grey       (502) staff       (20)      181 2023-05-23 16:58:01.000000 cloudmesh-rivanna-4.3.8/requirements.txt
+-rw-r--r--   0 grey       (502) staff       (20)       67 2023-05-23 17:04:53.800981 cloudmesh-rivanna-4.3.8/setup.cfg
+-rw-r--r--   0 grey       (502) staff       (20)     2811 2023-04-15 07:19:22.000000 cloudmesh-rivanna-4.3.8/setup.py
```

### Comparing `cloudmesh-rivanna-4.3.7/LICENSE` & `cloudmesh-rivanna-4.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudmesh-rivanna-4.3.7/PKG-INFO` & `cloudmesh-rivanna-4.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-rivanna
-Version: 4.3.7
+Version: 4.3.8
 Summary: A command called rivanna and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-rivanna
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `cloudmesh-rivanna-4.3.7/README.md` & `cloudmesh-rivanna-4.3.8/README.md`

 * *Files identical despite different names*

### Comparing `cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/command/rivanna.py` & `cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/command/rivanna.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,14 +18,19 @@
         """
         ::
 
           Usage:
                 rivanna storage info DIRECTORY [--info]
                 rivanna login gpu=GPU [--info]
                 rivanna tutorial [KEYWORD]
+                rivanna vpn on
+                rivanna vpn off
+                rivanna vpn info
+                rivanna vpn status
+
 
           This command simplifys access to rivanna.
 
           Arguments:
               DIRECTORY  a location of a directory on rivanna
 
           Options:
@@ -79,24 +84,64 @@
 
         map_parameters(arguments, "gpu")
 
         # VERBOSE(arguments)
 
         rivanna = Rivanna()
 
+        def VPN():
+            from cloudmesh.vpn.vpn import Vpn
+            vpn = Vpn(None,
+                      timeout=30)
+            return vpn
+
         if arguments.storage:
 
             Console.error("not implemented")
 
         elif arguments.login:
 
             content = rivanna.login(gpu=arguments.GPU)
             print(content)
             Console.error("not implemented")
 
+        elif arguments.vpn and arguments.on:
+
+            vpn = VPN()
+
+            Console.ok("Connecting ... ")
+            vpn.connect()
+            if vpn.enabled():
+                Console.ok("ok")
+            else:
+                Console.error("failed")
+
+        elif arguments.vpn and arguments.off:
+
+            vpn = VPN()
+
+            Console.ok("Disconnecting ... ")
+            vpn.disconnect()
+            if not vpn.enabled():
+                Console.ok("ok")
+            else:
+                Console.error("failed")
+
+        elif arguments.vpn and arguments.status:
+
+            vpn = VPN()
+
+            print(vpn.enabled())
+
+        elif arguments.vpn and arguments.info:
+
+            vpn = VPN()
+
+            print(vpn.info())
+
         elif arguments.tutorial:
 
             keyword = arguments.KEYWORD
 
             if keyword in ["pod"]:
                 rivanna.browser("https://infomall.org/uva/docs/tutorial/rivanna-superpod/")
```

### Comparing `cloudmesh-rivanna-4.3.7/cloudmesh/rivanna/rivanna.py` & `cloudmesh-rivanna-4.3.8/cloudmesh/rivanna/rivanna.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/PKG-INFO` & `cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-rivanna
-Version: 4.3.7
+Version: 4.3.8
 Summary: A command called rivanna and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-rivanna
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `cloudmesh-rivanna-4.3.7/cloudmesh_rivanna.egg-info/SOURCES.txt` & `cloudmesh-rivanna-4.3.8/cloudmesh_rivanna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-rivanna-4.3.7/setup.py` & `cloudmesh-rivanna-4.3.8/setup.py`

 * *Files identical despite different names*

