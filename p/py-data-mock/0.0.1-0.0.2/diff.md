# Comparing `tmp/py-data-mock-0.0.1.tar.gz` & `tmp/py-data-mock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-data-mock-0.0.1.tar", last modified: Tue May 23 05:19:23 2023, max compression
+gzip compressed data, was "py-data-mock-0.0.2.tar", last modified: Tue May 23 16:41:37 2023, max compression
```

## Comparing `py-data-mock-0.0.1.tar` & `py-data-mock-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.067957 py-data-mock-0.0.1/
--rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-05-20 20:50:55.000000 py-data-mock-0.0.1/LICENSE
--rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-23 05:19:23.067957 py-data-mock-0.0.1/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)       14 2023-05-20 20:50:55.000000 py-data-mock-0.0.1/README.md
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.063955 py-data-mock-0.0.1/data_mock/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.063955 py-data-mock-0.0.1/data_mock/google/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.063955 py-data-mock-0.0.1/data_mock/google/cloud/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.063955 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/
--rw-rw-r--   0 henry     (1000) henry     (1000)      583 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     4231 2023-05-23 05:11:08.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/client.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      301 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/dataset.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       85 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/exceptions.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.063955 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/job/
--rw-rw-r--   0 henry     (1000) henry     (1000)       70 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/job/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       80 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/job/query.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       22 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/retry.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      169 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/schema.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     2860 2023-05-23 05:11:08.000000 py-data-mock-0.0.1/data_mock/google/cloud/bigquery/table.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.063955 py-data-mock-0.0.1/data_mock/scripts/
--rw-rw-r--   0 henry     (1000) henry     (1000)     2245 2023-05-20 20:51:44.000000 py-data-mock-0.0.1/data_mock/scripts/mkmock.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.063955 py-data-mock-0.0.1/py_data_mock.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-23 05:19:23.000000 py-data-mock-0.0.1/py_data_mock.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)      605 2023-05-23 05:19:23.000000 py-data-mock-0.0.1/py_data_mock.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-05-23 05:19:23.000000 py-data-mock-0.0.1/py_data_mock.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       68 2023-05-23 05:19:23.000000 py-data-mock-0.0.1/py_data_mock.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-05-23 05:19:23.067957 py-data-mock-0.0.1/setup.cfg
--rw-rw-r--   0 henry     (1000) henry     (1000)      559 2023-05-23 05:19:04.000000 py-data-mock-0.0.1/setup.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 05:19:23.067957 py-data-mock-0.0.1/tests/
--rw-rw-r--   0 henry     (1000) henry     (1000)     1167 2023-05-20 20:54:11.000000 py-data-mock-0.0.1/tests/test1.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/
+-rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-05-20 20:50:55.000000 py-data-mock-0.0.2/LICENSE
+-rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3841 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/README.md
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.693477 py-data-mock-0.0.2/data_mock/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.693477 py-data-mock-0.0.2/data_mock/google/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.693477 py-data-mock-0.0.2/data_mock/google/cloud/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      583 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3969 2023-05-23 07:44:51.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/client.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      301 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/dataset.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       85 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/exceptions.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/job/
+-rw-rw-r--   0 henry     (1000) henry     (1000)       70 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/job/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       80 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/job/query.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       22 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/retry.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      169 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/schema.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2974 2023-05-23 07:44:51.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/table.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/google/cloud/storage/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      110 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1228 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/blob.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      522 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/bucket.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      445 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/client.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/mock_helpers/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1983 2023-05-23 07:44:51.000000 py-data-mock-0.0.2/data_mock/mock_helpers/provider.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      116 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/mock_helpers/writer.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/scripts/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2245 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/scripts/mkmock.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/py_data_mock.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)      837 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      122 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/top_level.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/setup.cfg
+-rw-rw-r--   0 henry     (1000) henry     (1000)      636 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/tests/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1167 2023-05-20 20:54:11.000000 py-data-mock-0.0.2/tests/test1.py
```

### Comparing `py-data-mock-0.0.1/LICENSE` & `py-data-mock-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.1/data_mock/google/cloud/bigquery/__init__.py` & `py-data-mock-0.0.2/data_mock/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.1/data_mock/google/cloud/bigquery/client.py` & `py-data-mock-0.0.2/data_mock/google/cloud/bigquery/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from . import exceptions
 from .  import table as _table
 from .job import query as job_query
 from . import retry as retries
 from . import dataset as _dataset
+import data_mock.mock_helpers.provider as provider
 
 from typing import Union, Optional
 
 # these values do nothing
 DEFAULT_RETRY = None
 DEFAULT_TIMEOUT = None
 DEFAULT_JOB_RETRY = None
 TimeoutType = Union[float, None]
 
 class Client:
 
-    def __init__(self, project = None, mock_data = [], 
+    def __init__(self, project = None, mock_data = None, 
             mock_list_of_tables = None):
-        self._test_valid_data(mock_data)
-        self.__data = mock_data
         self.project = project
-        self.__registered_data = {}
         self.__list_of_tables = mock_list_of_tables
+        self._data_provider = provider.ProvideData()
+        if mock_data:
+            self._data_provider.add_data(data = mock_data, tag = 'default_')
 
     def register_mock_data(self, key, mock_data):
-        self._test_valid_data(mock_data)
-        self.__registered_data[key] = mock_data
+        self._data_provider.add_data(data = mock_data, tag = key)
 
     def query(self, query,
         job_config: job_query.QueryJobConfig = None,
         job_id: str = None,
         job_id_prefix: str = None,
         location: str = None,
         project: str = None,
@@ -37,20 +37,20 @@
         job_retry: retries.Retry = DEFAULT_JOB_RETRY,
               ):
         """
         all args ignored except query
         """
         key = self._get_sql_key(query)
         if key:
-            data = self.__registered_data.get(key)
+            data, m = self._data_provider.get_data(key)
             if not data:
                 raise exceptions.InvalidMockData(f'{key} not found in registered_data')
         else:
-            data = self.__data
-        return _table.RowIterator(data = data)
+            data, m = self._data_provider.get_data('default_')
+        return _table.RowIterator(data = data, m = m)
 
     def create_table(self,
             table: Union[str, _table.Table, _table.TableReference, _table.TableListItem],
             exists_ok: bool = False,
             retry: retries.Retry = DEFAULT_RETRY,
             timeout: TimeoutType = DEFAULT_TIMEOUT,
         ):
@@ -109,17 +109,7 @@
         for line in query.split('\n'):
             if 'py-bigquery-mock-register:' in line:
                 fields = line.split(':')
                 if len(fields) != 2:
                     raise exceptions.InvalidMockData('hint should be in format "py-bigquery-mock-register: key"')
                 return fields[1].strip()
 
-    def _test_valid_data(self, data):
-        if not isinstance(data, list):
-            raise exceptions.InvalidMockData(f'{data} is not a list')
-        errors = []
-        for n, i in enumerate(data):
-            if not isinstance(i, list):
-                errors.append((n, i, 'not a list'))
-        if len(errors) != 0:
-            raise exceptions.InvalidMockData(errors)
-
```

### Comparing `py-data-mock-0.0.1/data_mock/google/cloud/bigquery/table.py` & `py-data-mock-0.0.2/data_mock/google/cloud/bigquery/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,51 +40,57 @@
 
 class Row():
 
     def __init__(self, row):
         self.__info = {}
         l = []
         for i in row:
-            self.__info[i[0]] = i[1]
-            l.append(i[1])
+            self.__info[i.name] = i.value
+            l.append(i.value)
         self.__values = tuple(l)
         self.row = row
 
     def get(self, *args, **kwargs):
         if args:
             return self.__info.get(args[0])
         return self.__info.get(kwargs['key'])
 
     def items(self, *args, **kwargs):
         for i in self.row:
-            yield i
+            yield i.name, i.value
 
     def values(self, *args, **kwargs):
         return self.__values
 
     def keys(self, *args, **kwargs):
         return self.__info.keys()
 
 class RowIterator:
 
-    def __init__(self, data):
-        self.__counter = 0
-        self.total_rows = len(data)
-        self.__data = data
-        self.schema = [schema.SchemaField(name = 'todo', field_type='INTEGER')]
+    def __init__(self, data, m):
+        if data == None:
+            def none_generator():
+                return
+                yield
+            self.__data = none_generator()
+            self.total_rows = 0
+        else:
+            self.__data = data
+            self.total_rows = m.get('total_rows')
+            self.schema = m.get('schema')
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        if self.__counter< self.total_rows:
-            self.__counter += 1
-            return Row(row = self.__data[self.__counter -1])
-        else:
+        v = next(self.__data)
+        if not v:
             raise StopIteration
+        else:
+            return Row(row = v)
 
     def result(self):
         return self
 
 
 class TimePartitioningType:
     """Specifies the type of time partitioning to perform."""
```

### Comparing `py-data-mock-0.0.1/data_mock/scripts/mkmock.py` & `py-data-mock-0.0.2/data_mock/scripts/mkmock.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.1/py_data_mock.egg-info/SOURCES.txt` & `py-data-mock-0.0.2/py_data_mock.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,13 +6,19 @@
 data_mock/google/cloud/bigquery/dataset.py
 data_mock/google/cloud/bigquery/exceptions.py
 data_mock/google/cloud/bigquery/retry.py
 data_mock/google/cloud/bigquery/schema.py
 data_mock/google/cloud/bigquery/table.py
 data_mock/google/cloud/bigquery/job/__init__.py
 data_mock/google/cloud/bigquery/job/query.py
+data_mock/google/cloud/storage/__init__.py
+data_mock/google/cloud/storage/blob.py
+data_mock/google/cloud/storage/bucket.py
+data_mock/google/cloud/storage/client.py
+data_mock/mock_helpers/provider.py
+data_mock/mock_helpers/writer.py
 data_mock/scripts/mkmock.py
 py_data_mock.egg-info/PKG-INFO
 py_data_mock.egg-info/SOURCES.txt
 py_data_mock.egg-info/dependency_links.txt
 py_data_mock.egg-info/top_level.txt
 tests/test1.py
```

### Comparing `py-data-mock-0.0.1/tests/test1.py` & `py-data-mock-0.0.2/tests/test1.py`

 * *Files identical despite different names*

