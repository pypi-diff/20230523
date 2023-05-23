# Comparing `tmp/foxglove-data-platform-0.6.0.tar.gz` & `tmp/foxglove-data-platform-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-data-platform-0.6.0.tar", last modified: Tue May 16 21:24:15 2023, max compression
+gzip compressed data, was "foxglove-data-platform-0.7.0.tar", last modified: Tue May 23 18:22:20 2023, max compression
```

## Comparing `foxglove-data-platform-0.6.0.tar` & `foxglove-data-platform-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/foxglove_data_platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/foxglove_data_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26827 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/foxglove_data_platform/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/foxglove_data_platform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 21:24:15.543779 foxglove-data-platform-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/api_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/string_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_json_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_protobuf_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_ros1_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_ros2_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.561392 foxglove-data-platform-0.7.0/foxglove_data_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/foxglove_data_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26812 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/foxglove_data_platform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/foxglove_data_platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.561392 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/string_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_json_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_protobuf_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_ros1_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_ros2_messages.py
```

### Comparing `foxglove-data-platform-0.6.0/LICENSE` & `foxglove-data-platform-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/PKG-INFO` & `foxglove-data-platform-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.6.0
+Version: 0.7.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.6.0/README.md` & `foxglove-data-platform-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/foxglove_data_platform/client.py` & `foxglove-data-platform-0.7.0/foxglove_data_platform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,24 +484,23 @@
         """
         response = requests.delete(
             self.__url__(f"/v1/devices/{device_id}"),
             headers=self.__headers,
         )
         json_or_raise(response)
 
-    def delete_import(self, *, device_id: str, import_id: str):
+    def delete_import(self, *, device_id: Optional[str] = None, import_id: str):
         """
         Deletes an existing import.
 
-        :param device_id: The id of the device associated with the import.
+        :param device_id: The id of the device associated with the import. (Deprecated; ignored.)
         :param import_id: The id of the import to delete.
         """
         response = requests.delete(
             self.__url__(f"/v1/data/imports/{import_id}"),
-            params={"deviceId": device_id},
             headers=self.__headers,
         )
         json_or_raise(response)
 
     def get_imports(
         self,
         *,
@@ -702,15 +701,15 @@
         self,
         *,
         id: str,
         callback: Optional[ProgressCallback] = None,
     ):
         """Download an attachment by ID.
 
-        :param attachment_id: the attachment ID.
+        :param id: the attachment ID.
         :param callback: a callback to track download progress
         :returns: The downloaded attachment bytes.
         """
         return _download_stream_with_progress(
             self.__url__(f"/v1/recording-attachments/{id}/download"),
             headers=self.__headers,
             callback=callback,
```

### Comparing `foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/PKG-INFO` & `foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.6.0
+Version: 0.7.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/SOURCES.txt` & `foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/setup.cfg` & `foxglove-data-platform-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-data-platform
-version = 0.6.0
+version = 0.7.0
 description = Client library for Foxglove Data Platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/py-data-platform
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `foxglove-data-platform-0.6.0/tests/generate.py` & `foxglove-data-platform-0.7.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/string_message_pb2.py` & `foxglove-data-platform-0.7.0/tests/string_message_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_attachments.py` & `foxglove-data-platform-0.7.0/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_client.py` & `foxglove-data-platform-0.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_coverage.py` & `foxglove-data-platform-0.7.0/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_data.py` & `foxglove-data-platform-0.7.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_devices.py` & `foxglove-data-platform-0.7.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_events.py` & `foxglove-data-platform-0.7.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_imports.py` & `foxglove-data-platform-0.7.0/tests/test_imports.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 from .api_url import api_url
 
 fake = Faker()
 
 
 @responses.activate
 def test_delete_import():
-    device_id = fake.uuid4()
     import_id = fake.uuid4()
     responses.add(
         responses.DELETE,
-        api_url(f"/v1/data/imports/{import_id}?deviceId={device_id}"),
+        api_url(f"/v1/data/imports/{import_id}"),
         json={"success": True},
     )
     try:
         client = Client("test")
-        client.delete_import(device_id=device_id, import_id=import_id)
+        client.delete_import(import_id=import_id)
     except:
         assert False
 
 
 @responses.activate
 def test_get_imports():
     device_id = "my_device_id"
```

### Comparing `foxglove-data-platform-0.6.0/tests/test_protobuf_messages.py` & `foxglove-data-platform-0.7.0/tests/test_protobuf_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_recordings.py` & `foxglove-data-platform-0.7.0/tests/test_recordings.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_ros1_messages.py` & `foxglove-data-platform-0.7.0/tests/test_ros1_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.6.0/tests/test_ros2_messages.py` & `foxglove-data-platform-0.7.0/tests/test_ros2_messages.py`

 * *Files identical despite different names*

