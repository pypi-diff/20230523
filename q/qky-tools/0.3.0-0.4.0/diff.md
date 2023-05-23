# Comparing `tmp/qky-tools-0.3.0.tar.gz` & `tmp/qky-tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qky-tools-0.3.0.tar", last modified: Mon May 22 06:08:28 2023, max compression
+gzip compressed data, was "qky-tools-0.4.0.tar", last modified: Tue May 23 07:26:32 2023, max compression
```

## Comparing `qky-tools-0.3.0.tar` & `qky-tools-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 06:08:28.096767 qky-tools-0.3.0/
--rw-rw-rw-   0        0        0     1088 2023-05-18 00:09:54.000000 qky-tools-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      690 2023-05-22 06:08:28.095770 qky-tools-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-18 00:10:33.000000 qky-tools-0.3.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 06:08:28.065848 qky-tools-0.3.0/qky_tools/
--rw-rw-rw-   0        0        0       84 2023-05-22 06:07:16.000000 qky-tools-0.3.0/qky_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:08:28.086794 qky-tools-0.3.0/qky_tools/db_tools/
--rw-rw-rw-   0        0        0     5338 2023-05-18 00:24:47.000000 qky-tools-0.3.0/qky_tools/db_tools/MySQL.py
--rw-rw-rw-   0        0        0       42 2023-05-22 06:05:29.000000 qky-tools-0.3.0/qky_tools/db_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:08:28.093776 qky-tools-0.3.0/qky_tools/req_tools/
--rw-rw-rw-   0        0        0       90 2023-05-22 06:06:52.000000 qky-tools-0.3.0/qky_tools/req_tools/__init__.py
--rw-rw-rw-   0        0        0     3250 2023-05-18 01:19:46.000000 qky-tools-0.3.0/qky_tools/req_tools/cacheReq.py
--rw-rw-rw-   0        0        0      191 2023-05-18 01:01:36.000000 qky-tools-0.3.0/qky_tools/req_tools/proxyReq.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:08:28.083801 qky-tools-0.3.0/qky_tools.egg-info/
--rw-rw-rw-   0        0        0      690 2023-05-22 06:08:27.000000 qky-tools-0.3.0/qky_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-22 06:08:28.000000 qky-tools-0.3.0/qky_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 06:08:27.000000 qky-tools-0.3.0/qky_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 06:08:27.000000 qky-tools-0.3.0/qky_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-22 06:08:27.000000 qky-tools-0.3.0/qky_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 06:08:28.096767 qky-tools-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     3932 2023-05-22 06:08:25.000000 qky-tools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:26:32.065821 qky-tools-0.4.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-18 00:09:54.000000 qky-tools-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      690 2023-05-23 07:26:32.063814 qky-tools-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-18 00:10:33.000000 qky-tools-0.4.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 07:26:32.031897 qky-tools-0.4.0/qky_tools/
+-rw-rw-rw-   0        0        0       84 2023-05-22 06:07:16.000000 qky-tools-0.4.0/qky_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:26:32.056833 qky-tools-0.4.0/qky_tools/db_tools/
+-rw-rw-rw-   0        0        0     5338 2023-05-18 00:24:47.000000 qky-tools-0.4.0/qky_tools/db_tools/MySQL.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:05:29.000000 qky-tools-0.4.0/qky_tools/db_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:26:32.062816 qky-tools-0.4.0/qky_tools/req_tools/
+-rw-rw-rw-   0        0        0       90 2023-05-22 06:06:52.000000 qky-tools-0.4.0/qky_tools/req_tools/__init__.py
+-rw-rw-rw-   0        0        0     3621 2023-05-23 07:24:52.000000 qky-tools-0.4.0/qky_tools/req_tools/cacheReq.py
+-rw-rw-rw-   0        0        0      191 2023-05-18 01:01:36.000000 qky-tools-0.4.0/qky_tools/req_tools/proxyReq.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:26:32.053840 qky-tools-0.4.0/qky_tools.egg-info/
+-rw-rw-rw-   0        0        0      690 2023-05-23 07:26:31.000000 qky-tools-0.4.0/qky_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-23 07:26:32.000000 qky-tools-0.4.0/qky_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:26:31.000000 qky-tools-0.4.0/qky_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 07:26:31.000000 qky-tools-0.4.0/qky_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-23 07:26:31.000000 qky-tools-0.4.0/qky_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:26:32.065821 qky-tools-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     3932 2023-05-23 07:26:28.000000 qky-tools-0.4.0/setup.py
```

### Comparing `qky-tools-0.3.0/LICENSE.txt` & `qky-tools-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qky-tools-0.3.0/PKG-INFO` & `qky-tools-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qky-tools
-Version: 0.3.0
+Version: 0.4.0
 Summary: python tools collection
 Home-page: https://github.com/qiaokuoyuan/py-tools
 Author: qiaokuoyuan
 Author-email: 457361577@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qky-tools-0.3.0/qky_tools/db_tools/MySQL.py` & `qky-tools-0.4.0/qky_tools/db_tools/MySQL.py`

 * *Files identical despite different names*

### Comparing `qky-tools-0.3.0/qky_tools/req_tools/cacheReq.py` & `qky-tools-0.4.0/qky_tools/req_tools/cacheReq.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 def mongo_cache_request_and_pack(request_action: typing.Callable,
                                  is_success: typing.Callable,
                                  mongo_collection,
                                  query: typing.Dict,
                                  save_key: typing.Dict,
                                  fail_action: typing.Callable = None,
+                                 request_success_action: typing.Callable = None,
                                  mongo_cache_request_id_name='request_id',
                                  mongo_cache_response_name='response',
                                  mongo_cache_timestamp_name='claw_date',
                                  try_times=3) -> typing.Tuple[typing.Dict, str]:
     if try_times < 1:
         raise f"mongo_cache_request_and_pack 多次尝试失败"
 
@@ -24,38 +25,43 @@
     else:
         try:
             r = request_action()
 
             if r and is_success(r):
                 request_id = nanoid.generate()
 
+                if request_success_action:
+                    request_success_action(r)
+
                 save_key.update({
                     mongo_cache_timestamp_name: datetime.datetime.now(),
                     mongo_cache_request_id_name: request_id,
                     mongo_cache_response_name: r
                 })
 
                 mongo_collection.insert_one(save_key)
                 return mongo_cache_request_and_pack(request_action=request_action,
                                                     is_success=is_success,
                                                     mongo_collection=mongo_collection,
                                                     query=query,
                                                     save_key=save_key,
                                                     fail_action=fail_action,
+                                                    request_success_action=request_success_action,
                                                     mongo_cache_request_id_name=mongo_cache_request_id_name,
                                                     mongo_cache_response_name=mongo_cache_response_name,
                                                     mongo_cache_timestamp_name=mongo_cache_timestamp_name,
                                                     try_times=try_times)
         except Exception as e:
             if fail_action:
                 fail_action()
 
             return mongo_cache_request_and_pack(request_action=request_action,
                                                 is_success=is_success,
                                                 mongo_collection=mongo_collection,
+                                                request_success_action=request_success_action,
                                                 query=query,
                                                 save_key=save_key,
                                                 fail_action=fail_action,
                                                 mongo_cache_request_id_name=mongo_cache_request_id_name,
                                                 mongo_cache_response_name=mongo_cache_response_name,
                                                 mongo_cache_timestamp_name=mongo_cache_timestamp_name,
                                                 try_times=try_times - 1)
```

### Comparing `qky-tools-0.3.0/qky_tools.egg-info/PKG-INFO` & `qky-tools-0.4.0/qky_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qky-tools
-Version: 0.3.0
+Version: 0.4.0
 Summary: python tools collection
 Home-page: https://github.com/qiaokuoyuan/py-tools
 Author: qiaokuoyuan
 Author-email: 457361577@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qky-tools-0.3.0/setup.py` & `qky-tools-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'qky-tools'
 DESCRIPTION = 'python tools collection'
 URL = 'https://github.com/qiaokuoyuan/py-tools'
 EMAIL = '457361577@qq.com'
 AUTHOR = 'qiaokuoyuan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     'pymysql', 'nanoid'
 ]
```

