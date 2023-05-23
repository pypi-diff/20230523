# Comparing `tmp/ih_common-2.7.1.tar.gz` & `tmp/ih_common-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ih_common-2.7.1.tar", last modified: Wed May  4 13:56:03 2022, max compression
+gzip compressed data, was "ih_common-2.8.0.tar", last modified: Tue May 24 08:12:40 2022, max compression
```

## Comparing `ih_common-2.7.1.tar` & `ih_common-2.8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:56:03.809963 ih_common-2.7.1/
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     1069 2022-04-02 09:34:07.000000 ih_common-2.7.1/LICENSE
--rw-r--r--   0 hanchuanjun   (501) staff       (20)      575 2022-05-04 13:56:03.809833 ih_common-2.7.1/PKG-INFO
--rw-r--r--   0 hanchuanjun   (501) staff       (20)       86 2022-04-02 09:34:07.000000 ih_common-2.7.1/README.md
-drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:56:03.805882 ih_common-2.7.1/ih_common.egg-info/
--rw-r--r--   0 hanchuanjun   (501) staff       (20)      575 2022-05-04 13:56:03.000000 ih_common-2.7.1/ih_common.egg-info/PKG-INFO
--rw-r--r--   0 hanchuanjun   (501) staff       (20)      824 2022-05-04 13:56:03.000000 ih_common-2.7.1/ih_common.egg-info/SOURCES.txt
--rw-r--r--   0 hanchuanjun   (501) staff       (20)        1 2022-05-04 13:56:03.000000 ih_common-2.7.1/ih_common.egg-info/dependency_links.txt
--rw-r--r--   0 hanchuanjun   (501) staff       (20)        7 2022-05-04 13:56:03.000000 ih_common-2.7.1/ih_common.egg-info/top_level.txt
-drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:56:03.806001 ih_common-2.7.1/inhand/
--rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/__init__.py
-drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:56:03.806341 ih_common-2.7.1/inhand/cloud/
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     4107 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/cloud/Information.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/cloud/__init__.py
-drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:56:03.806705 ih_common-2.7.1/inhand/dto/
--rw-r--r--   0 hanchuanjun   (501) staff       (20)      499 2022-04-27 14:46:30.000000 ih_common-2.7.1/inhand/dto/RestAPIResult.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/dto/__init__.py
-drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:56:03.808470 ih_common-2.7.1/inhand/service/
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     1511 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/CacheService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     2622 2022-04-28 09:25:30.000000 ih_common-2.7.1/inhand/service/CalendarService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     1867 2022-05-04 13:56:00.000000 ih_common-2.7.1/inhand/service/ConsulService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     2172 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/FSService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     2665 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/HdfsService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)      480 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/IHException.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)    10506 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/LBSService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     2509 2022-04-28 08:59:36.000000 ih_common-2.7.1/inhand/service/MQSender.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     5929 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/MongoService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)    13734 2022-04-28 08:59:36.000000 ih_common-2.7.1/inhand/service/RDBService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     4982 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/SettingService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     2966 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/ZkService.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/service/__init__.py
-drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:56:03.809673 ih_common-2.7.1/inhand/utilities/
--rw-r--r--   0 hanchuanjun   (501) staff       (20)    10374 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/utilities/DateTimeUtility.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)     5835 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/utilities/GNSSTools.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)      786 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/utilities/URLUtility.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)    10029 2022-05-02 00:23:43.000000 ih_common-2.7.1/inhand/utilities/Utility.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.7.1/inhand/utilities/__init__.py
--rw-r--r--   0 hanchuanjun   (501) staff       (20)       38 2022-05-04 13:56:03.810003 ih_common-2.7.1/setup.cfg
--rw-r--r--   0 hanchuanjun   (501) staff       (20)      777 2022-05-04 13:50:07.000000 ih_common-2.7.1/setup.py
+drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-24 08:12:40.703625 ih_common-2.8.0/
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     1069 2022-05-04 13:57:12.000000 ih_common-2.8.0/LICENSE
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)      575 2022-05-24 08:12:40.703499 ih_common-2.8.0/PKG-INFO
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)       86 2022-05-04 13:57:12.000000 ih_common-2.8.0/README.md
+drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-24 08:12:40.698746 ih_common-2.8.0/ih_common.egg-info/
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)      575 2022-05-24 08:12:40.000000 ih_common-2.8.0/ih_common.egg-info/PKG-INFO
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)      824 2022-05-24 08:12:40.000000 ih_common-2.8.0/ih_common.egg-info/SOURCES.txt
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)        1 2022-05-24 08:12:40.000000 ih_common-2.8.0/ih_common.egg-info/dependency_links.txt
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)        7 2022-05-24 08:12:40.000000 ih_common-2.8.0/ih_common.egg-info/top_level.txt
+drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-24 08:12:40.698851 ih_common-2.8.0/inhand/
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/__init__.py
+drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-24 08:12:40.699303 ih_common-2.8.0/inhand/cloud/
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     4107 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/cloud/Information.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/cloud/__init__.py
+drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-24 08:12:40.699634 ih_common-2.8.0/inhand/dto/
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)      499 2022-05-04 13:57:12.000000 ih_common-2.8.0/inhand/dto/RestAPIResult.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-05-04 13:57:12.000000 ih_common-2.8.0/inhand/dto/__init__.py
+drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-24 08:12:40.702164 ih_common-2.8.0/inhand/service/
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     1511 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/service/CacheService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     2622 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/service/CalendarService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     1943 2022-05-24 08:06:51.000000 ih_common-2.8.0/inhand/service/ConsulService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     2172 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/service/FSService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     2665 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/service/HdfsService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)      480 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/service/IHException.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)    10506 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/service/LBSService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     2509 2022-05-04 13:57:12.000000 ih_common-2.8.0/inhand/service/MQSender.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     5929 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/service/MongoService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)    13734 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/service/RDBService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     4982 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/service/SettingService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     2966 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/service/ZkService.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/service/__init__.py
+drwxr-xr-x   0 hanchuanjun   (501) staff       (20)        0 2022-05-24 08:12:40.703354 ih_common-2.8.0/inhand/utilities/
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)    10374 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/utilities/DateTimeUtility.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)     5835 2022-05-24 08:03:17.000000 ih_common-2.8.0/inhand/utilities/GNSSTools.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)      786 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/utilities/URLUtility.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)    10029 2022-05-22 04:40:49.000000 ih_common-2.8.0/inhand/utilities/Utility.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)        0 2022-04-02 09:33:59.000000 ih_common-2.8.0/inhand/utilities/__init__.py
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)       38 2022-05-24 08:12:40.703662 ih_common-2.8.0/setup.cfg
+-rw-r--r--   0 hanchuanjun   (501) staff       (20)      777 2022-05-24 08:06:51.000000 ih_common-2.8.0/setup.py
```

### Comparing `ih_common-2.7.1/LICENSE` & `ih_common-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/PKG-INFO` & `ih_common-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ih_common
-Version: 2.7.1
+Version: 2.8.0
 Summary: tool
 Home-page: https://gitlab.inhand.design/hancj-dev/py-common
 Author: hanchuanjun
 Author-email: han@inhand.com.cn
 License: MIT
 Description: # py-common
```

### Comparing `ih_common-2.7.1/ih_common.egg-info/PKG-INFO` & `ih_common-2.8.0/ih_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ih-common
-Version: 2.7.1
+Version: 2.8.0
 Summary: tool
 Home-page: https://gitlab.inhand.design/hancj-dev/py-common
 Author: hanchuanjun
 Author-email: han@inhand.com.cn
 License: MIT
 Description: # py-common
```

### Comparing `ih_common-2.7.1/ih_common.egg-info/SOURCES.txt` & `ih_common-2.8.0/ih_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/cloud/Information.py` & `ih_common-2.8.0/inhand/cloud/Information.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/CacheService.py` & `ih_common-2.8.0/inhand/service/CacheService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/CalendarService.py` & `ih_common-2.8.0/inhand/service/CalendarService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/ConsulService.py` & `ih_common-2.8.0/inhand/service/ConsulService.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import consul
 
 class ConsulService(object):
     def __init__(self, host, port):
         '''初始化，连接consul服务器'''
         self._consul = consul.Consul(host, port)
 
-    def registerService(self, name, service_id,host,port, tags=None):
+    def registerService(self, name, service_id,host,port,health_entry='/health', tags=None):
         tags = tags or []
         # 注册服务
         self._consul.agent.service.register(
             name=name,
             service_id=service_id,
             address=host,
             port=port,
             tags=tags,
             # 健康检查ip端口，检查时间：5,超时时间：30，注销时间：30s
-            check=consul.Check().http("http://{}:{}".format(host,port), "5s", "30s", "30s",None))
+            check=consul.Check().http("http://{}:{}{}".format(host,port,health_entry), "5s", "30s", "30s",None))
 
-    def check(self,host,port, interval, timeout=None, deregister=None,header=None):
-        return consul.Check.http("http://{}:{}".format(host,port),interval,timeout,deregister,header)
+    def check(self,host,port, interval, timeout=None, deregister=None,header=None,health_entry='/health'):
+        return consul.Check.http("http://{}:{}{}".format(host,port,health_entry),interval,timeout,deregister,header)
 
     def getService(self, name):
         services = self._consul.agent.services()
         service = services.get(name)
         if not service:
             return None, None
         addr = "{0}:{1}".format(service['Address'], service['Port'])
```

### Comparing `ih_common-2.7.1/inhand/service/FSService.py` & `ih_common-2.8.0/inhand/service/FSService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/HdfsService.py` & `ih_common-2.8.0/inhand/service/HdfsService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/LBSService.py` & `ih_common-2.8.0/inhand/service/LBSService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/MQSender.py` & `ih_common-2.8.0/inhand/service/MQSender.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/MongoService.py` & `ih_common-2.8.0/inhand/service/MongoService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/RDBService.py` & `ih_common-2.8.0/inhand/service/RDBService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/SettingService.py` & `ih_common-2.8.0/inhand/service/SettingService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/service/ZkService.py` & `ih_common-2.8.0/inhand/service/ZkService.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/utilities/DateTimeUtility.py` & `ih_common-2.8.0/inhand/utilities/DateTimeUtility.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/utilities/GNSSTools.py` & `ih_common-2.8.0/inhand/utilities/GNSSTools.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/utilities/URLUtility.py` & `ih_common-2.8.0/inhand/utilities/URLUtility.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/inhand/utilities/Utility.py` & `ih_common-2.8.0/inhand/utilities/Utility.py`

 * *Files identical despite different names*

### Comparing `ih_common-2.7.1/setup.py` & `ih_common-2.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from setuptools import setup
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup (
     name = 'ih_common',
-    version = '2.7.1',
+    version = '2.8.0',
     author = 'hanchuanjun',
     author_email = 'han@inhand.com.cn',
     url = 'https://gitlab.inhand.design/hancj-dev/py-common',
     description = 'tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

