# Comparing `tmp/funke_enrichment_core-1.8.tar.gz` & `tmp/funke_enrichment_core-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funke_enrichment_core-1.8.tar", last modified: Tue Mar  7 12:30:23 2023, max compression
+gzip compressed data, was "funke_enrichment_core-1.9.tar", last modified: Wed Mar  8 09:54:59 2023, max compression
```

## Comparing `funke_enrichment_core-1.8.tar` & `funke_enrichment_core-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-07 12:30:23.098890 funke_enrichment_core-1.8/
--rw-r--r--   0 worker    (1000) worker    (1000)      285 2023-03-07 12:30:23.098890 funke_enrichment_core-1.8/PKG-INFO
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-07 12:30:23.096890 funke_enrichment_core-1.8/funke_enrichment_core/
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-03-01 12:35:19.000000 funke_enrichment_core-1.8/funke_enrichment_core/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6720 2023-03-05 10:45:52.000000 funke_enrichment_core-1.8/funke_enrichment_core/control.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8584 2023-03-07 12:30:18.000000 funke_enrichment_core-1.8/funke_enrichment_core/helper.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2533 2023-03-07 12:30:18.000000 funke_enrichment_core-1.8/funke_enrichment_core/io.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-07 12:30:23.097890 funke_enrichment_core-1.8/funke_enrichment_core.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)      285 2023-03-07 12:30:23.000000 funke_enrichment_core-1.8/funke_enrichment_core.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)      359 2023-03-07 12:30:23.000000 funke_enrichment_core-1.8/funke_enrichment_core.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-03-07 12:30:23.000000 funke_enrichment_core-1.8/funke_enrichment_core.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)      131 2023-03-07 12:30:23.000000 funke_enrichment_core-1.8/funke_enrichment_core.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       22 2023-03-07 12:30:23.000000 funke_enrichment_core-1.8/funke_enrichment_core.egg-info/top_level.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       38 2023-03-07 12:30:23.098890 funke_enrichment_core-1.8/setup.cfg
--rw-rw-rw-   0 worker    (1000) worker    (1000)      608 2023-03-07 12:30:18.000000 funke_enrichment_core-1.8/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-08 09:54:59.382442 funke_enrichment_core-1.9/
+-rw-r--r--   0 worker    (1000) worker    (1000)      285 2023-03-08 09:54:59.382442 funke_enrichment_core-1.9/PKG-INFO
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-08 09:54:59.380442 funke_enrichment_core-1.9/funke_enrichment_core/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-03-01 12:35:19.000000 funke_enrichment_core-1.9/funke_enrichment_core/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6720 2023-03-05 10:45:52.000000 funke_enrichment_core-1.9/funke_enrichment_core/control.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8586 2023-03-08 09:53:55.000000 funke_enrichment_core-1.9/funke_enrichment_core/helper.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2616 2023-03-08 09:53:55.000000 funke_enrichment_core-1.9/funke_enrichment_core/io.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-08 09:54:59.381442 funke_enrichment_core-1.9/funke_enrichment_core.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)      285 2023-03-08 09:54:59.000000 funke_enrichment_core-1.9/funke_enrichment_core.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)      359 2023-03-08 09:54:59.000000 funke_enrichment_core-1.9/funke_enrichment_core.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-03-08 09:54:59.000000 funke_enrichment_core-1.9/funke_enrichment_core.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)      131 2023-03-08 09:54:59.000000 funke_enrichment_core-1.9/funke_enrichment_core.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       22 2023-03-08 09:54:59.000000 funke_enrichment_core-1.9/funke_enrichment_core.egg-info/top_level.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       38 2023-03-08 09:54:59.382442 funke_enrichment_core-1.9/setup.cfg
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      608 2023-03-08 09:54:55.000000 funke_enrichment_core-1.9/setup.py
```

### Comparing `funke_enrichment_core-1.8/funke_enrichment_core/control.py` & `funke_enrichment_core-1.9/funke_enrichment_core/control.py`

 * *Files identical despite different names*

### Comparing `funke_enrichment_core-1.8/funke_enrichment_core/helper.py` & `funke_enrichment_core-1.9/funke_enrichment_core/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
 def publish_data_to_pubsub_topic(topic_path, data, filter_attrs={}, encoding='utf-8'):
     """
     Publish given data to a Pub/Sub topic as a bytes converted json string.
 
     topic_path: Full path of the Pub/Sub topic.
     data: Json serialziable data to publish.
-    recipients: List of filter keys to add to the message with the value "True"
+    filter_attrs: List of filter keys to add to the message with the value "True"
     encoding: How to encode the json string. Default is utf-8.
     return: Returns the Future object and None in case of an error.
     """
     if not (topic_path and isinstance(topic_path, str)):
         raise ValueError('topic_path needs to be a non empty string!')
     if data is None:
         raise ValueError('data needs to be given!')
```

### Comparing `funke_enrichment_core-1.8/funke_enrichment_core/io.py` & `funke_enrichment_core-1.9/funke_enrichment_core/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,19 @@
         return self.payload
 
 
 class WriteToBigQuery():
     """
     Class to write to BQ
     """
-    def __init__(self, table_path, table_schema, write_disposition, allow_missing_columns):
+    def __init__(self, table_path, table_schema, write_disposition, default_missing_columns=False):
         self.table = table_path
         self.job_config = bigquery.LoadJobConfig(schema=table_schema,
                                                  write_disposition=write_disposition,
-                                                 allow_jagged_rows=allow_missing_columns
+                                                 allow_jagged_rows=default_missing_columns
                                                 )
 
     async def process(self, inp_data):
         job_future = save_dict_as_row_to_bq(inp_data, self.table, self.job_config)
         await asyncio.sleep(0.1)
         for _ in range(600):
             if job_future.done():
@@ -47,32 +47,32 @@
         
         
 
 class PublishOnPubSubTopic():
     """
     Class to publish to a pubsub topic
     """
-    def __init__(self, topic_path):
+    def __init__(self, topic_path, filter_attrs):
         self.topic_path = topic_path
-
+        self.filter_attrs = filter_attrs
 
     def _make_dict_json_serializable(self, json_dict):
         for key, value in json_dict.items():
             if isinstance(value, datetime):
                 json_dict[key] = value.strftime("%Y-%m-%dT%H:%M:%S")
             elif isinstance(value, dict):
                 json_dict[key] = self._make_dict_json_serializable(value)
             else:
                 json_dict[key] = value
 
         return json_dict
 
     async def process(self, inp_data):
         pubsub_dict = self._make_dict_json_serializable(inp_data)
-        job_future = publish_data_to_pubsub_topic(self.topic_path, pubsub_dict)
+        job_future = publish_data_to_pubsub_topic(self.topic_path, pubsub_dict, self.filter_attrs)
         await asyncio.sleep(0.1)
         for _ in range(600):
             if job_future.done():
                 return {self.topic_path: True}
             else:
                 await asyncio.sleep(0.5)
```

### Comparing `funke_enrichment_core-1.8/setup.py` & `funke_enrichment_core-1.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='funke_enrichment_core',
-    version='1.8',
+    version='1.9',
     author='Friedrich Schmidt',
     author_email='friedrich.schmidt@funkemedien.de',
     packages=['funke_enrichment_core'],
     scripts=[],
     license='MIT',
     description='This package contains everthing to orchestrate several microservices in the GCP',
     install_requires=[
```

