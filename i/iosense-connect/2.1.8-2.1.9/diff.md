# Comparing `tmp/iosense_connect-2.1.8.tar.gz` & `tmp/iosense_connect-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.8.tar", last modified: Tue May 23 05:25:51 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.9.tar", last modified: Tue May 23 12:02:33 2023, max compression
```

## Comparing `iosense_connect-2.1.8.tar` & `iosense_connect-2.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 05:25:51.619149 iosense_connect-2.1.8/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-23 05:25:51.617235 iosense_connect-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 05:25:51.577475 iosense_connect-2.1.8/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.8/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    23642 2023-05-23 05:25:41.000000 iosense_connect-2.1.8/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-23 05:25:51.606228 iosense_connect-2.1.8/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-23 05:25:51.000000 iosense_connect-2.1.8/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 05:25:51.619149 iosense_connect-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-23 05:25:41.000000 iosense_connect-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:02:32.932432 iosense_connect-2.1.9/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-23 12:02:32.930210 iosense_connect-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:02:32.766475 iosense_connect-2.1.9/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.9/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    23839 2023-05-23 12:00:24.000000 iosense_connect-2.1.9/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:02:32.926677 iosense_connect-2.1.9/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-23 12:02:32.000000 iosense_connect-2.1.9/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-23 12:02:32.000000 iosense_connect-2.1.9/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 12:02:32.000000 iosense_connect-2.1.9/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 12:02:32.000000 iosense_connect-2.1.9/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 12:02:32.932432 iosense_connect-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-23 12:02:23.000000 iosense_connect-2.1.9/setup.py
```

### Comparing `iosense_connect-2.1.8/LICENSE.txt` & `iosense_connect-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.8/PKG-INFO` & `iosense_connect-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.1.8
+Version: 2.1.9
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.8/README.md` & `iosense_connect-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.8/iosense_connect/data_access.py` & `iosense_connect-2.1.9/iosense_connect/data_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,21 @@
         :return: df
 
         If requested data exists in feature store fetch data from the container.
         IF data is not available the data is fetched from influxdb
 
         """
         try:
+            try:
+                end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
+            except Exception:
+                if type(end_time) == str:
+                    end_time = str(end_time) + " 23:59:59"
+                pass
+            unique_id = random.randint(10000, 100000000)
             df = pd.DataFrame()
             metadata = {}
             folder_path = f"{device_id}/"
             blob_svc = BlobServiceClient.from_connection_string(conn_str=self.connection_string)
             container_client = blob_svc.get_container_client(self.container_name)
             processed_blobs = [blob.name[len(folder_path):].lstrip("/").rsplit(".", 1)[0].split("-") for blob in
                                container_client.list_blobs(name_starts_with=folder_path)]
@@ -427,19 +434,19 @@
                 filtered_list = [*set(temp_list)]
                 date_range = sort_dates(filtered_list)
                 list_of_dates_in_azure = list(set(date_month_list).intersection(date_range))
                 return list_of_dates_in_azure
 
             def read_one(blobfile):
                 blob = blob_svc.get_blob_client(self.container_name, device_id + '/' + blobfile + '.parquet')
-                with open(blobfile + '.parquet', "wb") as my_blob:
-                    blob_data = blob.download_blob()
+                blob_data = blob.download_blob()
+                with open(str(unique_id)+'_'+blobfile+ '.parquet', "wb") as my_blob:
                     blob_data.readinto(my_blob)
-                df = pd.read_parquet(blobfile + '.parquet')
-                os.remove(blobfile + '.parquet')
+                df = pd.read_parquet(str(unique_id)+'_'+blobfile+ '.parquet')
+                os.remove(str(unique_id)+'_'+blobfile+ '.parquet')
                 return df
 
             def thread_read():
                 results = []
                 blob_list = get_dates()
                 if len(blob_list) !=0:
                     with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
@@ -454,20 +461,14 @@
                 return fetched_df
 
             flag = check_device(device_id)
             if flag and api==False:
                 df = thread_read()
                 if len(df) != 0:
                     try:
-                        end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
-                    except Exception:
-                        if type(end_time) == str:
-                            end_time = str(end_time) + " 23:59:59"
-                        pass
-                    try:
                         start_time = datetime.strptime(start_time, '%Y-%m-%d %H:%M:%S')
                         end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
                         df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
                     except ValueError:
                         df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
                         pass
                     except Exception as e:
@@ -480,25 +481,27 @@
                         sensor_list_df.remove('time')
                         sensors_filtered = list(set(sensor_list_df).intersection(sensors))
                         if sensors != None and len(sensors_filtered) != 0:
                             sensors_filtered.insert(0,'time')
                             df =  df[sensors_filtered]
                         if len(sensors_filtered) == 0:
                             df = pd.DataFrame()
+                        df.sort_values(['time'], inplace=True)
                         df.reset_index(drop=True, inplace=True)
                         last_date = df['time'].iloc[len(df) - 1]
                         start_date = last_date.date() + timedelta(days=1)
                         end_time = pd.to_datetime(end_time)
                         if last_date.date() != end_time.date():
                             df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
                             df = pd.concat([df, df1])
+                            df.reset_index(drop=True, inplace=True)
                         else:
                             df1 = DataAccess.fetch_data(self, device_id,start_time=str(last_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
                             df = pd.concat([df, df1])
-                        df.reset_index(drop=True, inplace=True)
+                            df.reset_index(drop=True, inplace=True)
             else:
                 df_devices = DataAccess.get_device_details(self,onpremise=onpremise)
                 device_list = df_devices['devID'].tolist()
                 if device_id in device_list:
                     df = DataAccess.fetch_data(self, device_id, start_time,end_time, alias,sensors=sensors,echo=True,onpremise=onpremise,IST=IST)
                 else:
                     raise Exception('Message: Device not added in account')
```

### Comparing `iosense_connect-2.1.8/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.9/iosense_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.1.8
+Version: 2.1.9
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.8/setup.py` & `iosense_connect-2.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.8",
+    version = "2.1.9",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

