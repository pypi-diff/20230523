# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.5.23.1684849413.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.5.23.1684849413.tar", last modified: Tue May 23 13:43:34 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar", last modified: Sun May  7 10:38:50 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413.tar` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13467 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3326 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     7404 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1879 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    10693 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    12497 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7019 2023-05-23 13:42:38.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 13:43:34.000000 zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13467 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3326 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7404 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7245 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    10693 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    12497 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     6791 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.5.23.1684849413
+Version: 1.0.2023.5.7.1683455929
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/README.md` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/setup.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/step_instructions.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,7 @@
 
 ###### TODO: END discuss with Osher
 
 
 @dataclass
 class RemoveDiskCloud(CloudInstruction):
     volume_id: str
-
-
-@dataclass
-class StartMigrationMachine(MachineInstruction):
-    fs_id: str  # will there be ability to grab this from context?
-    account_id: str
-    action_id: str
-    fs_mount_path: str
-    volume_id: str
-    dev_path: str
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.5.23.1684849413
+Version: 1.0.2023.5.7.1683455929
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.23.1684849413/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

