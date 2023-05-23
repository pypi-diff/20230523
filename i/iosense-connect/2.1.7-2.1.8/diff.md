# Comparing `tmp/iosense_connect-2.1.7.tar.gz` & `tmp/iosense_connect-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.7.tar", last modified: Thu May 18 09:17:55 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.8.tar", last modified: Tue May 23 05:25:51 2023, max compression
```

## Comparing `iosense_connect-2.1.7.tar` & `iosense_connect-2.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 09:17:55.916821 iosense_connect-2.1.7/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-18 09:17:55.913871 iosense_connect-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 09:17:55.878542 iosense_connect-2.1.7/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.7/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    23617 2023-05-18 09:17:04.000000 iosense_connect-2.1.7/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:17:55.909823 iosense_connect-2.1.7/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 09:17:55.917825 iosense_connect-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-18 09:17:53.000000 iosense_connect-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:25:51.619149 iosense_connect-2.1.8/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-23 05:25:51.617235 iosense_connect-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 05:25:51.577475 iosense_connect-2.1.8/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.8/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    23642 2023-05-23 05:25:41.000000 iosense_connect-2.1.8/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:25:51.606228 iosense_connect-2.1.8/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 05:25:51.619149 iosense_connect-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-23 05:25:41.000000 iosense_connect-2.1.8/setup.py
```

### Comparing `iosense_connect-2.1.7/LICENSE.txt` & `iosense_connect-2.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.7/PKG-INFO` & `iosense_connect-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.1.7
+Version: 2.1.8
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.7/README.md` & `iosense_connect-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.7/iosense_connect/data_access.py` & `iosense_connect-2.1.8/iosense_connect/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
             if len(df.columns) == 2:
                 df['sensor'] = sensors[0]
             if str(alias).lower() == "true":
                 df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata,onpremise=onpremise)
             df = DataAccess.get_cleaned_table(self, df)
         return df
 
-    def data_query(self, device_id, sensors,start_time, end_time=str(datetime.now()), alias=True,cal=True, bands=None,onpremise=False,compute=None,IST=True):
+    def data_query(self, device_id, sensors,start_time, end_time=str(datetime.now()), alias=True,cal=True, bands=None,onpremise=False,compute=None,api=False,IST=True):
         """
 
         :param device_id: string
         :param start_time: yyyy-MM-dd HH:MM:SS
         :param end_time: yyyy-MM-dd HH:MM:SS
         :param cal: bool
         :param bands: None
@@ -450,15 +450,15 @@
                         results = executor.map(read_one, blob_list)
                     fetched_df = pd.concat(results, axis=0)
                 else:
                     fetched_df=pd.DataFrame()
                 return fetched_df
 
             flag = check_device(device_id)
-            if flag:
+            if flag and api==False:
                 df = thread_read()
                 if len(df) != 0:
                     try:
                         end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
                     except Exception:
                         if type(end_time) == str:
                             end_time = str(end_time) + " 23:59:59"
```

### Comparing `iosense_connect-2.1.7/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.8/iosense_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.1.7
+Version: 2.1.8
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.7/setup.py` & `iosense_connect-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.7",
+    version = "2.1.8",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

