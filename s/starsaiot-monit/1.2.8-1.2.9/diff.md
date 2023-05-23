# Comparing `tmp/starsaiot-monit-1.2.8.tar.gz` & `tmp/starsaiot-monit-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\starsaiot-monit-1.2.8.tar", last modified: Thu Mar 30 06:12:54 2023, max compression
+gzip compressed data, was "dist\starsaiot-monit-1.2.9.tar", last modified: Thu Mar 30 06:28:52 2023, max compression
```

## Comparing `starsaiot-monit-1.2.8.tar` & `starsaiot-monit-1.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/
--rw-rw-rw-   0        0        0       43 2022-12-15 06:45:49.000000 starsaiot-monit-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1226 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      424 2022-12-15 06:45:49.000000 starsaiot-monit-1.2.8/README.md
--rw-rw-rw-   0        0        0      218 2023-03-24 09:29:48.000000 starsaiot-monit-1.2.8/requirements.txt
--rw-rw-rw-   0        0        0      118 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1538 2023-03-30 06:12:48.000000 starsaiot-monit-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit/
--rw-rw-rw-   0        0        0     2771 2023-02-11 09:47:37.000000 starsaiot-monit-1.2.8/starsaiot_monit/conf.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit/config/
--rw-rw-rw-   0        0        0        0 2022-12-09 06:46:13.000000 starsaiot-monit-1.2.8/starsaiot_monit/config/__init__.py
--rw-rw-rw-   0        0        0     2926 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.8/starsaiot_monit/logger.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/
--rw-rw-rw-   0        0        0    11528 2023-03-24 06:28:32.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/monit_service.py
--rw-rw-rw-   0        0        0    17991 2023-03-30 06:12:37.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/mqtt_connector.py
--rw-rw-rw-   0        0        0     2714 2022-12-26 02:41:28.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/test.py
--rw-rw-rw-   0        0        0     1271 2023-03-27 03:37:13.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/test01.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/
--rw-rw-rw-   0        0        0     1589 2023-02-08 02:52:20.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/device_utils.py
--rw-rw-rw-   0        0        0     7431 2023-02-13 08:32:36.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/local_storage.py
--rw-rw-rw-   0        0        0     2872 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/local_storage_old.py
--rw-rw-rw-   0        0        0      643 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/md5.py
--rw-rw-rw-   0        0        0     1682 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/sftp.py
--rw-rw-rw-   0        0        0    24630 2023-03-27 03:37:13.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/simInfo.py
--rw-rw-rw-   0        0        0        0 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-09 06:46:04.000000 starsaiot-monit-1.2.8/starsaiot_monit/monit/__init__.py
--rw-rw-rw-   0        0        0      504 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.8/starsaiot_monit/smonit.py
--rw-rw-rw-   0        0        0      115 2022-12-09 06:34:09.000000 starsaiot-monit-1.2.8/starsaiot_monit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1226 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      110 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit.egg-info/requires.txt
--rw-rw-rw-   0        0        0      895 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2023-03-30 06:12:54.000000 starsaiot-monit-1.2.8/starsaiot_monit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/
+-rw-rw-rw-   0        0        0       43 2022-12-15 06:45:49.000000 starsaiot-monit-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1226 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2022-12-15 06:45:49.000000 starsaiot-monit-1.2.9/README.md
+-rw-rw-rw-   0        0        0      218 2023-03-24 09:29:48.000000 starsaiot-monit-1.2.9/requirements.txt
+-rw-rw-rw-   0        0        0      118 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2023-03-30 06:28:47.000000 starsaiot-monit-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit/
+-rw-rw-rw-   0        0        0     2771 2023-02-11 09:47:37.000000 starsaiot-monit-1.2.9/starsaiot_monit/conf.py
+drwxrwxrwx   0        0        0        0 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit/config/
+-rw-rw-rw-   0        0        0        0 2022-12-09 06:46:13.000000 starsaiot-monit-1.2.9/starsaiot_monit/config/__init__.py
+-rw-rw-rw-   0        0        0     2926 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.9/starsaiot_monit/logger.py
+drwxrwxrwx   0        0        0        0 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/
+-rw-rw-rw-   0        0        0    11528 2023-03-24 06:28:32.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/monit_service.py
+-rw-rw-rw-   0        0        0    18024 2023-03-30 06:23:41.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/mqtt_connector.py
+-rw-rw-rw-   0        0        0     2714 2022-12-26 02:41:28.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/test.py
+-rw-rw-rw-   0        0        0     1271 2023-03-27 03:37:13.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/test01.py
+drwxrwxrwx   0        0        0        0 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/
+-rw-rw-rw-   0        0        0     1589 2023-02-08 02:52:20.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/device_utils.py
+-rw-rw-rw-   0        0        0     7431 2023-02-13 08:32:36.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/local_storage.py
+-rw-rw-rw-   0        0        0     2872 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/local_storage_old.py
+-rw-rw-rw-   0        0        0      643 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/md5.py
+-rw-rw-rw-   0        0        0     1682 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/sftp.py
+-rw-rw-rw-   0        0        0    24630 2023-03-27 03:37:13.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/simInfo.py
+-rw-rw-rw-   0        0        0        0 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-12-09 06:46:04.000000 starsaiot-monit-1.2.9/starsaiot_monit/monit/__init__.py
+-rw-rw-rw-   0        0        0      504 2022-12-27 10:22:21.000000 starsaiot-monit-1.2.9/starsaiot_monit/smonit.py
+-rw-rw-rw-   0        0        0      115 2022-12-09 06:34:09.000000 starsaiot-monit-1.2.9/starsaiot_monit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1226 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      895 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2023-03-30 06:28:52.000000 starsaiot-monit-1.2.9/starsaiot_monit.egg-info/top_level.txt
```

### Comparing `starsaiot-monit-1.2.8/PKG-INFO` & `starsaiot-monit-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: starsaiot-monit
-Version: 1.2.8
+Version: 1.2.9
 Summary: 监控平台
 Home-page: https://github.com/huamoai/starsaiot_monit
 Author: wangning
 Author-email: 879619544@qq.com
 License: BSD
-Download-URL: https://github.com/huamoai/starsaiot_monit/tarball/1.2.8
+Download-URL: https://github.com/huamoai/starsaiot_monit/tarball/1.2.9
 Description: starsaiot_monit
         ===============================
         
         version number: 1.0.0
         author: wangning
         
         Overview
```

### Comparing `starsaiot-monit-1.2.8/setup.py` & `starsaiot-monit-1.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = '1.2.8'
+__version__ = '1.2.9'
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/conf.py` & `starsaiot-monit-1.2.9/starsaiot_monit/conf.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/logger.py` & `starsaiot-monit-1.2.9/starsaiot_monit/logger.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/monit_service.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/monit_service.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/mqtt_connector.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/mqtt_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,16 @@
                 _msg['msgVersion'] = 'V3.0.0'
                 _msg['sendTime'] = current_time
                 _msg['tenantId'] = msg['tenantId']
                 data = json.dumps(_msg)
                 self.sendMsg("/sys/platform/device/ack", data, 1)
 
                 # status, output = subprocess.getstatusoutput("pip3 install starsaiot-monit==" + appVersionName)
-                result = self.install_package_ycwl('starsaiot-monit', appVersionName)
+                # result = self.install_package_ycwl('starsaiot-monit', appVersionName)
+                result = True
                 if result:
                     msg_body['laterVersionCode'] = appVersionCode
                     msg_body['laterVersionName'] = appVersionName
                     msg_body['action'] = 'installSuccess'
                     msg_body['taskId'] = taskId
                 else:
                     msg_body['failLog'] = '安装失败'
```

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/test.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/test.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/test01.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/test01.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/device_utils.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/device_utils.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/local_storage.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/local_storage.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/local_storage_old.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/local_storage_old.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/md5.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/md5.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/sftp.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/sftp.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit/monit/utils/simInfo.py` & `starsaiot-monit-1.2.9/starsaiot_monit/monit/utils/simInfo.py`

 * *Files identical despite different names*

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit.egg-info/PKG-INFO` & `starsaiot-monit-1.2.9/starsaiot_monit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: starsaiot-monit
-Version: 1.2.8
+Version: 1.2.9
 Summary: 监控平台
 Home-page: https://github.com/huamoai/starsaiot_monit
 Author: wangning
 Author-email: 879619544@qq.com
 License: BSD
-Download-URL: https://github.com/huamoai/starsaiot_monit/tarball/1.2.8
+Download-URL: https://github.com/huamoai/starsaiot_monit/tarball/1.2.9
 Description: starsaiot_monit
         ===============================
         
         version number: 1.0.0
         author: wangning
         
         Overview
```

### Comparing `starsaiot-monit-1.2.8/starsaiot_monit.egg-info/SOURCES.txt` & `starsaiot-monit-1.2.9/starsaiot_monit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

