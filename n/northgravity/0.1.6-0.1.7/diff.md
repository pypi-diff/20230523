# Comparing `tmp/northgravity-0.1.6.tar.gz` & `tmp/northgravity-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "northgravity-0.1.6.tar", last modified: Thu May 18 09:41:56 2023, max compression
+gzip compressed data, was "northgravity-0.1.7.tar", last modified: Tue May 23 13:57:31 2023, max compression
```

## Comparing `northgravity-0.1.6.tar` & `northgravity-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:41:56.023805 northgravity-0.1.6/
--rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    29830 2023-05-18 09:41:56.023805 northgravity-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29397 2023-05-18 09:41:55.000000 northgravity-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:41:56.019805 northgravity-0.1.6/northgravity/
--rw-rw-r--   0 root         (0) root         (0)     1327 2023-05-18 09:33:33.000000 northgravity-0.1.6/northgravity/Authenticator.py
--rw-rw-r--   0 root         (0) root         (0)     9175 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/DatalakeHandler.py
--rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/ExceptionHandler.py
--rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/HTTPCalller.py
--rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/StatusHandler.py
--rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/TaskHandler.py
--rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/Timeseries.py
--rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/__init__.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:41:56.023805 northgravity-0.1.6/northgravity.egg-info/
--rw-r--r--   0 root         (0) root         (0)    29830 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 09:41:56.023805 northgravity-0.1.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:57:31.444412 northgravity-0.1.7/
+-rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 13:57:31.444412 northgravity-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29397 2023-05-23 13:57:31.000000 northgravity-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:57:31.444412 northgravity-0.1.7/northgravity/
+-rw-rw-r--   0 root         (0) root         (0)     1327 2023-05-18 09:33:33.000000 northgravity-0.1.7/northgravity/Authenticator.py
+-rw-rw-r--   0 root         (0) root         (0)     9912 2023-05-23 13:44:00.000000 northgravity-0.1.7/northgravity/DatalakeHandler.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/ExceptionHandler.py
+-rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/HTTPCalller.py
+-rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/StatusHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/TaskHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/Timeseries.py
+-rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:57:31.444412 northgravity-0.1.7/northgravity.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:57:31.444412 northgravity-0.1.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.7/setup.py
```

### Comparing `northgravity-0.1.6/LICENSE` & `northgravity-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.6/PKG-INFO` & `northgravity-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.6
+pip3 install northgravity==0.1.7
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.6
+northgravity==0.1.7
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.6/README.md` & `northgravity-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.6
+pip3 install northgravity==0.1.7
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.6
+northgravity==0.1.7
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.6/northgravity/Authenticator.py` & `northgravity-0.1.7/northgravity/Authenticator.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.6/northgravity/DatalakeHandler.py` & `northgravity-0.1.7/northgravity/DatalakeHandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,32 +9,39 @@
 log = logging.getLogger(LOGGER_NAME)
 
 
 class DatalakeHandler:
     def __init__(self):
         self.caller = HTTPCaller()
 
-    def search_file(self, file_name, file_type=None, group_name=None, size=100, from_page=0):
+    def search_file(self, file_name=None, file_type=None, group_name=None, metadata_field=None, metadata_value=None, size=100, from_page=0):
         '''
         Searching Method to find files on the datalake of the current stage
         for given file name, and optionally group_name or type
 
         :param file_name: name of the file stored on the lake group
         :param file_type: datalake file type: NCSV, SOURCE, JUPYTER, ...
         :param group_name: group on datalake where to search; if None, in the entire datalake
+        :param metadata_field: name of the metadata field to search by. If it is passed, the metadata_value should also exist.
+        :param metadata_value: value in the metadata field to seatch for. 
         :param size: size of the results to return, most recent first
         :param from_page: iteration parameter
 
         :return: the file matches on the datalake and their attributes
         '''
+        if metadata_field not in ['', None]:
+            assert metadata_value not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_value parameter'
+        if metadata_value not in ['', None]:
+            assert metadata_field not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_field parameter'
 
+        metadata_field = 'fields.'+ metadata_field
         log.debug(f'Search file: {file_name} of type {file_type} on group {group_name}')
 
         # Prepare query parameters
-        init_query = {"name": file_name, "type": file_type, "uuid": None, "groupName": group_name}
+        init_query = {"name": file_name, "type": file_type, "uuid": None, "groupName": group_name, metadata_field:metadata_value}
         query = format_query(init_query)
 
         path = f'/file/search?size={size}&from={from_page}&query={query}'
         r = self.caller.get(path)
 
         log.debug(f'{r.url} \n {r.request.headers} \n {r.json()}')
         return r.json()
```

### Comparing `northgravity-0.1.6/northgravity/HTTPCalller.py` & `northgravity-0.1.7/northgravity/HTTPCalller.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.6/northgravity/StatusHandler.py` & `northgravity-0.1.7/northgravity/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.6/northgravity/TaskHandler.py` & `northgravity-0.1.7/northgravity/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.6/northgravity/Timeseries.py` & `northgravity-0.1.7/northgravity/Timeseries.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.6/northgravity/__init__.py` & `northgravity-0.1.7/northgravity/__init__.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.6/northgravity.egg-info/PKG-INFO` & `northgravity-0.1.7/northgravity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.6
+pip3 install northgravity==0.1.7
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.6
+northgravity==0.1.7
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.6/setup.py` & `northgravity-0.1.7/setup.py`

 * *Files identical despite different names*

