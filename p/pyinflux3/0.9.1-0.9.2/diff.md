# Comparing `tmp/pyinflux3-0.9.1.tar.gz` & `tmp/pyinflux3-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.9.1.tar", last modified: Tue May 23 11:36:16 2023, max compression
+gzip compressed data, was "pyinflux3-0.9.2.tar", last modified: Tue May 23 13:08:55 2023, max compression
```

## Comparing `pyinflux3-0.9.1.tar` & `pyinflux3-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:36:16.950678 pyinflux3-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-23 11:36:16.950678 pyinflux3-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-23 11:36:10.000000 pyinflux3-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:36:16.950678 pyinflux3-0.9.1/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-23 11:36:10.000000 pyinflux3-0.9.1/influxdb_client_3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:36:16.950678 pyinflux3-0.9.1/pyinflux3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-23 11:36:16.000000 pyinflux3-0.9.1/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 11:36:16.000000 pyinflux3-0.9.1/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:36:16.000000 pyinflux3-0.9.1/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 11:36:16.000000 pyinflux3-0.9.1/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 11:36:16.000000 pyinflux3-0.9.1/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-23 11:36:10.000000 pyinflux3-0.9.1/setup-client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:36:16.950678 pyinflux3-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:55.882438 pyinflux3-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-23 13:08:55.882438 pyinflux3-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-23 13:08:49.000000 pyinflux3-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:55.882438 pyinflux3-0.9.2/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-23 13:08:49.000000 pyinflux3-0.9.2/influxdb_client_3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:55.882438 pyinflux3-0.9.2/pyinflux3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-23 13:08:55.000000 pyinflux3-0.9.2/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 13:08:55.000000 pyinflux3-0.9.2/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:08:55.000000 pyinflux3-0.9.2/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 13:08:55.000000 pyinflux3-0.9.2/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:08:55.000000 pyinflux3-0.9.2/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-23 13:08:49.000000 pyinflux3-0.9.2/setup-client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:08:55.882438 pyinflux3-0.9.2/setup.cfg
```

### Comparing `pyinflux3-0.9.1/PKG-INFO` & `pyinflux3-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.9.1
+Version: 0.9.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.9.1/README.md` & `pyinflux3-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.9.1/influxdb_client_3/__init__.py` & `pyinflux3-0.9.2/influxdb_client_3/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,34 +10,41 @@
 from influxdb_client.domain.write_precision import WritePrecision
 from influxdb_client import Point
 import json
 
 def write_options(**kwargs):
    return  _WriteOptions(**kwargs)
 
+def flight_client_options(**kwargs):
+    return kwargs  # You can replace this with a specific data structure if needed
+
+
+
 
 
 
 class InfluxDBClient3:
-    def __init__(self, host=None, org=None, database=None, token=None, write_options=None, **kwargs):
+    def __init__(self, host=None, org=None, database=None, token=None, write_options=None, flight_client_options=None ,**kwargs):
         """
         This class provides an interface for interacting with an InfluxDB server, simplifying common operations such as writing, querying.
         * host (str, optional): The hostname or IP address of the InfluxDB server. Defaults to None.
         * org (str, optional): The InfluxDB organization name to be used for operations. Defaults to None.
         * database (str, optional): The database to be used for InfluxDB operations. Defaults to None.
         * token (str, optional): The authentication token for accessing the InfluxDB server. Defaults to None.
         * write_options (enum, optional): Specifies the write mode (synchronous or asynchronous) to use when writing data points to InfluxDB. Defaults to SYNCHRONOUS.
         * **kwargs: Additional arguments to be passed to the InfluxDB Client.
         """
         self._org = org
         self._database = database
         self.write_options = write_options if write_options is not None else SYNCHRONOUS
         self._client = _InfluxDBClient(url=f"https://{host}", token=token, org=self._org, **kwargs )
         self._write_api = _WriteApi(self._client, write_options=self.write_options )
-        self._flight_client = FlightClient(f"grpc+tls://{host}:443")
+
+        self._flight_client_options = flight_client_options if flight_client_options is not None else {}
+        self._flight_client = FlightClient(f"grpc+tls://{host}:443", **self._flight_client_options)
         # create an authorization header
         self._options = FlightCallOptions(headers=[(b"authorization",f"Bearer {token}".encode('utf-8'))])
 
     def write(self, record=None, **kwargs):
         """
         Write data to InfluxDB.
 
@@ -105,8 +112,8 @@
     
     def __enter__(self):
         return self
     
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
-__all__ = ["InfluxDBClient3", "Point", "PointSettings", "SYNCHRONOUS", "ASYNCHRONOUS", "write_options", "WritePrecision"]
+__all__ = ["InfluxDBClient3", "Point", "PointSettings", "SYNCHRONOUS", "ASYNCHRONOUS", "write_options", "WritePrecision", "flight_client_options"]
```

### Comparing `pyinflux3-0.9.1/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.9.2/pyinflux3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.9.1
+Version: 0.9.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.9.1/setup-client.py` & `pyinflux3-0.9.2/setup-client.py`

 * *Files identical despite different names*

