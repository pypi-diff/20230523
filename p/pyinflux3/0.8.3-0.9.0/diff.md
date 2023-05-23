# Comparing `tmp/pyinflux3-0.8.3.tar.gz` & `tmp/pyinflux3-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.8.3.tar", last modified: Wed May  3 14:06:51 2023, max compression
+gzip compressed data, was "pyinflux3-0.9.0.tar", last modified: Mon May 22 12:56:46 2023, max compression
```

## Comparing `pyinflux3-0.8.3.tar` & `pyinflux3-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-03 14:06:45.000000 pyinflux3-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-03 14:06:45.000000 pyinflux3-0.8.3/influxdb_client_3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/pyinflux3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-03 14:06:45.000000 pyinflux3-0.8.3/setup-client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:46.590803 pyinflux3-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-22 12:56:46.590803 pyinflux3-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-22 12:56:36.000000 pyinflux3-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:46.586802 pyinflux3-0.9.0/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-22 12:56:36.000000 pyinflux3-0.9.0/influxdb_client_3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:46.590803 pyinflux3-0.9.0/pyinflux3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-22 12:56:46.000000 pyinflux3-0.9.0/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 12:56:46.000000 pyinflux3-0.9.0/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:56:46.000000 pyinflux3-0.9.0/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-22 12:56:46.000000 pyinflux3-0.9.0/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 12:56:46.000000 pyinflux3-0.9.0/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-22 12:56:36.000000 pyinflux3-0.9.0/setup-client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:56:46.590803 pyinflux3-0.9.0/setup.cfg
```

### Comparing `pyinflux3-0.8.3/PKG-INFO` & `pyinflux3-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.8.3
+Version: 0.9.0
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,87 +22,133 @@
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
 
 # Install
 To install only the client:
+
 ```bash
 python3 -m pip install pyinflux3
 ```
+
 To install the client and CLI:
+
 ```bash
 sudo python3 -m pip install "pyinflux3[cli]"
 ```
+
 ***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
 
 # Add a Config
-You can drop a config file called config.json in the directory where you are running the influx3 command:
+
+To configure `pyinflux3` and the CLI, do one of the following:
+
+You can drop a config file called `config.json` in the directory where you are running the `influx3` command:
 
 ```json
 {
-{
     "my-config": {
         "database": "your-database",
         "host": "your-host",
         "token": "your-token",
         "org": "your-org-id",
         "active": true
     }
 }
-}
 ```
 
-Or you can use the config command to create or modify a config:
-```
-% influx3 config --name="my-config" --database="<database or bucket name>" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --org="<your org ID>"
-```
 
-If you are running against InfluxDB Cloud Serverless, then use the bucket name for the database in you configuration.
+- Use the `config` command to create or modify a config:
+
+    ```
+    influx3 config \
+    --name="my-config" \
+    --database="<database or bucket name>" \
+    --host="us-east-1-1.aws.cloud2.influxdata.com" \
+    --token="<your token>" \
+    --org="<your org ID>"
+    ```
+
+If you are running against InfluxDB Cloud Serverless, then use the _bucket name_ as the database in your configuration.
 
 # Run as a Command
+
 ```
-% influx3 sql "select * from anomalies"
+influx3 sql "select * from anomalies"
 ```
 
 ```
-% influx3 write testmes f=7 
+influx3 write testmes f=7 
 ```
 
 # Query and Write Interactively
 
+In your terminal, enter the following command:
+
+```
+influx3
+```
+
+`influx3` displays the `(>)` interactive prompt and waits for input.
 
 ```
-% influx3
 Welcome to my IOx CLI.
 
+(>)
+```
+
+To query, type `sql` at the prompt.
+
+```
 (>) sql
-(sql >) select * from anomalies
-    check    id  observed                          time     type user_id  value
-0       1  None       NaN 2023-02-03 20:56:57.513279776    error       1  400.0
-1       1  None       NaN 2023-02-03 17:52:54.328785835  latency       1  900.0
 ```
 
+At the `(sql >)` prompt, enter your query statement:
+
+```
+(sql >) select * from home
+```
+
+The `influx3` CLI displays query results in Markdown table format--for example:
+
+```
+|     |   co |   hum | room        |   temp | time                          |
+|----:|-----:|------:|:------------|-------:|:------------------------------|
+|   0 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:00           |
+|   1 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:50           |
+```
+
+To write, type `write` at the `(>)` prompt.
+
+```
+(>) write
+```
+
+At the `(write >)` prompt, enter line protocol data.
+
 ```
 (>) write 
-testmes f=5 boring-observability
+home,room=kitchen temp=70.5,hum=80
 ```
 
+To exit a prompt, enter `exit`.
+
 # Write from a File
+
 Both the InfluxDB CLI and Client libary support writing from a CSV file. The CSV file must have a header row with the column names. The there must be a column containing a timestamp. Here are the parse options:
 * `--file` - The path to the csv file.
 * `--time` - The name of the column containing the timestamp.
-* `--measurment` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
+* `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
 * `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
 
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
-
 # Client library
 This project also includes a new client library that strives for utter simplicity. It includes 3 functions, a constuctor, write(), and read().
 
 # Contribution
 If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. This can currently be achived using the following method:
 ```bash
 python3 -m venv .venv
```

### Comparing `pyinflux3-0.8.3/influxdb_client_3/__init__.py` & `pyinflux3-0.9.0/influxdb_client_3/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 # influxdb_client_3/__init__.py
 
 from pyarrow import csv
-import pyarrow.flight as flight
-from flightsql import FlightSQLClient
+from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
 from influxdb_client import InfluxDBClient as _InfluxDBClient
+from influxdb_client import WriteOptions as _WriteOptions
 from influxdb_client.client.write_api import WriteApi as _WriteApi
 from influxdb_client.client.write_api import SYNCHRONOUS, ASYNCHRONOUS
 from influxdb_client import Point
+import json
+
+def write_options(**kwargs):
+   return  _WriteOptions(**kwargs)
+
+
 
 class InfluxDBClient3:
-    def __init__(self, host=None, org=None, database=None, token=None, write_options="SYNCHRONOUS", **kwargs):
+    def __init__(self, host=None, org=None, database=None, token=None, write_options=None, **kwargs):
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
+        self.write_options = write_options
 
-        if write_options == "SYNCHRONOUS":
+        if self.write_options == None:
             self.write_options = SYNCHRONOUS
-        elif write_options == "ASYNCHRONOUS":
-            self.write_options = ASYNCHRONOUS
-        else:
-            raise ValueError("write_options must be SYNCHRONOUS or ASYNCHRONOUS")
 
      
         self._client = _InfluxDBClient(url=f"https://{host}", token=token, org=self._org, **kwargs )
         self._write_api = _WriteApi(self._client, write_options=self.write_options )
-        self._flight_sql_client = FlightSQLClient(host=host,
-                                                  token=token,
-                                                  metadata={'bucket-name':database})
+        
+        self._flight_client = FlightClient(f"grpc+tls://{host}:443")
+        # create an authorization header
+        self._options = FlightCallOptions(headers=[(b"authorization",f"Bearer {token}".encode('utf-8'))])
 
     def write(self, record=None, **kwargs):
         """
         Write data to InfluxDB.
 
         :type database: str
         :param record: The data point(s) to write.
@@ -69,23 +73,31 @@
                                   data_frame_timestamp_column = timestamp_column )
         except Exception as e:
             print(e)
     
 
 
 
-    def query(self, sql_query):
-        """
-        Query data from InfluxDB IOx using FlightSQL.
-
-        :param sql_query: The SQL query string to execute.
-        :type sql_query: str
-        :return: pyarrow.Table
-        """
-        query = self._flight_sql_client.execute(sql_query)
-        return self._flight_sql_client.do_get(query.endpoints[0].ticket)
+    def query(self, query, language="sql"):
+        # create a flight client pointing to the InfluxDB
+        # create a ticket
+        ticket_data = {
+        "database": self._database,
+        "sql_query": query,
+        "query_type": language}
+        
+        ticket_bytes = json.dumps(ticket_data)
+        ticket = Ticket(ticket_bytes)
+        
+        # execute the query and return all the data
+        flight_reader = self._flight_client.do_get(ticket, self._options)
+
+        # use read_all() to get all of the data as an Arrow table
+        # there are other functions to iterate through rows or read only parts of the data
+        # which is useful if you have huge data sets
+        return flight_reader.read_all()
 
     def __del__(self):
         self._write_api.__del__()
         return self._client.__del__()
 
 __all__ = ["InfluxDBClient3", "Point"]
```

### Comparing `pyinflux3-0.8.3/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.9.0/pyinflux3.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.8.3
+Version: 0.9.0
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,87 +22,133 @@
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
 
 # Install
 To install only the client:
+
 ```bash
 python3 -m pip install pyinflux3
 ```
+
 To install the client and CLI:
+
 ```bash
 sudo python3 -m pip install "pyinflux3[cli]"
 ```
+
 ***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
 
 # Add a Config
-You can drop a config file called config.json in the directory where you are running the influx3 command:
+
+To configure `pyinflux3` and the CLI, do one of the following:
+
+You can drop a config file called `config.json` in the directory where you are running the `influx3` command:
 
 ```json
 {
-{
     "my-config": {
         "database": "your-database",
         "host": "your-host",
         "token": "your-token",
         "org": "your-org-id",
         "active": true
     }
 }
-}
 ```
 
-Or you can use the config command to create or modify a config:
-```
-% influx3 config --name="my-config" --database="<database or bucket name>" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --org="<your org ID>"
-```
 
-If you are running against InfluxDB Cloud Serverless, then use the bucket name for the database in you configuration.
+- Use the `config` command to create or modify a config:
+
+    ```
+    influx3 config \
+    --name="my-config" \
+    --database="<database or bucket name>" \
+    --host="us-east-1-1.aws.cloud2.influxdata.com" \
+    --token="<your token>" \
+    --org="<your org ID>"
+    ```
+
+If you are running against InfluxDB Cloud Serverless, then use the _bucket name_ as the database in your configuration.
 
 # Run as a Command
+
 ```
-% influx3 sql "select * from anomalies"
+influx3 sql "select * from anomalies"
 ```
 
 ```
-% influx3 write testmes f=7 
+influx3 write testmes f=7 
 ```
 
 # Query and Write Interactively
 
+In your terminal, enter the following command:
+
+```
+influx3
+```
+
+`influx3` displays the `(>)` interactive prompt and waits for input.
 
 ```
-% influx3
 Welcome to my IOx CLI.
 
+(>)
+```
+
+To query, type `sql` at the prompt.
+
+```
 (>) sql
-(sql >) select * from anomalies
-    check    id  observed                          time     type user_id  value
-0       1  None       NaN 2023-02-03 20:56:57.513279776    error       1  400.0
-1       1  None       NaN 2023-02-03 17:52:54.328785835  latency       1  900.0
 ```
 
+At the `(sql >)` prompt, enter your query statement:
+
+```
+(sql >) select * from home
+```
+
+The `influx3` CLI displays query results in Markdown table format--for example:
+
+```
+|     |   co |   hum | room        |   temp | time                          |
+|----:|-----:|------:|:------------|-------:|:------------------------------|
+|   0 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:00           |
+|   1 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:50           |
+```
+
+To write, type `write` at the `(>)` prompt.
+
+```
+(>) write
+```
+
+At the `(write >)` prompt, enter line protocol data.
+
 ```
 (>) write 
-testmes f=5 boring-observability
+home,room=kitchen temp=70.5,hum=80
 ```
 
+To exit a prompt, enter `exit`.
+
 # Write from a File
+
 Both the InfluxDB CLI and Client libary support writing from a CSV file. The CSV file must have a header row with the column names. The there must be a column containing a timestamp. Here are the parse options:
 * `--file` - The path to the csv file.
 * `--time` - The name of the column containing the timestamp.
-* `--measurment` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
+* `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
 * `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
 
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
-
 # Client library
 This project also includes a new client library that strives for utter simplicity. It includes 3 functions, a constuctor, write(), and read().
 
 # Contribution
 If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. This can currently be achived using the following method:
 ```bash
 python3 -m venv .venv
```

### Comparing `pyinflux3-0.8.3/setup-client.py` & `pyinflux3-0.9.0/setup-client.py`

 * *Files identical despite different names*

