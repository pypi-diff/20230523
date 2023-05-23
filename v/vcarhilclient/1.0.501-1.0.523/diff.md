# Comparing `tmp/vcarhilclient-1.0.501.tar.gz` & `tmp/vcarhilclient-1.0.523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcarhilclient-1.0.501.tar", last modified: Fri May  5 09:45:21 2023, max compression
+gzip compressed data, was "vcarhilclient-1.0.523.tar", last modified: Tue May 23 10:17:15 2023, max compression
```

## Comparing `vcarhilclient-1.0.501.tar` & `vcarhilclient-1.0.523.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:45:21.543086 vcarhilclient-1.0.501/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.501/LICENSE
--rw-rw-rw-   0        0        0     2644 2023-05-05 09:45:21.544086 vcarhilclient-1.0.501/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.501/README.md
--rw-rw-rw-   0        0        0       86 2023-05-05 09:45:21.544086 vcarhilclient-1.0.501/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-05-05 09:43:01.000000 vcarhilclient-1.0.501/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:45:21.532489 vcarhilclient-1.0.501/vcarhilclient/
--rw-rw-rw-   0        0        0     5869 2023-04-26 08:02:47.000000 vcarhilclient-1.0.501/vcarhilclient/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.501/vcarhilclient/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.501/vcarhilclient/drt_structures.py
--rw-rw-rw-   0        0        0     3447 2023-04-26 08:02:47.000000 vcarhilclient-1.0.501/vcarhilclient/kunyi_ma.py
--rw-rw-rw-   0        0        0    48165 2023-05-05 09:43:01.000000 vcarhilclient-1.0.501/vcarhilclient/kunyi_mrt.py
--rw-rw-rw-   0        0        0    11499 2023-05-05 09:43:01.000000 vcarhilclient-1.0.501/vcarhilclient/kunyi_project.py
--rw-rw-rw-   0        0        0    11805 2023-05-05 09:43:01.000000 vcarhilclient-1.0.501/vcarhilclient/kunyi_util.py
--rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.501/vcarhilclient/minio_handld.py
--rw-rw-rw-   0        0        0     2000 2023-05-05 09:43:01.000000 vcarhilclient-1.0.501/vcarhilclient/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.501/vcarhilclient/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:45:21.542087 vcarhilclient-1.0.501/vcarhilclient.egg-info/
--rw-rw-rw-   0        0        0     2644 2023-05-05 09:45:21.000000 vcarhilclient-1.0.501/vcarhilclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-05 09:45:21.000000 vcarhilclient-1.0.501/vcarhilclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:45:21.000000 vcarhilclient-1.0.501/vcarhilclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 09:45:21.000000 vcarhilclient-1.0.501/vcarhilclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 09:45:21.000000 vcarhilclient-1.0.501/vcarhilclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 10:17:15.895763 vcarhilclient-1.0.523/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.523/LICENSE
+-rw-rw-rw-   0        0        0     2644 2023-05-23 10:17:15.895763 vcarhilclient-1.0.523/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.523/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-23 10:17:15.896763 vcarhilclient-1.0.523/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-05-23 10:03:09.000000 vcarhilclient-1.0.523/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:17:15.880306 vcarhilclient-1.0.523/vcarhilclient/
+-rw-rw-rw-   0        0        0     6908 2023-05-06 03:10:40.000000 vcarhilclient-1.0.523/vcarhilclient/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.523/vcarhilclient/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.523/vcarhilclient/drt_structures.py
+-rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_ma.py
+-rw-rw-rw-   0        0        0    50292 2023-05-23 10:04:11.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    14731 2023-05-23 05:14:59.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_project.py
+-rw-rw-rw-   0        0        0    12030 2023-05-23 05:14:01.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_util.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.523/vcarhilclient/minio_handld.py
+-rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.523/vcarhilclient/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.523/vcarhilclient/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:17:15.893766 vcarhilclient-1.0.523/vcarhilclient.egg-info/
+-rw-rw-rw-   0        0        0     2644 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/top_level.txt
```

### Comparing `vcarhilclient-1.0.501/LICENSE` & `vcarhilclient-1.0.523/LICENSE`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.501/PKG-INFO` & `vcarhilclient-1.0.523/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.501
+Version: 1.0.523
 Summary: vcarhilclient
 Home-page: UNKNOWN
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vcarhilclient-1.0.501/README.md` & `vcarhilclient-1.0.523/README.md`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.501/setup.py` & `vcarhilclient-1.0.523/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vcarhilclient",  # 包名
-    version="1.0.501",
+    version="1.0.523",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="vcarhilclient",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `vcarhilclient-1.0.501/vcarhilclient/Enums.py` & `vcarhilclient-1.0.523/vcarhilclient/Enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,38 @@
     MRT_ERR_FILE_ID_NOT_MATCH = -8,
     MRT_ERR_RPC_CALL_TIMEOUT = -9,
     MRT_ERR_INVALID_NAME = -10,
     MRT_ERR_DAQ_DATA_OBJ_INVALID = -11,
     MRT_ERR_SVC_EXEC_ERROR = -12,
     MRT_ERR_NOT_IMPLEMENT = -13,
     MRT_ERR_INVALID_RPC_RESP_SIZE = -14,
+    MRT_ERR_SVC_ROUTE_FAIL = -1024,
+    MRT_VRPC_ERR_SVC_NOT_IMPLEMENTED = -1023,
+    MRT_VRPC_ERR_SVC_MALLOC_FAIL = -1022,
+    MRT_VRPC_ERR_SVC_IN_PROGRESS = -1021,
+    MRT_VRPC_ERR_RESP_BUF_SIZE_INVALID = -1020,
+    MRT_VRPC_ERR_TIMEOUT = -1019,
+    MRT_VRPC_ERR_GENERIC_ERROR = -1018,
+    MRT_VRPC_ERR_SVC_SIGNATURE_INVALID = -1017,
+    MRT_VRPC_ERR_INVALID_ARG = -1016,
+    MRT_VRPC_ERR_CLI_SVC_NAME_INVALID = -1015,
+    MRT_VRPC_ERR_CLI_SOCK_INVALID = -1014,
+    MRT_VRPC_ERR_CLI_INVALID_DATA_SIZE = -1013,
+    MRT_VRPC_ERR_CLI_INVALID_FN_ID = -1012,
+    MRT_VRPC_ERR_CLI_INVALID_SN = -1011,
+    MRT_VRPC_ERR_CLI_INVALID_RESP = -1010,
+    MRT_VRPC_ERR_CLI_RECV_FAIL = -1009,
+    MRT_VRPC_ERR_CLI_SEND_FAIL = -1008,
+    MRT_VRPC_ERR_CLI_MSG_INIT_FAIL = -1007,
+    MRT_VRPC_ERR_CLI_ARG_INVALID = -1006,
+    MRT_VRPC_ERR_SVC_ARG_INVALID = -1005,
+    MRT_VRPC_ERR_MSG_DATA_INVALID = -1004,
+    MRT_VRPC_ERR_MSG_INIT_FAIL = -1003,
+    MRT_VRPC_ERR_DATA_SIZE_INVALID = -1002,
+    MRT_VRPC_ERR_FN_ID_INVALID = -1001,
     NO_USE = -99
 
 
 class mrt_port_type_t(enum_base):
     MRT_INPUT_PORT = 0,
     MRT_OUTPUT_PORT = 1,
     MRT_MEASUREMENT = 2,
```

### Comparing `vcarhilclient-1.0.501/vcarhilclient/kunyi_mrt.py` & `vcarhilclient-1.0.523/vcarhilclient/kunyi_mrt.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,20 @@
     dispatch_progress = 0
 
     def __init__(self, host, managerment_port=8888, push_port=8889, subscription_port=8890):
         self.host = host
         self.mgr_port = managerment_port
         self.push_port = push_port
         self.subs_port = subscription_port
-        self.envs = {}
+        self.envs = []
         self.record_env = ''
         self.context = None
         self.daqs = {}
+        self.log_writter = None
+        self.log_reader = None
         self.data_listTemp = []
         self.recodeStatus = 0
         self.writeNo = 1
         self.fileNum = 1
         self.temp_size = 1024*1024*10
         self.isrecord = False
         self.record_start = False
@@ -56,14 +58,18 @@
 
         mrt_lib.mrt_create_context.restype = c_void_p
         self.context = mrt_lib.mrt_create_context(POINTER(c_char)(),con_str_pointer, p_ec)
 
         return error_code
 
     def disconnect(self):
+        if self.log_writter != None:
+            self.close_log_writter()
+        if self.log_reader != None:
+            self.close_log_reader()
         if self.context == None:
             return 0
         mrt_lib.mrt_destroy_context.argtypes = [c_void_p]
         mrt_lib.mrt_destroy_context.restype = mrt_status_t
         error_code = mrt_lib.mrt_destroy_context(self.context)
         if error_code == 0:
             self.context = None
@@ -72,28 +78,28 @@
     def create_test_env(self, env_name):
         bs = env_name.encode('utf-8')
         name_pointer = c_char_p(bs)
         mrt_lib.mrt_create_enviroment.argtypes = [c_void_p, c_char_p]
         mrt_lib.mrt_create_enviroment.restype = mrt_status_t
         error_code = mrt_lib.mrt_create_enviroment(self.context, name_pointer)
         if error_code.value == 0:
-            self.envs[env_name] = None
+            self.envs.append(env_name)
         return error_code
 
     def delete_test_env(self, env_name):
         # if env_name not in self.envs:
         #    return mrt_status_t.MRT_ERR_OBJECT_NOT_EXIST
         bs = env_name.encode('utf-8')
         name_pointer = c_char_p(bs)
         mrt_lib.mrt_destroy_enviroment.argtypes = [c_void_p, c_char_p]
         mrt_lib.mrt_destroy_enviroment.restype = mrt_status_t
         error_code = mrt_lib.mrt_destroy_enviroment(self.context, name_pointer)
         if error_code.value == 0:
             try:
-                del self.envs[env_name]
+                self.envs.remove(env_name)
             except:
                 pass
         return error_code
 
     def load_test_resources_to_env(self, env_name, fileid):
         bs = env_name.encode('utf-8')
         name_pointer = c_char_p(bs)
@@ -203,28 +209,14 @@
         CALLBACK = CFUNCTYPE(None, mrt_status_t, c_int, c_int)
         mrt_lib.mrt_download_file.argtypes = [c_void_p, c_char_p, CALLBACK, POINTER(c_uint64)]
         mrt_lib.mrt_download_file.restype = mrt_status_t
         my_callback = CALLBACK(mrt_client.call_back)
         error_code = mrt_lib.mrt_download_file(self.context, path_pointer, my_callback, file_id_pointer)
         return error_code, file_id_pointer.contents.value
 
-    def get_env_file_id(self, env_name):
-        pass
-
-    def list_envs(self):
-        pass
-
-    def list_running_env(self):
-        pass
-
-    def get_test_env_detail(self):
-        pass
-
-    def dump_test_env(self):
-        pass
 
     def get_input_port_value(self, env_name, instance_name, port_name, signal_data_type, item_count, struct_detail=None, **sub_struct_detail):
         return self.get_port_value(env_name, instance_name, port_name,
                                    mrt_port_type_t.MRT_INPUT_PORT, signal_data_type, item_count, struct_detail, **sub_struct_detail)
 
     def get_output_port_value(self, env_name, instance_name, port_name, signal_data_type, item_count, struct_detail=None, **sub_struct_detail):
         return self.get_port_value(env_name, instance_name, port_name,
@@ -465,14 +457,43 @@
         mrt_lib.mrt_daq_set_port.restype = mrt_status_t
         error_code = mrt_lib.mrt_daq_set_port(self.context, en_pointer, c_uint64(daq_handle), c_uint32(port_index),
                                               mn_pointer, pn_pointer, port_type[0])
         if error_code.value == 0:
             self.daqs[(daq_handle,env_name)][port_index] = (model_instance_name, port_name, port_type[0], port_datatype)
         return error_code
 
+    def daq_set_multiple_ports(self, env_name, daq_handle, port_index, port_info_list, port_num):
+
+        bs = env_name.encode('utf-8')
+        en_pointer = c_char_p(bs)
+        tt = (mrt_daq_port_cfg_t*port_num)()
+        for i in range(port_num):
+            tt[i].port_type = port_info_list[i]['port_type'][0]
+            model_name = port_info_list[i]["model_instance_name"].encode('utf-8')
+            tt[i].model_instance_name = c_char_p(model_name)
+            port_name = port_info_list[i]["port_name"].encode('utf-8')
+            tt[i].port_name = c_char_p(port_name)
+
+
+        # model_name = port_info_list[0]["model_instance_name"].encode('utf-8')
+        # tt.model_instance_name = c_char_p(model_name)
+        # port_name = port_info_list[0]["port_name"].encode('utf-8')
+        # tt.port_name = c_char_p(port_name)
+
+        p_a = cast(pointer(tt), c_void_p)
+        p_b = cast(p_a, POINTER(mrt_daq_port_cfg_t))
+        mrt_lib.mrt_daq_set_multi_ports.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32,
+                                                   POINTER(mrt_daq_port_cfg_t), c_uint32]
+        mrt_lib.mrt_daq_set_multi_ports.restype = c_int32
+        c_p = cast(self.context, c_void_p)
+        error_code = mrt_lib.mrt_daq_set_multi_ports(c_p, en_pointer, c_uint64(daq_handle),
+                                                     c_uint32(port_index), p_b, port_num)
+
+        return error_code
+
     def daq_clear_port(self, env_name, daq_handle, port_index):
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         mrt_lib.mrt_daq_clear_port.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32]
         mrt_lib.mrt_daq_clear_port.restype = mrt_status_t
         error_code = mrt_lib.mrt_daq_clear_port(self.context, en_pointer, c_uint64(daq_handle), c_uint32(port_index))
         if error_code == 0:
@@ -520,28 +541,28 @@
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         mrt_lib.mrt_daq_clear_trigger_events.argtypes = [c_void_p, c_char_p, c_uint64]
         mrt_lib.mrt_daq_clear_trigger_events.restype = mrt_status_t
         error_code = mrt_lib.mrt_daq_clear_trigger_events(self.context, en_pointer, c_uint64(daq_handle))
         return error_code
 
-    def daq_get_trigger_event(self, env_name, daq_handle, port_index, model_instance_name, event_name):
+    def daq_get_trigger_event(self, env_name, daq_handle, event_index, model_instance_name, event_name):
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         modelName = model_instance_name.encode('utf-8')
         # mn_pointer = c_char(modelName)
         eventName = event_name.encode('utf-8')
         # eventn_pointer = c_char(eventName)
         evinfo = mrt_daq_trigger_event_info_t(modelName, eventName)
         evinfo_p = pointer(evinfo)
         mrt_lib.mrt_daq_get_trigger_event.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32,
                                                       POINTER(mrt_daq_trigger_event_info_t)]
         mrt_lib.mrt_daq_get_trigger_event.restype = mrt_status_t
         error_code = mrt_lib.mrt_daq_get_trigger_event(self.context, en_pointer, c_uint64(daq_handle),
-                                                       c_uint32(port_index), byref(evinfo))
+                                                       c_uint32(event_index), byref(evinfo))
         return error_code, evinfo_p
 
     def start_daq(self, env_name, daq_handle):
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         mrt_lib.mrt_start_daq.argtypes = [c_void_p, c_char_p, c_uint64]
         mrt_lib.mrt_start_daq.restype = mrt_status_t
@@ -565,25 +586,27 @@
         addr_pointer = c_char_p(addr_bs)
 
         mrt_lib.mrt_log_writer_open.argtypes = [c_char_p]
         mrt_lib.mrt_log_writer_open.restype = c_void_p
         self.log_writter = mrt_lib.mrt_log_writer_open(addr_pointer)
         return self.log_writter
 
-    def log_write(self,leave,own,log_text):
+    def log_write(self, level, own, log_text):
+        if self.log_writter == None:
+            self.open_log_writter()
         own2 = "pymrt:"+own
         bs = own2.encode('utf-8')
         fmtbs = log_text.encode('utf-8')
         logtext_pointer = c_char_p(bs)
         fmtbs_pointer = c_char_p(fmtbs)
-        c_void = self. open_log_writter()
+        c_void = self.open_log_writter()
         time.sleep(0.1)
         mrt_lib.mrt_log_write.argtypes = [c_void_p,c_int32,c_char_p,c_char_p]
         mrt_lib.mrt_log_write.restype = c_int32
-        self.log = mrt_lib.mrt_log_write(c_void,c_int32(leave),logtext_pointer,fmtbs_pointer)
+        self.log = mrt_lib.mrt_log_write(c_void,c_int32(level),logtext_pointer,fmtbs_pointer)
         time.sleep(0.1)
         self.close_log_writter()
         return self.log
 
 
     def close_log_reader(self):
 
@@ -612,14 +635,16 @@
         mrt_lib.mrt_log_writer_close.restype = mrt_status_t
         ec = mrt_lib.mrt_log_writer_close(self.log_writter)
         if ec.value == 0:
             self.log_writter = None
         return ec
 
     def fetch_log(self, buf_size):
+        if self.log_reader == None:
+            self.open_log_reader()
         arr = bytearray(buf_size)
         char_array = c_char * len(arr)
         buf_c = char_array.from_buffer(arr)
 
         mrt_lib.mrt_log_read.argtypes = [c_void_p, c_char_p, c_int32, c_int32]
         mrt_lib.mrt_log_read.restype = c_int32
         size = mrt_lib.mrt_log_read(self.log_reader, buf_c, buf_size, 5)
@@ -706,14 +731,15 @@
             raise ex
         finally:
             if is_release:
                 releaseInfo = self.daq_msg_release(msg_arr_obj[0])
                 if releaseInfo.value != 0:
                     raise Exception("rtcp error after read daq data")
 
+
     def daq_msg_release(self, msg):
 
         mrt_lib.mrt_daq_msg_release.argtypes = [c_void_p, POINTER(mrt_daq_msg_t)]
         mrt_lib.mrt_daq_msg_release.restype = mrt_status_t
         error_code = mrt_lib.mrt_daq_msg_release(self.context, msg)
         return error_code
 
@@ -992,9 +1018,22 @@
         if self.record_trigger(envN,instance_name, port_name, trigger_mode,signal_value,signal_value2):
             return True
 
     def record_trigger_stop(self,envN,instance_name, port_name, trigger_mode,signal_value,signal_value2=None):
         if self.record_trigger(envN,instance_name, port_name, trigger_mode, signal_value, signal_value2):
             return True
 
-
-
+    def mrt_version(self):
+        arr = bytearray(512)
+        char_array = c_char * len(arr)
+        buf_c = char_array.from_buffer(arr)
+        mrt_lib.mrt_version.argtypes = [c_void_p]
+        mrt_lib.mrt_version.restype = c_char_p
+        version = mrt_lib.mrt_version(buf_c)
+        return version.decode('utf-8')
+
+    def mrtd_version(self):
+
+        mrt_lib.mrtd_version.argtypes = [c_void_p]
+        mrt_lib.mrtd_version.restype = c_char_p
+        version = mrt_lib.mrtd_version(self.context)
+        return version.decode('utf-8')
```

### Comparing `vcarhilclient-1.0.501/vcarhilclient/kunyi_project.py` & `vcarhilclient-1.0.523/vcarhilclient/kunyi_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,20 +41,88 @@
 
             self.instances_orig = self.hil_json["Instances"]
             self.instances = {}
             for item in self.instances_orig:
                 self.instances[item["InstanceName"]] = item
             self.model_meta_files_orig = self.hil_json["ModelMetaFiles"]
             self.model_meta_files = {}
+            self.modelPath = {}
             for item in self.model_meta_files_orig:
                 self.model_meta_files[item["ModelMetaFile"]] = item
+                self.modelPath[item["ModelMetaFile"]] = os.path.join(os.path.dirname(ipr_path),item["File"]["Path"])
+            pass
 
         except Exception as ex:
             raise Exception("hil file content is not correct")
 
+    def get_Calibrations(self,instance,signal_type,cal_type,signal_name):
+        instance_is_found = False
+        signal_name_is_found =False
+        cal_type_is_found =False
+        st,stid = self.get_signalType(signal_type)
+        for k , v in self.modelPath.items():
+            if instance == k:
+                instance_is_found = True
+                with open(v) as f:
+                    try:
+                        instance_json = json.load(f)
+                    except Exception as ex:
+                        raise Exception(f"{v} is not a valid json file")
+                    for cal_t,cal_v in instance_json[st].items():
+                        if cal_t.lower() == cal_type.lower():
+                            cal_type_is_found = True
+                            for cal in cal_v:
+                                if signal_name == cal["Name"]:
+                                    signal_name_is_found = True
+                                    return signal_name , stid
+        if not instance_is_found:
+            raise Exception(f"not found {instance},Please check the json parameters'var_instance'")
+        if not cal_type_is_found:
+            raise Exception(f"not found {cal_type},Please check the json parameters'var_cal_type'")
+        if not signal_name_is_found:
+            raise Exception(f"not found {signal_name},Please check the json parameters'var_signal_name'")
+
+    def get_dataType_itemcount(self,instance,signal_type,signal_name):
+        instance_is_found = False
+        signal_name_is_found =False
+        st,stid = self.get_signalType(signal_type)
+        for k , v in self.modelPath.items():
+            if instance == k:
+                instance_is_found = True
+                with open(v) as f:
+                    try:
+                        instance_json = json.load(f)
+                    except Exception as ex:
+                        raise Exception(f"{v} is not a valid json file")
+                    for s in instance_json[st]:
+                        if s["Name"] == signal_name:
+                            signal_name_is_found = True
+                            return s["Type"] , s["ItemCount"],stid
+        if not instance_is_found:
+            raise Exception(f"not found {instance},Please check the json parameters'var_instance'")
+        if not signal_name_is_found:
+            raise Exception(f"not found {signal_name},Please check the json parameters'var_signal_name'")
+
+    def get_signalType(self,signal_type):
+        st = signal_type.lower()
+        if st == "inputport" or st == "inputports":
+            return "InputPorts",(0,)
+        if st == "outputport" or st == "outputports":
+            return "OutputPorts",(1,)
+        if st == "measurement" or st == "measurements" :
+            return "Measurements",(2,)
+        if st == "calibration" or st == "calibrations" :
+            return "Calibrations",(3,)
+
+        else:
+            raise Exception(f"signal type error! ,Please check the json parameters'var_type'")
+
+
+
+
     def get_packageName(self,packageName):
         package_path = os.path.join(self.project_root_dir, "Packages", packageName)
         packagefileList = os.listdir(package_path)
         # self.model_json_path = os.path.join(self.project_root_dir, "Packages", packageName, "*.json")
         return package_path,packagefileList
 
     def build_zip(self):
@@ -255,10 +323,8 @@
         if model_meta_file not in self.model_meta_files:
             raise Exception("Wrong model metafile name pass in")
         all_struct = self.get_model_detail(model_meta_file, "Structs")
         the_struct = None
         for struct in all_struct:
             if struct["Name"] == struct_name:
                 the_struct = struct
-        return the_struct
-
-
+        return the_struct
```

### Comparing `vcarhilclient-1.0.501/vcarhilclient/kunyi_util.py` & `vcarhilclient-1.0.523/vcarhilclient/kunyi_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
                      "UInt8": 1,
                      "UInt16": 2,
                      "UInt32": 4,
                      "UInt64": 8,
                      "Float": 4,
                      "Double": 8,
                      "Bool": 1,
-                     "ASCII": 2000,
-                     "UTF8": 2000}
+                     "ASCII": 1,
+                     "UTF8": 2}
 
         if signal_type == "Struct":
             if struct_detail == None:
                 raise Exception("No struct detail for counting the length")
             total_length = 0
             for member in struct_detail["Member"]:
                 if member["Type"] == "Struct":
@@ -185,16 +185,18 @@
                 if type(data_value) != list:
                     raise Exception("Data value is not enough for the array type")
                 for mi in range(item_count):
                     if datatype in decode_charactor:
                         bytes_result = bytes_result + struct.pack(decode_charactor[datatype], data_value[mi])
                     elif datatype == "ASCII":
                         bytes_result = bytes_result + data_value[mi].encode("ascii")
+                        break
                     elif datatype == "UTF8":
                         bytes_result = bytes_result + data_value[mi].encode("utf-8")
+                        break
                     else:
                         raise Exception("Unsupportted type for counting the bytes")
             else:
                 value = data_value
                 if isinstance(data_value, collections.abc.Sequence):
                     value = data_value[0]
                 if datatype in decode_charactor:
@@ -213,14 +215,20 @@
     @staticmethod
     def file_compress(root_path, out_zip_file):
         import shutil
         shutil.make_archive(out_zip_file, 'zip', root_path)
         return out_zip_file + ".zip"
 
     @staticmethod
+    def file_uncompress(filPath, targetPath):
+        import shutil
+        shutil.unpack_archive(filPath,targetPath)
+        return targetPath
+
+    @staticmethod
     def mrt_datatype_to_hil_datatype(mrt_datatype):
         all_dt = {
             "MRT_DATA_TYPE_UINT8": "UInt8",
             "MRT_DATA_TYPE_UINT16": "UInt16",
             "MRT_DATA_TYPE_UINT32": "UInt32",
             "MRT_DATA_TYPE_UINT64": "UInt64",
             "MRT_DATA_TYPE_INT8": "Int8",
```

### Comparing `vcarhilclient-1.0.501/vcarhilclient/minio_handld.py` & `vcarhilclient-1.0.523/vcarhilclient/minio_handld.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.501/vcarhilclient/mrt_strunctures.py` & `vcarhilclient-1.0.523/vcarhilclient/mrt_strunctures.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 
 class mrt_daq_info_t(Structure):
     _fields_ = [
         ("port_num", c_uint32), ("trigger_event_num", c_uint32),("period_ms", c_uint32),
         ("offset_ms", c_uint32),("msg_data_size", c_uint32)
     ]
 
+class mrt_daq_port_cfg_t(Structure):
+    _fields_ = [
+        ("port_type", c_uint32), ("model_instance_name", c_char_p), ("port_name", c_char_p)
+    ]
+
 class mrt_daq_trigger_event_info_t(Structure):
     _fields_ = [
         ("model_instance_name", c_char*mrt_name_size), ("event_name",c_char*mrt_name_size)
     ]
 
 class mrt_daq_port_info_t(Structure):
     _fields_ = [
```

### Comparing `vcarhilclient-1.0.501/vcarhilclient/signal_daq.py` & `vcarhilclient-1.0.523/vcarhilclient/signal_daq.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.501/vcarhilclient.egg-info/PKG-INFO` & `vcarhilclient-1.0.523/vcarhilclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.501
+Version: 1.0.523
 Summary: vcarhilclient
 Home-page: UNKNOWN
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

