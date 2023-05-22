# Comparing `tmp/EllucianEthosPythonClient-0.2.8.tar.gz` & `tmp/EllucianEthosPythonClient-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EllucianEthosPythonClient-0.2.8.tar", last modified: Thu Jul  2 14:21:32 2020, max compression
+gzip compressed data, was "dist/EllucianEthosPythonClient-0.2.9.tar", last modified: Mon Jul 20 15:06:22 2020, max compression
```

## Comparing `EllucianEthosPythonClient-0.2.8.tar` & `EllucianEthosPythonClient-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/
--rw-r--r--   0 robert    (1000) robert    (1000)    68611 2020-06-17 16:29:24.000000 EllucianEthosPythonClient-0.2.8/versioneer.py
--rw-r--r--   0 robert    (1000) robert    (1000)      325 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     2043 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/PKG-INFO
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/
--rw-rw-r--   0 robert    (1000) robert    (1000)     3248 2020-07-02 12:37:17.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/EthosChangeNotificationPollerThread.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2466 2020-07-02 14:04:24.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ChangeNotificationUtils.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/APIClients/
--rw-rw-r--   0 robert    (1000) robert    (1000)     5911 2020-06-23 08:42:34.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/APIClients/Mock.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4567 2020-06-25 07:42:55.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/APIClients/APIClientBase.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      503 2020-06-17 17:39:19.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/APIClients/LoginSession.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      158 2020-06-17 17:38:37.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/APIClients/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     6691 2020-07-02 14:02:41.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/EllucianEthosAPIClient.py
--rw-r--r--   0 robert    (1000) robert    (1000)      497 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/_version.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      846 2020-06-25 12:01:55.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ListBasedResourceIterator.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2544 2020-07-02 13:41:50.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ChangeNotificationMessage.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2214 2020-06-22 15:05:20.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/WorkerThread.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1938 2020-06-25 12:41:00.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/ResPersons.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      545 2020-06-19 16:06:38.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/ResourceWrapperFactory.py
--rw-rw-r--   0 robert    (1000) robert    (1000)       56 2020-06-18 10:36:30.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2569 2020-06-25 12:36:13.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/BaseResourceWrapper.py
--rw-r--r--   0 robert    (1000) robert    (1000)      309 2020-06-22 14:48:09.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1976 2020-06-25 11:57:47.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceIterator.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1608 2020-06-23 12:08:27.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/EthosLoginSession.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2020-07-02 14:21:32.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     1285 2020-07-02 14:21:31.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     2043 2020-07-02 14:21:31.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2020-07-02 14:21:31.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       53 2020-07-02 14:21:31.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       26 2020-07-02 14:21:31.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2020-06-17 16:34:30.000000 EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/not-zip-safe
--rw-r--r--   0 robert    (1000) robert    (1000)     1115 2020-07-02 14:21:00.000000 EllucianEthosPythonClient-0.2.8/setup.py
--rw-r--r--   0 robert    (1000) robert    (1000)       68 2020-06-17 16:29:24.000000 EllucianEthosPythonClient-0.2.8/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     1436 2020-06-27 07:45:29.000000 EllucianEthosPythonClient-0.2.8/README.md
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/
+-rw-r--r--   0 robert    (1000) robert    (1000)    68611 2020-06-17 16:29:24.000000 EllucianEthosPythonClient-0.2.9/versioneer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      325 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2043 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/PKG-INFO
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3248 2020-07-02 12:37:17.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/EthosChangeNotificationPollerThread.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2466 2020-07-02 14:04:24.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ChangeNotificationUtils.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/APIClients/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5911 2020-06-23 08:42:34.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/APIClients/Mock.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4567 2020-06-25 07:42:55.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/APIClients/APIClientBase.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      503 2020-06-17 17:39:19.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/APIClients/LoginSession.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      158 2020-06-17 17:38:37.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/APIClients/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     6691 2020-07-02 14:02:41.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/EllucianEthosAPIClient.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      497 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/_version.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      846 2020-06-25 12:01:55.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ListBasedResourceIterator.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2544 2020-07-02 13:41:50.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ChangeNotificationMessage.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2214 2020-06-22 15:05:20.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/WorkerThread.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1938 2020-06-25 12:41:00.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/ResPersons.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      545 2020-06-19 16:06:38.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/ResourceWrapperFactory.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)       56 2020-06-18 10:36:30.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2702 2020-07-20 15:04:54.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/BaseResourceWrapper.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      309 2020-06-22 14:48:09.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1976 2020-06-25 11:57:47.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceIterator.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1608 2020-06-23 12:08:27.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/EthosLoginSession.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2020-07-20 15:06:22.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1285 2020-07-20 15:06:21.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     2043 2020-07-20 15:06:21.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2020-07-20 15:06:21.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       53 2020-07-20 15:06:21.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       26 2020-07-20 15:06:21.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2020-06-17 16:34:30.000000 EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/not-zip-safe
+-rw-r--r--   0 robert    (1000) robert    (1000)     1115 2020-07-02 14:21:00.000000 EllucianEthosPythonClient-0.2.9/setup.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       68 2020-06-17 16:29:24.000000 EllucianEthosPythonClient-0.2.9/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     1436 2020-06-27 07:45:29.000000 EllucianEthosPythonClient-0.2.9/README.md
```

### Comparing `EllucianEthosPythonClient-0.2.8/versioneer.py` & `EllucianEthosPythonClient-0.2.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/PKG-INFO` & `EllucianEthosPythonClient-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllucianEthosPythonClient
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python package which provides Ellucian Ethos Client
 Home-page: https://github.com/rmetcalf9/EllucianEthosPythonClient
 Author: Robert Metcalf
 Author-email: rmetcalf9@googlemail.com
 License: MIT
 Description:  # EllucianEthosPythonClient
```

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/EthosChangeNotificationPollerThread.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/EthosChangeNotificationPollerThread.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ChangeNotificationUtils.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ChangeNotificationUtils.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/APIClients/Mock.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/APIClients/Mock.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/APIClients/APIClientBase.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/APIClients/APIClientBase.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/EllucianEthosAPIClient.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/EllucianEthosAPIClient.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ListBasedResourceIterator.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ListBasedResourceIterator.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ChangeNotificationMessage.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ChangeNotificationMessage.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/WorkerThread.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/WorkerThread.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/ResPersons.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/ResPersons.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/ResourceWrapperFactory.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/ResourceWrapperFactory.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceWrappers/BaseResourceWrapper.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceWrappers/BaseResourceWrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,26 @@
   resourceName = None
   resourceID = None
   def __init__(self, clientAPIInstance, dict, version, resourceName):
     self.clientAPIInstance = clientAPIInstance
     self.dict = dict
     self.version = version
     self.resourceName = resourceName
-    if "id" not in dict:
-      raise Exception("Invalid resource dict (missing id)")
     if not isinstance(version , str):
       raise Exception("Version passed must be a string")
-    self.resourceID = dict["id"]
+    self.resourceID = self._getResourceIDFromDict(dict)
     self._afterDictChanged()
 
+  def _getResourceIDFromDict(self, dict):
+    if "id" in dict:
+      return dict["id"]
+    if "guid" in dict:
+      return dict["guid"]
+    raise Exception("Invalid resource dict (missing id)")
+
   def getMajorVersion(self):
     return self.version.split(".")[0]
 
   def _getDictForPut(self):
     return copy.deepcopy(self.dict)
 
   def save(self, loginSession):
```

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/ResourceIterator.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/ResourceIterator.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient/EthosLoginSession.py` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient/EthosLoginSession.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/SOURCES.txt` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/EllucianEthosPythonClient.egg-info/PKG-INFO` & `EllucianEthosPythonClient-0.2.9/EllucianEthosPythonClient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllucianEthosPythonClient
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python package which provides Ellucian Ethos Client
 Home-page: https://github.com/rmetcalf9/EllucianEthosPythonClient
 Author: Robert Metcalf
 Author-email: rmetcalf9@googlemail.com
 License: MIT
 Description:  # EllucianEthosPythonClient
```

### Comparing `EllucianEthosPythonClient-0.2.8/setup.py` & `EllucianEthosPythonClient-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `EllucianEthosPythonClient-0.2.8/README.md` & `EllucianEthosPythonClient-0.2.9/README.md`

 * *Files identical despite different names*

