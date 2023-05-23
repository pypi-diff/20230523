# Comparing `tmp/pyLSV2-1.1.2.tar.gz` & `tmp/pyLSV2-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLSV2-1.1.2.tar", last modified: Sat Apr 15 19:54:58 2023, max compression
+gzip compressed data, was "pyLSV2-1.2.tar", last modified: Tue May 23 17:44:43 2023, max compression
```

## Comparing `pyLSV2-1.1.2.tar` & `pyLSV2-1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.432547 pyLSV2-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-15 19:54:58.432547 pyLSV2-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.428547 pyLSV2-1.1.2/pyLSV2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78997 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    31344 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/dat_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/err.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.428547 pyLSV2-1.1.2/pyLSV2/locales/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.428547 pyLSV2-1.1.2/pyLSV2/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.428547 pyLSV2-1.1.2/pyLSV2/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-15 19:54:57.000000 pyLSV2-1.1.2/pyLSV2/locales/de/LC_MESSAGES/error_text.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-15 19:54:57.000000 pyLSV2-1.1.2/pyLSV2/locales/de/LC_MESSAGES/message_text.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.428547 pyLSV2-1.1.2/pyLSV2/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.432547 pyLSV2-1.1.2/pyLSV2/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-15 19:54:57.000000 pyLSV2-1.1.2/pyLSV2/locales/en/LC_MESSAGES/error_text.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-15 19:54:57.000000 pyLSV2-1.1.2/pyLSV2/locales/en/LC_MESSAGES/message_text.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/low_level_com.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/misc_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    22001 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/table_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/pyLSV2/translate_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.428547 pyLSV2-1.1.2/pyLSV2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-15 19:54:58.000000 pyLSV2-1.1.2/pyLSV2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-15 19:54:58.000000 pyLSV2-1.1.2/pyLSV2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:54:58.000000 pyLSV2-1.1.2/pyLSV2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 19:54:58.000000 pyLSV2-1.1.2/pyLSV2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:54:58.432547 pyLSV2-1.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/lsv2_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/lsv2cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/real_time_readings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/scope2csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/scope_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/signals_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/ssh_tunnel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/scripts/tab2csv.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:54:58.432547 pyLSV2-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-15 19:54:48.000000 pyLSV2-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.888125 pyLSV2-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 17:44:31.000000 pyLSV2-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 17:44:31.000000 pyLSV2-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-23 17:44:43.888125 pyLSV2-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-23 17:44:31.000000 pyLSV2-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.884125 pyLSV2-1.2/pyLSV2/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80008 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31344 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/dat_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/err.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.880125 pyLSV2-1.2/pyLSV2/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.880125 pyLSV2-1.2/pyLSV2/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.884125 pyLSV2-1.2/pyLSV2/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-23 17:44:42.000000 pyLSV2-1.2/pyLSV2/locales/de/LC_MESSAGES/error_text.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-23 17:44:42.000000 pyLSV2-1.2/pyLSV2/locales/de/LC_MESSAGES/message_text.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.880125 pyLSV2-1.2/pyLSV2/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.884125 pyLSV2-1.2/pyLSV2/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-23 17:44:42.000000 pyLSV2-1.2/pyLSV2/locales/en/LC_MESSAGES/error_text.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-23 17:44:42.000000 pyLSV2-1.2/pyLSV2/locales/en/LC_MESSAGES/message_text.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/low_level_com.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/misc_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/table_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-05-23 17:44:31.000000 pyLSV2-1.2/pyLSV2/translate_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.884125 pyLSV2-1.2/pyLSV2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-23 17:44:43.000000 pyLSV2-1.2/pyLSV2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-23 17:44:43.000000 pyLSV2-1.2/pyLSV2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:44:43.000000 pyLSV2-1.2/pyLSV2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 17:44:43.000000 pyLSV2-1.2/pyLSV2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:44:43.888125 pyLSV2-1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/lsv2_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/lsv2cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/real_time_readings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/scope2csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/scope_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/signals_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/ssh_tunnel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-23 17:44:31.000000 pyLSV2-1.2/scripts/tab2csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:44:43.888125 pyLSV2-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-23 17:44:31.000000 pyLSV2-1.2/setup.py
```

### Comparing `pyLSV2-1.1.2/LICENSE` & `pyLSV2-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/PKG-INFO` & `pyLSV2-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyLSV2
-Version: 1.1.2
+Version: 1.2
 Summary: A pure Python3 implementation of the LSV2 protocol
 Home-page: https://github.com/drunsinn/pyLSV2
 Author: drunsinn
 Author-email: dr.unsinn@googlemail.com
 License: MIT
 Keywords: LSV2 cnc communication transfer plc
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -133,40 +132,51 @@
  The following command reads 15 marker (bits) starting at address 32. This returns a list with 15 boolean values.
 
 ```
  con.read_plc_memory(32, pyLSV2.MemoryType.MARKER, 15)
 ```
  See [lsv2_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/lsv2_demo.py) for more examples.
 
- The available memory aread and their python data type
+ The available memory areas and their python data type
 | Memory Type              | Python Type |
 |--------------------------|-------------|
 | PLC_MEM_TYPE_MARKER      | bool        |
 | PLC_MEM_TYPE_INPUT       | bool        |
 | PLC_MEM_TYPE_OUTPUT      | bool        |
 | PLC_MEM_TYPE_COUNTER     | bool        |
 | PLC_MEM_TYPE_TIMER       | bool        |
 | PLC_MEM_TYPE_BYTE        | integer     |
 | PLC_MEM_TYPE_WORD        | integer     |
 | PLC_MEM_TYPE_DWORD       | integer     |
 | PLC_MEM_TYPE_STRING      | str         |
 | PLC_MEM_TYPE_INPUT_WORD  | integer     |
 | PLC_MEM_TYPE_OUTPUT_WORD | integer     |
 
+ Reading the values from the memory address takes the size of each memory type into account.
+
 #### Reading via Data Path
  The following command reads values from the control not via a memory address but via supplying a data access path. This will only work on iTNC controls!
  The advantage is that it also allows you to access tables like the tool table without reading the complete file.
 
 ```
  con.read_data_path('/PLC/memory/K/1')
  con.read_data_path('/TABLE/TOOL/T/1/DOC')
 ```
- 
+
  See [lsv2_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/lsv2_demo.py) for more examples.
 
+ Note that reading values from memory does not take into account the actual size in the control memory. This leads to an offset between the values read with `read_data_path` and `read_plc_memory`. As a workaround you have to multiply the address value with the number of bytes the data type requires. The following example tries to show how this can be accomplished:
+
+```
+ for mem_address in [0, 1, 2, 4, 8, 12, 68, 69, 151, 300, 368]:
+    v1 = lsv2.read_plc_memory(mem_address, pyLSV2.MemoryType.DWORD, 1)[0]
+    v2 = lsv2.read_data_path("/PLC/memory/D/%d" % (mem_address * 4))
+    assert v1 == v2
+```
+
 ### SSH Tunnel
  Newer controls allow the use of ssh to encrypt the communication via LSV2. 
  See [ssh_tunnel_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/ssh_tunnel_demo.py) for an example on
  how to use the python library [sshtunnel](https://github.com/pahaz/sshtunnel) to achieve a secure connection.
 
 ## Compatibility
  Since there are a lot of different software versions and machine configurations out there
```

### Comparing `pyLSV2-1.1.2/README.md` & `pyLSV2-1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -104,40 +104,51 @@
  The following command reads 15 marker (bits) starting at address 32. This returns a list with 15 boolean values.
 
 ```
  con.read_plc_memory(32, pyLSV2.MemoryType.MARKER, 15)
 ```
  See [lsv2_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/lsv2_demo.py) for more examples.
 
- The available memory aread and their python data type
+ The available memory areas and their python data type
 | Memory Type              | Python Type |
 |--------------------------|-------------|
 | PLC_MEM_TYPE_MARKER      | bool        |
 | PLC_MEM_TYPE_INPUT       | bool        |
 | PLC_MEM_TYPE_OUTPUT      | bool        |
 | PLC_MEM_TYPE_COUNTER     | bool        |
 | PLC_MEM_TYPE_TIMER       | bool        |
 | PLC_MEM_TYPE_BYTE        | integer     |
 | PLC_MEM_TYPE_WORD        | integer     |
 | PLC_MEM_TYPE_DWORD       | integer     |
 | PLC_MEM_TYPE_STRING      | str         |
 | PLC_MEM_TYPE_INPUT_WORD  | integer     |
 | PLC_MEM_TYPE_OUTPUT_WORD | integer     |
 
+ Reading the values from the memory address takes the size of each memory type into account.
+
 #### Reading via Data Path
  The following command reads values from the control not via a memory address but via supplying a data access path. This will only work on iTNC controls!
  The advantage is that it also allows you to access tables like the tool table without reading the complete file.
 
 ```
  con.read_data_path('/PLC/memory/K/1')
  con.read_data_path('/TABLE/TOOL/T/1/DOC')
 ```
- 
+
  See [lsv2_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/lsv2_demo.py) for more examples.
 
+ Note that reading values from memory does not take into account the actual size in the control memory. This leads to an offset between the values read with `read_data_path` and `read_plc_memory`. As a workaround you have to multiply the address value with the number of bytes the data type requires. The following example tries to show how this can be accomplished:
+
+```
+ for mem_address in [0, 1, 2, 4, 8, 12, 68, 69, 151, 300, 368]:
+    v1 = lsv2.read_plc_memory(mem_address, pyLSV2.MemoryType.DWORD, 1)[0]
+    v2 = lsv2.read_data_path("/PLC/memory/D/%d" % (mem_address * 4))
+    assert v1 == v2
+```
+
 ### SSH Tunnel
  Newer controls allow the use of ssh to encrypt the communication via LSV2. 
  See [ssh_tunnel_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/ssh_tunnel_demo.py) for an example on
  how to use the python library [sshtunnel](https://github.com/pahaz/sshtunnel) to achieve a secure connection.
 
 ## Compatibility
  Since there are a lot of different software versions and machine configurations out there
```

### Comparing `pyLSV2-1.1.2/pyLSV2/client.py` & `pyLSV2-1.2/pyLSV2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -750,4189 +750,4252 @@
 00002ed0: 2020 2020 2020 2520 7365 6c65 6374 6564        % selected
 00002ee0: 5f73 697a 650a 2020 2020 2020 2020 2020  _size.          
 00002ef0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
 00002f00: 2069 6620 6e6f 7420 7365 6c66 2e5f 7365   if not self._se
 00002f10: 6e64 5f72 6563 6976 6528 0a20 2020 2020  nd_recive(.     
 00002f20: 2020 2020 2020 206c 632e 434d 442e 435f         lc.CMD.C_
 00002f30: 4343 2c20 7374 7275 6374 2e70 6163 6b28  CC, struct.pack(
-00002f40: 2221 4822 2c20 6c63 2e50 6172 4343 432e  "!H", lc.ParCCC.
-00002f50: 5345 4355 5245 5f46 494c 455f 5345 4e44  SECURE_FILE_SEND
-00002f60: 292c 206c 632e 5253 502e 545f 4f4b 0a20  ), lc.RSP.T_OK. 
-00002f70: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00002f80: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-00002f90: 6572 2e64 6562 7567 2822 7365 6375 7265  er.debug("secure
-00002fa0: 2066 696c 6520 7472 616e 7366 6572 206e   file transfer n
-00002fb0: 6f74 2073 7570 706f 7274 6564 3f20 7573  ot supported? us
-00002fc0: 6520 6661 6c6c 6261 636b 2229 0a20 2020  e fallback").   
-00002fd0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
-00002fe0: 6563 7572 655f 6669 6c65 5f73 656e 6420  ecure_file_send 
-00002ff0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00003000: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003010: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e64    self._logger.d
-00003020: 6562 7567 2822 7365 6375 7265 2066 696c  ebug("secure fil
-00003030: 6520 7365 6e64 2069 7320 656e 6162 6c65  e send is enable
-00003040: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
-00003050: 7365 6c66 2e5f 7365 6375 7265 5f66 696c  self._secure_fil
-00003060: 655f 7365 6e64 203d 2054 7275 650a 0a20  e_send = True.. 
-00003070: 2020 2020 2020 2073 656c 662e 6c6f 6769         self.logi
-00003080: 6e28 6c6f 6769 6e3d 6c63 2e4c 6f67 696e  n(login=lc.Login
-00003090: 2e46 494c 4554 5241 4e53 4645 5229 0a0a  .FILETRANSFER)..
-000030a0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-000030b0: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-000030c0: 2020 2020 2020 2022 7375 6363 6573 7366         "successf
-000030d0: 756c 6c79 2063 6f6e 6669 6775 7265 6420  ully configured 
-000030e0: 636f 6e6e 6563 7469 6f6e 2070 6172 616d  connection param
-000030f0: 6574 6572 7320 616e 6420 6261 7369 6320  eters and basic 
-00003100: 6c6f 6769 6e73 220a 2020 2020 2020 2020  logins".        
-00003110: 290a 0a20 2020 2064 6566 206c 6f67 696e  )..    def login
-00003120: 2873 656c 662c 206c 6f67 696e 3a20 6c63  (self, login: lc
-00003130: 2e4c 6f67 696e 2c20 7061 7373 776f 7264  .Login, password
-00003140: 3a20 7374 7220 3d20 2222 2920 2d3e 2062  : str = "") -> b
-00003150: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00003160: 0a20 2020 2020 2020 2052 6571 7565 7374  .        Request
-00003170: 2061 6464 6974 696f 6e61 6c20 6163 6365   additional acce
-00003180: 7373 2072 6967 6874 732e 2054 6f20 656c  ss rights. To el
-00003190: 6576 6174 6520 7468 6973 206c 6576 656c  evate this level
-000031a0: 2061 206c 6f67 6f6e 2068 6173 2074 6f20   a logon has to 
-000031b0: 6265 2070 6572 666f 726d 6564 2e0a 2020  be performed..  
-000031c0: 2020 2020 2020 536f 6d65 206c 6576 656c        Some level
-000031d0: 7320 7265 7175 6972 6520 6120 7061 7373  s require a pass
-000031e0: 776f 7264 2e0a 2020 2020 2020 2020 5265  word..        Re
-000031f0: 7475 726e 7320 6060 5472 7565 6060 2069  turns ``True`` i
-00003200: 6620 6578 6563 7574 696f 6e20 7761 7320  f execution was 
-00003210: 7375 6363 6573 7366 756c 2e0a 0a20 2020  successful...   
-00003220: 2020 2020 203a 7061 7261 6d20 6c6f 6769       :param logi
-00003230: 6e3a 204f 6e65 206f 6620 7468 6520 6b6e  n: One of the kn
-00003240: 6f77 6e20 6c6f 6769 6e20 7374 7269 6e67  own login string
-00003250: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-00003260: 2070 6173 7377 6f72 643a 206f 7074 696f   password: optio
-00003270: 6e61 6c2e 2050 6173 7377 6f72 6420 666f  nal. Password fo
-00003280: 7220 6c6f 6769 6e0a 2020 2020 2020 2020  r login.        
-00003290: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
-000032a0: 6c6f 6769 6e20 696e 2073 656c 662e 5f61  login in self._a
-000032b0: 6374 6976 655f 6c6f 6769 6e73 3a0a 2020  ctive_logins:.  
-000032c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000032d0: 6c6f 6767 6572 2e64 6562 7567 2822 6c6f  logger.debug("lo
-000032e0: 6769 6e20 616c 7265 6164 7920 6163 7469  gin already acti
-000032f0: 7665 2229 0a20 2020 2020 2020 2020 2020  ve").           
-00003300: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-00003310: 2020 2020 2020 6966 206c 6f67 696e 206e        if login n
-00003320: 6f74 2069 6e20 7365 6c66 2e5f 6b6e 6f77  ot in self._know
-00003330: 6e5f 6c6f 6769 6e73 3a0a 2020 2020 2020  n_logins:.      
-00003340: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-00003350: 6572 2e77 6172 6e69 6e67 2822 756e 6b6e  er.warning("unkn
-00003360: 6f77 6e20 6f72 2075 6e73 7570 706f 7274  own or unsupport
-00003370: 6564 206c 6f67 696e 2229 0a20 2020 2020  ed login").     
-00003380: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00003390: 6c73 650a 0a20 2020 2020 2020 2070 6179  lse..        pay
-000033a0: 6c6f 6164 203d 206c 6d2e 7573 7472 5f74  load = lm.ustr_t
-000033b0: 6f5f 6261 286c 6f67 696e 2e76 616c 7565  o_ba(login.value
-000033c0: 290a 0a20 2020 2020 2020 2069 6620 7061  )..        if pa
-000033d0: 7373 776f 7264 2069 7320 6e6f 7420 4e6f  ssword is not No
-000033e0: 6e65 2061 6e64 206c 656e 2870 6173 7377  ne and len(passw
-000033f0: 6f72 6429 203e 2030 3a0a 2020 2020 2020  ord) > 0:.      
-00003400: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
-00003410: 7465 6e64 286c 6d2e 7573 7472 5f74 6f5f  tend(lm.ustr_to_
-00003420: 6261 2870 6173 7377 6f72 6429 290a 0a20  ba(password)).. 
-00003430: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-00003440: 7365 6e64 5f72 6563 6976 6528 6c63 2e43  send_recive(lc.C
-00003450: 4d44 2e41 5f4c 472c 2070 6179 6c6f 6164  MD.A_LG, payload
-00003460: 2c20 6c63 2e52 5350 2e54 5f4f 4b29 3a0a  , lc.RSP.T_OK):.
-00003470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003480: 2e5f 6c6f 6767 6572 2e64 6562 7567 2822  ._logger.debug("
-00003490: 6c6f 6769 6e20 6578 6563 7574 6564 2073  login executed s
-000034a0: 7563 6365 7373 6675 6c6c 7920 666f 7220  uccessfully for 
-000034b0: 6c6f 6769 6e20 2573 222c 206c 6f67 696e  login %s", login
-000034c0: 2e76 616c 7565 290a 2020 2020 2020 2020  .value).        
-000034d0: 2020 2020 7365 6c66 2e5f 6163 7469 7665      self._active
-000034e0: 5f6c 6f67 696e 732e 6170 7065 6e64 286c  _logins.append(l
-000034f0: 6f67 696e 290a 2020 2020 2020 2020 2020  ogin).          
-00003500: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-00003510: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-00003520: 6765 722e 7761 726e 696e 6728 2265 7272  ger.warning("err
-00003530: 6f72 206c 6f67 6769 6e67 2069 6e20 6173  or logging in as
-00003540: 2025 7322 2c20 6c6f 6769 6e2e 7661 6c75   %s", login.valu
-00003550: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-00003560: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00003570: 206c 6f67 6f75 7428 7365 6c66 2c20 6c6f   logout(self, lo
-00003580: 6769 6e3a 2055 6e69 6f6e 5b6c 632e 4c6f  gin: Union[lc.Lo
-00003590: 6769 6e2c 204e 6f6e 655d 203d 204e 6f6e  gin, None] = Non
-000035a0: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
-000035b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000035c0: 4472 6f70 206f 6e65 206f 7220 616c 6c20  Drop one or all 
-000035d0: 6163 6365 7373 2072 6967 6874 2e20 4966  access right. If
-000035e0: 206e 6f20 6c6f 6769 6e20 6973 2073 7570   no login is sup
-000035f0: 706c 6965 6420 616c 6c20 6163 7469 7665  plied all active
-00003600: 2061 6363 6573 7320 7269 6768 7473 2061   access rights a
-00003610: 7265 2064 726f 7070 6564 2e0a 2020 2020  re dropped..    
-00003620: 2020 2020 5265 7475 726e 7320 6060 5472      Returns ``Tr
-00003630: 7565 6060 2069 6620 6578 6563 7574 696f  ue`` if executio
-00003640: 6e20 7761 7320 7375 6363 6573 7366 756c  n was successful
-00003650: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00003660: 6d20 6c6f 6769 6e3a 206f 7074 696f 6e61  m login: optiona
-00003670: 6c2e 204f 6e65 206f 6620 7468 6520 6b6e  l. One of the kn
-00003680: 6f77 6e20 6c6f 6769 6e20 7374 7269 6e67  own login string
-00003690: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
-000036a0: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-000036b0: 6279 7465 6172 7261 7928 290a 0a20 2020  bytearray()..   
-000036c0: 2020 2020 2069 6620 6c6f 6769 6e20 6973       if login is
-000036d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000036e0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000036f0: 616e 6365 286c 6f67 696e 2c20 286c 632e  ance(login, (lc.
-00003700: 4c6f 6769 6e2c 2929 3a0a 2020 2020 2020  Login,)):.      
-00003710: 2020 2020 2020 2020 2020 6966 206c 6f67            if log
-00003720: 696e 2069 6e20 7365 6c66 2e5f 6163 7469  in in self._acti
-00003730: 7665 5f6c 6f67 696e 733a 0a20 2020 2020  ve_logins:.     
-00003740: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00003750: 6179 6c6f 6164 2e65 7874 656e 6428 6c6d  ayload.extend(lm
-00003760: 2e75 7374 725f 746f 5f62 6128 6c6f 6769  .ustr_to_ba(logi
-00003770: 6e2e 7661 6c75 6529 290a 2020 2020 2020  n.value)).      
-00003780: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037a0: 2020 2020 2320 6c6f 6769 6e20 6973 206e      # login is n
-000037b0: 6f74 2061 6374 6976 650a 2020 2020 2020  ot active.      
-000037c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000037d0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-000037e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000037f0: 2020 2020 2020 2020 2020 2020 2320 756e              # un
-00003800: 6b6e 6f77 6e20 6c6f 6769 6e0a 2020 2020  known login.    
-00003810: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003820: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-00003830: 2020 6966 2073 656c 662e 5f73 656e 645f    if self._send_
-00003840: 7265 6369 7665 286c 632e 434d 442e 415f  recive(lc.CMD.A_
-00003850: 4c4f 2c20 7061 796c 6f61 642c 206c 632e  LO, payload, lc.
-00003860: 5253 502e 545f 4f4b 293a 0a20 2020 2020  RSP.T_OK):.     
-00003870: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-00003880: 6765 722e 696e 666f 2822 6c6f 676f 7574  ger.info("logout
-00003890: 2065 7865 6375 7465 6420 7375 6363 6573   executed succes
-000038a0: 7366 756c 6c79 2066 6f72 206c 6f67 696e  sfully for login
-000038b0: 2025 7322 2c20 6c6f 6769 6e29 0a20 2020   %s", login).   
-000038c0: 2020 2020 2020 2020 2069 6620 6c6f 6769           if logi
-000038d0: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-000038e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000038f0: 5f61 6374 6976 655f 6c6f 6769 6e73 203d  _active_logins =
-00003900: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-00003910: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003920: 2020 2020 2020 7365 6c66 2e5f 6163 7469        self._acti
-00003930: 7665 5f6c 6f67 696e 732e 7265 6d6f 7665  ve_logins.remove
-00003940: 286c 6f67 696e 290a 2020 2020 2020 2020  (login).        
-00003950: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00003960: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00003970: 616c 7365 0a0a 2020 2020 6465 6620 5f72  alse..    def _r
-00003980: 6561 645f 7061 7261 6d65 7465 7273 2873  ead_parameters(s
-00003990: 656c 662c 2066 6f72 6365 3a20 626f 6f6c  elf, force: bool
-000039a0: 203d 2046 616c 7365 2920 2d3e 206c 642e   = False) -> ld.
-000039b0: 5379 7374 656d 5061 7261 6d65 7465 7273  SystemParameters
-000039c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000039d0: 2020 2020 2020 5265 6164 2061 6c6c 2061        Read all a
-000039e0: 7661 696c 6162 6c65 2073 7973 7465 6d20  vailable system 
-000039f0: 7061 7261 6d65 7465 7220 656e 7472 6965  parameter entrie
-00003a00: 732e 2054 6865 2072 6573 756c 7473 2061  s. The results a
-00003a10: 7265 2062 7566 6665 7265 6420 7369 6e63  re buffered sinc
-00003a20: 6520 6974 2069 7320 616c 736f 2075 7365  e it is also use
-00003a30: 6420 696e 7465 726e 616c 6c79 2e0a 2020  d internally..  
-00003a40: 2020 2020 2020 5468 6973 206d 6561 6e73        This means
-00003a50: 2061 6464 6974 696f 6e61 6c20 6361 6c6c   additional call
-00003a60: 7320 646f 6e74 2063 6175 7365 2063 6f6d  s dont cause com
-00003a70: 6d75 6e69 6361 7469 6f6e 2077 6974 6820  munication with 
-00003a80: 7468 6520 636f 6e74 726f 6c2e 0a0a 2020  the control...  
-00003a90: 2020 2020 2020 3a70 6172 616d 2066 6f72        :param for
-00003aa0: 6365 3a20 6966 2060 6054 7275 6560 6020  ce: if ``True`` 
-00003ab0: 7468 6520 696e 666f 726d 6174 696f 6e20  the information 
-00003ac0: 6973 2072 652d 7265 6164 2065 7665 6e20  is re-read even 
-00003ad0: 6966 2069 7420 6973 2061 6c72 6561 6479  if it is already
-00003ae0: 2062 7566 6665 7265 640a 2020 2020 2020   buffered.      
-00003af0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00003b00: 2073 656c 662e 5f73 7973 5f70 6172 2e6c   self._sys_par.l
-00003b10: 7376 325f 7665 7273 696f 6e20 213d 202d  sv2_version != -
-00003b20: 3120 616e 6420 666f 7263 6520 6973 2046  1 and force is F
-00003b30: 616c 7365 3a0a 2020 2020 2020 2020 2020  alse:.          
-00003b40: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e64    self._logger.d
-00003b50: 6562 7567 280a 2020 2020 2020 2020 2020  ebug(.          
-00003b60: 2020 2020 2020 2273 7973 7465 6d20 7061        "system pa
-00003b70: 7261 6d65 7465 7273 2061 6c72 6561 6479  rameters already
-00003b80: 2069 6e20 6d65 6d6f 7279 2c20 7265 7475   in memory, retu
-00003b90: 726e 2070 7265 7669 6f75 7320 7661 6c75  rn previous valu
-00003ba0: 6573 220a 2020 2020 2020 2020 2020 2020  es".            
-00003bb0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00003bc0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00003bd0: 6c74 203d 2073 656c 662e 5f73 656e 645f  lt = self._send_
-00003be0: 7265 6369 7665 286c 632e 434d 442e 525f  recive(lc.CMD.R_
-00003bf0: 5052 2c20 4e6f 6e65 2c20 6c63 2e52 5350  PR, None, lc.RSP
-00003c00: 2e53 5f50 5229 0a20 2020 2020 2020 2020  .S_PR).         
-00003c10: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00003c20: 2872 6573 756c 742c 2028 6279 7465 6172  (result, (bytear
-00003c30: 7261 792c 2929 3a0a 2020 2020 2020 2020  ray,)):.        
-00003c40: 2020 2020 2020 2020 7365 6c66 2e5f 7379          self._sy
-00003c50: 735f 7061 7220 3d20 6c6d 2e64 6563 6f64  s_par = lm.decod
-00003c60: 655f 7379 7374 656d 5f70 6172 616d 6574  e_system_paramet
-00003c70: 6572 7328 7265 7375 6c74 290a 2020 2020  ers(result).    
+00002f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f50: 2022 2148 222c 206c 632e 5061 7243 4343   "!H", lc.ParCCC
+00002f60: 2e53 4543 5552 455f 4649 4c45 5f53 454e  .SECURE_FILE_SEN
+00002f70: 4429 2c20 6c63 2e52 5350 2e54 5f4f 4b0a  D), lc.RSP.T_OK.
+00002f80: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00002f90: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+00002fa0: 6765 722e 6465 6275 6728 0a20 2020 2020  ger.debug(.     
+00002fb0: 2020 2020 2020 2020 2020 2022 7365 6375             "secu
+00002fc0: 7265 2066 696c 6520 7472 616e 7366 6572  re file transfer
+00002fd0: 206e 6f74 2073 7570 706f 7274 6564 3f20   not supported? 
+00002fe0: 7573 6520 6661 6c6c 6261 636b 2229 0a20  use fallback"). 
+00002ff0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003000: 5f73 6563 7572 655f 6669 6c65 5f73 656e  _secure_file_sen
+00003010: 6420 3d20 4661 6c73 650a 2020 2020 2020  d = False.      
+00003020: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003030: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+00003040: 2e64 6562 7567 2822 7365 6375 7265 2066  .debug("secure f
+00003050: 696c 6520 7365 6e64 2069 7320 656e 6162  ile send is enab
+00003060: 6c65 6422 290a 2020 2020 2020 2020 2020  led").          
+00003070: 2020 7365 6c66 2e5f 7365 6375 7265 5f66    self._secure_f
+00003080: 696c 655f 7365 6e64 203d 2054 7275 650a  ile_send = True.
+00003090: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+000030a0: 6769 6e28 6c6f 6769 6e3d 6c63 2e4c 6f67  gin(login=lc.Log
+000030b0: 696e 2e46 494c 4554 5241 4e53 4645 5229  in.FILETRANSFER)
+000030c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000030d0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+000030e0: 2020 2020 2020 2020 2022 7375 6363 6573           "succes
+000030f0: 7366 756c 6c79 2063 6f6e 6669 6775 7265  sfully configure
+00003100: 6420 636f 6e6e 6563 7469 6f6e 2070 6172  d connection par
+00003110: 616d 6574 6572 7320 616e 6420 6261 7369  ameters and basi
+00003120: 6320 6c6f 6769 6e73 220a 2020 2020 2020  c logins".      
+00003130: 2020 290a 0a20 2020 2064 6566 206c 6f67    )..    def log
+00003140: 696e 2873 656c 662c 206c 6f67 696e 3a20  in(self, login: 
+00003150: 6c63 2e4c 6f67 696e 2c20 7061 7373 776f  lc.Login, passwo
+00003160: 7264 3a20 7374 7220 3d20 2222 2920 2d3e  rd: str = "") ->
+00003170: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00003180: 2222 0a20 2020 2020 2020 2052 6571 7565  "".        Reque
+00003190: 7374 2061 6464 6974 696f 6e61 6c20 6163  st additional ac
+000031a0: 6365 7373 2072 6967 6874 732e 2054 6f20  cess rights. To 
+000031b0: 656c 6576 6174 6520 7468 6973 206c 6576  elevate this lev
+000031c0: 656c 2061 206c 6f67 6f6e 2068 6173 2074  el a logon has t
+000031d0: 6f20 6265 2070 6572 666f 726d 6564 2e0a  o be performed..
+000031e0: 2020 2020 2020 2020 536f 6d65 206c 6576          Some lev
+000031f0: 656c 7320 7265 7175 6972 6520 6120 7061  els require a pa
+00003200: 7373 776f 7264 2e0a 2020 2020 2020 2020  ssword..        
+00003210: 5265 7475 726e 7320 6060 5472 7565 6060  Returns ``True``
+00003220: 2069 6620 6578 6563 7574 696f 6e20 7761   if execution wa
+00003230: 7320 7375 6363 6573 7366 756c 2e0a 0a20  s successful... 
+00003240: 2020 2020 2020 203a 7061 7261 6d20 6c6f         :param lo
+00003250: 6769 6e3a 204f 6e65 206f 6620 7468 6520  gin: One of the 
+00003260: 6b6e 6f77 6e20 6c6f 6769 6e20 7374 7269  known login stri
+00003270: 6e67 730a 2020 2020 2020 2020 3a70 6172  ngs.        :par
+00003280: 616d 2070 6173 7377 6f72 643a 206f 7074  am password: opt
+00003290: 696f 6e61 6c2e 2050 6173 7377 6f72 6420  ional. Password 
+000032a0: 666f 7220 6c6f 6769 6e0a 2020 2020 2020  for login.      
+000032b0: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
+000032c0: 6620 6c6f 6769 6e20 696e 2073 656c 662e  f login in self.
+000032d0: 5f61 6374 6976 655f 6c6f 6769 6e73 3a0a  _active_logins:.
+000032e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000032f0: 2e5f 6c6f 6767 6572 2e64 6562 7567 2822  ._logger.debug("
+00003300: 6c6f 6769 6e20 616c 7265 6164 7920 6163  login already ac
+00003310: 7469 7665 2229 0a20 2020 2020 2020 2020  tive").         
+00003320: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+00003330: 2020 2020 2020 2020 6966 206c 6f67 696e          if login
+00003340: 206e 6f74 2069 6e20 7365 6c66 2e5f 6b6e   not in self._kn
+00003350: 6f77 6e5f 6c6f 6769 6e73 3a0a 2020 2020  own_logins:.    
+00003360: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+00003370: 6767 6572 2e77 6172 6e69 6e67 2822 756e  gger.warning("un
+00003380: 6b6e 6f77 6e20 6f72 2075 6e73 7570 706f  known or unsuppo
+00003390: 7274 6564 206c 6f67 696e 2229 0a20 2020  rted login").   
+000033a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000033b0: 4661 6c73 650a 0a20 2020 2020 2020 2070  False..        p
+000033c0: 6179 6c6f 6164 203d 206c 6d2e 7573 7472  ayload = lm.ustr
+000033d0: 5f74 6f5f 6261 286c 6f67 696e 2e76 616c  _to_ba(login.val
+000033e0: 7565 290a 0a20 2020 2020 2020 2069 6620  ue)..        if 
+000033f0: 7061 7373 776f 7264 2069 7320 6e6f 7420  password is not 
+00003400: 4e6f 6e65 2061 6e64 206c 656e 2870 6173  None and len(pas
+00003410: 7377 6f72 6429 203e 2030 3a0a 2020 2020  sword) > 0:.    
+00003420: 2020 2020 2020 2020 7061 796c 6f61 642e          payload.
+00003430: 6578 7465 6e64 286c 6d2e 7573 7472 5f74  extend(lm.ustr_t
+00003440: 6f5f 6261 2870 6173 7377 6f72 6429 290a  o_ba(password)).
+00003450: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00003460: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
+00003470: 2e43 4d44 2e41 5f4c 472c 2070 6179 6c6f  .CMD.A_LG, paylo
+00003480: 6164 2c20 6c63 2e52 5350 2e54 5f4f 4b29  ad, lc.RSP.T_OK)
+00003490: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000034a0: 6c66 2e5f 6c6f 6767 6572 2e64 6562 7567  lf._logger.debug
+000034b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000034c0: 2020 226c 6f67 696e 2065 7865 6375 7465    "login execute
+000034d0: 6420 7375 6363 6573 7366 756c 6c79 2066  d successfully f
+000034e0: 6f72 206c 6f67 696e 2025 7322 2c20 6c6f  or login %s", lo
+000034f0: 6769 6e2e 7661 6c75 6529 0a20 2020 2020  gin.value).     
+00003500: 2020 2020 2020 2073 656c 662e 5f61 6374         self._act
+00003510: 6976 655f 6c6f 6769 6e73 2e61 7070 656e  ive_logins.appen
+00003520: 6428 6c6f 6769 6e29 0a20 2020 2020 2020  d(login).       
+00003530: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00003540: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00003550: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+00003560: 6572 726f 7220 6c6f 6767 696e 6720 696e  error logging in
+00003570: 2061 7320 2573 222c 206c 6f67 696e 2e76   as %s", login.v
+00003580: 616c 7565 290a 2020 2020 2020 2020 7265  alue).        re
+00003590: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+000035a0: 6465 6620 6c6f 676f 7574 2873 656c 662c  def logout(self,
+000035b0: 206c 6f67 696e 3a20 556e 696f 6e5b 6c63   login: Union[lc
+000035c0: 2e4c 6f67 696e 2c20 4e6f 6e65 5d20 3d20  .Login, None] = 
+000035d0: 4e6f 6e65 2920 2d3e 2062 6f6f 6c3a 0a20  None) -> bool:. 
+000035e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000035f0: 2020 2044 726f 7020 6f6e 6520 6f72 2061     Drop one or a
+00003600: 6c6c 2061 6363 6573 7320 7269 6768 742e  ll access right.
+00003610: 2049 6620 6e6f 206c 6f67 696e 2069 7320   If no login is 
+00003620: 7375 7070 6c69 6564 2061 6c6c 2061 6374  supplied all act
+00003630: 6976 6520 6163 6365 7373 2072 6967 6874  ive access right
+00003640: 7320 6172 6520 6472 6f70 7065 642e 0a20  s are dropped.. 
+00003650: 2020 2020 2020 2052 6574 7572 6e73 2060         Returns `
+00003660: 6054 7275 6560 6020 6966 2065 7865 6375  `True`` if execu
+00003670: 7469 6f6e 2077 6173 2073 7563 6365 7373  tion was success
+00003680: 6675 6c2e 0a0a 2020 2020 2020 2020 3a70  ful...        :p
+00003690: 6172 616d 206c 6f67 696e 3a20 6f70 7469  aram login: opti
+000036a0: 6f6e 616c 2e20 4f6e 6520 6f66 2074 6865  onal. One of the
+000036b0: 206b 6e6f 776e 206c 6f67 696e 2073 7472   known login str
+000036c0: 696e 6773 0a20 2020 2020 2020 2022 2222  ings.        """
+000036d0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+000036e0: 203d 2062 7974 6561 7272 6179 2829 0a0a   = bytearray()..
+000036f0: 2020 2020 2020 2020 6966 206c 6f67 696e          if login
+00003700: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00003710: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00003720: 6e73 7461 6e63 6528 6c6f 6769 6e2c 2028  nstance(login, (
+00003730: 6c63 2e4c 6f67 696e 2c29 293a 0a20 2020  lc.Login,)):.   
+00003740: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003750: 6c6f 6769 6e20 696e 2073 656c 662e 5f61  login in self._a
+00003760: 6374 6976 655f 6c6f 6769 6e73 3a0a 2020  ctive_logins:.  
+00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003780: 2020 7061 796c 6f61 642e 6578 7465 6e64    payload.extend
+00003790: 286c 6d2e 7573 7472 5f74 6f5f 6261 286c  (lm.ustr_to_ba(l
+000037a0: 6f67 696e 2e76 616c 7565 2929 0a20 2020  ogin.value)).   
+000037b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000037c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000037d0: 2020 2020 2020 2023 206c 6f67 696e 2069         # login i
+000037e0: 7320 6e6f 7420 6163 7469 7665 0a20 2020  s not active.   
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003800: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00003810: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00003820: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00003830: 2075 6e6b 6e6f 776e 206c 6f67 696e 0a20   unknown login. 
+00003840: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00003850: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00003860: 2020 2020 2069 6620 7365 6c66 2e5f 7365       if self._se
+00003870: 6e64 5f72 6563 6976 6528 6c63 2e43 4d44  nd_recive(lc.CMD
+00003880: 2e41 5f4c 4f2c 2070 6179 6c6f 6164 2c20  .A_LO, payload, 
+00003890: 6c63 2e52 5350 2e54 5f4f 4b29 3a0a 2020  lc.RSP.T_OK):.  
+000038a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000038b0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+000038c0: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
+000038d0: 676f 7574 2065 7865 6375 7465 6420 7375  gout executed su
+000038e0: 6363 6573 7366 756c 6c79 2066 6f72 206c  ccessfully for l
+000038f0: 6f67 696e 2025 7322 2c20 6c6f 6769 6e29  ogin %s", login)
+00003900: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003910: 6c6f 6769 6e20 6973 204e 6f6e 653a 0a20  login is None:. 
+00003920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003930: 656c 662e 5f61 6374 6976 655f 6c6f 6769  elf._active_logi
+00003940: 6e73 203d 205b 5d0a 2020 2020 2020 2020  ns = [].        
+00003950: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00003960: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00003970: 6163 7469 7665 5f6c 6f67 696e 732e 7265  active_logins.re
+00003980: 6d6f 7665 286c 6f67 696e 290a 2020 2020  move(login).    
+00003990: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+000039a0: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+000039b0: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
+000039c0: 6620 5f72 6561 645f 7061 7261 6d65 7465  f _read_paramete
+000039d0: 7273 2873 656c 662c 2066 6f72 6365 3a20  rs(self, force: 
+000039e0: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
+000039f0: 206c 642e 5379 7374 656d 5061 7261 6d65   ld.SystemParame
+00003a00: 7465 7273 3a0a 2020 2020 2020 2020 2222  ters:.        ""
+00003a10: 220a 2020 2020 2020 2020 5265 6164 2061  ".        Read a
+00003a20: 6c6c 2061 7661 696c 6162 6c65 2073 7973  ll available sys
+00003a30: 7465 6d20 7061 7261 6d65 7465 7220 656e  tem parameter en
+00003a40: 7472 6965 732e 2054 6865 2072 6573 756c  tries. The resul
+00003a50: 7473 2061 7265 2062 7566 6665 7265 6420  ts are buffered 
+00003a60: 7369 6e63 6520 6974 2069 7320 616c 736f  since it is also
+00003a70: 2075 7365 6420 696e 7465 726e 616c 6c79   used internally
+00003a80: 2e0a 2020 2020 2020 2020 5468 6973 206d  ..        This m
+00003a90: 6561 6e73 2061 6464 6974 696f 6e61 6c20  eans additional 
+00003aa0: 6361 6c6c 7320 646f 6e74 2063 6175 7365  calls dont cause
+00003ab0: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2077   communication w
+00003ac0: 6974 6820 7468 6520 636f 6e74 726f 6c2e  ith the control.
+00003ad0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00003ae0: 2066 6f72 6365 3a20 6966 2060 6054 7275   force: if ``Tru
+00003af0: 6560 6020 7468 6520 696e 666f 726d 6174  e`` the informat
+00003b00: 696f 6e20 6973 2072 652d 7265 6164 2065  ion is re-read e
+00003b10: 7665 6e20 6966 2069 7420 6973 2061 6c72  ven if it is alr
+00003b20: 6561 6479 2062 7566 6665 7265 640a 2020  eady buffered.  
+00003b30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00003b40: 2020 6966 2073 656c 662e 5f73 7973 5f70    if self._sys_p
+00003b50: 6172 2e6c 7376 325f 7665 7273 696f 6e20  ar.lsv2_version 
+00003b60: 213d 202d 3120 616e 6420 666f 7263 6520  != -1 and force 
+00003b70: 6973 2046 616c 7365 3a0a 2020 2020 2020  is False:.      
+00003b80: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+00003b90: 6572 2e64 6562 7567 280a 2020 2020 2020  er.debug(.      
+00003ba0: 2020 2020 2020 2020 2020 2273 7973 7465            "syste
+00003bb0: 6d20 7061 7261 6d65 7465 7273 2061 6c72  m parameters alr
+00003bc0: 6561 6479 2069 6e20 6d65 6d6f 7279 2c20  eady in memory, 
+00003bd0: 7265 7475 726e 2070 7265 7669 6f75 7320  return previous 
+00003be0: 7661 6c75 6573 220a 2020 2020 2020 2020  values".        
+00003bf0: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00003c00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00003c10: 7265 7375 6c74 203d 2073 656c 662e 5f73  result = self._s
+00003c20: 656e 645f 7265 6369 7665 286c 632e 434d  end_recive(lc.CM
+00003c30: 442e 525f 5052 2c20 4e6f 6e65 2c20 6c63  D.R_PR, None, lc
+00003c40: 2e52 5350 2e53 5f50 5229 0a20 2020 2020  .RSP.S_PR).     
+00003c50: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00003c60: 616e 6365 2872 6573 756c 742c 2028 6279  ance(result, (by
+00003c70: 7465 6172 7261 792c 2929 3a0a 2020 2020  tearray,)):.    
 00003c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003c90: 2e5f 6c6f 6767 6572 2e64 6562 7567 2822  ._logger.debug("
-00003ca0: 676f 7420 7379 7374 656d 2070 6172 616d  got system param
-00003cb0: 6574 6572 733a 2025 7322 2c20 7365 6c66  eters: %s", self
-00003cc0: 2e5f 7379 735f 7061 7229 0a20 2020 2020  ._sys_par).     
-00003cd0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003ce0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003cf0: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
-00003d00: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-00003d10: 2020 2020 2020 2022 616e 2065 7272 6f72         "an error
-00003d20: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
-00003d30: 7175 6572 7969 6e67 2073 7973 7465 6d20  querying system 
-00003d40: 7061 7261 6d65 7465 7273 220a 2020 2020  parameters".    
-00003d50: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00003d60: 2020 2020 2020 2020 2020 2070 6179 6c6f             paylo
-00003d70: 6164 203d 2073 7472 7563 742e 7061 636b  ad = struct.pack
-00003d80: 2822 214c 222c 206c 632e 5061 7252 4349  ("!L", lc.ParRCI
-00003d90: 2e54 5552 424f 5f4d 4f44 4529 0a20 2020  .TURBO_MODE).   
-00003da0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00003db0: 3d20 7365 6c66 2e5f 7365 6e64 5f72 6563  = self._send_rec
-00003dc0: 6976 6528 6c63 2e43 4d44 2e52 5f43 492c  ive(lc.CMD.R_CI,
-00003dd0: 2070 6179 6c6f 6164 2c20 6c63 2e52 5350   payload, lc.RSP
-00003de0: 2e53 5f43 4929 0a20 2020 2020 2020 2020  .S_CI).         
-00003df0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00003e00: 2872 6573 756c 742c 2028 6279 7465 6172  (result, (bytear
-00003e10: 7261 792c 2929 2061 6e64 206c 656e 2872  ray,)) and len(r
-00003e20: 6573 756c 7429 203e 2030 3a0a 2020 2020  esult) > 0:.    
-00003e30: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00003e40: 203d 206c 6d2e 6465 636f 6465 5f73 7973   = lm.decode_sys
-00003e50: 7465 6d5f 696e 666f 726d 6174 696f 6e28  tem_information(
-00003e60: 7265 7375 6c74 290a 2020 2020 2020 2020  result).        
-00003e70: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00003e80: 7369 6e73 7461 6e63 6528 6461 7461 2c20  sinstance(data, 
-00003e90: 626f 6f6c 293a 0a20 2020 2020 2020 2020  bool):.         
-00003ea0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003eb0: 204c 5356 3244 6174 6145 7863 6570 7469   LSV2DataExcepti
-00003ec0: 6f6e 2822 6578 7065 6374 6564 2062 6f6f  on("expected boo
-00003ed0: 6c65 616e 2229 0a20 2020 2020 2020 2020  lean").         
-00003ee0: 2020 2020 2020 2073 656c 662e 5f73 7973         self._sys
-00003ef0: 5f70 6172 2e74 7572 626f 5f6d 6f64 655f  _par.turbo_mode_
-00003f00: 6163 7469 7665 203d 2064 6174 610a 2020  active = data.  
-00003f10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f30: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-00003f40: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
-00003f50: 2020 2020 2020 2020 2020 2261 6e20 6572            "an er
-00003f60: 726f 7220 6f63 6375 7272 6564 2077 6869  ror occurred whi
-00003f70: 6c65 2071 7565 7279 696e 6720 7379 7374  le querying syst
-00003f80: 656d 2069 6e66 6f72 6d61 7469 6f6e 206f  em information o
-00003f90: 6e20 7475 7262 6f20 6d6f 6465 220a 2020  n turbo mode".  
-00003fa0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00003fb0: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
-00003fc0: 6c6f 6164 203d 2073 7472 7563 742e 7061  load = struct.pa
-00003fd0: 636b 2822 214c 222c 206c 632e 5061 7252  ck("!L", lc.ParR
-00003fe0: 4349 2e44 4e43 5f41 4c4c 4f57 4544 290a  CI.DNC_ALLOWED).
-00003ff0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00004000: 6c74 203d 2073 656c 662e 5f73 656e 645f  lt = self._send_
-00004010: 7265 6369 7665 286c 632e 434d 442e 525f  recive(lc.CMD.R_
-00004020: 4349 2c20 7061 796c 6f61 642c 206c 632e  CI, payload, lc.
-00004030: 5253 502e 535f 4349 290a 2020 2020 2020  RSP.S_CI).      
-00004040: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00004050: 6e63 6528 7265 7375 6c74 2c20 2862 7974  nce(result, (byt
-00004060: 6561 7272 6179 2c29 2920 616e 6420 6c65  earray,)) and le
-00004070: 6e28 7265 7375 6c74 2920 3e20 303a 0a20  n(result) > 0:. 
-00004080: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004090: 6174 6120 3d20 6c6d 2e64 6563 6f64 655f  ata = lm.decode_
-000040a0: 7379 7374 656d 5f69 6e66 6f72 6d61 7469  system_informati
-000040b0: 6f6e 2872 6573 756c 7429 0a20 2020 2020  on(result).     
-000040c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000040d0: 7420 6973 696e 7374 616e 6365 2864 6174  t isinstance(dat
-000040e0: 612c 2062 6f6f 6c29 3a0a 2020 2020 2020  a, bool):.      
-000040f0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00004100: 6973 6520 4c53 5632 4461 7461 4578 6365  ise LSV2DataExce
-00004110: 7074 696f 6e28 2265 7870 6563 7465 6420  ption("expected 
-00004120: 626f 6f6c 6561 6e22 290a 2020 2020 2020  boolean").      
-00004130: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00004140: 7379 735f 7061 722e 646e 635f 6d6f 6465  sys_par.dnc_mode
-00004150: 5f61 6c6c 6f77 6564 203d 2064 6174 610a  _allowed = data.
-00004160: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00004170: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004180: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e77    self._logger.w
-00004190: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-000041a0: 2020 2020 2020 2020 2020 2020 2261 6e20              "an 
-000041b0: 6572 726f 7220 6f63 6375 7272 6564 2077  error occurred w
-000041c0: 6869 6c65 2071 7565 7279 696e 6720 7379  hile querying sy
-000041d0: 7374 656d 2069 6e66 6f72 6d61 7469 6f6e  stem information
-000041e0: 206f 6e20 646e 6320 6d6f 6465 220a 2020   on dnc mode".  
-000041f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00004200: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
-00004210: 6c6f 6164 203d 2073 7472 7563 742e 7061  load = struct.pa
-00004220: 636b 2822 214c 222c 206c 632e 5061 7252  ck("!L", lc.ParR
-00004230: 4349 2e41 5845 535f 5341 4d50 4c49 4e47  CI.AXES_SAMPLING
-00004240: 5f52 4154 4529 0a20 2020 2020 2020 2020  _RATE).         
-00004250: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-00004260: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
-00004270: 2e43 4d44 2e52 5f43 492c 2070 6179 6c6f  .CMD.R_CI, paylo
-00004280: 6164 2c20 6c63 2e52 5350 2e53 5f43 4929  ad, lc.RSP.S_CI)
-00004290: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000042a0: 6973 696e 7374 616e 6365 2872 6573 756c  isinstance(resul
-000042b0: 742c 2028 6279 7465 6172 7261 792c 2929  t, (bytearray,))
-000042c0: 2061 6e64 206c 656e 2872 6573 756c 7429   and len(result)
-000042d0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-000042e0: 2020 2020 2020 6461 7461 203d 206c 6d2e        data = lm.
-000042f0: 6465 636f 6465 5f73 7973 7465 6d5f 696e  decode_system_in
-00004300: 666f 726d 6174 696f 6e28 7265 7375 6c74  formation(result
-00004310: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004320: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00004330: 6e63 6528 6461 7461 2c20 696e 7429 3a0a  nce(data, int):.
-00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004350: 2020 2020 7261 6973 6520 4c53 5632 4461      raise LSV2Da
-00004360: 7461 4578 6365 7074 696f 6e28 2265 7870  taException("exp
-00004370: 6563 7465 6420 696e 7422 290a 2020 2020  ected int").    
-00004380: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004390: 2e5f 7379 735f 7061 722e 6178 6573 5f73  ._sys_par.axes_s
-000043a0: 616d 706c 696e 675f 7261 7465 203d 2064  ampling_rate = d
-000043b0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-000043c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000043d0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-000043e0: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
-000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004400: 2261 6e20 6572 726f 7220 6f63 6375 7272  "an error occurr
-00004410: 6564 2077 6869 6c65 2071 7565 7279 696e  ed while queryin
-00004420: 6720 7379 7374 656d 2069 6e66 6f72 6d61  g system informa
-00004430: 7469 6f6e 206f 6e20 6178 6573 2073 616d  tion on axes sam
-00004440: 6c69 6e67 2072 6174 6522 0a20 2020 2020  ling rate".     
-00004450: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00004460: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00004470: 2e5f 7379 735f 7061 720a 0a20 2020 2064  ._sys_par..    d
-00004480: 6566 205f 7265 6164 5f76 6572 7369 6f6e  ef _read_version
-00004490: 2873 656c 662c 2066 6f72 6365 3d46 616c  (self, force=Fal
-000044a0: 7365 2920 2d3e 206c 642e 5665 7273 696f  se) -> ld.Versio
-000044b0: 6e49 6e66 6f3a 0a20 2020 2020 2020 2022  nInfo:.        "
-000044c0: 2222 0a20 2020 2020 2020 2052 6561 6420  "".        Read 
-000044d0: 616c 6c20 6176 6169 6c61 626c 6520 7665  all available ve
-000044e0: 7273 696f 6e20 696e 666f 726d 6174 696f  rsion informatio
-000044f0: 6e20 656e 7472 6965 732e 2054 6865 2072  n entries. The r
-00004500: 6573 756c 7473 2061 7265 2062 7566 6665  esults are buffe
-00004510: 7265 6420 7369 6e63 6520 6974 2069 7320  red since it is 
-00004520: 616c 736f 2075 7365 6420 696e 7465 726e  also used intern
-00004530: 616c 6c79 2e0a 2020 2020 2020 2020 5468  ally..        Th
-00004540: 6973 206d 6561 6e73 2061 6464 6974 696f  is means additio
-00004550: 6e61 6c20 6361 6c6c 7320 646f 6e74 2063  nal calls dont c
-00004560: 6175 7365 2063 6f6d 6d75 6e69 6361 7469  ause communicati
-00004570: 6f6e 2077 6974 6820 7468 6520 636f 6e74  on with the cont
-00004580: 726f 6c2e 0a0a 2020 2020 2020 2020 3a70  rol...        :p
-00004590: 6172 616d 2066 6f72 6365 3a20 6966 2060  aram force: if `
-000045a0: 6054 7275 6560 6020 7468 6520 696e 666f  `True`` the info
-000045b0: 726d 6174 696f 6e20 6973 2072 652d 7265  rmation is re-re
-000045c0: 6164 2065 7665 6e20 6966 2069 7420 6973  ad even if it is
-000045d0: 2061 6c72 6561 6479 2062 7566 6665 7265   already buffere
-000045e0: 640a 0a20 2020 2020 2020 203a 7261 6973  d..        :rais
-000045f0: 6573 204c 5356 3244 6174 6145 7863 6570  es LSV2DataExcep
-00004600: 7469 6f6e 3a20 6966 2062 6173 6963 2069  tion: if basic i
-00004610: 6e66 6f72 6d61 7469 6f6e 2063 6f75 6c64  nformation could
-00004620: 206e 6f74 2062 6520 7265 6164 2066 726f   not be read fro
-00004630: 6d20 636f 6e74 726f 6c0a 2020 2020 2020  m control.      
-00004640: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00004650: 206c 656e 2873 656c 662e 5f76 6572 7369   len(self._versi
-00004660: 6f6e 732e 636f 6e74 726f 6c29 203e 2030  ons.control) > 0
-00004670: 2061 6e64 2066 6f72 6365 2069 7320 4661   and force is Fa
-00004680: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00004690: 2073 656c 662e 5f6c 6f67 6765 722e 6465   self._logger.de
-000046a0: 6275 6728 2276 6572 7369 6f6e 2069 6e66  bug("version inf
-000046b0: 6f20 616c 7265 6164 7920 696e 206d 656d  o already in mem
-000046c0: 6f72 792c 2072 6574 7572 6e20 7072 6576  ory, return prev
-000046d0: 696f 7573 2076 616c 7565 7322 290a 2020  ious values").  
-000046e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000046f0: 2020 2020 2020 2020 696e 666f 5f64 6174          info_dat
-00004700: 6120 3d20 6c64 2e56 6572 7369 6f6e 496e  a = ld.VersionIn
-00004710: 666f 2829 0a0a 2020 2020 2020 2020 2020  fo()..          
-00004720: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00004730: 5f73 656e 645f 7265 6369 7665 280a 2020  _send_recive(.  
-00004740: 2020 2020 2020 2020 2020 2020 2020 6c63                lc
-00004750: 2e43 4d44 2e52 5f56 522c 2073 7472 7563  .CMD.R_VR, struc
-00004760: 742e 7061 636b 2822 2142 222c 206c 632e  t.pack("!B", lc.
-00004770: 5061 7252 5652 2e43 4f4e 5452 4f4c 292c  ParRVR.CONTROL),
-00004780: 206c 632e 5253 502e 535f 5652 0a20 2020   lc.RSP.S_VR.   
-00004790: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000047a0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000047b0: 616e 6365 2872 6573 756c 742c 2028 6279  ance(result, (by
-000047c0: 7465 6172 7261 792c 2929 2061 6e64 206c  tearray,)) and l
-000047d0: 656e 2872 6573 756c 7429 203e 2030 3a0a  en(result) > 0:.
-000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047f0: 696e 666f 5f64 6174 612e 636f 6e74 726f  info_data.contro
-00004800: 6c20 3d20 6c6d 2e62 615f 746f 5f75 7374  l = lm.ba_to_ust
-00004810: 7228 7265 7375 6c74 290a 2020 2020 2020  r(result).      
-00004820: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00004830: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00004840: 6520 4c53 5632 4461 7461 4578 6365 7074  e LSV2DataExcept
-00004850: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00004860: 2020 2020 2020 2020 2022 436f 756c 6420           "Could 
-00004870: 6e6f 7420 7265 6164 2076 6572 7369 6f6e  not read version
-00004880: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
-00004890: 6d20 636f 6e74 726f 6c22 0a20 2020 2020  m control".     
-000048a0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-000048b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000048c0: 203d 2073 656c 662e 5f73 656e 645f 7265   = self._send_re
-000048d0: 6369 7665 280a 2020 2020 2020 2020 2020  cive(.          
-000048e0: 2020 2020 2020 6c63 2e43 4d44 2e52 5f56        lc.CMD.R_V
-000048f0: 522c 0a20 2020 2020 2020 2020 2020 2020  R,.             
-00004900: 2020 2073 7472 7563 742e 7061 636b 2822     struct.pack("
-00004910: 2142 222c 206c 632e 5061 7252 5652 2e4e  !B", lc.ParRVR.N
-00004920: 435f 5645 5253 494f 4e29 2c0a 2020 2020  C_VERSION),.    
-00004930: 2020 2020 2020 2020 2020 2020 6c63 2e52              lc.R
-00004940: 5350 2e53 5f56 522c 0a20 2020 2020 2020  SP.S_VR,.       
-00004950: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00004960: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00004970: 2872 6573 756c 742c 2028 6279 7465 6172  (result, (bytear
-00004980: 7261 792c 2929 2061 6e64 206c 656e 2872  ray,)) and len(r
-00004990: 6573 756c 7429 203e 2030 3a0a 2020 2020  esult) > 0:.    
-000049a0: 2020 2020 2020 2020 2020 2020 696e 666f              info
-000049b0: 5f64 6174 612e 6e63 5f73 7720 3d20 6c6d  _data.nc_sw = lm
-000049c0: 2e62 615f 746f 5f75 7374 7228 7265 7375  .ba_to_ustr(resu
-000049d0: 6c74 290a 0a20 2020 2020 2020 2020 2020  lt)..           
-000049e0: 2072 6573 756c 7420 3d20 7365 6c66 2e5f   result = self._
-000049f0: 7365 6e64 5f72 6563 6976 6528 0a20 2020  send_recive(.   
-00004a00: 2020 2020 2020 2020 2020 2020 206c 632e               lc.
-00004a10: 434d 442e 525f 5652 2c0a 2020 2020 2020  CMD.R_VR,.      
-00004a20: 2020 2020 2020 2020 2020 7374 7275 6374            struct
-00004a30: 2e70 6163 6b28 2221 4222 2c20 6c63 2e50  .pack("!B", lc.P
-00004a40: 6172 5256 522e 504c 435f 5645 5253 494f  arRVR.PLC_VERSIO
-00004a50: 4e29 2c0a 2020 2020 2020 2020 2020 2020  N),.            
-00004a60: 2020 2020 6c63 2e52 5350 2e53 5f56 522c      lc.RSP.S_VR,
-00004a70: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00004a80: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00004a90: 696e 7374 616e 6365 2872 6573 756c 742c  instance(result,
-00004aa0: 2028 6279 7465 6172 7261 792c 2929 2061   (bytearray,)) a
-00004ab0: 6e64 206c 656e 2872 6573 756c 7429 203e  nd len(result) >
-00004ac0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00004ad0: 2020 2020 696e 666f 5f64 6174 612e 706c      info_data.pl
-00004ae0: 6320 3d20 6c6d 2e62 615f 746f 5f75 7374  c = lm.ba_to_ust
-00004af0: 7228 7265 7375 6c74 290a 0a20 2020 2020  r(result)..     
-00004b00: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00004b10: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
-00004b20: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00004b30: 2020 206c 632e 434d 442e 525f 5652 2c0a     lc.CMD.R_VR,.
-00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b50: 7374 7275 6374 2e70 6163 6b28 2221 4222  struct.pack("!B"
-00004b60: 2c20 6c63 2e50 6172 5256 522e 4f50 5449  , lc.ParRVR.OPTI
-00004b70: 4f4e 5329 2c0a 2020 2020 2020 2020 2020  ONS),.          
-00004b80: 2020 2020 2020 6c63 2e52 5350 2e53 5f56        lc.RSP.S_V
-00004b90: 522c 0a20 2020 2020 2020 2020 2020 2029  R,.            )
-00004ba0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004bb0: 6973 696e 7374 616e 6365 2872 6573 756c  isinstance(resul
-00004bc0: 742c 2028 6279 7465 6172 7261 792c 2929  t, (bytearray,))
-00004bd0: 2061 6e64 206c 656e 2872 6573 756c 7429   and len(result)
-00004be0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-00004bf0: 2020 2020 2020 696e 666f 5f64 6174 612e        info_data.
-00004c00: 6f70 7469 6f6e 5f62 6974 7320 3d20 6c6d  option_bits = lm
-00004c10: 2e62 615f 746f 5f75 7374 7228 7265 7375  .ba_to_ustr(resu
-00004c20: 6c74 290a 0a20 2020 2020 2020 2020 2020  lt)..           
-00004c30: 2072 6573 756c 7420 3d20 7365 6c66 2e5f   result = self._
-00004c40: 7365 6e64 5f72 6563 6976 6528 0a20 2020  send_recive(.   
-00004c50: 2020 2020 2020 2020 2020 2020 206c 632e               lc.
-00004c60: 434d 442e 525f 5652 2c0a 2020 2020 2020  CMD.R_VR,.      
-00004c70: 2020 2020 2020 2020 2020 7374 7275 6374            struct
-00004c80: 2e70 6163 6b28 2221 4222 2c20 6c63 2e50  .pack("!B", lc.P
-00004c90: 6172 5256 522e 4944 292c 0a20 2020 2020  arRVR.ID),.     
-00004ca0: 2020 2020 2020 2020 2020 206c 632e 5253             lc.RS
-00004cb0: 502e 535f 5652 2c0a 2020 2020 2020 2020  P.S_VR,.        
-00004cc0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00004cd0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00004ce0: 7265 7375 6c74 2c20 2862 7974 6561 7272  result, (bytearr
-00004cf0: 6179 2c29 2920 616e 6420 6c65 6e28 7265  ay,)) and len(re
-00004d00: 7375 6c74 2920 3e20 303a 0a20 2020 2020  sult) > 0:.     
-00004d10: 2020 2020 2020 2020 2020 2069 6e66 6f5f             info_
-00004d20: 6461 7461 2e69 645f 6e75 6d62 6572 203d  data.id_number =
-00004d30: 206c 6d2e 6261 5f74 6f5f 7573 7472 2872   lm.ba_to_ustr(r
-00004d40: 6573 756c 7429 0a0a 2020 2020 2020 2020  esult)..        
-00004d50: 2020 2020 6966 2022 6974 6e63 2220 696e      if "itnc" in
-00004d60: 2069 6e66 6f5f 6461 7461 2e63 6f6e 7472   info_data.contr
-00004d70: 6f6c 2e6c 6f77 6572 2829 3a0a 2020 2020  ol.lower():.    
-00004d80: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00004d90: 5f64 6174 612e 7265 6c65 6173 6520 3d20  _data.release = 
-00004da0: 226e 6f74 2073 7570 706f 7274 6564 220a  "not supported".
-00004db0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00004dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004dd0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00004de0: 5f73 656e 645f 7265 6369 7665 280a 2020  _send_recive(.  
-00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e00: 2020 6c63 2e43 4d44 2e52 5f56 522c 0a20    lc.CMD.R_VR,. 
-00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e20: 2020 2073 7472 7563 742e 7061 636b 2822     struct.pack("
-00004e30: 2142 222c 206c 632e 5061 7252 5652 2e52  !B", lc.ParRVR.R
-00004e40: 454c 4541 5345 5f54 5950 4529 2c0a 2020  ELEASE_TYPE),.  
-00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e60: 2020 6c63 2e52 5350 2e53 5f56 522c 0a20    lc.RSP.S_VR,. 
-00004e70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00004e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e90: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-00004ea0: 6573 756c 742c 2028 6279 7465 6172 7261  esult, (bytearra
-00004eb0: 792c 2929 2061 6e64 206c 656e 2872 6573  y,)) and len(res
-00004ec0: 756c 7429 203e 2030 3a0a 2020 2020 2020  ult) > 0:.      
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00004ee0: 666f 5f64 6174 612e 7265 6c65 6173 6520  fo_data.release 
-00004ef0: 3d20 6c6d 2e62 615f 746f 5f75 7374 7228  = lm.ba_to_ustr(
-00004f00: 7265 7375 6c74 290a 0a20 2020 2020 2020  result)..       
-00004f10: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00004f20: 6c66 2e5f 7365 6e64 5f72 6563 6976 6528  lf._send_recive(
-00004f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004f40: 206c 632e 434d 442e 525f 5652 2c0a 2020   lc.CMD.R_VR,.  
-00004f50: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00004f60: 7275 6374 2e70 6163 6b28 2221 4222 2c20  ruct.pack("!B", 
-00004f70: 6c63 2e50 6172 5256 522e 5350 4c43 5f56  lc.ParRVR.SPLC_V
-00004f80: 4552 5349 4f4e 292c 0a20 2020 2020 2020  ERSION),.       
-00004f90: 2020 2020 2020 2020 206c 632e 5253 502e           lc.RSP.
-00004fa0: 535f 5652 2c0a 2020 2020 2020 2020 2020  S_VR,.          
-00004fb0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00004fc0: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
-00004fd0: 7375 6c74 2c20 2862 7974 6561 7272 6179  sult, (bytearray
-00004fe0: 2c29 2920 616e 6420 6c65 6e28 7265 7375  ,)) and len(resu
-00004ff0: 6c74 2920 3e20 303a 0a20 2020 2020 2020  lt) > 0:.       
-00005000: 2020 2020 2020 2020 2069 6e66 6f5f 6461           info_da
-00005010: 7461 2e73 706c 6320 3d20 6c6d 2e62 615f  ta.splc = lm.ba_
-00005020: 746f 5f75 7374 7228 7265 7375 6c74 290a  to_ustr(result).
-00005030: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00005040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005050: 2020 696e 666f 5f64 6174 612e 7370 6c63    info_data.splc
-00005060: 203d 2022 6e6f 7420 7375 7070 6f72 7465   = "not supporte
-00005070: 6422 0a0a 2020 2020 2020 2020 2020 2020  d"..            
-00005080: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
-00005090: 7567 2822 676f 7420 7665 7273 696f 6e20  ug("got version 
-000050a0: 696e 666f 3a20 2573 222c 2069 6e66 6f5f  info: %s", info_
-000050b0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-000050c0: 2020 7365 6c66 2e5f 7665 7273 696f 6e73    self._versions
-000050d0: 203d 2069 6e66 6f5f 6461 7461 0a0a 2020   = info_data..  
-000050e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000050f0: 662e 5f76 6572 7369 6f6e 730a 0a20 2020  f._versions..   
-00005100: 2064 6566 2070 726f 6772 616d 5f73 7461   def program_sta
-00005110: 7475 7328 7365 6c66 2920 2d3e 206c 632e  tus(self) -> lc.
-00005120: 5067 6d53 7461 7465 3a0a 2020 2020 2020  PgmState:.      
-00005130: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00005140: 7420 7374 6174 7573 2063 6f64 6520 6f66  t status code of
-00005150: 2063 7572 7265 6e74 6c79 2061 6374 6976   currently activ
-00005160: 6520 7072 6f67 7261 6d2e 0a20 2020 2020  e program..     
-00005170: 2020 2052 6571 7569 7265 7320 6163 6365     Requires acce
-00005180: 7373 206c 6576 656c 2060 6044 4e43 6060  ss level ``DNC``
-00005190: 2074 6f20 776f 726b 2e0a 2020 2020 2020   to work..      
-000051a0: 2020 5365 6520 6874 7470 733a 2f2f 6769    See https://gi
-000051b0: 7468 7562 2e63 6f6d 2f74 6669 7363 6865  thub.com/tfische
-000051c0: 7237 332f 4563 6c69 7073 652d 506c 7567  r73/Eclipse-Plug
-000051d0: 696e 2d48 6569 6465 6e68 6169 6e2f 6973  in-Heidenhain/is
-000051e0: 7375 6573 2f31 0a20 2020 2020 2020 2022  sues/1.        "
-000051f0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00005200: 7420 7365 6c66 2e6c 6f67 696e 286c 6f67  t self.login(log
-00005210: 696e 3d6c 632e 4c6f 6769 6e2e 444e 4329  in=lc.Login.DNC)
-00005220: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00005230: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
-00005240: 6e67 2822 636f 756c 6420 6e6f 7420 6c6f  ng("could not lo
-00005250: 6720 696e 2061 7320 7573 6572 2044 4e43  g in as user DNC
-00005260: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00005270: 6574 7572 6e20 6c63 2e50 676d 5374 6174  eturn lc.PgmStat
-00005280: 652e 554e 4445 4649 4e45 440a 0a20 2020  e.UNDEFINED..   
-00005290: 2020 2020 2070 6179 6c6f 6164 203d 2073       payload = s
-000052a0: 7472 7563 742e 7061 636b 2822 2148 222c  truct.pack("!H",
-000052b0: 206c 632e 5061 7252 5249 2e50 474d 5f53   lc.ParRRI.PGM_S
-000052c0: 5441 5445 290a 2020 2020 2020 2020 7265  TATE).        re
-000052d0: 7375 6c74 203d 2073 656c 662e 5f73 656e  sult = self._sen
-000052e0: 645f 7265 6369 7665 286c 632e 434d 442e  d_recive(lc.CMD.
-000052f0: 525f 5249 2c20 7061 796c 6f61 642c 206c  R_RI, payload, l
-00005300: 632e 5253 502e 535f 5249 290a 2020 2020  c.RSP.S_RI).    
-00005310: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00005320: 6528 7265 7375 6c74 2c20 2862 7974 6561  e(result, (bytea
-00005330: 7272 6179 2c29 293a 0a20 2020 2020 2020  rray,)):.       
-00005340: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00005350: 722e 6465 6275 6728 0a20 2020 2020 2020  r.debug(.       
-00005360: 2020 2020 2020 2020 2022 7375 6363 6573           "succes
-00005370: 7366 756c 6c79 2072 6561 6420 7374 6174  sfully read stat
-00005380: 6520 6f66 2061 6374 6976 6520 7072 6f67  e of active prog
-00005390: 7261 6d3a 2025 7322 2c0a 2020 2020 2020  ram: %s",.      
-000053a0: 2020 2020 2020 2020 2020 7374 7275 6374            struct
-000053b0: 2e75 6e70 6163 6b28 2221 4822 2c20 7265  .unpack("!H", re
-000053c0: 7375 6c74 295b 305d 2c0a 2020 2020 2020  sult)[0],.      
-000053d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000053e0: 2020 2020 7265 7475 726e 206c 632e 5067      return lc.Pg
-000053f0: 6d53 7461 7465 2873 7472 7563 742e 756e  mState(struct.un
-00005400: 7061 636b 2822 2148 222c 2072 6573 756c  pack("!H", resul
-00005410: 7429 5b30 5d29 0a20 2020 2020 2020 2073  t)[0]).        s
-00005420: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
-00005430: 696e 6728 2261 6e20 6572 726f 7220 6f63  ing("an error oc
-00005440: 6375 7272 6564 2077 6869 6c65 2071 7565  curred while que
-00005450: 7279 696e 6720 7072 6f67 7261 6d20 7374  rying program st
-00005460: 6174 6522 290a 2020 2020 2020 2020 7265  ate").        re
-00005470: 7475 726e 206c 632e 5067 6d53 7461 7465  turn lc.PgmState
-00005480: 2e55 4e44 4546 494e 4544 0a0a 2020 2020  .UNDEFINED..    
-00005490: 6465 6620 7072 6f67 7261 6d5f 7374 6163  def program_stac
-000054a0: 6b28 7365 6c66 2920 2d3e 2055 6e69 6f6e  k(self) -> Union
-000054b0: 5b6c 642e 5374 6163 6b53 7461 7465 2c20  [ld.StackState, 
-000054c0: 4e6f 6e65 5d3a 0a20 2020 2020 2020 2022  None]:.        "
-000054d0: 2222 0a20 2020 2020 2020 2047 6574 2070  "".        Get p
-000054e0: 6174 6820 6f66 2063 7572 7265 6e74 6c79  ath of currently
-000054f0: 2061 6374 6976 6520 6e63 2070 726f 6772   active nc progr
-00005500: 616d 2873 2920 616e 6420 6375 7272 656e  am(s) and curren
-00005510: 7420 6c69 6e65 206e 756d 6265 722e 0a20  t line number.. 
-00005520: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
-00005530: 6163 6365 7373 206c 6576 656c 2060 6044  access level ``D
-00005540: 4e43 6060 2074 6f20 776f 726b 2e0a 2020  NC`` to work..  
-00005550: 2020 2020 2020 5365 6520 6874 7470 733a        See https:
-00005560: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6669  //github.com/tfi
-00005570: 7363 6865 7237 332f 4563 6c69 7073 652d  scher73/Eclipse-
-00005580: 506c 7567 696e 2d48 6569 6465 6e68 6169  Plugin-Heidenhai
-00005590: 6e2f 6973 7375 6573 2f31 0a20 2020 2020  n/issues/1.     
-000055a0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000055b0: 6620 6e6f 7420 7365 6c66 2e6c 6f67 696e  f not self.login
-000055c0: 286c 6f67 696e 3d6c 632e 4c6f 6769 6e2e  (login=lc.Login.
-000055d0: 444e 4329 3a0a 2020 2020 2020 2020 2020  DNC):.          
-000055e0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e77    self._logger.w
-000055f0: 6172 6e69 6e67 2822 636f 756c 6420 6e6f  arning("could no
-00005600: 7420 6c6f 6720 696e 2061 7320 7573 6572  t log in as user
-00005610: 2044 4e43 2229 0a20 2020 2020 2020 2020   DNC").         
-00005620: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00005630: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
-00005640: 3d20 7374 7275 6374 2e70 6163 6b28 2221  = struct.pack("!
-00005650: 4822 2c20 6c63 2e50 6172 5252 492e 5345  H", lc.ParRRI.SE
-00005660: 4c45 4354 4544 5f50 474d 290a 2020 2020  LECTED_PGM).    
-00005670: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00005680: 662e 5f73 656e 645f 7265 6369 7665 286c  f._send_recive(l
-00005690: 632e 434d 442e 525f 5249 2c20 7061 796c  c.CMD.R_RI, payl
-000056a0: 6f61 642c 206c 632e 5253 502e 535f 5249  oad, lc.RSP.S_RI
-000056b0: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
-000056c0: 6e73 7461 6e63 6528 7265 7375 6c74 2c20  nstance(result, 
-000056d0: 2862 7974 6561 7272 6179 2c29 2920 616e  (bytearray,)) an
-000056e0: 6420 6c65 6e28 7265 7375 6c74 2920 3e20  d len(result) > 
-000056f0: 303a 0a20 2020 2020 2020 2020 2020 2073  0:.            s
-00005700: 7461 636b 5f69 6e66 6f20 3d20 6c6d 2e64  tack_info = lm.d
-00005710: 6563 6f64 655f 7374 6163 6b5f 696e 666f  ecode_stack_info
-00005720: 2872 6573 756c 7429 0a20 2020 2020 2020  (result).       
-00005730: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00005740: 722e 6465 6275 6728 2273 7563 6365 7373  r.debug("success
-00005750: 6675 6c6c 7920 7265 6164 2061 6374 6976  fully read activ
-00005760: 6520 7072 6f67 7261 6d20 7374 6163 6b3a  e program stack:
-00005770: 2025 7322 2c20 7374 6163 6b5f 696e 666f   %s", stack_info
-00005780: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00005790: 7475 726e 2073 7461 636b 5f69 6e66 6f0a  turn stack_info.
-000057a0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-000057b0: 6767 6572 2e77 6172 6e69 6e67 2822 616e  gger.warning("an
-000057c0: 2065 7272 6f72 206f 6363 7572 7265 6420   error occurred 
-000057d0: 7768 696c 6520 7175 6572 7969 6e67 2061  while querying a
-000057e0: 6374 6976 6520 7072 6f67 7261 6d20 7374  ctive program st
-000057f0: 6174 6522 290a 0a20 2020 2020 2020 2072  ate")..        r
-00005800: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00005810: 6465 6620 6578 6563 7574 696f 6e5f 7374  def execution_st
-00005820: 6174 6528 7365 6c66 2920 2d3e 206c 632e  ate(self) -> lc.
-00005830: 4578 6563 5374 6174 653a 0a20 2020 2020  ExecState:.     
-00005840: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00005850: 6574 2073 7461 7475 7320 636f 6465 206f  et status code o
-00005860: 6620 7072 6f67 7261 6d20 7374 6174 650a  f program state.
-00005870: 2020 2020 2020 2020 5265 7175 6972 6573          Requires
-00005880: 2061 6363 6573 7320 6c65 7665 6c20 6060   access level ``
-00005890: 444e 4360 6020 746f 2077 6f72 6b2e 0a20  DNC`` to work.. 
-000058a0: 2020 2020 2020 2053 6565 2068 7474 7073         See https
-000058b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6472  ://github.com/dr
-000058c0: 756e 7369 6e6e 2f70 794c 5356 322f 6973  unsinn/pyLSV2/is
-000058d0: 7375 6573 2f31 0a20 2020 2020 2020 2022  sues/1.        "
-000058e0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-000058f0: 7420 7365 6c66 2e6c 6f67 696e 286c 6f67  t self.login(log
-00005900: 696e 3d6c 632e 4c6f 6769 6e2e 444e 4329  in=lc.Login.DNC)
-00005910: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00005920: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
-00005930: 6e67 2822 636f 756c 6420 6e6f 7420 6c6f  ng("could not lo
-00005940: 6720 696e 2061 7320 7573 6572 2044 4e43  g in as user DNC
-00005950: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00005960: 6574 7572 6e20 6c63 2e45 7865 6353 7461  eturn lc.ExecSta
-00005970: 7465 2e55 4e44 4546 494e 4544 0a0a 2020  te.UNDEFINED..  
-00005980: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-00005990: 7374 7275 6374 2e70 6163 6b28 2221 4822  struct.pack("!H"
-000059a0: 2c20 6c63 2e50 6172 5252 492e 4558 4543  , lc.ParRRI.EXEC
-000059b0: 5f53 5441 5445 290a 0a20 2020 2020 2020  _STATE)..       
-000059c0: 2072 6573 756c 7420 3d20 7365 6c66 2e5f   result = self._
-000059d0: 7365 6e64 5f72 6563 6976 6528 6c63 2e43  send_recive(lc.C
-000059e0: 4d44 2e52 5f52 492c 2070 6179 6c6f 6164  MD.R_RI, payload
-000059f0: 2c20 6c63 2e52 5350 2e53 5f52 4929 0a20  , lc.RSP.S_RI). 
-00005a00: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00005a10: 616e 6365 2872 6573 756c 742c 2028 6279  ance(result, (by
-00005a20: 7465 6172 7261 792c 2929 3a0a 2020 2020  tearray,)):.    
-00005a30: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00005a40: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-00005a50: 2020 2020 2020 2020 2020 2020 2272 6561              "rea
-00005a60: 6420 6578 6563 7574 696f 6e20 7374 6174  d execution stat
-00005a70: 6520 2564 222c 2073 7472 7563 742e 756e  e %d", struct.un
-00005a80: 7061 636b 2822 2148 222c 2072 6573 756c  pack("!H", resul
-00005a90: 7429 5b30 5d0a 2020 2020 2020 2020 2020  t)[0].          
-00005aa0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00005ab0: 7265 7475 726e 206c 632e 4578 6563 5374  return lc.ExecSt
-00005ac0: 6174 6528 7374 7275 6374 2e75 6e70 6163  ate(struct.unpac
-00005ad0: 6b28 2221 4822 2c20 7265 7375 6c74 295b  k("!H", result)[
-00005ae0: 305d 290a 2020 2020 2020 2020 7365 6c66  0]).        self
-00005af0: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
-00005b00: 2822 616e 2065 7272 6f72 206f 6363 7572  ("an error occur
-00005b10: 7265 6420 7768 696c 6520 7175 6572 7969  red while queryi
-00005b20: 6e67 2065 7865 6375 7469 6f6e 2073 7461  ng execution sta
-00005b30: 7465 2229 0a20 2020 2020 2020 2072 6574  te").        ret
-00005b40: 7572 6e20 6c63 2e45 7865 6353 7461 7465  urn lc.ExecState
-00005b50: 2e55 4e44 4546 494e 4544 0a0a 2020 2020  .UNDEFINED..    
-00005b60: 6465 6620 6469 7265 6374 6f72 795f 696e  def directory_in
-00005b70: 666f 2873 656c 662c 2072 656d 6f74 655f  fo(self, remote_
-00005b80: 6469 7265 6374 6f72 793a 2073 7472 203d  directory: str =
-00005b90: 2022 2229 202d 3e20 6c64 2e44 6972 6563   "") -> ld.Direc
-00005ba0: 746f 7279 456e 7472 793a 0a20 2020 2020  toryEntry:.     
-00005bb0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00005bc0: 6561 6420 696e 666f 726d 6174 696f 6e20  ead information 
-00005bd0: 6162 6f75 7420 7468 6520 6375 7272 656e  about the curren
-00005be0: 6374 2077 6f72 6b69 6e67 2064 6972 6563  ct working direc
-00005bf0: 746f 7279 206f 6e20 7468 6520 636f 6e74  tory on the cont
-00005c00: 726f 6c2e 0a20 2020 2020 2020 2052 6571  rol..        Req
-00005c10: 7569 7265 7320 6163 6365 7373 206c 6576  uires access lev
-00005c20: 656c 2060 6046 494c 4554 5241 4e53 4645  el ``FILETRANSFE
-00005c30: 5260 6020 746f 2077 6f72 6b2e 0a0a 2020  R`` to work...  
-00005c40: 2020 2020 2020 3a70 6172 616d 2072 656d        :param rem
-00005c50: 6f74 655f 6469 7265 6374 6f72 793a 206f  ote_directory: o
-00005c60: 7074 696f 6e61 6c2e 2063 6861 6e67 6520  ptional. change 
-00005c70: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
-00005c80: 7920 6265 666f 7265 2072 6561 6469 6e67  y before reading
-00005c90: 2069 6e66 6f0a 2020 2020 2020 2020 2222   info.        ""
-00005ca0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00005cb0: 2073 656c 662e 6c6f 6769 6e28 6c63 2e4c   self.login(lc.L
-00005cc0: 6f67 696e 2e46 494c 4554 5241 4e53 4645  ogin.FILETRANSFE
-00005cd0: 5229 3a0a 2020 2020 2020 2020 2020 2020  R):.            
-00005ce0: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-00005cf0: 6e69 6e67 2822 636f 756c 6420 6e6f 7420  ning("could not 
-00005d00: 6c6f 6720 696e 2061 7320 7573 6572 2046  log in as user F
-00005d10: 494c 4522 290a 2020 2020 2020 2020 2020  ILE").          
-00005d20: 2020 7265 7475 726e 206c 642e 4469 7265    return ld.Dire
-00005d30: 6374 6f72 7945 6e74 7279 2829 0a0a 2020  ctoryEntry()..  
-00005d40: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-00005d50: 2020 2020 2020 206c 656e 2872 656d 6f74         len(remot
-00005d60: 655f 6469 7265 6374 6f72 7929 203e 2030  e_directory) > 0
-00005d70: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00005d80: 2073 656c 662e 6368 616e 6765 5f64 6972   self.change_dir
-00005d90: 6563 746f 7279 2872 656d 6f74 655f 6469  ectory(remote_di
-00005da0: 7265 6374 6f72 7929 2069 7320 4661 6c73  rectory) is Fals
-00005db0: 650a 2020 2020 2020 2020 293a 0a20 2020  e.        ):.   
-00005dc0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00005dd0: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
-00005de0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005df0: 636f 756c 6420 6e6f 7420 6368 616e 6765  could not change
-00005e00: 2063 7572 7265 6e74 2064 6972 6563 746f   current directo
-00005e10: 7279 2074 6f20 7265 6164 2064 6972 6563  ry to read direc
-00005e20: 746f 7279 2069 6e66 6f20 666f 7220 2573  tory info for %s
-00005e30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005e40: 2020 2072 656d 6f74 655f 6469 7265 6374     remote_direct
-00005e50: 6f72 792c 0a20 2020 2020 2020 2020 2020  ory,.           
-00005e60: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-00005e70: 6574 7572 6e20 6c64 2e44 6972 6563 746f  eturn ld.Directo
-00005e80: 7279 456e 7472 7928 290a 2020 2020 2020  ryEntry().      
-00005e90: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00005ea0: 5f73 656e 645f 7265 6369 7665 286c 632e  _send_recive(lc.
-00005eb0: 434d 442e 525f 4449 2c20 4e6f 6e65 2c20  CMD.R_DI, None, 
-00005ec0: 6c63 2e52 5350 2e53 5f44 4929 0a20 2020  lc.RSP.S_DI).   
-00005ed0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00005ee0: 6365 2872 6573 756c 742c 2028 6279 7465  ce(result, (byte
-00005ef0: 6172 7261 792c 2929 2061 6e64 206c 656e  array,)) and len
-00005f00: 2872 6573 756c 7429 203e 2030 3a0a 2020  (result) > 0:.  
-00005f10: 2020 2020 2020 2020 2020 6469 725f 696e            dir_in
-00005f20: 666f 203d 206c 6d2e 6465 636f 6465 5f64  fo = lm.decode_d
-00005f30: 6972 6563 746f 7279 5f69 6e66 6f28 7265  irectory_info(re
-00005f40: 7375 6c74 290a 2020 2020 2020 2020 2020  sult).          
-00005f50: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e64    self._logger.d
-00005f60: 6562 7567 280a 2020 2020 2020 2020 2020  ebug(.          
-00005f70: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
-00005f80: 6c6c 7920 7265 6365 6976 6564 2064 6972  lly received dir
-00005f90: 6563 746f 7279 2069 6e66 6f72 6d61 7469  ectory informati
-00005fa0: 6f6e 2066 6f72 2025 7322 2c20 6469 725f  on for %s", dir_
-00005fb0: 696e 666f 2e70 6174 680a 2020 2020 2020  info.path.      
-00005fc0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00005fd0: 2020 2020 7265 7475 726e 2064 6972 5f69      return dir_i
-00005fe0: 6e66 6f0a 2020 2020 2020 2020 7365 6c66  nfo.        self
-00005ff0: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
-00006000: 2822 616e 2065 7272 6f72 206f 6363 7572  ("an error occur
-00006010: 7265 6420 7768 696c 6520 7175 6572 7969  red while queryi
-00006020: 6e67 2064 6972 6563 746f 7279 2069 6e66  ng directory inf
-00006030: 6f22 290a 0a20 2020 2020 2020 2072 6574  o")..        ret
-00006040: 7572 6e20 6c64 2e44 6972 6563 746f 7279  urn ld.Directory
-00006050: 456e 7472 7928 290a 0a20 2020 2064 6566  Entry()..    def
-00006060: 2063 6861 6e67 655f 6469 7265 6374 6f72   change_director
-00006070: 7928 7365 6c66 2c20 7265 6d6f 7465 5f64  y(self, remote_d
-00006080: 6972 6563 746f 7279 3a20 7374 7229 202d  irectory: str) -
-00006090: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-000060a0: 2222 220a 2020 2020 2020 2020 6368 616e  """.        chan
-000060b0: 6765 2074 6865 2063 7572 7265 6e74 2077  ge the current w
-000060c0: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
-000060d0: 206f 6e20 7468 6520 636f 6e74 726f 6c2e   on the control.
-000060e0: 0a20 2020 2020 2020 2052 6571 7569 7265  .        Require
-000060f0: 7320 6163 6365 7373 206c 6576 656c 2060  s access level `
-00006100: 6046 494c 4554 5241 4e53 4645 5260 6020  `FILETRANSFER`` 
-00006110: 746f 2077 6f72 6b2e 0a20 2020 2020 2020  to work..       
-00006120: 2052 6574 7572 6e73 2060 6054 7275 6560   Returns ``True`
-00006130: 6020 6966 2063 6f6d 706c 6574 6564 2073  ` if completed s
-00006140: 7563 6365 7373 6675 6c6c 792e 0a0a 2020  uccessfully...  
-00006150: 2020 2020 2020 3a70 6172 616d 2072 656d        :param rem
-00006160: 6f74 655f 6469 7265 6374 6f72 793a 2070  ote_directory: p
-00006170: 6174 6820 6f66 2064 6972 6563 746f 7279  ath of directory
-00006180: 206f 6e20 7468 6520 636f 6e74 726f 6c0a   on the control.
-00006190: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000061a0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-000061b0: 6c6f 6769 6e28 6c63 2e4c 6f67 696e 2e46  login(lc.Login.F
-000061c0: 494c 4554 5241 4e53 4645 5229 3a0a 2020  ILETRANSFER):.  
-000061d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000061e0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
-000061f0: 636f 756c 6420 6e6f 7420 6c6f 6720 696e  could not log in
-00006200: 2061 7320 7573 6572 2046 494c 4522 290a   as user FILE").
-00006210: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006220: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-00006230: 2020 6469 725f 7061 7468 203d 2072 656d    dir_path = rem
-00006240: 6f74 655f 6469 7265 6374 6f72 792e 7265  ote_directory.re
-00006250: 706c 6163 6528 222f 222c 206c 632e 5041  place("/", lc.PA
-00006260: 5448 5f53 4550 290a 2020 2020 2020 2020  TH_SEP).        
-00006270: 7061 796c 6f61 6420 3d20 6c6d 2e75 7374  payload = lm.ust
-00006280: 725f 746f 5f62 6128 6469 725f 7061 7468  r_to_ba(dir_path
-00006290: 290a 0a20 2020 2020 2020 2072 6573 756c  )..        resul
-000062a0: 7420 3d20 7365 6c66 2e5f 7365 6e64 5f72  t = self._send_r
-000062b0: 6563 6976 6528 6c63 2e43 4d44 2e43 5f44  ecive(lc.CMD.C_D
-000062c0: 432c 2070 6179 6c6f 6164 2c20 6c63 2e52  C, payload, lc.R
-000062d0: 5350 2e54 5f4f 4b29 0a20 2020 2020 2020  SP.T_OK).       
-000062e0: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-000062f0: 6573 756c 742c 2028 626f 6f6c 2c29 2920  esult, (bool,)) 
-00006300: 616e 6420 7265 7375 6c74 2069 7320 5472  and result is Tr
-00006310: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-00006320: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
-00006330: 7567 2822 6368 616e 6765 6420 776f 726b  ug("changed work
-00006340: 696e 6720 6469 7265 6374 6f72 7920 746f  ing directory to
-00006350: 2025 7322 2c20 6469 725f 7061 7468 290a   %s", dir_path).
-00006360: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006370: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00006380: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-00006390: 6e69 6e67 2822 616e 2065 7272 6f72 206f  ning("an error o
-000063a0: 6363 7572 7265 6420 7768 696c 6520 6368  ccurred while ch
-000063b0: 616e 6769 6e67 2064 6972 6563 746f 7279  anging directory
-000063c0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-000063d0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-000063e0: 2066 696c 655f 696e 666f 2873 656c 662c   file_info(self,
-000063f0: 2072 656d 6f74 655f 6669 6c65 5f70 6174   remote_file_pat
-00006400: 683a 2073 7472 2920 2d3e 2055 6e69 6f6e  h: str) -> Union
-00006410: 5b6c 642e 4669 6c65 456e 7472 792c 204e  [ld.FileEntry, N
-00006420: 6f6e 655d 3a0a 2020 2020 2020 2020 2222  one]:.        ""
-00006430: 220a 2020 2020 2020 2020 5175 6572 7920  ".        Query 
-00006440: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
-00006450: 7420 6120 6669 6c65 2e0a 2020 2020 2020  t a file..      
-00006460: 2020 5265 7175 6972 6573 2061 6363 6573    Requires acces
-00006470: 7320 6c65 7665 6c20 6060 4649 4c45 5452  s level ``FILETR
-00006480: 414e 5346 4552 6060 2074 6f20 776f 726b  ANSFER`` to work
-00006490: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000064a0: 7320 6060 4e6f 6e65 6060 206f 6620 6669  s ``None`` of fi
-000064b0: 6c65 2064 6f65 736e 2774 2065 7869 7374  le doesn't exist
-000064c0: 206f 7220 6d69 7373 696e 6720 6163 6365   or missing acce
-000064d0: 7373 2072 6967 6874 730a 0a20 2020 2020  ss rights..     
-000064e0: 2020 203a 7061 7261 6d20 7265 6d6f 7465     :param remote
-000064f0: 5f66 696c 655f 7061 7468 3a20 7061 7468  _file_path: path
-00006500: 206f 6620 6669 6c65 206f 6e20 7468 6520   of file on the 
-00006510: 636f 6e74 726f 6c0a 0a20 2020 2020 2020  control..       
-00006520: 203a 7261 6973 6573 204c 5356 3250 726f   :raises LSV2Pro
-00006530: 746f 636f 6c45 7863 6570 7469 6f6e 3a20  tocolException: 
-00006540: 6966 2061 6e20 6572 726f 7220 6f63 6375  if an error occu
-00006550: 7272 6564 2064 7572 696e 6720 7265 6164  rred during read
-00006560: 696e 6720 6f66 2066 696c 6520 696e 666f  ing of file info
-00006570: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006580: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00006590: 2e6c 6f67 696e 286c 632e 4c6f 6769 6e2e  .login(lc.Login.
-000065a0: 4649 4c45 5452 414e 5346 4552 293a 0a20  FILETRANSFER):. 
-000065b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000065c0: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
-000065d0: 2263 6f75 6c64 206e 6f74 206c 6f67 2069  "could not log i
-000065e0: 6e20 6173 2075 7365 7220 4649 4c45 2229  n as user FILE")
-000065f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00006600: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-00006610: 2020 6669 6c65 5f70 6174 6820 3d20 7265    file_path = re
-00006620: 6d6f 7465 5f66 696c 655f 7061 7468 2e72  mote_file_path.r
-00006630: 6570 6c61 6365 2822 2f22 2c20 6c63 2e50  eplace("/", lc.P
-00006640: 4154 485f 5345 5029 0a20 2020 2020 2020  ATH_SEP).       
-00006650: 2070 6179 6c6f 6164 203d 206c 6d2e 7573   payload = lm.us
-00006660: 7472 5f74 6f5f 6261 2866 696c 655f 7061  tr_to_ba(file_pa
-00006670: 7468 290a 0a20 2020 2020 2020 2072 6573  th)..        res
-00006680: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
-00006690: 5f72 6563 6976 6528 6c63 2e43 4d44 2e52  _recive(lc.CMD.R
-000066a0: 5f46 492c 2070 6179 6c6f 6164 2c20 6c63  _FI, payload, lc
-000066b0: 2e52 5350 2e53 5f46 4929 0a20 2020 2020  .RSP.S_FI).     
-000066c0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000066d0: 2872 6573 756c 742c 2028 6279 7465 6172  (result, (bytear
-000066e0: 7261 792c 2929 2061 6e64 206c 656e 2872  ray,)) and len(r
-000066f0: 6573 756c 7429 203e 2030 3a0a 2020 2020  esult) > 0:.    
-00006700: 2020 2020 2020 2020 6669 6c65 5f69 6e66          file_inf
-00006710: 6f20 3d20 6c6d 2e64 6563 6f64 655f 6669  o = lm.decode_fi
-00006720: 6c65 5f73 7973 7465 6d5f 696e 666f 2872  le_system_info(r
-00006730: 6573 756c 742c 2073 656c 662e 5f76 6572  esult, self._ver
-00006740: 7369 6f6e 732e 7479 7065 290a 2020 2020  sions.type).    
-00006750: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00006760: 6767 6572 2e64 6562 7567 2822 7265 6365  gger.debug("rece
-00006770: 6976 6564 2066 696c 6520 696e 666f 726d  ived file inform
-00006780: 6174 696f 6e20 666f 7220 2573 222c 2066  ation for %s", f
-00006790: 696c 655f 696e 666f 2e6e 616d 6529 0a20  ile_info.name). 
-000067a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000067b0: 6e20 6669 6c65 5f69 6e66 6f0a 0a20 2020  n file_info..   
-000067c0: 2020 2020 2069 6620 7365 6c66 2e6c 6173       if self.las
-000067d0: 745f 6572 726f 722e 655f 636f 6465 203d  t_error.e_code =
-000067e0: 3d20 6c63 2e4c 5356 3253 7461 7475 7343  = lc.LSV2StatusC
-000067f0: 6f64 652e 545f 4552 5f4e 4f5f 4649 4c45  ode.T_ER_NO_FILE
-00006800: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00006810: 6c66 2e5f 6c6f 6767 6572 2e64 6562 7567  lf._logger.debug
-00006820: 2822 6669 6c65 2064 6f65 7320 6e6f 7420  ("file does not 
-00006830: 6578 6973 7422 290a 2020 2020 2020 2020  exist").        
-00006840: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00006850: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
-00006860: 6f67 6765 722e 6572 726f 7228 0a20 2020  ogger.error(.   
-00006870: 2020 2020 2020 2020 2022 616e 2065 7272           "an err
-00006880: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
-00006890: 6520 7175 6572 7969 6e67 2066 696c 6520  e querying file 
-000068a0: 696e 666f 2066 6f72 2025 7320 3a20 2725  info for %s : '%
-000068b0: 7327 222c 0a20 2020 2020 2020 2020 2020  s'",.           
-000068c0: 2072 656d 6f74 655f 6669 6c65 5f70 6174   remote_file_pat
-000068d0: 682c 0a20 2020 2020 2020 2020 2020 206c  h,.            l
-000068e0: 742e 6765 745f 6572 726f 725f 7465 7874  t.get_error_text
-000068f0: 2873 656c 662e 6c61 7374 5f65 7272 6f72  (self.last_error
-00006900: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
-00006910: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00006920: 0a0a 2020 2020 6465 6620 6469 7265 6374  ..    def direct
-00006930: 6f72 795f 636f 6e74 656e 7428 7365 6c66  ory_content(self
-00006940: 2920 2d3e 204c 6973 745b 6c64 2e46 696c  ) -> List[ld.Fil
-00006950: 6545 6e74 7279 5d3a 0a20 2020 2020 2020  eEntry]:.       
-00006960: 2022 2222 0a20 2020 2020 2020 2051 7565   """.        Que
-00006970: 7279 2063 6f6e 7465 6e74 206f 6620 6375  ry content of cu
-00006980: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
-00006990: 7265 6374 6f72 7920 6672 6f6d 2074 6865  rectory from the
-000069a0: 2063 6f6e 7472 6f6c 2e20 496e 2073 6f6d   control. In som
-000069b0: 6520 7369 7475 6174 696f 6e73 2069 7420  e situations it 
-000069c0: 6973 206e 6563 6573 7361 7279 2074 6f0a  is necessary to.
-000069d0: 2020 2020 2020 2020 6669 7374 2063 616c          fist cal
-000069e0: 6c20 3a70 793a 6675 6e63 3a60 7e70 794c  l :py:func:`~pyL
-000069f0: 5356 322e 4c53 5632 2e64 6972 6563 746f  SV2.LSV2.directo
-00006a00: 7279 5f69 6e66 6f60 206f 7220 656c 7365  ry_info` or else
-00006a10: 2074 6865 2061 7474 7269 6275 7465 7320   the attributes 
-00006a20: 776f 6e27 7420 6265 2063 6f72 7265 6374  won't be correct
-00006a30: 2e0a 2020 2020 2020 2020 5265 7175 6972  ..        Requir
-00006a40: 6573 2061 6363 6573 7320 6c65 7665 6c20  es access level 
-00006a50: 6060 4649 4c45 5452 414e 5346 4552 6060  ``FILETRANSFER``
-00006a60: 2074 6f20 776f 726b 2e0a 2020 2020 2020   to work..      
-00006a70: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
-00006a80: 6620 6e6f 7420 7365 6c66 2e6c 6f67 696e  f not self.login
-00006a90: 286c 632e 4c6f 6769 6e2e 4649 4c45 5452  (lc.Login.FILETR
-00006aa0: 414e 5346 4552 293a 0a20 2020 2020 2020  ANSFER):.       
-00006ab0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00006ac0: 722e 7761 726e 696e 6728 2263 6f75 6c64  r.warning("could
-00006ad0: 206e 6f74 206c 6f67 2069 6e20 6173 2075   not log in as u
-00006ae0: 7365 7220 4649 4c45 2229 0a20 2020 2020  ser FILE").     
-00006af0: 2020 2020 2020 2072 6574 7572 6e20 5b5d         return []
-00006b00: 0a0a 2020 2020 2020 2020 6469 725f 636f  ..        dir_co
-00006b10: 6e74 656e 7420 3d20 5b5d 0a20 2020 2020  ntent = [].     
-00006b20: 2020 2070 6179 6c6f 6164 203d 2062 7974     payload = byt
-00006b30: 6561 7272 6179 2873 7472 7563 742e 7061  earray(struct.pa
-00006b40: 636b 2822 2142 222c 206c 632e 5061 7252  ck("!B", lc.ParR
-00006b50: 4452 2e53 494e 474c 4529 290a 0a20 2020  DR.SINGLE))..   
-00006b60: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00006b70: 6c66 2e5f 7365 6e64 5f72 6563 6976 655f  lf._send_recive_
-00006b80: 626c 6f63 6b28 6c63 2e43 4d44 2e52 5f44  block(lc.CMD.R_D
-00006b90: 522c 2070 6179 6c6f 6164 2c20 6c63 2e52  R, payload, lc.R
-00006ba0: 5350 2e53 5f44 5229 0a20 2020 2020 2020  SP.S_DR).       
-00006bb0: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-00006bc0: 6573 756c 742c 2028 6c69 7374 2c29 293a  esult, (list,)):
-00006bd0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00006be0: 2065 6e74 7279 2069 6e20 7265 7375 6c74   entry in result
-00006bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006c00: 2020 6469 725f 636f 6e74 656e 742e 6170    dir_content.ap
-00006c10: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
-00006c20: 2020 2020 2020 2020 2020 6c6d 2e64 6563            lm.dec
-00006c30: 6f64 655f 6669 6c65 5f73 7973 7465 6d5f  ode_file_system_
-00006c40: 696e 666f 2865 6e74 7279 2c20 7365 6c66  info(entry, self
-00006c50: 2e5f 7665 7273 696f 6e73 2e74 7970 6529  ._versions.type)
-00006c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006c70: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00006c80: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
-00006c90: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
-00006ca0: 2020 2020 2272 6563 6569 7665 6420 2564      "received %d
-00006cb0: 2070 6163 6b61 6765 7320 666f 7220 6469   packages for di
-00006cc0: 7265 6374 6f72 7920 636f 6e74 656e 7422  rectory content"
-00006cd0: 2c20 6c65 6e28 6469 725f 636f 6e74 656e  , len(dir_conten
-00006ce0: 7429 0a20 2020 2020 2020 2020 2020 2029  t).            )
-00006cf0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00006d00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006d10: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
-00006d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d30: 2022 616e 2065 7272 6f72 206f 6363 7572   "an error occur
-00006d40: 7265 6420 7768 696c 6520 6469 7265 6374  red while direct
-00006d50: 6f72 7920 636f 6e74 656e 7420 696e 666f  ory content info
-00006d60: 3a20 2725 7327 222c 0a20 2020 2020 2020  : '%s'",.       
-00006d70: 2020 2020 2020 2020 206c 742e 6765 745f           lt.get_
-00006d80: 6572 726f 725f 7465 7874 2873 656c 662e  error_text(self.
-00006d90: 6c61 7374 5f65 7272 6f72 292c 0a20 2020  last_error),.   
-00006da0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00006db0: 2020 2072 6574 7572 6e20 6469 725f 636f     return dir_co
-00006dc0: 6e74 656e 740a 0a20 2020 2064 6566 2064  ntent..    def d
-00006dd0: 7269 7665 5f69 6e66 6f28 7365 6c66 2920  rive_info(self) 
-00006de0: 2d3e 204c 6973 745b 6c64 2e44 7269 7665  -> List[ld.Drive
-00006df0: 456e 7472 795d 3a0a 2020 2020 2020 2020  Entry]:.        
-00006e00: 2222 220a 2020 2020 2020 2020 5265 6164  """.        Read
-00006e10: 2069 6e66 6f20 616c 6c20 6472 6976 6573   info all drives
-00006e20: 2061 6e64 2070 6172 7469 7469 6f6e 7320   and partitions 
-00006e30: 6672 6f6d 2074 6865 2063 6f6e 7472 6f6c  from the control
-00006e40: 2e0a 2020 2020 2020 2020 5265 7175 6972  ..        Requir
-00006e50: 6573 2061 6363 6573 7320 6c65 7665 6c20  es access level 
-00006e60: 6060 4649 4c45 5452 414e 5346 4552 6060  ``FILETRANSFER``
-00006e70: 2074 6f20 776f 726b 2e0a 2020 2020 2020   to work..      
-00006e80: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
-00006e90: 6620 6e6f 7420 7365 6c66 2e6c 6f67 696e  f not self.login
-00006ea0: 286c 632e 4c6f 6769 6e2e 4649 4c45 5452  (lc.Login.FILETR
-00006eb0: 414e 5346 4552 293a 0a20 2020 2020 2020  ANSFER):.       
-00006ec0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00006ed0: 722e 7761 726e 696e 6728 2263 6f75 6c64  r.warning("could
-00006ee0: 206e 6f74 206c 6f67 2069 6e20 6173 2075   not log in as u
-00006ef0: 7365 7220 4649 4c45 2229 0a20 2020 2020  ser FILE").     
-00006f00: 2020 2020 2020 2072 6574 7572 6e20 5b5d         return []
-00006f10: 0a0a 2020 2020 2020 2020 6472 6976 6573  ..        drives
-00006f20: 5f6c 6973 7420 3d20 5b5d 0a20 2020 2020  _list = [].     
-00006f30: 2020 2070 6179 6c6f 6164 203d 2062 7974     payload = byt
-00006f40: 6561 7272 6179 2873 7472 7563 742e 7061  earray(struct.pa
-00006f50: 636b 2822 2142 222c 206c 632e 5061 7252  ck("!B", lc.ParR
-00006f60: 4452 2e44 5249 5645 5329 290a 2020 2020  DR.DRIVES)).    
-00006f70: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00006f80: 662e 5f73 656e 645f 7265 6369 7665 5f62  f._send_recive_b
-00006f90: 6c6f 636b 286c 632e 434d 442e 525f 4452  lock(lc.CMD.R_DR
-00006fa0: 2c20 7061 796c 6f61 642c 206c 632e 5253  , payload, lc.RS
-00006fb0: 502e 535f 4452 290a 2020 2020 2020 2020  P.S_DR).        
-00006fc0: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
-00006fd0: 7375 6c74 2c20 286c 6973 742c 2929 3a0a  sult, (list,)):.
-00006fe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00006ff0: 656e 7472 7920 696e 2072 6573 756c 743a  entry in result:
-00007000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007010: 2064 7269 7665 735f 6c69 7374 2e65 7874   drives_list.ext
-00007020: 656e 6428 6c6d 2e64 6563 6f64 655f 6472  end(lm.decode_dr
-00007030: 6976 655f 696e 666f 2865 6e74 7279 2929  ive_info(entry))
-00007040: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007050: 6c66 2e5f 6c6f 6767 6572 2e64 6562 7567  lf._logger.debug
-00007060: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00007070: 2020 2273 7563 6365 7373 6675 6c6c 7920    "successfully 
-00007080: 7265 6365 6976 6564 2025 6420 7061 636b  received %d pack
-00007090: 6167 6573 2066 6f72 2064 7269 7665 2069  ages for drive i
-000070a0: 6e66 6f72 6d61 7469 6f6e 2025 7322 2c0a  nformation %s",.
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 6c65 6e28 7265 7375 6c74 292c 0a20 2020  len(result),.   
-000070d0: 2020 2020 2020 2020 2020 2020 2064 7269               dri
-000070e0: 7665 735f 6c69 7374 2c0a 2020 2020 2020  ves_list,.      
-000070f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00007100: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00007110: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e77    self._logger.w
-00007120: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-00007130: 2020 2020 2020 2020 2261 6e20 6572 726f          "an erro
-00007140: 7220 6f63 6375 7272 6564 2077 6869 6c65  r occurred while
-00007150: 2072 6561 6469 6e67 2064 7269 7665 2069   reading drive i
-00007160: 6e66 6f3a 2027 2573 2722 2c0a 2020 2020  nfo: '%s'",.    
-00007170: 2020 2020 2020 2020 2020 2020 6c74 2e67              lt.g
-00007180: 6574 5f65 7272 6f72 5f74 6578 7428 7365  et_error_text(se
-00007190: 6c66 2e6c 6173 745f 6572 726f 7229 2c0a  lf.last_error),.
-000071a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000071b0: 2020 2020 2020 7265 7475 726e 2064 7269        return dri
-000071c0: 7665 735f 6c69 7374 0a0a 2020 2020 6465  ves_list..    de
-000071d0: 6620 6d61 6b65 5f64 6972 6563 746f 7279  f make_directory
-000071e0: 2873 656c 662c 2064 6972 5f70 6174 683a  (self, dir_path:
-000071f0: 2073 7472 2920 2d3e 2062 6f6f 6c3a 0a20   str) -> bool:. 
-00007200: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007210: 2020 2043 7265 6174 6520 6120 6469 7265     Create a dire
-00007220: 6374 6f72 7920 6f6e 2063 6f6e 7472 6f6c  ctory on control
-00007230: 2e20 4966 206e 6563 6573 7361 7279 2061  . If necessary a
-00007240: 6c73 6f20 6372 6561 7465 7320 7061 7265  lso creates pare
-00007250: 6e74 2064 6972 6563 746f 7269 6573 2e0a  nt directories..
-00007260: 2020 2020 2020 2020 5265 7175 6972 6573          Requires
-00007270: 2061 6363 6573 7320 6c65 7665 6c20 6060   access level ``
-00007280: 4649 4c45 5452 414e 5346 4552 6060 2074  FILETRANSFER`` t
-00007290: 6f20 776f 726b 2e0a 2020 2020 2020 2020  o work..        
-000072a0: 5265 7475 726e 7320 6060 5472 7565 6060  Returns ``True``
-000072b0: 2069 6620 636f 6d70 6c65 7465 6420 7375   if completed su
-000072c0: 6363 6573 7366 756c 6c79 2e0a 0a20 2020  ccessfully...   
-000072d0: 2020 2020 203a 7061 7261 6d20 6469 725f       :param dir_
-000072e0: 7061 7468 3a20 7061 7468 206f 6620 6469  path: path of di
-000072f0: 7265 6374 6f72 7920 6f6e 2074 6865 2063  rectory on the c
-00007300: 6f6e 7472 6f6c 0a20 2020 2020 2020 2022  ontrol.        "
-00007310: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00007320: 7420 7365 6c66 2e6c 6f67 696e 286c 632e  t self.login(lc.
-00007330: 4c6f 6769 6e2e 4649 4c45 5452 414e 5346  Login.FILETRANSF
-00007340: 4552 293a 0a20 2020 2020 2020 2020 2020  ER):.           
-00007350: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
-00007360: 726e 696e 6728 2263 6f75 6c64 206e 6f74  rning("could not
-00007370: 206c 6f67 2069 6e20 6173 2075 7365 7220   log in as user 
-00007380: 4649 4c45 2229 0a20 2020 2020 2020 2020  FILE").         
-00007390: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-000073a0: 0a20 2020 2020 2020 2070 6174 685f 7061  .        path_pa
-000073b0: 7274 7320 3d20 6469 725f 7061 7468 2e72  rts = dir_path.r
-000073c0: 6570 6c61 6365 2822 2f22 2c20 6c63 2e50  eplace("/", lc.P
-000073d0: 4154 485f 5345 5029 2e73 706c 6974 280a  ATH_SEP).split(.
-000073e0: 2020 2020 2020 2020 2020 2020 6c63 2e50              lc.P
-000073f0: 4154 485f 5345 500a 2020 2020 2020 2020  ATH_SEP.        
-00007400: 2920 2023 2063 6f6e 7665 7274 2070 6174  )  # convert pat
-00007410: 680a 2020 2020 2020 2020 7061 7468 5f74  h.        path_t
-00007420: 6f5f 6368 6563 6b20 3d20 2222 0a0a 2020  o_check = ""..  
-00007430: 2020 2020 2020 666f 7220 7061 7274 2069        for part i
-00007440: 6e20 7061 7468 5f70 6172 7473 3a0a 2020  n path_parts:.  
-00007450: 2020 2020 2020 2020 2020 7061 7468 5f74            path_t
-00007460: 6f5f 6368 6563 6b20 2b3d 2070 6172 7420  o_check += part 
-00007470: 2b20 6c63 2e50 4154 485f 5345 500a 2020  + lc.PATH_SEP.  
-00007480: 2020 2020 2020 2020 2020 2320 6e6f 2066            # no f
-00007490: 696c 6520 696e 666f 202d 3e20 646f 6573  ile info -> does
-000074a0: 206e 6f74 2065 7869 7374 2061 6e64 2068   not exist and h
-000074b0: 6173 2074 6f20 6265 2063 7265 6174 6564  as to be created
-000074c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000074d0: 7365 6c66 2e66 696c 655f 696e 666f 2870  self.file_info(p
-000074e0: 6174 685f 746f 5f63 6865 636b 2920 6973  ath_to_check) is
-000074f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007500: 2020 2020 2020 2070 6179 6c6f 6164 203d         payload =
-00007510: 206c 6d2e 7573 7472 5f74 6f5f 6261 2870   lm.ustr_to_ba(p
-00007520: 6174 685f 746f 5f63 6865 636b 290a 0a20  ath_to_check).. 
-00007530: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007540: 6573 756c 7420 3d20 7365 6c66 2e5f 7365  esult = self._se
-00007550: 6e64 5f72 6563 6976 6528 6c63 2e43 4d44  nd_recive(lc.CMD
-00007560: 2e43 5f44 4d2c 2070 6179 6c6f 6164 2c20  .C_DM, payload, 
-00007570: 6c63 2e52 5350 2e54 5f4f 4b29 0a20 2020  lc.RSP.T_OK).   
-00007580: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007590: 6973 696e 7374 616e 6365 2872 6573 756c  isinstance(resul
-000075a0: 742c 2028 626f 6f6c 2c29 2920 616e 6420  t, (bool,)) and 
-000075b0: 7265 7375 6c74 2069 7320 5472 7565 3a0a  result is True:.
+00003c90: 2e5f 7379 735f 7061 7220 3d20 6c6d 2e64  ._sys_par = lm.d
+00003ca0: 6563 6f64 655f 7379 7374 656d 5f70 6172  ecode_system_par
+00003cb0: 616d 6574 6572 7328 7265 7375 6c74 290a  ameters(result).
+00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cd0: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
+00003ce0: 7567 2822 676f 7420 7379 7374 656d 2070  ug("got system p
+00003cf0: 6172 616d 6574 6572 733a 2025 7322 2c20  arameters: %s", 
+00003d00: 7365 6c66 2e5f 7379 735f 7061 7229 0a20  self._sys_par). 
+00003d10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d30: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
+00003d40: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+00003d50: 2020 2020 2020 2020 2020 2022 616e 2065             "an e
+00003d60: 7272 6f72 206f 6363 7572 7265 6420 7768  rror occurred wh
+00003d70: 696c 6520 7175 6572 7969 6e67 2073 7973  ile querying sys
+00003d80: 7465 6d20 7061 7261 6d65 7465 7273 220a  tem parameters".
+00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003da0: 290a 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00003db0: 6179 6c6f 6164 203d 2073 7472 7563 742e  ayload = struct.
+00003dc0: 7061 636b 2822 214c 222c 206c 632e 5061  pack("!L", lc.Pa
+00003dd0: 7252 4349 2e54 5552 424f 5f4d 4f44 4529  rRCI.TURBO_MODE)
+00003de0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00003df0: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
+00003e00: 5f72 6563 6976 6528 6c63 2e43 4d44 2e52  _recive(lc.CMD.R
+00003e10: 5f43 492c 2070 6179 6c6f 6164 2c20 6c63  _CI, payload, lc
+00003e20: 2e52 5350 2e53 5f43 4929 0a20 2020 2020  .RSP.S_CI).     
+00003e30: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00003e40: 616e 6365 2872 6573 756c 742c 2028 6279  ance(result, (by
+00003e50: 7465 6172 7261 792c 2929 2061 6e64 206c  tearray,)) and l
+00003e60: 656e 2872 6573 756c 7429 203e 2030 3a0a  en(result) > 0:.
+00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e80: 6461 7461 203d 206c 6d2e 6465 636f 6465  data = lm.decode
+00003e90: 5f73 7973 7465 6d5f 696e 666f 726d 6174  _system_informat
+00003ea0: 696f 6e28 7265 7375 6c74 290a 2020 2020  ion(result).    
+00003eb0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00003ec0: 6f74 2069 7369 6e73 7461 6e63 6528 6461  ot isinstance(da
+00003ed0: 7461 2c20 626f 6f6c 293a 0a20 2020 2020  ta, bool):.     
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00003ef0: 6169 7365 204c 5356 3244 6174 6145 7863  aise LSV2DataExc
+00003f00: 6570 7469 6f6e 2822 6578 7065 6374 6564  eption("expected
+00003f10: 2062 6f6f 6c65 616e 2229 0a20 2020 2020   boolean").     
+00003f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003f30: 5f73 7973 5f70 6172 2e74 7572 626f 5f6d  _sys_par.turbo_m
+00003f40: 6f64 655f 6163 7469 7665 203d 2064 6174  ode_active = dat
+00003f50: 610a 2020 2020 2020 2020 2020 2020 656c  a.            el
+00003f60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00003f70: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+00003f80: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+00003f90: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00003fa0: 6e20 6572 726f 7220 6f63 6375 7272 6564  n error occurred
+00003fb0: 2077 6869 6c65 2071 7565 7279 696e 6720   while querying 
+00003fc0: 7379 7374 656d 2069 6e66 6f72 6d61 7469  system informati
+00003fd0: 6f6e 206f 6e20 7475 7262 6f20 6d6f 6465  on on turbo mode
+00003fe0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00003ff0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00004000: 2070 6179 6c6f 6164 203d 2073 7472 7563   payload = struc
+00004010: 742e 7061 636b 2822 214c 222c 206c 632e  t.pack("!L", lc.
+00004020: 5061 7252 4349 2e44 4e43 5f41 4c4c 4f57  ParRCI.DNC_ALLOW
+00004030: 4544 290a 2020 2020 2020 2020 2020 2020  ED).            
+00004040: 7265 7375 6c74 203d 2073 656c 662e 5f73  result = self._s
+00004050: 656e 645f 7265 6369 7665 286c 632e 434d  end_recive(lc.CM
+00004060: 442e 525f 4349 2c20 7061 796c 6f61 642c  D.R_CI, payload,
+00004070: 206c 632e 5253 502e 535f 4349 290a 2020   lc.RSP.S_CI).  
+00004080: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00004090: 6e73 7461 6e63 6528 7265 7375 6c74 2c20  nstance(result, 
+000040a0: 2862 7974 6561 7272 6179 2c29 2920 616e  (bytearray,)) an
+000040b0: 6420 6c65 6e28 7265 7375 6c74 2920 3e20  d len(result) > 
+000040c0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+000040d0: 2020 2064 6174 6120 3d20 6c6d 2e64 6563     data = lm.dec
+000040e0: 6f64 655f 7379 7374 656d 5f69 6e66 6f72  ode_system_infor
+000040f0: 6d61 7469 6f6e 2872 6573 756c 7429 0a20  mation(result). 
+00004100: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004110: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00004120: 2864 6174 612c 2062 6f6f 6c29 3a0a 2020  (data, bool):.  
+00004130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004140: 2020 7261 6973 6520 4c53 5632 4461 7461    raise LSV2Data
+00004150: 4578 6365 7074 696f 6e28 2265 7870 6563  Exception("expec
+00004160: 7465 6420 626f 6f6c 6561 6e22 290a 2020  ted boolean").  
+00004170: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004180: 6c66 2e5f 7379 735f 7061 722e 646e 635f  lf._sys_par.dnc_
+00004190: 6d6f 6465 5f61 6c6c 6f77 6564 203d 2064  mode_allowed = d
+000041a0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+000041b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000041c0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+000041d0: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
+000041e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041f0: 2261 6e20 6572 726f 7220 6f63 6375 7272  "an error occurr
+00004200: 6564 2077 6869 6c65 2071 7565 7279 696e  ed while queryin
+00004210: 6720 7379 7374 656d 2069 6e66 6f72 6d61  g system informa
+00004220: 7469 6f6e 206f 6e20 646e 6320 6d6f 6465  tion on dnc mode
+00004230: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004240: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00004250: 2070 6179 6c6f 6164 203d 2073 7472 7563   payload = struc
+00004260: 742e 7061 636b 2822 214c 222c 206c 632e  t.pack("!L", lc.
+00004270: 5061 7252 4349 2e41 5845 535f 5341 4d50  ParRCI.AXES_SAMP
+00004280: 4c49 4e47 5f52 4154 4529 0a20 2020 2020  LING_RATE).     
+00004290: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000042a0: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
+000042b0: 6528 6c63 2e43 4d44 2e52 5f43 492c 2070  e(lc.CMD.R_CI, p
+000042c0: 6179 6c6f 6164 2c20 6c63 2e52 5350 2e53  ayload, lc.RSP.S
+000042d0: 5f43 4929 0a20 2020 2020 2020 2020 2020  _CI).           
+000042e0: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+000042f0: 6573 756c 742c 2028 6279 7465 6172 7261  esult, (bytearra
+00004300: 792c 2929 2061 6e64 206c 656e 2872 6573  y,)) and len(res
+00004310: 756c 7429 203e 2030 3a0a 2020 2020 2020  ult) > 0:.      
+00004320: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00004330: 206c 6d2e 6465 636f 6465 5f73 7973 7465   lm.decode_syste
+00004340: 6d5f 696e 666f 726d 6174 696f 6e28 7265  m_information(re
+00004350: 7375 6c74 290a 2020 2020 2020 2020 2020  sult).          
+00004360: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+00004370: 6e73 7461 6e63 6528 6461 7461 2c20 696e  nstance(data, in
+00004380: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00004390: 2020 2020 2020 2020 7261 6973 6520 4c53          raise LS
+000043a0: 5632 4461 7461 4578 6365 7074 696f 6e28  V2DataException(
+000043b0: 2265 7870 6563 7465 6420 696e 7422 290a  "expected int").
+000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043d0: 7365 6c66 2e5f 7379 735f 7061 722e 6178  self._sys_par.ax
+000043e0: 6573 5f73 616d 706c 696e 675f 7261 7465  es_sampling_rate
+000043f0: 203d 2064 6174 610a 2020 2020 2020 2020   = data.        
+00004400: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00004410: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00004420: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
+00004430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004440: 2020 2020 2261 6e20 6572 726f 7220 6f63      "an error oc
+00004450: 6375 7272 6564 2077 6869 6c65 2071 7565  curred while que
+00004460: 7279 696e 6720 7379 7374 656d 2069 6e66  rying system inf
+00004470: 6f72 6d61 7469 6f6e 206f 6e20 6178 6573  ormation on axes
+00004480: 2073 616d 6c69 6e67 2072 6174 6522 0a20   samling rate". 
+00004490: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000044a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000044b0: 7365 6c66 2e5f 7379 735f 7061 720a 0a20  self._sys_par.. 
+000044c0: 2020 2064 6566 205f 7265 6164 5f76 6572     def _read_ver
+000044d0: 7369 6f6e 2873 656c 662c 2066 6f72 6365  sion(self, force
+000044e0: 3d46 616c 7365 2920 2d3e 206c 642e 5665  =False) -> ld.Ve
+000044f0: 7273 696f 6e49 6e66 6f3a 0a20 2020 2020  rsionInfo:.     
+00004500: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00004510: 6561 6420 616c 6c20 6176 6169 6c61 626c  ead all availabl
+00004520: 6520 7665 7273 696f 6e20 696e 666f 726d  e version inform
+00004530: 6174 696f 6e20 656e 7472 6965 732e 2054  ation entries. T
+00004540: 6865 2072 6573 756c 7473 2061 7265 2062  he results are b
+00004550: 7566 6665 7265 6420 7369 6e63 6520 6974  uffered since it
+00004560: 2069 7320 616c 736f 2075 7365 6420 696e   is also used in
+00004570: 7465 726e 616c 6c79 2e0a 2020 2020 2020  ternally..      
+00004580: 2020 5468 6973 206d 6561 6e73 2061 6464    This means add
+00004590: 6974 696f 6e61 6c20 6361 6c6c 7320 646f  itional calls do
+000045a0: 6e74 2063 6175 7365 2063 6f6d 6d75 6e69  nt cause communi
+000045b0: 6361 7469 6f6e 2077 6974 6820 7468 6520  cation with the 
+000045c0: 636f 6e74 726f 6c2e 0a0a 2020 2020 2020  control...      
+000045d0: 2020 3a70 6172 616d 2066 6f72 6365 3a20    :param force: 
+000045e0: 6966 2060 6054 7275 6560 6020 7468 6520  if ``True`` the 
+000045f0: 696e 666f 726d 6174 696f 6e20 6973 2072  information is r
+00004600: 652d 7265 6164 2065 7665 6e20 6966 2069  e-read even if i
+00004610: 7420 6973 2061 6c72 6561 6479 2062 7566  t is already buf
+00004620: 6665 7265 640a 0a20 2020 2020 2020 203a  fered..        :
+00004630: 7261 6973 6573 204c 5356 3244 6174 6145  raises LSV2DataE
+00004640: 7863 6570 7469 6f6e 3a20 6966 2062 6173  xception: if bas
+00004650: 6963 2069 6e66 6f72 6d61 7469 6f6e 2063  ic information c
+00004660: 6f75 6c64 206e 6f74 2062 6520 7265 6164  ould not be read
+00004670: 2066 726f 6d20 636f 6e74 726f 6c0a 2020   from control.  
+00004680: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004690: 2020 6966 206c 656e 2873 656c 662e 5f76    if len(self._v
+000046a0: 6572 7369 6f6e 732e 636f 6e74 726f 6c29  ersions.control)
+000046b0: 203e 2030 2061 6e64 2066 6f72 6365 2069   > 0 and force i
+000046c0: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
+000046d0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+000046e0: 722e 6465 6275 6728 0a20 2020 2020 2020  r.debug(.       
+000046f0: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
+00004700: 6e20 696e 666f 2061 6c72 6561 6479 2069  n info already i
+00004710: 6e20 6d65 6d6f 7279 2c20 7265 7475 726e  n memory, return
+00004720: 2070 7265 7669 6f75 7320 7661 6c75 6573   previous values
+00004730: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00004740: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
+00004750: 6f5f 6461 7461 203d 206c 642e 5665 7273  o_data = ld.Vers
+00004760: 696f 6e49 6e66 6f28 290a 0a20 2020 2020  ionInfo()..     
+00004770: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00004780: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
+00004790: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+000047a0: 2020 206c 632e 434d 442e 525f 5652 2c20     lc.CMD.R_VR, 
+000047b0: 7374 7275 6374 2e70 6163 6b28 2221 4222  struct.pack("!B"
+000047c0: 2c20 6c63 2e50 6172 5256 522e 434f 4e54  , lc.ParRVR.CONT
+000047d0: 524f 4c29 2c20 6c63 2e52 5350 2e53 5f56  ROL), lc.RSP.S_V
+000047e0: 520a 2020 2020 2020 2020 2020 2020 290a  R.            ).
+000047f0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00004800: 7369 6e73 7461 6e63 6528 7265 7375 6c74  sinstance(result
+00004810: 2c20 2862 7974 6561 7272 6179 2c29 2920  , (bytearray,)) 
+00004820: 616e 6420 6c65 6e28 7265 7375 6c74 2920  and len(result) 
+00004830: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00004840: 2020 2020 2069 6e66 6f5f 6461 7461 2e63       info_data.c
+00004850: 6f6e 7472 6f6c 203d 206c 6d2e 6261 5f74  ontrol = lm.ba_t
+00004860: 6f5f 7573 7472 2872 6573 756c 7429 0a20  o_ustr(result). 
+00004870: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00004880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004890: 2072 6169 7365 204c 5356 3244 6174 6145   raise LSV2DataE
+000048a0: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+000048b0: 2020 2020 2020 2020 2020 2020 2020 2243                "C
+000048c0: 6f75 6c64 206e 6f74 2072 6561 6420 7665  ould not read ve
+000048d0: 7273 696f 6e20 696e 666f 726d 6174 696f  rsion informatio
+000048e0: 6e20 6672 6f6d 2063 6f6e 7472 6f6c 220a  n from control".
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00004910: 6573 756c 7420 3d20 7365 6c66 2e5f 7365  esult = self._se
+00004920: 6e64 5f72 6563 6976 6528 0a20 2020 2020  nd_recive(.     
+00004930: 2020 2020 2020 2020 2020 206c 632e 434d             lc.CM
+00004940: 442e 525f 5652 2c0a 2020 2020 2020 2020  D.R_VR,.        
+00004950: 2020 2020 2020 2020 7374 7275 6374 2e70          struct.p
+00004960: 6163 6b28 2221 4222 2c20 6c63 2e50 6172  ack("!B", lc.Par
+00004970: 5256 522e 4e43 5f56 4552 5349 4f4e 292c  RVR.NC_VERSION),
+00004980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004990: 206c 632e 5253 502e 535f 5652 2c0a 2020   lc.RSP.S_VR,.  
+000049a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000049b0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000049c0: 7461 6e63 6528 7265 7375 6c74 2c20 2862  tance(result, (b
+000049d0: 7974 6561 7272 6179 2c29 2920 616e 6420  ytearray,)) and 
+000049e0: 6c65 6e28 7265 7375 6c74 2920 3e20 303a  len(result) > 0:
+000049f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004a00: 2069 6e66 6f5f 6461 7461 2e6e 635f 7377   info_data.nc_sw
+00004a10: 203d 206c 6d2e 6261 5f74 6f5f 7573 7472   = lm.ba_to_ustr
+00004a20: 2872 6573 756c 7429 0a0a 2020 2020 2020  (result)..      
+00004a30: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00004a40: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
+00004a50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004a60: 2020 6c63 2e43 4d44 2e52 5f56 522c 0a20    lc.CMD.R_VR,. 
+00004a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004a80: 7472 7563 742e 7061 636b 2822 2142 222c  truct.pack("!B",
+00004a90: 206c 632e 5061 7252 5652 2e50 4c43 5f56   lc.ParRVR.PLC_V
+00004aa0: 4552 5349 4f4e 292c 0a20 2020 2020 2020  ERSION),.       
+00004ab0: 2020 2020 2020 2020 206c 632e 5253 502e           lc.RSP.
+00004ac0: 535f 5652 2c0a 2020 2020 2020 2020 2020  S_VR,.          
+00004ad0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00004ae0: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
+00004af0: 7375 6c74 2c20 2862 7974 6561 7272 6179  sult, (bytearray
+00004b00: 2c29 2920 616e 6420 6c65 6e28 7265 7375  ,)) and len(resu
+00004b10: 6c74 2920 3e20 303a 0a20 2020 2020 2020  lt) > 0:.       
+00004b20: 2020 2020 2020 2020 2069 6e66 6f5f 6461           info_da
+00004b30: 7461 2e70 6c63 203d 206c 6d2e 6261 5f74  ta.plc = lm.ba_t
+00004b40: 6f5f 7573 7472 2872 6573 756c 7429 0a0a  o_ustr(result)..
+00004b50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00004b60: 6c74 203d 2073 656c 662e 5f73 656e 645f  lt = self._send_
+00004b70: 7265 6369 7665 280a 2020 2020 2020 2020  recive(.        
+00004b80: 2020 2020 2020 2020 6c63 2e43 4d44 2e52          lc.CMD.R
+00004b90: 5f56 522c 0a20 2020 2020 2020 2020 2020  _VR,.           
+00004ba0: 2020 2020 2073 7472 7563 742e 7061 636b       struct.pack
+00004bb0: 2822 2142 222c 206c 632e 5061 7252 5652  ("!B", lc.ParRVR
+00004bc0: 2e4f 5054 494f 4e53 292c 0a20 2020 2020  .OPTIONS),.     
+00004bd0: 2020 2020 2020 2020 2020 206c 632e 5253             lc.RS
+00004be0: 502e 535f 5652 2c0a 2020 2020 2020 2020  P.S_VR,.        
+00004bf0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00004c00: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00004c10: 7265 7375 6c74 2c20 2862 7974 6561 7272  result, (bytearr
+00004c20: 6179 2c29 2920 616e 6420 6c65 6e28 7265  ay,)) and len(re
+00004c30: 7375 6c74 2920 3e20 303a 0a20 2020 2020  sult) > 0:.     
+00004c40: 2020 2020 2020 2020 2020 2069 6e66 6f5f             info_
+00004c50: 6461 7461 2e6f 7074 696f 6e5f 6269 7473  data.option_bits
+00004c60: 203d 206c 6d2e 6261 5f74 6f5f 7573 7472   = lm.ba_to_ustr
+00004c70: 2872 6573 756c 7429 0a0a 2020 2020 2020  (result)..      
+00004c80: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00004c90: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
+00004ca0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004cb0: 2020 6c63 2e43 4d44 2e52 5f56 522c 0a20    lc.CMD.R_VR,. 
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004cd0: 7472 7563 742e 7061 636b 2822 2142 222c  truct.pack("!B",
+00004ce0: 206c 632e 5061 7252 5652 2e49 4429 2c0a   lc.ParRVR.ID),.
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 6c63 2e52 5350 2e53 5f56 522c 0a20 2020  lc.RSP.S_VR,.   
+00004d10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00004d20: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00004d30: 616e 6365 2872 6573 756c 742c 2028 6279  ance(result, (by
+00004d40: 7465 6172 7261 792c 2929 2061 6e64 206c  tearray,)) and l
+00004d50: 656e 2872 6573 756c 7429 203e 2030 3a0a  en(result) > 0:.
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 696e 666f 5f64 6174 612e 6964 5f6e 756d  info_data.id_num
+00004d80: 6265 7220 3d20 6c6d 2e62 615f 746f 5f75  ber = lm.ba_to_u
+00004d90: 7374 7228 7265 7375 6c74 290a 0a20 2020  str(result)..   
+00004da0: 2020 2020 2020 2020 2069 6620 2269 746e           if "itn
+00004db0: 6322 2069 6e20 696e 666f 5f64 6174 612e  c" in info_data.
+00004dc0: 636f 6e74 726f 6c2e 6c6f 7765 7228 293a  control.lower():
+00004dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004de0: 2069 6e66 6f5f 6461 7461 2e72 656c 6561   info_data.relea
+00004df0: 7365 203d 2022 6e6f 7420 7375 7070 6f72  se = "not suppor
+00004e00: 7465 6422 0a20 2020 2020 2020 2020 2020  ted".           
+00004e10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00004e20: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00004e30: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
+00004e40: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00004e50: 2020 2020 2020 206c 632e 434d 442e 525f         lc.CMD.R_
+00004e60: 5652 2c0a 2020 2020 2020 2020 2020 2020  VR,.            
+00004e70: 2020 2020 2020 2020 7374 7275 6374 2e70          struct.p
+00004e80: 6163 6b28 2221 4222 2c20 6c63 2e50 6172  ack("!B", lc.Par
+00004e90: 5256 522e 5245 4c45 4153 455f 5459 5045  RVR.RELEASE_TYPE
+00004ea0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00004eb0: 2020 2020 2020 206c 632e 5253 502e 535f         lc.RSP.S_
+00004ec0: 5652 2c0a 2020 2020 2020 2020 2020 2020  VR,.            
+00004ed0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00004ee0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00004ef0: 6e63 6528 7265 7375 6c74 2c20 2862 7974  nce(result, (byt
+00004f00: 6561 7272 6179 2c29 2920 616e 6420 6c65  earray,)) and le
+00004f10: 6e28 7265 7375 6c74 2920 3e20 303a 0a20  n(result) > 0:. 
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 2020 2069 6e66 6f5f 6461 7461 2e72 656c     info_data.rel
+00004f40: 6561 7365 203d 206c 6d2e 6261 5f74 6f5f  ease = lm.ba_to_
+00004f50: 7573 7472 2872 6573 756c 7429 0a0a 2020  ustr(result)..  
+00004f60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00004f70: 203d 2073 656c 662e 5f73 656e 645f 7265   = self._send_re
+00004f80: 6369 7665 280a 2020 2020 2020 2020 2020  cive(.          
+00004f90: 2020 2020 2020 6c63 2e43 4d44 2e52 5f56        lc.CMD.R_V
+00004fa0: 522c 0a20 2020 2020 2020 2020 2020 2020  R,.             
+00004fb0: 2020 2073 7472 7563 742e 7061 636b 2822     struct.pack("
+00004fc0: 2142 222c 206c 632e 5061 7252 5652 2e53  !B", lc.ParRVR.S
+00004fd0: 504c 435f 5645 5253 494f 4e29 2c0a 2020  PLC_VERSION),.  
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 6c63                lc
+00004ff0: 2e52 5350 2e53 5f56 522c 0a20 2020 2020  .RSP.S_VR,.     
+00005000: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005010: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00005020: 6365 2872 6573 756c 742c 2028 6279 7465  ce(result, (byte
+00005030: 6172 7261 792c 2929 2061 6e64 206c 656e  array,)) and len
+00005040: 2872 6573 756c 7429 203e 2030 3a0a 2020  (result) > 0:.  
+00005050: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00005060: 666f 5f64 6174 612e 7370 6c63 203d 206c  fo_data.splc = l
+00005070: 6d2e 6261 5f74 6f5f 7573 7472 2872 6573  m.ba_to_ustr(res
+00005080: 756c 7429 0a20 2020 2020 2020 2020 2020  ult).           
+00005090: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000050a0: 2020 2020 2020 2069 6e66 6f5f 6461 7461         info_data
+000050b0: 2e73 706c 6320 3d20 226e 6f74 2073 7570  .splc = "not sup
+000050c0: 706f 7274 6564 220a 0a20 2020 2020 2020  ported"..       
+000050d0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+000050e0: 722e 6465 6275 6728 2267 6f74 2076 6572  r.debug("got ver
+000050f0: 7369 6f6e 2069 6e66 6f3a 2025 7322 2c20  sion info: %s", 
+00005100: 696e 666f 5f64 6174 6129 0a20 2020 2020  info_data).     
+00005110: 2020 2020 2020 2073 656c 662e 5f76 6572         self._ver
+00005120: 7369 6f6e 7320 3d20 696e 666f 5f64 6174  sions = info_dat
+00005130: 610a 0a20 2020 2020 2020 2072 6574 7572  a..        retur
+00005140: 6e20 7365 6c66 2e5f 7665 7273 696f 6e73  n self._versions
+00005150: 0a0a 2020 2020 6465 6620 7072 6f67 7261  ..    def progra
+00005160: 6d5f 7374 6174 7573 2873 656c 6629 202d  m_status(self) -
+00005170: 3e20 6c63 2e50 676d 5374 6174 653a 0a20  > lc.PgmState:. 
+00005180: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005190: 2020 2052 6574 2073 7461 7475 7320 636f     Ret status co
+000051a0: 6465 206f 6620 6375 7272 656e 746c 7920  de of currently 
+000051b0: 6163 7469 7665 2070 726f 6772 616d 2e0a  active program..
+000051c0: 2020 2020 2020 2020 5265 7175 6972 6573          Requires
+000051d0: 2061 6363 6573 7320 6c65 7665 6c20 6060   access level ``
+000051e0: 444e 4360 6020 746f 2077 6f72 6b2e 0a20  DNC`` to work.. 
+000051f0: 2020 2020 2020 2053 6565 2068 7474 7073         See https
+00005200: 3a2f 2f67 6974 6875 622e 636f 6d2f 7466  ://github.com/tf
+00005210: 6973 6368 6572 3733 2f45 636c 6970 7365  ischer73/Eclipse
+00005220: 2d50 6c75 6769 6e2d 4865 6964 656e 6861  -Plugin-Heidenha
+00005230: 696e 2f69 7373 7565 732f 310a 2020 2020  in/issues/1.    
+00005240: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005250: 6966 206e 6f74 2073 656c 662e 6c6f 6769  if not self.logi
+00005260: 6e28 6c6f 6769 6e3d 6c63 2e4c 6f67 696e  n(login=lc.Login
+00005270: 2e44 4e43 293a 0a20 2020 2020 2020 2020  .DNC):.         
+00005280: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+00005290: 7761 726e 696e 6728 2263 6f75 6c64 206e  warning("could n
+000052a0: 6f74 206c 6f67 2069 6e20 6173 2075 7365  ot log in as use
+000052b0: 7220 444e 4322 290a 2020 2020 2020 2020  r DNC").        
+000052c0: 2020 2020 7265 7475 726e 206c 632e 5067      return lc.Pg
+000052d0: 6d53 7461 7465 2e55 4e44 4546 494e 4544  mState.UNDEFINED
+000052e0: 0a0a 2020 2020 2020 2020 7061 796c 6f61  ..        payloa
+000052f0: 6420 3d20 7374 7275 6374 2e70 6163 6b28  d = struct.pack(
+00005300: 2221 4822 2c20 6c63 2e50 6172 5252 492e  "!H", lc.ParRRI.
+00005310: 5047 4d5f 5354 4154 4529 0a20 2020 2020  PGM_STATE).     
+00005320: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+00005330: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
+00005340: 2e43 4d44 2e52 5f52 492c 2070 6179 6c6f  .CMD.R_RI, paylo
+00005350: 6164 2c20 6c63 2e52 5350 2e53 5f52 4929  ad, lc.RSP.S_RI)
+00005360: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00005370: 7374 616e 6365 2872 6573 756c 742c 2028  stance(result, (
+00005380: 6279 7465 6172 7261 792c 2929 3a0a 2020  bytearray,)):.  
+00005390: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000053a0: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
+000053b0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000053c0: 7563 6365 7373 6675 6c6c 7920 7265 6164  uccessfully read
+000053d0: 2073 7461 7465 206f 6620 6163 7469 7665   state of active
+000053e0: 2070 726f 6772 616d 3a20 2573 222c 0a20   program: %s",. 
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005400: 7472 7563 742e 756e 7061 636b 2822 2148  truct.unpack("!H
+00005410: 222c 2072 6573 756c 7429 5b30 5d2c 0a20  ", result)[0],. 
+00005420: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00005430: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00005440: 6c63 2e50 676d 5374 6174 6528 7374 7275  lc.PgmState(stru
+00005450: 6374 2e75 6e70 6163 6b28 2221 4822 2c20  ct.unpack("!H", 
+00005460: 7265 7375 6c74 295b 305d 290a 2020 2020  result)[0]).    
+00005470: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+00005480: 2e77 6172 6e69 6e67 2822 616e 2065 7272  .warning("an err
+00005490: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
+000054a0: 6520 7175 6572 7969 6e67 2070 726f 6772  e querying progr
+000054b0: 616d 2073 7461 7465 2229 0a20 2020 2020  am state").     
+000054c0: 2020 2072 6574 7572 6e20 6c63 2e50 676d     return lc.Pgm
+000054d0: 5374 6174 652e 554e 4445 4649 4e45 440a  State.UNDEFINED.
+000054e0: 0a20 2020 2064 6566 2070 726f 6772 616d  .    def program
+000054f0: 5f73 7461 636b 2873 656c 6629 202d 3e20  _stack(self) -> 
+00005500: 556e 696f 6e5b 6c64 2e53 7461 636b 5374  Union[ld.StackSt
+00005510: 6174 652c 204e 6f6e 655d 3a0a 2020 2020  ate, None]:.    
+00005520: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005530: 4765 7420 7061 7468 206f 6620 6375 7272  Get path of curr
+00005540: 656e 746c 7920 6163 7469 7665 206e 6320  ently active nc 
+00005550: 7072 6f67 7261 6d28 7329 2061 6e64 2063  program(s) and c
+00005560: 7572 7265 6e74 206c 696e 6520 6e75 6d62  urrent line numb
+00005570: 6572 2e0a 2020 2020 2020 2020 5265 7175  er..        Requ
+00005580: 6972 6573 2061 6363 6573 7320 6c65 7665  ires access leve
+00005590: 6c20 6060 444e 4360 6020 746f 2077 6f72  l ``DNC`` to wor
+000055a0: 6b2e 0a20 2020 2020 2020 2053 6565 2068  k..        See h
+000055b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000055c0: 6d2f 7466 6973 6368 6572 3733 2f45 636c  m/tfischer73/Ecl
+000055d0: 6970 7365 2d50 6c75 6769 6e2d 4865 6964  ipse-Plugin-Heid
+000055e0: 656e 6861 696e 2f69 7373 7565 732f 310a  enhain/issues/1.
+000055f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005600: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00005610: 6c6f 6769 6e28 6c6f 6769 6e3d 6c63 2e4c  login(login=lc.L
+00005620: 6f67 696e 2e44 4e43 293a 0a20 2020 2020  ogin.DNC):.     
+00005630: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+00005640: 6765 722e 7761 726e 696e 6728 2263 6f75  ger.warning("cou
+00005650: 6c64 206e 6f74 206c 6f67 2069 6e20 6173  ld not log in as
+00005660: 2075 7365 7220 444e 4322 290a 2020 2020   user DNC").    
+00005670: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00005680: 6f6e 650a 0a20 2020 2020 2020 2070 6179  one..        pay
+00005690: 6c6f 6164 203d 2073 7472 7563 742e 7061  load = struct.pa
+000056a0: 636b 2822 2148 222c 206c 632e 5061 7252  ck("!H", lc.ParR
+000056b0: 5249 2e53 454c 4543 5445 445f 5047 4d29  RI.SELECTED_PGM)
+000056c0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000056d0: 3d20 7365 6c66 2e5f 7365 6e64 5f72 6563  = self._send_rec
+000056e0: 6976 6528 6c63 2e43 4d44 2e52 5f52 492c  ive(lc.CMD.R_RI,
+000056f0: 2070 6179 6c6f 6164 2c20 6c63 2e52 5350   payload, lc.RSP
+00005700: 2e53 5f52 4929 0a20 2020 2020 2020 2069  .S_RI).        i
+00005710: 6620 6973 696e 7374 616e 6365 2872 6573  f isinstance(res
+00005720: 756c 742c 2028 6279 7465 6172 7261 792c  ult, (bytearray,
+00005730: 2929 2061 6e64 206c 656e 2872 6573 756c  )) and len(resul
+00005740: 7429 203e 2030 3a0a 2020 2020 2020 2020  t) > 0:.        
+00005750: 2020 2020 7374 6163 6b5f 696e 666f 203d      stack_info =
+00005760: 206c 6d2e 6465 636f 6465 5f73 7461 636b   lm.decode_stack
+00005770: 5f69 6e66 6f28 7265 7375 6c74 290a 2020  _info(result).  
+00005780: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00005790: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
+000057a0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000057b0: 7563 6365 7373 6675 6c6c 7920 7265 6164  uccessfully read
+000057c0: 2061 6374 6976 6520 7072 6f67 7261 6d20   active program 
+000057d0: 7374 6163 6b3a 2025 7322 2c20 7374 6163  stack: %s", stac
+000057e0: 6b5f 696e 666f 290a 2020 2020 2020 2020  k_info).        
+000057f0: 2020 2020 7265 7475 726e 2073 7461 636b      return stack
+00005800: 5f69 6e66 6f0a 2020 2020 2020 2020 7365  _info.        se
+00005810: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
+00005820: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00005830: 2261 6e20 6572 726f 7220 6f63 6375 7272  "an error occurr
+00005840: 6564 2077 6869 6c65 2071 7565 7279 696e  ed while queryin
+00005850: 6720 6163 7469 7665 2070 726f 6772 616d  g active program
+00005860: 2073 7461 7465 2229 0a0a 2020 2020 2020   state")..      
+00005870: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+00005880: 2020 2064 6566 2065 7865 6375 7469 6f6e     def execution
+00005890: 5f73 7461 7465 2873 656c 6629 202d 3e20  _state(self) -> 
+000058a0: 6c63 2e45 7865 6353 7461 7465 3a0a 2020  lc.ExecState:.  
+000058b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000058c0: 2020 4765 7420 7374 6174 7573 2063 6f64    Get status cod
+000058d0: 6520 6f66 2070 726f 6772 616d 2073 7461  e of program sta
+000058e0: 7465 0a20 2020 2020 2020 2052 6571 7569  te.        Requi
+000058f0: 7265 7320 6163 6365 7373 206c 6576 656c  res access level
+00005900: 2060 6044 4e43 6060 2074 6f20 776f 726b   ``DNC`` to work
+00005910: 2e0a 2020 2020 2020 2020 5365 6520 6874  ..        See ht
+00005920: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00005930: 2f64 7275 6e73 696e 6e2f 7079 4c53 5632  /drunsinn/pyLSV2
+00005940: 2f69 7373 7565 732f 310a 2020 2020 2020  /issues/1.      
+00005950: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00005960: 206e 6f74 2073 656c 662e 6c6f 6769 6e28   not self.login(
+00005970: 6c6f 6769 6e3d 6c63 2e4c 6f67 696e 2e44  login=lc.Login.D
+00005980: 4e43 293a 0a20 2020 2020 2020 2020 2020  NC):.           
+00005990: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
+000059a0: 726e 696e 6728 2263 6f75 6c64 206e 6f74  rning("could not
+000059b0: 206c 6f67 2069 6e20 6173 2075 7365 7220   log in as user 
+000059c0: 444e 4322 290a 2020 2020 2020 2020 2020  DNC").          
+000059d0: 2020 7265 7475 726e 206c 632e 4578 6563    return lc.Exec
+000059e0: 5374 6174 652e 554e 4445 4649 4e45 440a  State.UNDEFINED.
+000059f0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00005a00: 203d 2073 7472 7563 742e 7061 636b 2822   = struct.pack("
+00005a10: 2148 222c 206c 632e 5061 7252 5249 2e45  !H", lc.ParRRI.E
+00005a20: 5845 435f 5354 4154 4529 0a0a 2020 2020  XEC_STATE)..    
+00005a30: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+00005a40: 662e 5f73 656e 645f 7265 6369 7665 286c  f._send_recive(l
+00005a50: 632e 434d 442e 525f 5249 2c20 7061 796c  c.CMD.R_RI, payl
+00005a60: 6f61 642c 206c 632e 5253 502e 535f 5249  oad, lc.RSP.S_RI
+00005a70: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
+00005a80: 6e73 7461 6e63 6528 7265 7375 6c74 2c20  nstance(result, 
+00005a90: 2862 7974 6561 7272 6179 2c29 293a 0a20  (bytearray,)):. 
+00005aa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005ab0: 5f6c 6f67 6765 722e 6465 6275 6728 0a20  _logger.debug(. 
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005ad0: 7265 6164 2065 7865 6375 7469 6f6e 2073  read execution s
+00005ae0: 7461 7465 2025 6422 2c20 7374 7275 6374  tate %d", struct
+00005af0: 2e75 6e70 6163 6b28 2221 4822 2c20 7265  .unpack("!H", re
+00005b00: 7375 6c74 295b 305d 0a20 2020 2020 2020  sult)[0].       
+00005b10: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00005b20: 2020 2072 6574 7572 6e20 6c63 2e45 7865     return lc.Exe
+00005b30: 6353 7461 7465 2873 7472 7563 742e 756e  cState(struct.un
+00005b40: 7061 636b 2822 2148 222c 2072 6573 756c  pack("!H", resul
+00005b50: 7429 5b30 5d29 0a20 2020 2020 2020 2073  t)[0]).        s
+00005b60: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
+00005b70: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00005b80: 2022 616e 2065 7272 6f72 206f 6363 7572   "an error occur
+00005b90: 7265 6420 7768 696c 6520 7175 6572 7969  red while queryi
+00005ba0: 6e67 2065 7865 6375 7469 6f6e 2073 7461  ng execution sta
+00005bb0: 7465 2229 0a20 2020 2020 2020 2072 6574  te").        ret
+00005bc0: 7572 6e20 6c63 2e45 7865 6353 7461 7465  urn lc.ExecState
+00005bd0: 2e55 4e44 4546 494e 4544 0a0a 2020 2020  .UNDEFINED..    
+00005be0: 6465 6620 6469 7265 6374 6f72 795f 696e  def directory_in
+00005bf0: 666f 2873 656c 662c 2072 656d 6f74 655f  fo(self, remote_
+00005c00: 6469 7265 6374 6f72 793a 2073 7472 203d  directory: str =
+00005c10: 2022 2229 202d 3e20 6c64 2e44 6972 6563   "") -> ld.Direc
+00005c20: 746f 7279 456e 7472 793a 0a20 2020 2020  toryEntry:.     
+00005c30: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00005c40: 6561 6420 696e 666f 726d 6174 696f 6e20  ead information 
+00005c50: 6162 6f75 7420 7468 6520 6375 7272 656e  about the curren
+00005c60: 6374 2077 6f72 6b69 6e67 2064 6972 6563  ct working direc
+00005c70: 746f 7279 206f 6e20 7468 6520 636f 6e74  tory on the cont
+00005c80: 726f 6c2e 0a20 2020 2020 2020 2052 6571  rol..        Req
+00005c90: 7569 7265 7320 6163 6365 7373 206c 6576  uires access lev
+00005ca0: 656c 2060 6046 494c 4554 5241 4e53 4645  el ``FILETRANSFE
+00005cb0: 5260 6020 746f 2077 6f72 6b2e 0a0a 2020  R`` to work...  
+00005cc0: 2020 2020 2020 3a70 6172 616d 2072 656d        :param rem
+00005cd0: 6f74 655f 6469 7265 6374 6f72 793a 206f  ote_directory: o
+00005ce0: 7074 696f 6e61 6c2e 2063 6861 6e67 6520  ptional. change 
+00005cf0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+00005d00: 7920 6265 666f 7265 2072 6561 6469 6e67  y before reading
+00005d10: 2069 6e66 6f0a 2020 2020 2020 2020 2222   info.        ""
+00005d20: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+00005d30: 2073 656c 662e 6c6f 6769 6e28 6c63 2e4c   self.login(lc.L
+00005d40: 6f67 696e 2e46 494c 4554 5241 4e53 4645  ogin.FILETRANSFE
+00005d50: 5229 3a0a 2020 2020 2020 2020 2020 2020  R):.            
+00005d60: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
+00005d70: 6e69 6e67 2822 636f 756c 6420 6e6f 7420  ning("could not 
+00005d80: 6c6f 6720 696e 2061 7320 7573 6572 2046  log in as user F
+00005d90: 494c 4522 290a 2020 2020 2020 2020 2020  ILE").          
+00005da0: 2020 7265 7475 726e 206c 642e 4469 7265    return ld.Dire
+00005db0: 6374 6f72 7945 6e74 7279 2829 0a0a 2020  ctoryEntry()..  
+00005dc0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+00005dd0: 2020 2020 2020 206c 656e 2872 656d 6f74         len(remot
+00005de0: 655f 6469 7265 6374 6f72 7929 203e 2030  e_directory) > 0
+00005df0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00005e00: 2073 656c 662e 6368 616e 6765 5f64 6972   self.change_dir
+00005e10: 6563 746f 7279 2872 656d 6f74 655f 6469  ectory(remote_di
+00005e20: 7265 6374 6f72 7929 2069 7320 4661 6c73  rectory) is Fals
+00005e30: 650a 2020 2020 2020 2020 293a 0a20 2020  e.        ):.   
+00005e40: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+00005e50: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005e70: 636f 756c 6420 6e6f 7420 6368 616e 6765  could not change
+00005e80: 2063 7572 7265 6e74 2064 6972 6563 746f   current directo
+00005e90: 7279 2074 6f20 7265 6164 2064 6972 6563  ry to read direc
+00005ea0: 746f 7279 2069 6e66 6f20 666f 7220 2573  tory info for %s
+00005eb0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005ec0: 2020 2072 656d 6f74 655f 6469 7265 6374     remote_direct
+00005ed0: 6f72 792c 0a20 2020 2020 2020 2020 2020  ory,.           
+00005ee0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+00005ef0: 6574 7572 6e20 6c64 2e44 6972 6563 746f  eturn ld.Directo
+00005f00: 7279 456e 7472 7928 290a 2020 2020 2020  ryEntry().      
+00005f10: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+00005f20: 5f73 656e 645f 7265 6369 7665 286c 632e  _send_recive(lc.
+00005f30: 434d 442e 525f 4449 2c20 4e6f 6e65 2c20  CMD.R_DI, None, 
+00005f40: 6c63 2e52 5350 2e53 5f44 4929 0a20 2020  lc.RSP.S_DI).   
+00005f50: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00005f60: 6365 2872 6573 756c 742c 2028 6279 7465  ce(result, (byte
+00005f70: 6172 7261 792c 2929 2061 6e64 206c 656e  array,)) and len
+00005f80: 2872 6573 756c 7429 203e 2030 3a0a 2020  (result) > 0:.  
+00005f90: 2020 2020 2020 2020 2020 6469 725f 696e            dir_in
+00005fa0: 666f 203d 206c 6d2e 6465 636f 6465 5f64  fo = lm.decode_d
+00005fb0: 6972 6563 746f 7279 5f69 6e66 6f28 7265  irectory_info(re
+00005fc0: 7375 6c74 290a 2020 2020 2020 2020 2020  sult).          
+00005fd0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e64    self._logger.d
+00005fe0: 6562 7567 280a 2020 2020 2020 2020 2020  ebug(.          
+00005ff0: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
+00006000: 6c6c 7920 7265 6365 6976 6564 2064 6972  lly received dir
+00006010: 6563 746f 7279 2069 6e66 6f72 6d61 7469  ectory informati
+00006020: 6f6e 2066 6f72 2025 7322 2c20 6469 725f  on for %s", dir_
+00006030: 696e 666f 2e70 6174 680a 2020 2020 2020  info.path.      
+00006040: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00006050: 2020 2020 7265 7475 726e 2064 6972 5f69      return dir_i
+00006060: 6e66 6f0a 2020 2020 2020 2020 7365 6c66  nfo.        self
+00006070: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
+00006080: 2822 616e 2065 7272 6f72 206f 6363 7572  ("an error occur
+00006090: 7265 6420 7768 696c 6520 7175 6572 7969  red while queryi
+000060a0: 6e67 2064 6972 6563 746f 7279 2069 6e66  ng directory inf
+000060b0: 6f22 290a 0a20 2020 2020 2020 2072 6574  o")..        ret
+000060c0: 7572 6e20 6c64 2e44 6972 6563 746f 7279  urn ld.Directory
+000060d0: 456e 7472 7928 290a 0a20 2020 2064 6566  Entry()..    def
+000060e0: 2063 6861 6e67 655f 6469 7265 6374 6f72   change_director
+000060f0: 7928 7365 6c66 2c20 7265 6d6f 7465 5f64  y(self, remote_d
+00006100: 6972 6563 746f 7279 3a20 7374 7229 202d  irectory: str) -
+00006110: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00006120: 2222 220a 2020 2020 2020 2020 6368 616e  """.        chan
+00006130: 6765 2074 6865 2063 7572 7265 6e74 2077  ge the current w
+00006140: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
+00006150: 206f 6e20 7468 6520 636f 6e74 726f 6c2e   on the control.
+00006160: 0a20 2020 2020 2020 2052 6571 7569 7265  .        Require
+00006170: 7320 6163 6365 7373 206c 6576 656c 2060  s access level `
+00006180: 6046 494c 4554 5241 4e53 4645 5260 6020  `FILETRANSFER`` 
+00006190: 746f 2077 6f72 6b2e 0a20 2020 2020 2020  to work..       
+000061a0: 2052 6574 7572 6e73 2060 6054 7275 6560   Returns ``True`
+000061b0: 6020 6966 2063 6f6d 706c 6574 6564 2073  ` if completed s
+000061c0: 7563 6365 7373 6675 6c6c 792e 0a0a 2020  uccessfully...  
+000061d0: 2020 2020 2020 3a70 6172 616d 2072 656d        :param rem
+000061e0: 6f74 655f 6469 7265 6374 6f72 793a 2070  ote_directory: p
+000061f0: 6174 6820 6f66 2064 6972 6563 746f 7279  ath of directory
+00006200: 206f 6e20 7468 6520 636f 6e74 726f 6c0a   on the control.
+00006210: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006220: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00006230: 6c6f 6769 6e28 6c63 2e4c 6f67 696e 2e46  login(lc.Login.F
+00006240: 494c 4554 5241 4e53 4645 5229 3a0a 2020  ILETRANSFER):.  
+00006250: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00006260: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+00006270: 636f 756c 6420 6e6f 7420 6c6f 6720 696e  could not log in
+00006280: 2061 7320 7573 6572 2046 494c 4522 290a   as user FILE").
+00006290: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000062a0: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
+000062b0: 2020 6469 725f 7061 7468 203d 2072 656d    dir_path = rem
+000062c0: 6f74 655f 6469 7265 6374 6f72 792e 7265  ote_directory.re
+000062d0: 706c 6163 6528 222f 222c 206c 632e 5041  place("/", lc.PA
+000062e0: 5448 5f53 4550 290a 2020 2020 2020 2020  TH_SEP).        
+000062f0: 7061 796c 6f61 6420 3d20 6c6d 2e75 7374  payload = lm.ust
+00006300: 725f 746f 5f62 6128 6469 725f 7061 7468  r_to_ba(dir_path
+00006310: 290a 0a20 2020 2020 2020 2072 6573 756c  )..        resul
+00006320: 7420 3d20 7365 6c66 2e5f 7365 6e64 5f72  t = self._send_r
+00006330: 6563 6976 6528 6c63 2e43 4d44 2e43 5f44  ecive(lc.CMD.C_D
+00006340: 432c 2070 6179 6c6f 6164 2c20 6c63 2e52  C, payload, lc.R
+00006350: 5350 2e54 5f4f 4b29 0a20 2020 2020 2020  SP.T_OK).       
+00006360: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+00006370: 6573 756c 742c 2028 626f 6f6c 2c29 2920  esult, (bool,)) 
+00006380: 616e 6420 7265 7375 6c74 2069 7320 5472  and result is Tr
+00006390: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+000063a0: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
+000063b0: 7567 2822 6368 616e 6765 6420 776f 726b  ug("changed work
+000063c0: 696e 6720 6469 7265 6374 6f72 7920 746f  ing directory to
+000063d0: 2025 7322 2c20 6469 725f 7061 7468 290a   %s", dir_path).
+000063e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000063f0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+00006400: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
+00006410: 6e69 6e67 2822 616e 2065 7272 6f72 206f  ning("an error o
+00006420: 6363 7572 7265 6420 7768 696c 6520 6368  ccurred while ch
+00006430: 616e 6769 6e67 2064 6972 6563 746f 7279  anging directory
+00006440: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00006450: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00006460: 2066 696c 655f 696e 666f 2873 656c 662c   file_info(self,
+00006470: 2072 656d 6f74 655f 6669 6c65 5f70 6174   remote_file_pat
+00006480: 683a 2073 7472 2920 2d3e 2055 6e69 6f6e  h: str) -> Union
+00006490: 5b6c 642e 4669 6c65 456e 7472 792c 204e  [ld.FileEntry, N
+000064a0: 6f6e 655d 3a0a 2020 2020 2020 2020 2222  one]:.        ""
+000064b0: 220a 2020 2020 2020 2020 5175 6572 7920  ".        Query 
+000064c0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+000064d0: 7420 6120 6669 6c65 2e0a 2020 2020 2020  t a file..      
+000064e0: 2020 5265 7175 6972 6573 2061 6363 6573    Requires acces
+000064f0: 7320 6c65 7665 6c20 6060 4649 4c45 5452  s level ``FILETR
+00006500: 414e 5346 4552 6060 2074 6f20 776f 726b  ANSFER`` to work
+00006510: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00006520: 7320 6060 4e6f 6e65 6060 206f 6620 6669  s ``None`` of fi
+00006530: 6c65 2064 6f65 736e 2774 2065 7869 7374  le doesn't exist
+00006540: 206f 7220 6d69 7373 696e 6720 6163 6365   or missing acce
+00006550: 7373 2072 6967 6874 730a 0a20 2020 2020  ss rights..     
+00006560: 2020 203a 7061 7261 6d20 7265 6d6f 7465     :param remote
+00006570: 5f66 696c 655f 7061 7468 3a20 7061 7468  _file_path: path
+00006580: 206f 6620 6669 6c65 206f 6e20 7468 6520   of file on the 
+00006590: 636f 6e74 726f 6c0a 0a20 2020 2020 2020  control..       
+000065a0: 203a 7261 6973 6573 204c 5356 3250 726f   :raises LSV2Pro
+000065b0: 746f 636f 6c45 7863 6570 7469 6f6e 3a20  tocolException: 
+000065c0: 6966 2061 6e20 6572 726f 7220 6f63 6375  if an error occu
+000065d0: 7272 6564 2064 7572 696e 6720 7265 6164  rred during read
+000065e0: 696e 6720 6f66 2066 696c 6520 696e 666f  ing of file info
+000065f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006600: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00006610: 2e6c 6f67 696e 286c 632e 4c6f 6769 6e2e  .login(lc.Login.
+00006620: 4649 4c45 5452 414e 5346 4552 293a 0a20  FILETRANSFER):. 
+00006630: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006640: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
+00006650: 2263 6f75 6c64 206e 6f74 206c 6f67 2069  "could not log i
+00006660: 6e20 6173 2075 7365 7220 4649 4c45 2229  n as user FILE")
+00006670: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00006680: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00006690: 2020 6669 6c65 5f70 6174 6820 3d20 7265    file_path = re
+000066a0: 6d6f 7465 5f66 696c 655f 7061 7468 2e72  mote_file_path.r
+000066b0: 6570 6c61 6365 2822 2f22 2c20 6c63 2e50  eplace("/", lc.P
+000066c0: 4154 485f 5345 5029 0a20 2020 2020 2020  ATH_SEP).       
+000066d0: 2070 6179 6c6f 6164 203d 206c 6d2e 7573   payload = lm.us
+000066e0: 7472 5f74 6f5f 6261 2866 696c 655f 7061  tr_to_ba(file_pa
+000066f0: 7468 290a 0a20 2020 2020 2020 2072 6573  th)..        res
+00006700: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
+00006710: 5f72 6563 6976 6528 6c63 2e43 4d44 2e52  _recive(lc.CMD.R
+00006720: 5f46 492c 2070 6179 6c6f 6164 2c20 6c63  _FI, payload, lc
+00006730: 2e52 5350 2e53 5f46 4929 0a20 2020 2020  .RSP.S_FI).     
+00006740: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00006750: 2872 6573 756c 742c 2028 6279 7465 6172  (result, (bytear
+00006760: 7261 792c 2929 2061 6e64 206c 656e 2872  ray,)) and len(r
+00006770: 6573 756c 7429 203e 2030 3a0a 2020 2020  esult) > 0:.    
+00006780: 2020 2020 2020 2020 6669 6c65 5f69 6e66          file_inf
+00006790: 6f20 3d20 6c6d 2e64 6563 6f64 655f 6669  o = lm.decode_fi
+000067a0: 6c65 5f73 7973 7465 6d5f 696e 666f 2872  le_system_info(r
+000067b0: 6573 756c 742c 2073 656c 662e 5f76 6572  esult, self._ver
+000067c0: 7369 6f6e 732e 7479 7065 290a 2020 2020  sions.type).    
+000067d0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+000067e0: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+000067f0: 2020 2020 2020 2020 2020 2020 2272 6563              "rec
+00006800: 6569 7665 6420 6669 6c65 2069 6e66 6f72  eived file infor
+00006810: 6d61 7469 6f6e 2066 6f72 2025 7322 2c20  mation for %s", 
+00006820: 6669 6c65 5f69 6e66 6f2e 6e61 6d65 290a  file_info.name).
+00006830: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00006840: 726e 2066 696c 655f 696e 666f 0a0a 2020  rn file_info..  
+00006850: 2020 2020 2020 6966 2073 656c 662e 6c61        if self.la
+00006860: 7374 5f65 7272 6f72 2e65 5f63 6f64 6520  st_error.e_code 
+00006870: 3d3d 206c 632e 4c53 5632 5374 6174 7573  == lc.LSV2Status
+00006880: 436f 6465 2e54 5f45 525f 4e4f 5f46 494c  Code.T_ER_NO_FIL
+00006890: 453a 0a20 2020 2020 2020 2020 2020 2073  E:.            s
+000068a0: 656c 662e 5f6c 6f67 6765 722e 6465 6275  elf._logger.debu
+000068b0: 6728 2266 696c 6520 646f 6573 206e 6f74  g("file does not
+000068c0: 2065 7869 7374 2229 0a20 2020 2020 2020   exist").       
+000068d0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000068e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000068f0: 6c6f 6767 6572 2e65 7272 6f72 280a 2020  logger.error(.  
+00006900: 2020 2020 2020 2020 2020 2261 6e20 6572            "an er
+00006910: 726f 7220 6f63 6375 7272 6564 2077 6869  ror occurred whi
+00006920: 6c65 2071 7565 7279 696e 6720 6669 6c65  le querying file
+00006930: 2069 6e66 6f20 666f 7220 2573 203a 2027   info for %s : '
+00006940: 2573 2722 2c0a 2020 2020 2020 2020 2020  %s'",.          
+00006950: 2020 7265 6d6f 7465 5f66 696c 655f 7061    remote_file_pa
+00006960: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00006970: 6c74 2e67 6574 5f65 7272 6f72 5f74 6578  lt.get_error_tex
+00006980: 7428 7365 6c66 2e6c 6173 745f 6572 726f  t(self.last_erro
+00006990: 7229 2c0a 2020 2020 2020 2020 290a 2020  r),.        ).  
+000069a0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+000069b0: 650a 0a20 2020 2064 6566 2064 6972 6563  e..    def direc
+000069c0: 746f 7279 5f63 6f6e 7465 6e74 2873 656c  tory_content(sel
+000069d0: 6629 202d 3e20 4c69 7374 5b6c 642e 4669  f) -> List[ld.Fi
+000069e0: 6c65 456e 7472 795d 3a0a 2020 2020 2020  leEntry]:.      
+000069f0: 2020 2222 220a 2020 2020 2020 2020 5175    """.        Qu
+00006a00: 6572 7920 636f 6e74 656e 7420 6f66 2063  ery content of c
+00006a10: 7572 7265 6e74 2077 6f72 6b69 6e67 2064  urrent working d
+00006a20: 6972 6563 746f 7279 2066 726f 6d20 7468  irectory from th
+00006a30: 6520 636f 6e74 726f 6c2e 2049 6e20 736f  e control. In so
+00006a40: 6d65 2073 6974 7561 7469 6f6e 7320 6974  me situations it
+00006a50: 2069 7320 6e65 6365 7373 6172 7920 746f   is necessary to
+00006a60: 0a20 2020 2020 2020 2066 6973 7420 6361  .        fist ca
+00006a70: 6c6c 203a 7079 3a66 756e 633a 607e 7079  ll :py:func:`~py
+00006a80: 4c53 5632 2e4c 5356 322e 6469 7265 6374  LSV2.LSV2.direct
+00006a90: 6f72 795f 696e 666f 6020 6f72 2065 6c73  ory_info` or els
+00006aa0: 6520 7468 6520 6174 7472 6962 7574 6573  e the attributes
+00006ab0: 2077 6f6e 2774 2062 6520 636f 7272 6563   won't be correc
+00006ac0: 742e 0a20 2020 2020 2020 2052 6571 7569  t..        Requi
+00006ad0: 7265 7320 6163 6365 7373 206c 6576 656c  res access level
+00006ae0: 2060 6046 494c 4554 5241 4e53 4645 5260   ``FILETRANSFER`
+00006af0: 6020 746f 2077 6f72 6b2e 0a20 2020 2020  ` to work..     
+00006b00: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00006b10: 6966 206e 6f74 2073 656c 662e 6c6f 6769  if not self.logi
+00006b20: 6e28 6c63 2e4c 6f67 696e 2e46 494c 4554  n(lc.Login.FILET
+00006b30: 5241 4e53 4645 5229 3a0a 2020 2020 2020  RANSFER):.      
+00006b40: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+00006b50: 6572 2e77 6172 6e69 6e67 2822 636f 756c  er.warning("coul
+00006b60: 6420 6e6f 7420 6c6f 6720 696e 2061 7320  d not log in as 
+00006b70: 7573 6572 2046 494c 4522 290a 2020 2020  user FILE").    
+00006b80: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+00006b90: 5d0a 0a20 2020 2020 2020 2064 6972 5f63  ]..        dir_c
+00006ba0: 6f6e 7465 6e74 203d 205b 5d0a 2020 2020  ontent = [].    
+00006bb0: 2020 2020 7061 796c 6f61 6420 3d20 6279      payload = by
+00006bc0: 7465 6172 7261 7928 7374 7275 6374 2e70  tearray(struct.p
+00006bd0: 6163 6b28 2221 4222 2c20 6c63 2e50 6172  ack("!B", lc.Par
+00006be0: 5244 522e 5349 4e47 4c45 2929 0a0a 2020  RDR.SINGLE))..  
+00006bf0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00006c00: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
+00006c10: 5f62 6c6f 636b 286c 632e 434d 442e 525f  _block(lc.CMD.R_
+00006c20: 4452 2c20 7061 796c 6f61 642c 206c 632e  DR, payload, lc.
+00006c30: 5253 502e 535f 4452 290a 2020 2020 2020  RSP.S_DR).      
+00006c40: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00006c50: 7265 7375 6c74 2c20 286c 6973 742c 2929  result, (list,))
+00006c60: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00006c70: 7220 656e 7472 7920 696e 2072 6573 756c  r entry in resul
+00006c80: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00006c90: 2020 2064 6972 5f63 6f6e 7465 6e74 2e61     dir_content.a
+00006ca0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
+00006cb0: 2020 2020 2020 2020 2020 206c 6d2e 6465             lm.de
+00006cc0: 636f 6465 5f66 696c 655f 7379 7374 656d  code_file_system
+00006cd0: 5f69 6e66 6f28 656e 7472 792c 2073 656c  _info(entry, sel
+00006ce0: 662e 5f76 6572 7369 6f6e 732e 7479 7065  f._versions.type
+00006cf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006d00: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00006d10: 2073 656c 662e 5f6c 6f67 6765 722e 6465   self._logger.de
+00006d20: 6275 6728 0a20 2020 2020 2020 2020 2020  bug(.           
+00006d30: 2020 2020 2022 7265 6365 6976 6564 2025       "received %
+00006d40: 6420 7061 636b 6167 6573 2066 6f72 2064  d packages for d
+00006d50: 6972 6563 746f 7279 2063 6f6e 7465 6e74  irectory content
+00006d60: 222c 206c 656e 2864 6972 5f63 6f6e 7465  ", len(dir_conte
+00006d70: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+00006d80: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00006d90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006da0: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
+00006db0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00006dc0: 2020 2261 6e20 6572 726f 7220 6f63 6375    "an error occu
+00006dd0: 7272 6564 2077 6869 6c65 2064 6972 6563  rred while direc
+00006de0: 746f 7279 2063 6f6e 7465 6e74 2069 6e66  tory content inf
+00006df0: 6f3a 2027 2573 2722 2c0a 2020 2020 2020  o: '%s'",.      
+00006e00: 2020 2020 2020 2020 2020 6c74 2e67 6574            lt.get
+00006e10: 5f65 7272 6f72 5f74 6578 7428 7365 6c66  _error_text(self
+00006e20: 2e6c 6173 745f 6572 726f 7229 2c0a 2020  .last_error),.  
+00006e30: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00006e40: 2020 2020 7265 7475 726e 2064 6972 5f63      return dir_c
+00006e50: 6f6e 7465 6e74 0a0a 2020 2020 6465 6620  ontent..    def 
+00006e60: 6472 6976 655f 696e 666f 2873 656c 6629  drive_info(self)
+00006e70: 202d 3e20 4c69 7374 5b6c 642e 4472 6976   -> List[ld.Driv
+00006e80: 6545 6e74 7279 5d3a 0a20 2020 2020 2020  eEntry]:.       
+00006e90: 2022 2222 0a20 2020 2020 2020 2052 6561   """.        Rea
+00006ea0: 6420 696e 666f 2061 6c6c 2064 7269 7665  d info all drive
+00006eb0: 7320 616e 6420 7061 7274 6974 696f 6e73  s and partitions
+00006ec0: 2066 726f 6d20 7468 6520 636f 6e74 726f   from the contro
+00006ed0: 6c2e 0a20 2020 2020 2020 2052 6571 7569  l..        Requi
+00006ee0: 7265 7320 6163 6365 7373 206c 6576 656c  res access level
+00006ef0: 2060 6046 494c 4554 5241 4e53 4645 5260   ``FILETRANSFER`
+00006f00: 6020 746f 2077 6f72 6b2e 0a20 2020 2020  ` to work..     
+00006f10: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00006f20: 6966 206e 6f74 2073 656c 662e 6c6f 6769  if not self.logi
+00006f30: 6e28 6c63 2e4c 6f67 696e 2e46 494c 4554  n(lc.Login.FILET
+00006f40: 5241 4e53 4645 5229 3a0a 2020 2020 2020  RANSFER):.      
+00006f50: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+00006f60: 6572 2e77 6172 6e69 6e67 2822 636f 756c  er.warning("coul
+00006f70: 6420 6e6f 7420 6c6f 6720 696e 2061 7320  d not log in as 
+00006f80: 7573 6572 2046 494c 4522 290a 2020 2020  user FILE").    
+00006f90: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+00006fa0: 5d0a 0a20 2020 2020 2020 2064 7269 7665  ]..        drive
+00006fb0: 735f 6c69 7374 203d 205b 5d0a 2020 2020  s_list = [].    
+00006fc0: 2020 2020 7061 796c 6f61 6420 3d20 6279      payload = by
+00006fd0: 7465 6172 7261 7928 7374 7275 6374 2e70  tearray(struct.p
+00006fe0: 6163 6b28 2221 4222 2c20 6c63 2e50 6172  ack("!B", lc.Par
+00006ff0: 5244 522e 4452 4956 4553 2929 0a20 2020  RDR.DRIVES)).   
+00007000: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00007010: 6c66 2e5f 7365 6e64 5f72 6563 6976 655f  lf._send_recive_
+00007020: 626c 6f63 6b28 6c63 2e43 4d44 2e52 5f44  block(lc.CMD.R_D
+00007030: 522c 2070 6179 6c6f 6164 2c20 6c63 2e52  R, payload, lc.R
+00007040: 5350 2e53 5f44 5229 0a20 2020 2020 2020  SP.S_DR).       
+00007050: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+00007060: 6573 756c 742c 2028 6c69 7374 2c29 293a  esult, (list,)):
+00007070: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00007080: 2065 6e74 7279 2069 6e20 7265 7375 6c74   entry in result
+00007090: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000070a0: 2020 6472 6976 6573 5f6c 6973 742e 6578    drives_list.ex
+000070b0: 7465 6e64 286c 6d2e 6465 636f 6465 5f64  tend(lm.decode_d
+000070c0: 7269 7665 5f69 6e66 6f28 656e 7472 7929  rive_info(entry)
+000070d0: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+000070e0: 656c 662e 5f6c 6f67 6765 722e 6465 6275  elf._logger.debu
+000070f0: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+00007100: 2020 2022 7375 6363 6573 7366 756c 6c79     "successfully
+00007110: 2072 6563 6569 7665 6420 2564 2070 6163   received %d pac
+00007120: 6b61 6765 7320 666f 7220 6472 6976 6520  kages for drive 
+00007130: 696e 666f 726d 6174 696f 6e20 2573 222c  information %s",
+00007140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007150: 206c 656e 2872 6573 756c 7429 2c0a 2020   len(result),.  
+00007160: 2020 2020 2020 2020 2020 2020 2020 6472                dr
+00007170: 6976 6573 5f6c 6973 742c 0a20 2020 2020  ives_list,.     
+00007180: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00007190: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000071a0: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+000071b0: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+000071c0: 2020 2020 2020 2020 2022 616e 2065 7272           "an err
+000071d0: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
+000071e0: 6520 7265 6164 696e 6720 6472 6976 6520  e reading drive 
+000071f0: 696e 666f 3a20 2725 7327 222c 0a20 2020  info: '%s'",.   
+00007200: 2020 2020 2020 2020 2020 2020 206c 742e               lt.
+00007210: 6765 745f 6572 726f 725f 7465 7874 2873  get_error_text(s
+00007220: 656c 662e 6c61 7374 5f65 7272 6f72 292c  elf.last_error),
+00007230: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00007240: 2020 2020 2020 2072 6574 7572 6e20 6472         return dr
+00007250: 6976 6573 5f6c 6973 740a 0a20 2020 2064  ives_list..    d
+00007260: 6566 206d 616b 655f 6469 7265 6374 6f72  ef make_director
+00007270: 7928 7365 6c66 2c20 6469 725f 7061 7468  y(self, dir_path
+00007280: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
+00007290: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000072a0: 2020 2020 4372 6561 7465 2061 2064 6972      Create a dir
+000072b0: 6563 746f 7279 206f 6e20 636f 6e74 726f  ectory on contro
+000072c0: 6c2e 2049 6620 6e65 6365 7373 6172 7920  l. If necessary 
+000072d0: 616c 736f 2063 7265 6174 6573 2070 6172  also creates par
+000072e0: 656e 7420 6469 7265 6374 6f72 6965 732e  ent directories.
+000072f0: 0a20 2020 2020 2020 2052 6571 7569 7265  .        Require
+00007300: 7320 6163 6365 7373 206c 6576 656c 2060  s access level `
+00007310: 6046 494c 4554 5241 4e53 4645 5260 6020  `FILETRANSFER`` 
+00007320: 746f 2077 6f72 6b2e 0a20 2020 2020 2020  to work..       
+00007330: 2052 6574 7572 6e73 2060 6054 7275 6560   Returns ``True`
+00007340: 6020 6966 2063 6f6d 706c 6574 6564 2073  ` if completed s
+00007350: 7563 6365 7373 6675 6c6c 792e 0a0a 2020  uccessfully...  
+00007360: 2020 2020 2020 3a70 6172 616d 2064 6972        :param dir
+00007370: 5f70 6174 683a 2070 6174 6820 6f66 2064  _path: path of d
+00007380: 6972 6563 746f 7279 206f 6e20 7468 6520  irectory on the 
+00007390: 636f 6e74 726f 6c0a 2020 2020 2020 2020  control.        
+000073a0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+000073b0: 6f74 2073 656c 662e 6c6f 6769 6e28 6c63  ot self.login(lc
+000073c0: 2e4c 6f67 696e 2e46 494c 4554 5241 4e53  .Login.FILETRANS
+000073d0: 4645 5229 3a0a 2020 2020 2020 2020 2020  FER):.          
+000073e0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e77    self._logger.w
+000073f0: 6172 6e69 6e67 2822 636f 756c 6420 6e6f  arning("could no
+00007400: 7420 6c6f 6720 696e 2061 7320 7573 6572  t log in as user
+00007410: 2046 494c 4522 290a 2020 2020 2020 2020   FILE").        
+00007420: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00007430: 0a0a 2020 2020 2020 2020 7061 7468 5f70  ..        path_p
+00007440: 6172 7473 203d 2064 6972 5f70 6174 682e  arts = dir_path.
+00007450: 7265 706c 6163 6528 222f 222c 206c 632e  replace("/", lc.
+00007460: 5041 5448 5f53 4550 292e 7370 6c69 7428  PATH_SEP).split(
+00007470: 0a20 2020 2020 2020 2020 2020 206c 632e  .            lc.
+00007480: 5041 5448 5f53 4550 0a20 2020 2020 2020  PATH_SEP.       
+00007490: 2029 2020 2320 636f 6e76 6572 7420 7061   )  # convert pa
+000074a0: 7468 0a20 2020 2020 2020 2070 6174 685f  th.        path_
+000074b0: 746f 5f63 6865 636b 203d 2022 220a 0a20  to_check = "".. 
+000074c0: 2020 2020 2020 2066 6f72 2070 6172 7420         for part 
+000074d0: 696e 2070 6174 685f 7061 7274 733a 0a20  in path_parts:. 
+000074e0: 2020 2020 2020 2020 2020 2070 6174 685f             path_
+000074f0: 746f 5f63 6865 636b 202b 3d20 7061 7274  to_check += part
+00007500: 202b 206c 632e 5041 5448 5f53 4550 0a20   + lc.PATH_SEP. 
+00007510: 2020 2020 2020 2020 2020 2023 206e 6f20             # no 
+00007520: 6669 6c65 2069 6e66 6f20 2d3e 2064 6f65  file info -> doe
+00007530: 7320 6e6f 7420 6578 6973 7420 616e 6420  s not exist and 
+00007540: 6861 7320 746f 2062 6520 6372 6561 7465  has to be create
+00007550: 640a 2020 2020 2020 2020 2020 2020 6966  d.            if
+00007560: 2073 656c 662e 6669 6c65 5f69 6e66 6f28   self.file_info(
+00007570: 7061 7468 5f74 6f5f 6368 6563 6b29 2069  path_to_check) i
+00007580: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00007590: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
+000075a0: 3d20 6c6d 2e75 7374 725f 746f 5f62 6128  = lm.ustr_to_ba(
+000075b0: 7061 7468 5f74 6f5f 6368 6563 6b29 0a0a  path_to_check)..
 000075c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075d0: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-000075e0: 2e64 6562 7567 2822 4469 7265 6374 6f72  .debug("Director
-000075f0: 7920 6372 6561 7465 6420 7375 6363 6573  y created succes
-00007600: 7366 756c 6c79 2229 0a20 2020 2020 2020  sfully").       
-00007610: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007630: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
-00007640: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
-00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2022 616e 2065 7272 6f72 206f 6363 7572   "an error occur
-00007670: 7265 6420 7768 696c 6520 6372 6561 7469  red while creati
-00007680: 6e67 2064 6972 6563 746f 7279 2025 733a  ng directory %s:
-00007690: 2027 2573 2722 2c0a 2020 2020 2020 2020   '%s'",.        
-000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076b0: 6469 725f 7061 7468 2c0a 2020 2020 2020  dir_path,.      
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 6c74 2e67 6574 5f65 7272 6f72 5f74    lt.get_error_t
-000076e0: 6578 7428 7365 6c66 2e6c 6173 745f 6572  ext(self.last_er
-000076f0: 726f 7229 2c0a 2020 2020 2020 2020 2020  ror),.          
-00007700: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007720: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00007730: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00007740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007750: 656c 662e 5f6c 6f67 6765 722e 6465 6275  elf._logger.debu
-00007760: 6728 226e 6f74 6869 6e67 2074 6f20 646f  g("nothing to do
-00007770: 2061 7320 7468 6973 2073 6567 6d65 6e74   as this segment
-00007780: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
-00007790: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000077a0: 2054 7275 650a 0a20 2020 2064 6566 2064   True..    def d
-000077b0: 656c 6574 655f 656d 7074 795f 6469 7265  elete_empty_dire
-000077c0: 6374 6f72 7928 7365 6c66 2c20 6469 725f  ctory(self, dir_
-000077d0: 7061 7468 3a20 7374 7229 202d 3e20 626f  path: str) -> bo
-000077e0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-000077f0: 2020 2020 2020 2020 4465 6c65 7465 2065          Delete e
-00007800: 6d70 7479 2064 6972 6563 746f 7279 206f  mpty directory o
-00007810: 6e20 636f 6e74 726f 6c2e 0a20 2020 2020  n control..     
-00007820: 2020 2052 6571 7569 7265 7320 6163 6365     Requires acce
-00007830: 7373 206c 6576 656c 2060 6046 494c 4554  ss level ``FILET
-00007840: 5241 4e53 4645 5260 6020 746f 2077 6f72  RANSFER`` to wor
-00007850: 6b2e 0a20 2020 2020 2020 2052 6574 7572  k..        Retur
-00007860: 6e73 2060 6054 7275 6560 6020 6966 2063  ns ``True`` if c
-00007870: 6f6d 706c 6574 6564 2073 7563 6365 7373  ompleted success
-00007880: 6675 6c6c 792e 0a0a 2020 2020 2020 2020  fully...        
-00007890: 3a70 6172 616d 2066 696c 655f 7061 7468  :param file_path
-000078a0: 3a20 7061 7468 206f 6620 6469 7265 6374  : path of direct
-000078b0: 6f72 7920 6f6e 2074 6865 2063 6f6e 7472  ory on the contr
-000078c0: 6f6c 0a20 2020 2020 2020 2022 2222 0a20  ol.        """. 
-000078d0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-000078e0: 6c66 2e6c 6f67 696e 286c 632e 4c6f 6769  lf.login(lc.Logi
-000078f0: 6e2e 4649 4c45 5452 414e 5346 4552 293a  n.FILETRANSFER):
-00007900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007910: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
-00007920: 6728 2263 6f75 6c64 206e 6f74 206c 6f67  g("could not log
-00007930: 2069 6e20 6173 2075 7365 7220 4649 4c45   in as user FILE
-00007940: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00007950: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00007960: 2020 2020 2064 6972 5f70 6174 6820 3d20       dir_path = 
-00007970: 6469 725f 7061 7468 2e72 6570 6c61 6365  dir_path.replace
-00007980: 2822 2f22 2c20 6c63 2e50 4154 485f 5345  ("/", lc.PATH_SE
-00007990: 5029 0a20 2020 2020 2020 2070 6179 6c6f  P).        paylo
-000079a0: 6164 203d 206c 6d2e 7573 7472 5f74 6f5f  ad = lm.ustr_to_
-000079b0: 6261 2864 6972 5f70 6174 6829 0a0a 2020  ba(dir_path)..  
-000079c0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-000079d0: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
-000079e0: 286c 632e 434d 442e 435f 4444 2c20 7061  (lc.CMD.C_DD, pa
-000079f0: 796c 6f61 642c 206c 632e 5253 502e 545f  yload, lc.RSP.T_
-00007a00: 4f4b 290a 2020 2020 2020 2020 6966 2069  OK).        if i
-00007a10: 7369 6e73 7461 6e63 6528 7265 7375 6c74  sinstance(result
-00007a20: 2c20 2862 6f6f 6c29 2920 616e 6420 7265  , (bool)) and re
-00007a30: 7375 6c74 2069 7320 5472 7565 3a0a 2020  sult is True:.  
-00007a40: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007a50: 6c6f 6767 6572 2e64 6562 7567 2822 7375  logger.debug("su
-00007a60: 6363 6573 7366 756c 6c79 2064 656c 6574  ccessfully delet
-00007a70: 6564 2064 6972 6563 746f 7279 2025 7322  ed directory %s"
-00007a80: 2c20 6469 725f 7061 7468 290a 2020 2020  , dir_path).    
-00007a90: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00007aa0: 7275 650a 0a20 2020 2020 2020 2069 6620  rue..        if 
-00007ab0: 7365 6c66 2e6c 6173 745f 6572 726f 722e  self.last_error.
-00007ac0: 655f 636f 6465 203d 3d20 6c63 2e4c 5356  e_code == lc.LSV
-00007ad0: 3253 7461 7475 7343 6f64 652e 545f 4552  2StatusCode.T_ER
-00007ae0: 5f4e 4f5f 4449 523a 0a20 2020 2020 2020  _NO_DIR:.       
-00007af0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00007b00: 722e 6465 6275 6728 226e 6f74 696e 6720  r.debug("noting 
-00007b10: 746f 2064 6f2c 2064 6972 6563 746f 7279  to do, directory
-00007b20: 2025 7320 6469 646e 2774 2065 7869 7374   %s didn't exist
-00007b30: 222c 2064 6972 5f70 6174 6829 0a20 2020  ", dir_path).   
-00007b40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007b50: 5472 7565 0a0a 2020 2020 2020 2020 6966  True..        if
-00007b60: 2073 656c 662e 6c61 7374 5f65 7272 6f72   self.last_error
-00007b70: 2e65 5f63 6f64 6520 3d3d 206c 632e 4c53  .e_code == lc.LS
-00007b80: 5632 5374 6174 7573 436f 6465 2e54 5f45  V2StatusCode.T_E
-00007b90: 525f 4445 4c5f 4449 523a 0a20 2020 2020  R_DEL_DIR:.     
-00007ba0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-00007bb0: 6765 722e 6465 6275 6728 0a20 2020 2020  ger.debug(.     
-00007bc0: 2020 2020 2020 2020 2020 2022 636f 756c             "coul
-00007bd0: 6420 6e6f 7420 6465 6c65 7465 2064 6972  d not delete dir
-00007be0: 6563 746f 7279 2025 7320 7369 6e63 6520  ectory %s since 
-00007bf0: 6974 2069 7320 6e6f 7420 656d 7074 7922  it is not empty"
-00007c00: 2c20 6469 725f 7061 7468 0a20 2020 2020  , dir_path.     
-00007c10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00007c20: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00007c30: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00007c40: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
-00007c50: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
-00007c60: 2065 7272 6f72 206f 6363 7572 7265 6420   error occurred 
-00007c70: 7768 696c 6520 6465 6c65 7469 6e67 2064  while deleting d
-00007c80: 6972 6563 746f 7279 2025 7322 2c0a 2020  irectory %s",.  
-00007c90: 2020 2020 2020 2020 2020 6469 725f 7061            dir_pa
-00007ca0: 7468 2c0a 2020 2020 2020 2020 290a 2020  th,.        ).  
-00007cb0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00007cc0: 7365 0a0a 2020 2020 6465 6620 6465 6c65  se..    def dele
-00007cd0: 7465 5f66 696c 6528 7365 6c66 2c20 6669  te_file(self, fi
-00007ce0: 6c65 5f70 6174 683a 2073 7472 2920 2d3e  le_path: str) ->
-00007cf0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00007d00: 2222 0a20 2020 2020 2020 2044 656c 6574  "".        Delet
-00007d10: 6520 6669 6c65 206f 6e20 636f 6e74 726f  e file on contro
-00007d20: 6c2e 0a20 2020 2020 2020 2052 6571 7569  l..        Requi
-00007d30: 7265 7320 6163 6365 7373 206c 6576 656c  res access level
-00007d40: 2060 6046 494c 4554 5241 4e53 4645 5260   ``FILETRANSFER`
-00007d50: 6020 746f 2077 6f72 6b2e 0a20 2020 2020  ` to work..     
-00007d60: 2020 2052 6574 7572 6e73 2060 6054 7275     Returns ``Tru
-00007d70: 6560 6020 6966 2063 6f6d 706c 6574 6564  e`` if completed
-00007d80: 2073 7563 6365 7373 6675 6c6c 792e 0a0a   successfully...
-00007d90: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00007da0: 696c 655f 7061 7468 3a20 7061 7468 206f  ile_path: path o
-00007db0: 6620 6669 6c65 206f 6e20 7468 6520 636f  f file on the co
-00007dc0: 6e74 726f 6c0a 2020 2020 2020 2020 2222  ntrol.        ""
-00007dd0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00007de0: 2073 656c 662e 6c6f 6769 6e28 6c63 2e4c   self.login(lc.L
-00007df0: 6f67 696e 2e46 494c 4554 5241 4e53 4645  ogin.FILETRANSFE
-00007e00: 5229 3a0a 2020 2020 2020 2020 2020 2020  R):.            
-00007e10: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-00007e20: 6e69 6e67 2822 636f 756c 6420 6e6f 7420  ning("could not 
-00007e30: 6c6f 6720 696e 2061 7320 7573 6572 2046  log in as user F
-00007e40: 494c 4522 290a 2020 2020 2020 2020 2020  ILE").          
-00007e50: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00007e60: 2020 2020 2020 2020 6669 6c65 5f70 6174          file_pat
-00007e70: 6820 3d20 6669 6c65 5f70 6174 682e 7265  h = file_path.re
-00007e80: 706c 6163 6528 222f 222c 206c 632e 5041  place("/", lc.PA
-00007e90: 5448 5f53 4550 290a 2020 2020 2020 2020  TH_SEP).        
-00007ea0: 7061 796c 6f61 6420 3d20 6c6d 2e75 7374  payload = lm.ust
-00007eb0: 725f 746f 5f62 6128 6669 6c65 5f70 6174  r_to_ba(file_pat
-00007ec0: 6829 0a0a 2020 2020 2020 2020 6966 2073  h)..        if s
-00007ed0: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
-00007ee0: 286c 632e 434d 442e 435f 4644 2c20 7061  (lc.CMD.C_FD, pa
-00007ef0: 796c 6f61 642c 206c 632e 5253 502e 545f  yload, lc.RSP.T_
-00007f00: 4f4b 293a 0a20 2020 2020 2020 2020 2020  OK):.           
-00007f10: 2073 656c 662e 5f6c 6f67 6765 722e 6465   self._logger.de
-00007f20: 6275 6728 2273 7563 6365 7373 6675 6c6c  bug("successfull
-00007f30: 7920 6465 6c65 7465 6420 6669 6c65 2025  y deleted file %
-00007f40: 7322 2c20 6669 6c65 5f70 6174 6829 0a20  s", file_path). 
-00007f50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007f60: 6e20 5472 7565 0a0a 2020 2020 2020 2020  n True..        
-00007f70: 6966 2073 656c 662e 6c61 7374 5f65 7272  if self.last_err
-00007f80: 6f72 2e65 5f63 6f64 6520 3d3d 206c 632e  or.e_code == lc.
-00007f90: 4c53 5632 5374 6174 7573 436f 6465 2e54  LSV2StatusCode.T
-00007fa0: 5f45 525f 4e4f 5f46 494c 453a 0a20 2020  _ER_NO_FILE:.   
-00007fb0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00007fc0: 6f67 6765 722e 6465 6275 6728 226e 6f74  ogger.debug("not
-00007fd0: 696e 6720 746f 2064 6f2c 2066 696c 6520  ing to do, file 
-00007fe0: 2573 2064 6964 6e27 7420 6578 6973 7422  %s didn't exist"
-00007ff0: 2c20 6669 6c65 5f70 6174 6829 0a20 2020  , file_path).   
-00008000: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008010: 5472 7565 0a0a 2020 2020 2020 2020 6966  True..        if
-00008020: 2073 656c 662e 6c61 7374 5f65 7272 6f72   self.last_error
-00008030: 2e65 5f63 6f64 6520 3d3d 206c 632e 4c53  .e_code == lc.LS
-00008040: 5632 5374 6174 7573 436f 6465 2e54 5f45  V2StatusCode.T_E
-00008050: 525f 4e4f 5f44 454c 4554 453a 0a20 2020  R_NO_DELETE:.   
-00008060: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00008070: 6f67 6765 722e 696e 666f 2822 636f 756c  ogger.info("coul
-00008080: 6420 6e6f 7420 6465 6c65 7465 2066 696c  d not delete fil
-00008090: 6520 2573 2073 696e 6365 2069 7420 6973  e %s since it is
-000080a0: 2069 6e20 7573 6522 2c20 6669 6c65 5f70   in use", file_p
-000080b0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-000080c0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-000080d0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-000080e0: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
-000080f0: 2020 2020 2020 2020 2022 616e 2065 7272           "an err
-00008100: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
-00008110: 6520 6465 6c65 7469 6e67 2066 696c 6520  e deleting file 
-00008120: 2573 222c 0a20 2020 2020 2020 2020 2020  %s",.           
-00008130: 2066 696c 655f 7061 7468 2c0a 2020 2020   file_path,.    
-00008140: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-00008150: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-00008160: 6465 6620 636f 7079 5f72 656d 6f74 655f  def copy_remote_
-00008170: 6669 6c65 2873 656c 662c 2073 6f75 7263  file(self, sourc
-00008180: 655f 7061 7468 3a20 7374 722c 2074 6172  e_path: str, tar
-00008190: 6765 745f 7061 7468 3a20 7374 7229 202d  get_path: str) -
-000081a0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-000081b0: 2222 220a 2020 2020 2020 2020 436f 7079  """.        Copy
-000081c0: 2066 696c 6520 6f6e 2063 6f6e 7472 6f6c   file on control
-000081d0: 2066 726f 6d20 6f6e 6520 706c 6163 6520   from one place 
-000081e0: 746f 2061 6e6f 7468 6572 2e0a 2020 2020  to another..    
-000081f0: 2020 2020 5265 7175 6972 6573 2061 6363      Requires acc
-00008200: 6573 7320 6c65 7665 6c20 6060 4649 4c45  ess level ``FILE
-00008210: 5452 414e 5346 4552 6060 2074 6f20 776f  TRANSFER`` to wo
-00008220: 726b 2e0a 2020 2020 2020 2020 5265 7475  rk..        Retu
-00008230: 726e 7320 6060 5472 7565 6060 2069 6620  rns ``True`` if 
-00008240: 636f 6d70 6c65 7465 6420 7375 6363 6573  completed succes
-00008250: 7366 756c 6c79 2e0a 0a20 2020 2020 2020  sfully...       
-00008260: 203a 7061 7261 6d20 736f 7572 6365 5f70   :param source_p
-00008270: 6174 683a 2070 6174 6820 6f66 2066 696c  ath: path of fil
-00008280: 6520 6f6e 2074 6865 2063 6f6e 7472 6f6c  e on the control
-00008290: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000082a0: 7461 7267 6574 5f70 6174 683a 2070 6174  target_path: pat
-000082b0: 6820 6f66 2074 6172 6765 7420 6c6f 6361  h of target loca
-000082c0: 7469 6f6e 0a0a 2020 2020 2020 2020 3a72  tion..        :r
-000082d0: 6169 7365 7320 4c53 5632 5374 6174 6545  aises LSV2StateE
-000082e0: 7863 6570 7469 6f6e 3a20 6966 2074 6865  xception: if the
-000082f0: 2073 656c 6563 7465 6420 7061 7468 2063   selected path c
-00008300: 6f75 6c64 206e 6f74 2062 6520 666f 756e  ould not be foun
-00008310: 6420 6f72 0a20 2020 2020 2020 2020 2020  d or.           
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2020 2020 2074 6865 2070 6174           the pat
-00008340: 6820 6973 206e 6f74 2061 6363 6573 7369  h is not accessi
-00008350: 626c 650a 2020 2020 2020 2020 2222 220a  ble.        """.
-00008360: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00008370: 656c 662e 6c6f 6769 6e28 6c63 2e4c 6f67  elf.login(lc.Log
-00008380: 696e 2e46 494c 4554 5241 4e53 4645 5229  in.FILETRANSFER)
-00008390: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000083a0: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
-000083b0: 6e67 2822 636f 756c 6420 6e6f 7420 6c6f  ng("could not lo
-000083c0: 6720 696e 2061 7320 7573 6572 2046 494c  g in as user FIL
-000083d0: 4522 290a 2020 2020 2020 2020 2020 2020  E").            
-000083e0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-000083f0: 2020 2020 2020 736f 7572 6365 5f70 6174        source_pat
-00008400: 6820 3d20 736f 7572 6365 5f70 6174 682e  h = source_path.
-00008410: 7265 706c 6163 6528 222f 222c 206c 632e  replace("/", lc.
-00008420: 5041 5448 5f53 4550 290a 2020 2020 2020  PATH_SEP).      
-00008430: 2020 7461 7267 6574 5f70 6174 6820 3d20    target_path = 
-00008440: 7461 7267 6574 5f70 6174 682e 7265 706c  target_path.repl
-00008450: 6163 6528 222f 222c 206c 632e 5041 5448  ace("/", lc.PATH
-00008460: 5f53 4550 290a 0a20 2020 2020 2020 2069  _SEP)..        i
-00008470: 6620 6c63 2e50 4154 485f 5345 5020 696e  f lc.PATH_SEP in
-00008480: 2073 6f75 7263 655f 7061 7468 3a0a 2020   source_path:.  
-00008490: 2020 2020 2020 2020 2020 2320 6368 616e            # chan
-000084a0: 6765 2064 6972 6563 746f 7279 0a20 2020  ge directory.   
-000084b0: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
-000084c0: 6669 6c65 5f6e 616d 6520 3d20 736f 7572  file_name = sour
-000084d0: 6365 5f70 6174 682e 7370 6c69 7428 6c63  ce_path.split(lc
-000084e0: 2e50 4154 485f 5345 5029 5b2d 315d 0a20  .PATH_SEP)[-1]. 
-000084f0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-00008500: 655f 6469 7265 6374 6f72 7920 3d20 736f  e_directory = so
-00008510: 7572 6365 5f70 6174 682e 7273 7472 6970  urce_path.rstrip
-00008520: 2873 6f75 7263 655f 6669 6c65 5f6e 616d  (source_file_nam
-00008530: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
-00008540: 6620 6e6f 7420 7365 6c66 2e63 6861 6e67  f not self.chang
-00008550: 655f 6469 7265 6374 6f72 7928 7265 6d6f  e_directory(remo
-00008560: 7465 5f64 6972 6563 746f 7279 3d73 6f75  te_directory=sou
-00008570: 7263 655f 6469 7265 6374 6f72 7929 3a0a  rce_directory):.
-00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008590: 7261 6973 6520 4c53 5632 5374 6174 6545  raise LSV2StateE
-000085a0: 7863 6570 7469 6f6e 2822 636f 756c 6420  xception("could 
-000085b0: 6e6f 7420 6f70 656e 2074 6865 2073 6f75  not open the sou
-000085c0: 7263 6520 6469 7265 6374 6f72 7922 290a  rce directory").
-000085d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000085e0: 2020 2020 2020 2020 2020 736f 7572 6365            source
-000085f0: 5f66 696c 655f 6e61 6d65 203d 2073 6f75  _file_name = sou
-00008600: 7263 655f 7061 7468 0a20 2020 2020 2020  rce_path.       
-00008610: 2020 2020 2073 6f75 7263 655f 6469 7265       source_dire
-00008620: 6374 6f72 7920 3d20 222e 220a 0a20 2020  ctory = "."..   
-00008630: 2020 2020 2069 6620 7461 7267 6574 5f70       if target_p
-00008640: 6174 682e 656e 6473 7769 7468 286c 632e  ath.endswith(lc.
-00008650: 5041 5448 5f53 4550 293a 0a20 2020 2020  PATH_SEP):.     
-00008660: 2020 2020 2020 2074 6172 6765 745f 7061         target_pa
-00008670: 7468 202b 3d20 736f 7572 6365 5f66 696c  th += source_fil
-00008680: 655f 6e61 6d65 0a0a 2020 2020 2020 2020  e_name..        
-00008690: 7061 796c 6f61 6420 3d20 6c6d 2e75 7374  payload = lm.ust
-000086a0: 725f 746f 5f62 6128 736f 7572 6365 5f66  r_to_ba(source_f
-000086b0: 696c 655f 6e61 6d65 290a 2020 2020 2020  ile_name).      
-000086c0: 2020 7061 796c 6f61 642e 6578 7465 6e64    payload.extend
-000086d0: 286c 6d2e 7573 7472 5f74 6f5f 6261 2874  (lm.ustr_to_ba(t
-000086e0: 6172 6765 745f 7061 7468 2929 0a20 2020  arget_path)).   
-000086f0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00008700: 722e 6465 6275 6728 0a20 2020 2020 2020  r.debug(.       
-00008710: 2020 2020 2022 7072 6570 6172 6520 746f       "prepare to
-00008720: 2063 6f70 7920 6669 6c65 2025 7320 6672   copy file %s fr
-00008730: 6f6d 2025 7320 746f 2025 7322 2c0a 2020  om %s to %s",.  
-00008740: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00008750: 5f66 696c 655f 6e61 6d65 2c0a 2020 2020  _file_name,.    
-00008760: 2020 2020 2020 2020 736f 7572 6365 5f64          source_d
-00008770: 6972 6563 746f 7279 2c0a 2020 2020 2020  irectory,.      
-00008780: 2020 2020 2020 7461 7267 6574 5f70 6174        target_pat
-00008790: 682c 0a20 2020 2020 2020 2029 0a20 2020  h,.        ).   
-000087a0: 2020 2020 2069 6620 7365 6c66 2e5f 7365       if self._se
-000087b0: 6e64 5f72 6563 6976 6528 6c63 2e43 4d44  nd_recive(lc.CMD
-000087c0: 2e43 5f46 432c 2070 6179 6c6f 6164 2c20  .C_FC, payload, 
-000087d0: 6c63 2e52 5350 2e54 5f4f 4b29 3a0a 2020  lc.RSP.T_OK):.  
-000087e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000087f0: 6c6f 6767 6572 2e64 6562 7567 2822 7375  logger.debug("su
-00008800: 6363 6573 7366 756c 6c79 2063 6f70 6965  ccessfully copie
-00008810: 6420 6669 6c65 2025 7322 2c20 736f 7572  d file %s", sour
-00008820: 6365 5f70 6174 6829 0a20 2020 2020 2020  ce_path).       
-00008830: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00008840: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00008850: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
-00008860: 2020 2020 2020 2020 2020 2020 2261 6e20              "an 
-00008870: 6572 726f 7220 6f63 6375 7272 6564 2063  error occurred c
-00008880: 6f70 7969 6e67 2066 696c 6520 2573 2074  opying file %s t
-00008890: 6f20 2573 222c 2073 6f75 7263 655f 7061  o %s", source_pa
-000088a0: 7468 2c20 7461 7267 6574 5f70 6174 680a  th, target_path.
-000088b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000088c0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-000088d0: 2020 2020 6465 6620 6d6f 7665 5f66 696c      def move_fil
-000088e0: 6528 7365 6c66 2c20 736f 7572 6365 5f70  e(self, source_p
-000088f0: 6174 683a 2073 7472 2c20 7461 7267 6574  ath: str, target
-00008900: 5f70 6174 683a 2073 7472 2920 2d3e 2062  _path: str) -> b
-00008910: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00008920: 0a20 2020 2020 2020 204d 6f76 6520 6669  .        Move fi
-00008930: 6c65 206f 6e20 636f 6e74 726f 6c20 6672  le on control fr
-00008940: 6f6d 206f 6e65 2070 6c61 6365 2074 6f20  om one place to 
-00008950: 616e 6f74 6865 722e 0a20 2020 2020 2020  another..       
-00008960: 2052 6571 7569 7265 7320 6163 6365 7373   Requires access
-00008970: 206c 6576 656c 2060 6046 494c 4554 5241   level ``FILETRA
-00008980: 4e53 4645 5260 6020 746f 2077 6f72 6b2e  NSFER`` to work.
-00008990: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000089a0: 2060 6054 7275 6560 6020 6966 2063 7265   ``True`` if cre
-000089b0: 6174 696e 6720 6469 7265 6374 6f72 7920  ating directory 
-000089c0: 7761 7320 7375 6363 6573 7366 756c 2e0a  was successful..
-000089d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000089e0: 736f 7572 6365 5f70 6174 683a 2070 6174  source_path: pat
-000089f0: 6820 6f66 2066 696c 6520 6f6e 2074 6865  h of file on the
-00008a00: 2063 6f6e 7472 6f6c 0a20 2020 2020 2020   control.       
-00008a10: 203a 7061 7261 6d20 7461 7267 6574 5f70   :param target_p
-00008a20: 6174 683a 2070 6174 6820 6f66 2074 6172  ath: path of tar
-00008a30: 6765 7420 6c6f 6361 7469 6f6e 2077 6974  get location wit
-00008a40: 6820 6f72 2077 6974 686f 7574 2066 696c  h or without fil
-00008a50: 656e 616d 650a 0a20 2020 2020 2020 203a  ename..        :
-00008a60: 7261 6973 6573 204c 5356 3253 7461 7465  raises LSV2State
-00008a70: 4578 6365 7074 696f 6e3a 2069 6620 7468  Exception: if th
-00008a80: 6520 7365 6c65 6374 6564 2070 6174 6820  e selected path 
-00008a90: 636f 756c 6420 6e6f 7420 6265 2066 6f75  could not be fou
-00008aa0: 6e64 206f 720a 2020 2020 2020 2020 2020  nd or.          
-00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ac0: 2020 2020 2020 2020 2020 7468 6520 7061            the pa
-00008ad0: 7468 2069 7320 6e6f 7420 6163 6365 7373  th is not access
-00008ae0: 6962 6c65 0a20 2020 2020 2020 2022 2222  ible.        """
-00008af0: 0a20 2020 2020 2020 2073 6f75 7263 655f  .        source_
-00008b00: 7061 7468 203d 2073 6f75 7263 655f 7061  path = source_pa
-00008b10: 7468 2e72 6570 6c61 6365 2822 2f22 2c20  th.replace("/", 
-00008b20: 6c63 2e50 4154 485f 5345 5029 0a20 2020  lc.PATH_SEP).   
-00008b30: 2020 2020 2074 6172 6765 745f 7061 7468       target_path
-00008b40: 203d 2074 6172 6765 745f 7061 7468 2e72   = target_path.r
-00008b50: 6570 6c61 6365 2822 2f22 2c20 6c63 2e50  eplace("/", lc.P
-00008b60: 4154 485f 5345 5029 0a0a 2020 2020 2020  ATH_SEP)..      
-00008b70: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
-00008b80: 6769 6e28 6c63 2e4c 6f67 696e 2e46 494c  gin(lc.Login.FIL
-00008b90: 4554 5241 4e53 4645 5229 3a0a 2020 2020  ETRANSFER):.    
-00008ba0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00008bb0: 6767 6572 2e77 6172 6e69 6e67 2822 636f  gger.warning("co
-00008bc0: 756c 6420 6e6f 7420 6c6f 6720 696e 2061  uld not log in a
-00008bd0: 7320 7573 6572 2046 494c 4522 290a 2020  s user FILE").  
-00008be0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008bf0: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-00008c00: 6966 206c 632e 5041 5448 5f53 4550 2069  if lc.PATH_SEP i
-00008c10: 6e20 736f 7572 6365 5f70 6174 683a 0a20  n source_path:. 
-00008c20: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-00008c30: 655f 6669 6c65 5f6e 616d 6520 3d20 736f  e_file_name = so
-00008c40: 7572 6365 5f70 6174 682e 7370 6c69 7428  urce_path.split(
-00008c50: 6c63 2e50 4154 485f 5345 5029 5b2d 315d  lc.PATH_SEP)[-1]
-00008c60: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-00008c70: 7263 655f 6469 7265 6374 6f72 7920 3d20  rce_directory = 
-00008c80: 736f 7572 6365 5f70 6174 682e 7273 7472  source_path.rstr
-00008c90: 6970 2873 6f75 7263 655f 6669 6c65 5f6e  ip(source_file_n
-00008ca0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00008cb0: 2069 6620 6e6f 7420 7365 6c66 2e63 6861   if not self.cha
-00008cc0: 6e67 655f 6469 7265 6374 6f72 7928 7265  nge_directory(re
-00008cd0: 6d6f 7465 5f64 6972 6563 746f 7279 3d73  mote_directory=s
-00008ce0: 6f75 7263 655f 6469 7265 6374 6f72 7929  ource_directory)
-00008cf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008d00: 2020 7261 6973 6520 4c53 5632 5374 6174    raise LSV2Stat
-00008d10: 6545 7863 6570 7469 6f6e 2822 636f 756c  eException("coul
-00008d20: 6420 6e6f 7420 6f70 656e 2074 6865 2073  d not open the s
-00008d30: 6f75 7263 6520 6469 7265 6374 6f72 7922  ource directory"
-00008d40: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00008d50: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00008d60: 6365 5f66 696c 655f 6e61 6d65 203d 2073  ce_file_name = s
-00008d70: 6f75 7263 655f 7061 7468 0a20 2020 2020  ource_path.     
-00008d80: 2020 2020 2020 2073 6f75 7263 655f 6469         source_di
-00008d90: 7265 6374 6f72 7920 3d20 222e 220a 0a20  rectory = ".".. 
-00008da0: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00008db0: 5f70 6174 682e 656e 6473 7769 7468 286c  _path.endswith(l
-00008dc0: 632e 5041 5448 5f53 4550 293a 0a20 2020  c.PATH_SEP):.   
-00008dd0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00008de0: 7061 7468 202b 3d20 736f 7572 6365 5f66  path += source_f
-00008df0: 696c 655f 6e61 6d65 0a0a 2020 2020 2020  ile_name..      
-00008e00: 2020 7061 796c 6f61 6420 3d20 6c6d 2e75    payload = lm.u
-00008e10: 7374 725f 746f 5f62 6128 736f 7572 6365  str_to_ba(source
-00008e20: 5f66 696c 655f 6e61 6d65 290a 2020 2020  _file_name).    
-00008e30: 2020 2020 7061 796c 6f61 642e 6578 7465      payload.exte
-00008e40: 6e64 286c 6d2e 7573 7472 5f74 6f5f 6261  nd(lm.ustr_to_ba
-00008e50: 2874 6172 6765 745f 7061 7468 2929 0a0a  (target_path))..
-00008e60: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00008e70: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-00008e80: 2020 2020 2020 2020 2270 7265 7061 7265          "prepare
-00008e90: 2074 6f20 6d6f 7665 2066 696c 6520 2573   to move file %s
-00008ea0: 2066 726f 6d20 2573 2074 6f20 2573 222c   from %s to %s",
-00008eb0: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-00008ec0: 7263 655f 6669 6c65 5f6e 616d 652c 0a20  rce_file_name,. 
-00008ed0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-00008ee0: 655f 6469 7265 6374 6f72 792c 0a20 2020  e_directory,.   
-00008ef0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00008f00: 7061 7468 2c0a 2020 2020 2020 2020 290a  path,.        ).
-00008f10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008f20: 5f73 656e 645f 7265 6369 7665 286c 632e  _send_recive(lc.
-00008f30: 434d 442e 435f 4652 2c20 7061 796c 6f61  CMD.C_FR, payloa
-00008f40: 642c 206c 632e 5253 502e 545f 4f4b 293a  d, lc.RSP.T_OK):
-00008f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008f60: 662e 5f6c 6f67 6765 722e 6465 6275 6728  f._logger.debug(
-00008f70: 2273 7563 6365 7373 6675 6c6c 7920 6d6f  "successfully mo
-00008f80: 7665 6420 6669 6c65 2025 7322 2c20 736f  ved file %s", so
-00008f90: 7572 6365 5f70 6174 6829 0a20 2020 2020  urce_path).     
-00008fa0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00008fb0: 7565 0a0a 2020 2020 2020 2020 6966 2073  ue..        if s
-00008fc0: 656c 662e 6c61 7374 5f65 7272 6f72 2e65  elf.last_error.e
-00008fd0: 5f63 6f64 6520 3d3d 206c 632e 4c53 5632  _code == lc.LSV2
-00008fe0: 5374 6174 7573 436f 6465 2e54 5f45 525f  StatusCode.T_ER_
-00008ff0: 4649 4c45 5f45 5849 5354 533a 0a20 2020  FILE_EXISTS:.   
-00009000: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00009010: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
-00009020: 2020 2020 2020 2020 2020 2020 2263 6f75              "cou
-00009030: 6c64 206e 6f74 206d 6f76 6520 6669 6c65  ld not move file
-00009040: 2025 7320 746f 2025 7320 7369 6e63 6520   %s to %s since 
-00009050: 616c 7265 6164 7920 6578 6973 7473 222c  already exists",
-00009060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009070: 2073 6f75 7263 655f 7061 7468 2c0a 2020   source_path,.  
-00009080: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00009090: 7267 6574 5f70 6174 682c 0a20 2020 2020  rget_path,.     
-000090a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000090b0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000090c0: 650a 0a20 2020 2020 2020 2069 6620 7365  e..        if se
-000090d0: 6c66 2e6c 6173 745f 6572 726f 722e 655f  lf.last_error.e_
-000090e0: 636f 6465 203d 3d20 6c63 2e4c 5356 3253  code == lc.LSV2S
-000090f0: 7461 7475 7343 6f64 652e 545f 4552 5f4e  tatusCode.T_ER_N
-00009100: 4f5f 4649 4c45 3a0a 2020 2020 2020 2020  O_FILE:.        
-00009110: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-00009120: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-00009130: 2020 2020 2020 2022 636f 756c 6420 6e6f         "could no
-00009140: 7420 6d6f 7665 2066 696c 6520 7369 6e63  t move file sinc
-00009150: 6520 6569 7468 6572 2073 6f75 7263 6520  e either source 
-00009160: 6f72 2074 6172 6765 7420 7061 7468 2064  or target path d
-00009170: 6f65 7320 6e6f 7420 6578 6973 7422 2c0a  oes not exist",.
-00009180: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00009190: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000091a0: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-000091b0: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-000091c0: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
-000091d0: 2020 2261 6e20 6572 726f 7220 6f63 6375    "an error occu
-000091e0: 7272 6564 206d 6f76 696e 6720 6669 6c65  rred moving file
-000091f0: 2025 7320 746f 2025 7322 2c20 736f 7572   %s to %s", sour
-00009200: 6365 5f70 6174 682c 2074 6172 6765 745f  ce_path, target_
-00009210: 7061 7468 0a20 2020 2020 2020 2029 0a20  path.        ). 
-00009220: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00009230: 6c73 650a 0a20 2020 2064 6566 2073 656e  lse..    def sen
-00009240: 645f 6669 6c65 280a 2020 2020 2020 2020  d_file(.        
-00009250: 7365 6c66 2c0a 2020 2020 2020 2020 6c6f  self,.        lo
-00009260: 6361 6c5f 7061 7468 3a20 556e 696f 6e5b  cal_path: Union[
-00009270: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
-00009280: 685d 2c0a 2020 2020 2020 2020 7265 6d6f  h],.        remo
-00009290: 7465 5f70 6174 683a 2073 7472 2c0a 2020  te_path: str,.  
-000092a0: 2020 2020 2020 6f76 6572 7269 6465 5f66        override_f
-000092b0: 696c 653a 2062 6f6f 6c20 3d20 4661 6c73  ile: bool = Fals
-000092c0: 652c 0a20 2020 2020 2020 2062 696e 6172  e,.        binar
-000092d0: 795f 6d6f 6465 3a20 626f 6f6c 203d 2046  y_mode: bool = F
-000092e0: 616c 7365 2c0a 2020 2020 2920 2d3e 2062  alse,.    ) -> b
-000092f0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00009300: 0a20 2020 2020 2020 2055 706c 6f61 6420  .        Upload 
-00009310: 6120 6669 6c65 2074 6f20 636f 6e74 726f  a file to contro
-00009320: 6c0a 2020 2020 2020 2020 5265 7175 6972  l.        Requir
-00009330: 6573 2061 6363 6573 7320 6c65 7665 6c20  es access level 
-00009340: 6060 4649 4c45 5452 414e 5346 4552 6060  ``FILETRANSFER``
-00009350: 2074 6f20 776f 726b 2e0a 2020 2020 2020   to work..      
-00009360: 2020 5265 7475 726e 7320 6060 5472 7565    Returns ``True
-00009370: 6060 2069 6620 636f 6d70 6c65 7465 6420  `` if completed 
-00009380: 7375 6363 6573 7366 756c 6c79 2e0a 0a20  successfully... 
-00009390: 2020 2020 2020 203a 7061 7261 6d20 6c6f         :param lo
-000093a0: 6361 6c5f 7061 7468 3a20 7061 7468 206f  cal_path: path o
-000093b0: 6620 6669 6c65 2074 6f20 6265 2073 656e  f file to be sen
-000093c0: 7420 746f 2074 6865 2063 6f6e 7472 6f6c  t to the control
-000093d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000093e0: 7265 6d6f 7465 5f70 6174 683a 2070 6174  remote_path: pat
-000093f0: 6820 7769 7468 206f 7220 7769 7468 6f75  h with or withou
-00009400: 7420 7468 6520 6669 6c65 206e 616d 6520  t the file name 
-00009410: 6f6e 2074 6865 2063 6f6e 7472 6f6c 0a20  on the control. 
-00009420: 2020 2020 2020 203a 7061 7261 6d20 6f76         :param ov
-00009430: 6572 7269 6465 5f66 696c 653a 2066 6c61  erride_file: fla
-00009440: 6720 6966 2066 696c 6520 7368 6f75 6c64  g if file should
-00009450: 2062 6520 7265 706c 6163 6564 2069 6620   be replaced if 
-00009460: 6974 2061 6c72 6561 6479 2065 7869 7374  it already exist
-00009470: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-00009480: 2062 696e 6172 795f 6d6f 6465 3a20 666c   binary_mode: fl
-00009490: 6167 2069 6620 6269 6e61 7279 2074 7261  ag if binary tra
-000094a0: 6e73 6665 7220 6d6f 6465 2073 686f 756c  nsfer mode shoul
-000094b0: 6420 6265 2075 7365 642c 2069 6620 6e6f  d be used, if no
-000094c0: 7420 7365 7420 7468 650a 2020 2020 2020  t set the.      
-000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094e0: 2020 2020 2020 6669 6c65 206e 616d 6520        file name 
-000094f0: 6973 2063 6865 636b 6564 2066 6f72 206b  is checked for k
-00009500: 6e6f 776e 2062 696e 6172 7920 6669 6c65  nown binary file
-00009510: 2074 7970 650a 0a20 2020 2020 2020 203a   type..        :
-00009520: 7261 6973 6573 204c 5356 3253 7461 7465  raises LSV2State
-00009530: 4578 6365 7074 696f 6e3a 2069 6620 6c6f  Exception: if lo
-00009540: 6361 6c20 6669 6c65 2063 6f75 6c64 206e  cal file could n
-00009550: 6f74 2062 6520 6f70 656e 6564 2c0a 2020  ot be opened,.  
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009580: 2020 6465 7374 696e 6174 696f 6e20 6469    destination di
-00009590: 7265 6374 6f72 7920 636f 756c 6420 6e6f  rectory could no
-000095a0: 7420 6265 2061 6363 6573 7365 6420 6f72  t be accessed or
-000095b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-000095e0: 2066 696c 6520 636f 756c 6420 6e6f 7420   file could not 
-000095f0: 6265 2064 656c 6574 6564 0a20 2020 2020  be deleted.     
-00009600: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00009610: 6620 6e6f 7420 7365 6c66 2e6c 6f67 696e  f not self.login
-00009620: 286c 632e 4c6f 6769 6e2e 4649 4c45 5452  (lc.Login.FILETR
-00009630: 414e 5346 4552 293a 0a20 2020 2020 2020  ANSFER):.       
-00009640: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00009650: 722e 7761 726e 696e 6728 2263 6f75 6c64  r.warning("could
-00009660: 206e 6f74 206c 6f67 2069 6e20 6173 2075   not log in as u
-00009670: 7365 7220 4649 4c45 2229 0a20 2020 2020  ser FILE").     
-00009680: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00009690: 6c73 650a 0a20 2020 2020 2020 2069 6620  lse..        if 
-000096a0: 6973 696e 7374 616e 6365 286c 6f63 616c  isinstance(local
-000096b0: 5f70 6174 682c 2028 7374 722c 2929 3a0a  _path, (str,)):.
-000096c0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-000096d0: 6c5f 6669 6c65 203d 2070 6174 686c 6962  l_file = pathlib
-000096e0: 2e50 6174 6828 6c6f 6361 6c5f 7061 7468  .Path(local_path
-000096f0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00009700: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00009710: 6c5f 6669 6c65 203d 206c 6f63 616c 5f70  l_file = local_p
-00009720: 6174 680a 0a20 2020 2020 2020 2069 6620  ath..        if 
-00009730: 6e6f 7420 6c6f 6361 6c5f 6669 6c65 2e69  not local_file.i
-00009740: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
-00009750: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-00009760: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
-00009770: 2020 2020 2020 2020 2020 2020 2274 6865              "the
-00009780: 2073 7570 706c 6965 6420 7061 7468 2025   supplied path %
-00009790: 7320 6469 6420 6e6f 7420 7265 736f 6c76  s did not resolv
-000097a0: 6520 746f 2061 2066 696c 6522 2c20 6c6f  e to a file", lo
-000097b0: 6361 6c5f 6669 6c65 0a20 2020 2020 2020  cal_file.       
-000097c0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000097d0: 2020 2072 6169 7365 204c 5356 3253 7461     raise LSV2Sta
-000097e0: 7465 4578 6365 7074 696f 6e28 226c 6f63  teException("loc
-000097f0: 616c 2066 696c 6520 646f 6573 206e 6f74  al file does not
-00009800: 2065 7869 7374 2120 7b7d 222e 666f 726d   exist! {}".form
-00009810: 6174 286c 6f63 616c 5f66 696c 6529 290a  at(local_file)).
-00009820: 0a20 2020 2020 2020 2072 656d 6f74 655f  .        remote_
-00009830: 7061 7468 203d 2072 656d 6f74 655f 7061  path = remote_pa
-00009840: 7468 2e72 6570 6c61 6365 2822 2f22 2c20  th.replace("/", 
-00009850: 6c63 2e50 4154 485f 5345 5029 0a0a 2020  lc.PATH_SEP)..  
-00009860: 2020 2020 2020 6966 206c 632e 5041 5448        if lc.PATH
-00009870: 5f53 4550 2069 6e20 7265 6d6f 7465 5f70  _SEP in remote_p
-00009880: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
-00009890: 2069 6620 7265 6d6f 7465 5f70 6174 682e   if remote_path.
-000098a0: 656e 6473 7769 7468 286c 632e 5041 5448  endswith(lc.PATH
-000098b0: 5f53 4550 293a 2020 2320 6e6f 2066 696c  _SEP):  # no fil
-000098c0: 656e 616d 6520 6769 7665 6e0a 2020 2020  ename given.    
-000098d0: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
-000098e0: 7465 5f66 696c 655f 6e61 6d65 203d 206c  te_file_name = l
-000098f0: 6f63 616c 5f66 696c 652e 6e61 6d65 0a20  ocal_file.name. 
-00009900: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009910: 656d 6f74 655f 6469 7265 6374 6f72 7920  emote_directory 
-00009920: 3d20 7265 6d6f 7465 5f70 6174 680a 2020  = remote_path.  
-00009930: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 7265 6d6f 7465 5f66 696c 655f 6e61 6d65  remote_file_name
-00009960: 203d 2072 656d 6f74 655f 7061 7468 2e73   = remote_path.s
-00009970: 706c 6974 286c 632e 5041 5448 5f53 4550  plit(lc.PATH_SEP
-00009980: 295b 2d31 5d0a 2020 2020 2020 2020 2020  )[-1].          
-00009990: 2020 2020 2020 7265 6d6f 7465 5f64 6972        remote_dir
-000099a0: 6563 746f 7279 203d 2072 656d 6f74 655f  ectory = remote_
-000099b0: 7061 7468 2e72 7374 7269 7028 7265 6d6f  path.rstrip(remo
-000099c0: 7465 5f66 696c 655f 6e61 6d65 290a 2020  te_file_name).  
-000099d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000099e0: 206e 6f74 2073 656c 662e 6368 616e 6765   not self.change
-000099f0: 5f64 6972 6563 746f 7279 2872 656d 6f74  _directory(remot
-00009a00: 655f 6469 7265 6374 6f72 793d 7265 6d6f  e_directory=remo
-00009a10: 7465 5f64 6972 6563 746f 7279 293a 0a20  te_directory):. 
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 2072 6169 7365 204c 5356 3253 7461     raise LSV2Sta
-00009a40: 7465 4578 6365 7074 696f 6e28 0a20 2020  teException(.   
-00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a60: 2020 2020 2022 636f 756c 6420 6e6f 7420       "could not 
-00009a70: 6f70 656e 2074 6865 2064 6573 7469 6e61  open the destina
-00009a80: 7469 6f6e 2064 6972 6563 746f 7279 207b  tion directory {
-00009a90: 7d22 2e66 6f72 6d61 7428 0a20 2020 2020  }".format(.     
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2072 656d 6f74 655f 6469         remote_di
-00009ac0: 7265 6374 6f72 790a 2020 2020 2020 2020  rectory.        
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009af0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009b00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00009b10: 2020 7265 6d6f 7465 5f66 696c 655f 6e61    remote_file_na
-00009b20: 6d65 203d 2072 656d 6f74 655f 7061 7468  me = remote_path
-00009b30: 0a20 2020 2020 2020 2020 2020 2072 656d  .            rem
-00009b40: 6f74 655f 6469 7265 6374 6f72 7920 3d20  ote_directory = 
-00009b50: 7365 6c66 2e64 6972 6563 746f 7279 5f69  self.directory_i
-00009b60: 6e66 6f28 292e 7061 7468 2020 2320 6765  nfo().path  # ge
-00009b70: 7420 7077 640a 2020 2020 2020 2020 7265  t pwd.        re
-00009b80: 6d6f 7465 5f64 6972 6563 746f 7279 203d  mote_directory =
-00009b90: 2072 656d 6f74 655f 6469 7265 6374 6f72   remote_director
-00009ba0: 792e 7273 7472 6970 286c 632e 5041 5448  y.rstrip(lc.PATH
-00009bb0: 5f53 4550 290a 0a20 2020 2020 2020 2069  _SEP)..        i
-00009bc0: 6620 6e6f 7420 7365 6c66 2e64 6972 6563  f not self.direc
-00009bd0: 746f 7279 5f69 6e66 6f28 7265 6d6f 7465  tory_info(remote
-00009be0: 5f64 6972 6563 746f 7279 293a 0a20 2020  _directory):.   
-00009bf0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00009c00: 6f67 6765 722e 6465 6275 6728 2272 656d  ogger.debug("rem
-00009c10: 6f74 6520 7061 7468 2064 6f65 7320 6e6f  ote path does no
-00009c20: 7420 6578 6973 742c 2063 7265 6174 6520  t exist, create 
-00009c30: 6469 7265 6374 6f72 7928 7329 2229 0a20  directory(s)"). 
-00009c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009c50: 6d61 6b65 5f64 6972 6563 746f 7279 2872  make_directory(r
-00009c60: 656d 6f74 655f 6469 7265 6374 6f72 7929  emote_directory)
-00009c70: 0a0a 2020 2020 2020 2020 7265 6d6f 7465  ..        remote
-00009c80: 5f69 6e66 6f20 3d20 7365 6c66 2e66 696c  _info = self.fil
-00009c90: 655f 696e 666f 2872 656d 6f74 655f 6469  e_info(remote_di
-00009ca0: 7265 6374 6f72 7920 2b20 6c63 2e50 4154  rectory + lc.PAT
-00009cb0: 485f 5345 5020 2b20 7265 6d6f 7465 5f66  H_SEP + remote_f
-00009cc0: 696c 655f 6e61 6d65 290a 0a20 2020 2020  ile_name)..     
-00009cd0: 2020 2069 6620 7265 6d6f 7465 5f69 6e66     if remote_inf
-00009ce0: 6f3a 0a20 2020 2020 2020 2020 2020 2073  o:.            s
-00009cf0: 656c 662e 5f6c 6f67 6765 722e 6465 6275  elf._logger.debu
-00009d00: 6728 2272 656d 6f74 6520 7061 7468 2065  g("remote path e
-00009d10: 7869 7374 7320 616e 6420 706f 696e 7473  xists and points
-00009d20: 2074 6f20 6669 6c65 2773 2229 0a20 2020   to file's").   
-00009d30: 2020 2020 2020 2020 2069 6620 6f76 6572           if over
-00009d40: 7269 6465 5f66 696c 653a 0a20 2020 2020  ride_file:.     
-00009d50: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00009d60: 7420 7365 6c66 2e64 656c 6574 655f 6669  t self.delete_fi
-00009d70: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00009d80: 2020 2020 2020 2020 7265 6d6f 7465 5f64          remote_d
-00009d90: 6972 6563 746f 7279 202b 206c 632e 5041  irectory + lc.PA
-00009da0: 5448 5f53 4550 202b 2072 656d 6f74 655f  TH_SEP + remote_
-00009db0: 6669 6c65 5f6e 616d 650a 2020 2020 2020  file_name.      
-00009dc0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 2072 6169 7365 204c 5356 3253 7461 7465   raise LSV2State
-00009df0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e10: 2020 2022 736f 6d65 7468 696e 6720 7765     "something we
-00009e20: 6e74 2077 726f 6e67 2077 6869 6c65 2064  nt wrong while d
-00009e30: 656c 6574 696e 6720 6669 6c65 207b 7d22  eleting file {}"
-00009e40: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e60: 2020 2020 2072 656d 6f74 655f 6469 7265       remote_dire
-00009e70: 6374 6f72 7920 2b20 6c63 2e50 4154 485f  ctory + lc.PATH_
-00009e80: 5345 5020 2b20 7265 6d6f 7465 5f66 696c  SEP + remote_fil
-00009e90: 655f 6e61 6d65 0a20 2020 2020 2020 2020  e_name.         
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000075d0: 7265 7375 6c74 203d 2073 656c 662e 5f73  result = self._s
+000075e0: 656e 645f 7265 6369 7665 286c 632e 434d  end_recive(lc.CM
+000075f0: 442e 435f 444d 2c20 7061 796c 6f61 642c  D.C_DM, payload,
+00007600: 206c 632e 5253 502e 545f 4f4b 290a 2020   lc.RSP.T_OK).  
+00007610: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007620: 2069 7369 6e73 7461 6e63 6528 7265 7375   isinstance(resu
+00007630: 6c74 2c20 2862 6f6f 6c2c 2929 2061 6e64  lt, (bool,)) and
+00007640: 2072 6573 756c 7420 6973 2054 7275 653a   result is True:
+00007650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007660: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+00007670: 722e 6465 6275 6728 2244 6972 6563 746f  r.debug("Directo
+00007680: 7279 2063 7265 6174 6564 2073 7563 6365  ry created succe
+00007690: 7373 6675 6c6c 7922 290a 2020 2020 2020  ssfully").      
+000076a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076c0: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+000076d0: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 2020 2261 6e20 6572 726f 7220 6f63 6375    "an error occu
+00007700: 7272 6564 2077 6869 6c65 2063 7265 6174  rred while creat
+00007710: 696e 6720 6469 7265 6374 6f72 7920 2573  ing directory %s
+00007720: 3a20 2725 7327 222c 0a20 2020 2020 2020  : '%s'",.       
+00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007740: 2064 6972 5f70 6174 682c 0a20 2020 2020   dir_path,.     
+00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007760: 2020 206c 742e 6765 745f 6572 726f 725f     lt.get_error_
+00007770: 7465 7874 2873 656c 662e 6c61 7374 5f65  text(self.last_e
+00007780: 7272 6f72 292c 0a20 2020 2020 2020 2020  rror),.         
+00007790: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077b0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+000077c0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077e0: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
+000077f0: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
+00007800: 2020 2020 2020 2020 226e 6f74 6869 6e67          "nothing
+00007810: 2074 6f20 646f 2061 7320 7468 6973 2073   to do as this s
+00007820: 6567 6d65 6e74 2061 6c72 6561 6479 2065  egment already e
+00007830: 7869 7374 7322 290a 2020 2020 2020 2020  xists").        
+00007840: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00007850: 2064 6566 2064 656c 6574 655f 656d 7074   def delete_empt
+00007860: 795f 6469 7265 6374 6f72 7928 7365 6c66  y_directory(self
+00007870: 2c20 6469 725f 7061 7468 3a20 7374 7229  , dir_path: str)
+00007880: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00007890: 2020 2222 220a 2020 2020 2020 2020 4465    """.        De
+000078a0: 6c65 7465 2065 6d70 7479 2064 6972 6563  lete empty direc
+000078b0: 746f 7279 206f 6e20 636f 6e74 726f 6c2e  tory on control.
+000078c0: 0a20 2020 2020 2020 2052 6571 7569 7265  .        Require
+000078d0: 7320 6163 6365 7373 206c 6576 656c 2060  s access level `
+000078e0: 6046 494c 4554 5241 4e53 4645 5260 6020  `FILETRANSFER`` 
+000078f0: 746f 2077 6f72 6b2e 0a20 2020 2020 2020  to work..       
+00007900: 2052 6574 7572 6e73 2060 6054 7275 6560   Returns ``True`
+00007910: 6020 6966 2063 6f6d 706c 6574 6564 2073  ` if completed s
+00007920: 7563 6365 7373 6675 6c6c 792e 0a0a 2020  uccessfully...  
+00007930: 2020 2020 2020 3a70 6172 616d 2066 696c        :param fil
+00007940: 655f 7061 7468 3a20 7061 7468 206f 6620  e_path: path of 
+00007950: 6469 7265 6374 6f72 7920 6f6e 2074 6865  directory on the
+00007960: 2063 6f6e 7472 6f6c 0a20 2020 2020 2020   control.       
+00007970: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00007980: 6e6f 7420 7365 6c66 2e6c 6f67 696e 286c  not self.login(l
+00007990: 632e 4c6f 6769 6e2e 4649 4c45 5452 414e  c.Login.FILETRAN
+000079a0: 5346 4552 293a 0a20 2020 2020 2020 2020  SFER):.         
+000079b0: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+000079c0: 7761 726e 696e 6728 2263 6f75 6c64 206e  warning("could n
+000079d0: 6f74 206c 6f67 2069 6e20 6173 2075 7365  ot log in as use
+000079e0: 7220 4649 4c45 2229 0a20 2020 2020 2020  r FILE").       
+000079f0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00007a00: 650a 0a20 2020 2020 2020 2064 6972 5f70  e..        dir_p
+00007a10: 6174 6820 3d20 6469 725f 7061 7468 2e72  ath = dir_path.r
+00007a20: 6570 6c61 6365 2822 2f22 2c20 6c63 2e50  eplace("/", lc.P
+00007a30: 4154 485f 5345 5029 0a20 2020 2020 2020  ATH_SEP).       
+00007a40: 2070 6179 6c6f 6164 203d 206c 6d2e 7573   payload = lm.us
+00007a50: 7472 5f74 6f5f 6261 2864 6972 5f70 6174  tr_to_ba(dir_pat
+00007a60: 6829 0a0a 2020 2020 2020 2020 7265 7375  h)..        resu
+00007a70: 6c74 203d 2073 656c 662e 5f73 656e 645f  lt = self._send_
+00007a80: 7265 6369 7665 286c 632e 434d 442e 435f  recive(lc.CMD.C_
+00007a90: 4444 2c20 7061 796c 6f61 642c 206c 632e  DD, payload, lc.
+00007aa0: 5253 502e 545f 4f4b 290a 2020 2020 2020  RSP.T_OK).      
+00007ab0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00007ac0: 7265 7375 6c74 2c20 2862 6f6f 6c29 2920  result, (bool)) 
+00007ad0: 616e 6420 7265 7375 6c74 2069 7320 5472  and result is Tr
+00007ae0: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00007af0: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
+00007b00: 7567 2822 7375 6363 6573 7366 756c 6c79  ug("successfully
+00007b10: 2064 656c 6574 6564 2064 6972 6563 746f   deleted directo
+00007b20: 7279 2025 7322 2c20 6469 725f 7061 7468  ry %s", dir_path
+00007b30: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007b40: 7475 726e 2054 7275 650a 0a20 2020 2020  turn True..     
+00007b50: 2020 2069 6620 7365 6c66 2e6c 6173 745f     if self.last_
+00007b60: 6572 726f 722e 655f 636f 6465 203d 3d20  error.e_code == 
+00007b70: 6c63 2e4c 5356 3253 7461 7475 7343 6f64  lc.LSV2StatusCod
+00007b80: 652e 545f 4552 5f4e 4f5f 4449 523a 0a20  e.T_ER_NO_DIR:. 
+00007b90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007ba0: 5f6c 6f67 6765 722e 6465 6275 6728 0a20  _logger.debug(. 
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007bc0: 6e6f 7469 6e67 2074 6f20 646f 2c20 6469  noting to do, di
+00007bd0: 7265 6374 6f72 7920 2573 2064 6964 6e27  rectory %s didn'
+00007be0: 7420 6578 6973 7422 2c20 6469 725f 7061  t exist", dir_pa
+00007bf0: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+00007c00: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00007c10: 2020 2020 2069 6620 7365 6c66 2e6c 6173       if self.las
+00007c20: 745f 6572 726f 722e 655f 636f 6465 203d  t_error.e_code =
+00007c30: 3d20 6c63 2e4c 5356 3253 7461 7475 7343  = lc.LSV2StatusC
+00007c40: 6f64 652e 545f 4552 5f44 454c 5f44 4952  ode.T_ER_DEL_DIR
+00007c50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007c60: 6c66 2e5f 6c6f 6767 6572 2e64 6562 7567  lf._logger.debug
+00007c70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00007c80: 2020 2263 6f75 6c64 206e 6f74 2064 656c    "could not del
+00007c90: 6574 6520 6469 7265 6374 6f72 7920 2573  ete directory %s
+00007ca0: 2073 696e 6365 2069 7420 6973 206e 6f74   since it is not
+00007cb0: 2065 6d70 7479 222c 2064 6972 5f70 6174   empty", dir_pat
+00007cc0: 680a 2020 2020 2020 2020 2020 2020 290a  h.            ).
+00007cd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00007ce0: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
+00007cf0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e77    self._logger.w
+00007d00: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+00007d10: 2020 2020 2261 6e20 6572 726f 7220 6f63      "an error oc
+00007d20: 6375 7272 6564 2077 6869 6c65 2064 656c  curred while del
+00007d30: 6574 696e 6720 6469 7265 6374 6f72 7920  eting directory 
+00007d40: 2573 222c 0a20 2020 2020 2020 2020 2020  %s",.           
+00007d50: 2064 6972 5f70 6174 682c 0a20 2020 2020   dir_path,.     
+00007d60: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+00007d70: 7572 6e20 4661 6c73 650a 0a20 2020 2064  urn False..    d
+00007d80: 6566 2064 656c 6574 655f 6669 6c65 2873  ef delete_file(s
+00007d90: 656c 662c 2066 696c 655f 7061 7468 3a20  elf, file_path: 
+00007da0: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
+00007db0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007dc0: 2020 4465 6c65 7465 2066 696c 6520 6f6e    Delete file on
+00007dd0: 2063 6f6e 7472 6f6c 2e0a 2020 2020 2020   control..      
+00007de0: 2020 5265 7175 6972 6573 2061 6363 6573    Requires acces
+00007df0: 7320 6c65 7665 6c20 6060 4649 4c45 5452  s level ``FILETR
+00007e00: 414e 5346 4552 6060 2074 6f20 776f 726b  ANSFER`` to work
+00007e10: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00007e20: 7320 6060 5472 7565 6060 2069 6620 636f  s ``True`` if co
+00007e30: 6d70 6c65 7465 6420 7375 6363 6573 7366  mpleted successf
+00007e40: 756c 6c79 2e0a 0a20 2020 2020 2020 203a  ully...        :
+00007e50: 7061 7261 6d20 6669 6c65 5f70 6174 683a  param file_path:
+00007e60: 2070 6174 6820 6f66 2066 696c 6520 6f6e   path of file on
+00007e70: 2074 6865 2063 6f6e 7472 6f6c 0a20 2020   the control.   
+00007e80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007e90: 2069 6620 6e6f 7420 7365 6c66 2e6c 6f67   if not self.log
+00007ea0: 696e 286c 632e 4c6f 6769 6e2e 4649 4c45  in(lc.Login.FILE
+00007eb0: 5452 414e 5346 4552 293a 0a20 2020 2020  TRANSFER):.     
+00007ec0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+00007ed0: 6765 722e 7761 726e 696e 6728 2263 6f75  ger.warning("cou
+00007ee0: 6c64 206e 6f74 206c 6f67 2069 6e20 6173  ld not log in as
+00007ef0: 2075 7365 7220 4649 4c45 2229 0a20 2020   user FILE").   
+00007f00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007f10: 4661 6c73 650a 0a20 2020 2020 2020 2066  False..        f
+00007f20: 696c 655f 7061 7468 203d 2066 696c 655f  ile_path = file_
+00007f30: 7061 7468 2e72 6570 6c61 6365 2822 2f22  path.replace("/"
+00007f40: 2c20 6c63 2e50 4154 485f 5345 5029 0a20  , lc.PATH_SEP). 
+00007f50: 2020 2020 2020 2070 6179 6c6f 6164 203d         payload =
+00007f60: 206c 6d2e 7573 7472 5f74 6f5f 6261 2866   lm.ustr_to_ba(f
+00007f70: 696c 655f 7061 7468 290a 0a20 2020 2020  ile_path)..     
+00007f80: 2020 2069 6620 7365 6c66 2e5f 7365 6e64     if self._send
+00007f90: 5f72 6563 6976 6528 6c63 2e43 4d44 2e43  _recive(lc.CMD.C
+00007fa0: 5f46 442c 2070 6179 6c6f 6164 2c20 6c63  _FD, payload, lc
+00007fb0: 2e52 5350 2e54 5f4f 4b29 3a0a 2020 2020  .RSP.T_OK):.    
+00007fc0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+00007fd0: 6767 6572 2e64 6562 7567 2822 7375 6363  gger.debug("succ
+00007fe0: 6573 7366 756c 6c79 2064 656c 6574 6564  essfully deleted
+00007ff0: 2066 696c 6520 2573 222c 2066 696c 655f   file %s", file_
+00008000: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+00008010: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+00008020: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+00008030: 6173 745f 6572 726f 722e 655f 636f 6465  ast_error.e_code
+00008040: 203d 3d20 6c63 2e4c 5356 3253 7461 7475   == lc.LSV2Statu
+00008050: 7343 6f64 652e 545f 4552 5f4e 4f5f 4649  sCode.T_ER_NO_FI
+00008060: 4c45 3a0a 2020 2020 2020 2020 2020 2020  LE:.            
+00008070: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
+00008080: 7567 2822 6e6f 7469 6e67 2074 6f20 646f  ug("noting to do
+00008090: 2c20 6669 6c65 2025 7320 6469 646e 2774  , file %s didn't
+000080a0: 2065 7869 7374 222c 2066 696c 655f 7061   exist", file_pa
+000080b0: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+000080c0: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+000080d0: 2020 2020 2069 6620 7365 6c66 2e6c 6173       if self.las
+000080e0: 745f 6572 726f 722e 655f 636f 6465 203d  t_error.e_code =
+000080f0: 3d20 6c63 2e4c 5356 3253 7461 7475 7343  = lc.LSV2StatusC
+00008100: 6f64 652e 545f 4552 5f4e 4f5f 4445 4c45  ode.T_ER_NO_DELE
+00008110: 5445 3a0a 2020 2020 2020 2020 2020 2020  TE:.            
+00008120: 7365 6c66 2e5f 6c6f 6767 6572 2e69 6e66  self._logger.inf
+00008130: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
+00008140: 2020 2022 636f 756c 6420 6e6f 7420 6465     "could not de
+00008150: 6c65 7465 2066 696c 6520 2573 2073 696e  lete file %s sin
+00008160: 6365 2069 7420 6973 2069 6e20 7573 6522  ce it is in use"
+00008170: 2c20 6669 6c65 5f70 6174 6829 0a20 2020  , file_path).   
+00008180: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008190: 4661 6c73 650a 0a20 2020 2020 2020 2073  False..        s
+000081a0: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
+000081b0: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+000081c0: 2022 616e 2065 7272 6f72 206f 6363 7572   "an error occur
+000081d0: 7265 6420 7768 696c 6520 6465 6c65 7469  red while deleti
+000081e0: 6e67 2066 696c 6520 2573 222c 0a20 2020  ng file %s",.   
+000081f0: 2020 2020 2020 2020 2066 696c 655f 7061           file_pa
+00008200: 7468 2c0a 2020 2020 2020 2020 290a 2020  th,.        ).  
+00008210: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00008220: 7365 0a0a 2020 2020 6465 6620 636f 7079  se..    def copy
+00008230: 5f72 656d 6f74 655f 6669 6c65 2873 656c  _remote_file(sel
+00008240: 662c 2073 6f75 7263 655f 7061 7468 3a20  f, source_path: 
+00008250: 7374 722c 2074 6172 6765 745f 7061 7468  str, target_path
+00008260: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
+00008270: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008280: 2020 2020 436f 7079 2066 696c 6520 6f6e      Copy file on
+00008290: 2063 6f6e 7472 6f6c 2066 726f 6d20 6f6e   control from on
+000082a0: 6520 706c 6163 6520 746f 2061 6e6f 7468  e place to anoth
+000082b0: 6572 2e0a 2020 2020 2020 2020 5265 7175  er..        Requ
+000082c0: 6972 6573 2061 6363 6573 7320 6c65 7665  ires access leve
+000082d0: 6c20 6060 4649 4c45 5452 414e 5346 4552  l ``FILETRANSFER
+000082e0: 6060 2074 6f20 776f 726b 2e0a 2020 2020  `` to work..    
+000082f0: 2020 2020 5265 7475 726e 7320 6060 5472      Returns ``Tr
+00008300: 7565 6060 2069 6620 636f 6d70 6c65 7465  ue`` if complete
+00008310: 6420 7375 6363 6573 7366 756c 6c79 2e0a  d successfully..
+00008320: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00008330: 736f 7572 6365 5f70 6174 683a 2070 6174  source_path: pat
+00008340: 6820 6f66 2066 696c 6520 6f6e 2074 6865  h of file on the
+00008350: 2063 6f6e 7472 6f6c 0a20 2020 2020 2020   control.       
+00008360: 203a 7061 7261 6d20 7461 7267 6574 5f70   :param target_p
+00008370: 6174 683a 2070 6174 6820 6f66 2074 6172  ath: path of tar
+00008380: 6765 7420 6c6f 6361 7469 6f6e 0a0a 2020  get location..  
+00008390: 2020 2020 2020 3a72 6169 7365 7320 4c53        :raises LS
+000083a0: 5632 5374 6174 6545 7863 6570 7469 6f6e  V2StateException
+000083b0: 3a20 6966 2074 6865 2073 656c 6563 7465  : if the selecte
+000083c0: 6420 7061 7468 2063 6f75 6c64 206e 6f74  d path could not
+000083d0: 2062 6520 666f 756e 6420 6f72 0a20 2020   be found or.   
+000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008400: 2074 6865 2070 6174 6820 6973 206e 6f74   the path is not
+00008410: 2061 6363 6573 7369 626c 650a 2020 2020   accessible.    
+00008420: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008430: 6966 206e 6f74 2073 656c 662e 6c6f 6769  if not self.logi
+00008440: 6e28 6c63 2e4c 6f67 696e 2e46 494c 4554  n(lc.Login.FILET
+00008450: 5241 4e53 4645 5229 3a0a 2020 2020 2020  RANSFER):.      
+00008460: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+00008470: 6572 2e77 6172 6e69 6e67 2822 636f 756c  er.warning("coul
+00008480: 6420 6e6f 7420 6c6f 6720 696e 2061 7320  d not log in as 
+00008490: 7573 6572 2046 494c 4522 290a 2020 2020  user FILE").    
+000084a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000084b0: 616c 7365 0a0a 2020 2020 2020 2020 736f  alse..        so
+000084c0: 7572 6365 5f70 6174 6820 3d20 736f 7572  urce_path = sour
+000084d0: 6365 5f70 6174 682e 7265 706c 6163 6528  ce_path.replace(
+000084e0: 222f 222c 206c 632e 5041 5448 5f53 4550  "/", lc.PATH_SEP
+000084f0: 290a 2020 2020 2020 2020 7461 7267 6574  ).        target
+00008500: 5f70 6174 6820 3d20 7461 7267 6574 5f70  _path = target_p
+00008510: 6174 682e 7265 706c 6163 6528 222f 222c  ath.replace("/",
+00008520: 206c 632e 5041 5448 5f53 4550 290a 0a20   lc.PATH_SEP).. 
+00008530: 2020 2020 2020 2069 6620 6c63 2e50 4154         if lc.PAT
+00008540: 485f 5345 5020 696e 2073 6f75 7263 655f  H_SEP in source_
+00008550: 7061 7468 3a0a 2020 2020 2020 2020 2020  path:.          
+00008560: 2020 2320 6368 616e 6765 2064 6972 6563    # change direc
+00008570: 746f 7279 0a20 2020 2020 2020 2020 2020  tory.           
+00008580: 2073 6f75 7263 655f 6669 6c65 5f6e 616d   source_file_nam
+00008590: 6520 3d20 736f 7572 6365 5f70 6174 682e  e = source_path.
+000085a0: 7370 6c69 7428 6c63 2e50 4154 485f 5345  split(lc.PATH_SE
+000085b0: 5029 5b2d 315d 0a20 2020 2020 2020 2020  P)[-1].         
+000085c0: 2020 2073 6f75 7263 655f 6469 7265 6374     source_direct
+000085d0: 6f72 7920 3d20 736f 7572 6365 5f70 6174  ory = source_pat
+000085e0: 682e 7273 7472 6970 2873 6f75 7263 655f  h.rstrip(source_
+000085f0: 6669 6c65 5f6e 616d 6529 0a20 2020 2020  file_name).     
+00008600: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00008610: 6c66 2e63 6861 6e67 655f 6469 7265 6374  lf.change_direct
+00008620: 6f72 7928 7265 6d6f 7465 5f64 6972 6563  ory(remote_direc
+00008630: 746f 7279 3d73 6f75 7263 655f 6469 7265  tory=source_dire
+00008640: 6374 6f72 7929 3a0a 2020 2020 2020 2020  ctory):.        
+00008650: 2020 2020 2020 2020 7261 6973 6520 4c53          raise LS
+00008660: 5632 5374 6174 6545 7863 6570 7469 6f6e  V2StateException
+00008670: 2822 636f 756c 6420 6e6f 7420 6f70 656e  ("could not open
+00008680: 2074 6865 2073 6f75 7263 6520 6469 7265   the source dire
+00008690: 6374 6f72 7922 290a 2020 2020 2020 2020  ctory").        
+000086a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000086b0: 2020 736f 7572 6365 5f66 696c 655f 6e61    source_file_na
+000086c0: 6d65 203d 2073 6f75 7263 655f 7061 7468  me = source_path
+000086d0: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
+000086e0: 7263 655f 6469 7265 6374 6f72 7920 3d20  rce_directory = 
+000086f0: 222e 220a 0a20 2020 2020 2020 2069 6620  "."..        if 
+00008700: 7461 7267 6574 5f70 6174 682e 656e 6473  target_path.ends
+00008710: 7769 7468 286c 632e 5041 5448 5f53 4550  with(lc.PATH_SEP
+00008720: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+00008730: 6172 6765 745f 7061 7468 202b 3d20 736f  arget_path += so
+00008740: 7572 6365 5f66 696c 655f 6e61 6d65 0a0a  urce_file_name..
+00008750: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
+00008760: 3d20 6c6d 2e75 7374 725f 746f 5f62 6128  = lm.ustr_to_ba(
+00008770: 736f 7572 6365 5f66 696c 655f 6e61 6d65  source_file_name
+00008780: 290a 2020 2020 2020 2020 7061 796c 6f61  ).        payloa
+00008790: 642e 6578 7465 6e64 286c 6d2e 7573 7472  d.extend(lm.ustr
+000087a0: 5f74 6f5f 6261 2874 6172 6765 745f 7061  _to_ba(target_pa
+000087b0: 7468 2929 0a20 2020 2020 2020 2073 656c  th)).        sel
+000087c0: 662e 5f6c 6f67 6765 722e 6465 6275 6728  f._logger.debug(
+000087d0: 0a20 2020 2020 2020 2020 2020 2022 7072  .            "pr
+000087e0: 6570 6172 6520 746f 2063 6f70 7920 6669  epare to copy fi
+000087f0: 6c65 2025 7320 6672 6f6d 2025 7320 746f  le %s from %s to
+00008800: 2025 7322 2c0a 2020 2020 2020 2020 2020   %s",.          
+00008810: 2020 736f 7572 6365 5f66 696c 655f 6e61    source_file_na
+00008820: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00008830: 736f 7572 6365 5f64 6972 6563 746f 7279  source_directory
+00008840: 2c0a 2020 2020 2020 2020 2020 2020 7461  ,.            ta
+00008850: 7267 6574 5f70 6174 682c 0a20 2020 2020  rget_path,.     
+00008860: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00008870: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
+00008880: 6528 6c63 2e43 4d44 2e43 5f46 432c 2070  e(lc.CMD.C_FC, p
+00008890: 6179 6c6f 6164 2c20 6c63 2e52 5350 2e54  ayload, lc.RSP.T
+000088a0: 5f4f 4b29 3a0a 2020 2020 2020 2020 2020  _OK):.          
+000088b0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e64    self._logger.d
+000088c0: 6562 7567 2822 7375 6363 6573 7366 756c  ebug("successful
+000088d0: 6c79 2063 6f70 6965 6420 6669 6c65 2025  ly copied file %
+000088e0: 7322 2c20 736f 7572 6365 5f70 6174 6829  s", source_path)
+000088f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008900: 7572 6e20 5472 7565 0a0a 2020 2020 2020  urn True..      
+00008910: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e77    self._logger.w
+00008920: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+00008930: 2020 2020 2261 6e20 6572 726f 7220 6f63      "an error oc
+00008940: 6375 7272 6564 2063 6f70 7969 6e67 2066  curred copying f
+00008950: 696c 6520 2573 2074 6f20 2573 222c 2073  ile %s to %s", s
+00008960: 6f75 7263 655f 7061 7468 2c20 7461 7267  ource_path, targ
+00008970: 6574 5f70 6174 680a 2020 2020 2020 2020  et_path.        
+00008980: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00008990: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
+000089a0: 6d6f 7665 5f66 696c 6528 7365 6c66 2c20  move_file(self, 
+000089b0: 736f 7572 6365 5f70 6174 683a 2073 7472  source_path: str
+000089c0: 2c20 7461 7267 6574 5f70 6174 683a 2073  , target_path: s
+000089d0: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
+000089e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000089f0: 204d 6f76 6520 6669 6c65 206f 6e20 636f   Move file on co
+00008a00: 6e74 726f 6c20 6672 6f6d 206f 6e65 2070  ntrol from one p
+00008a10: 6c61 6365 2074 6f20 616e 6f74 6865 722e  lace to another.
+00008a20: 0a20 2020 2020 2020 2052 6571 7569 7265  .        Require
+00008a30: 7320 6163 6365 7373 206c 6576 656c 2060  s access level `
+00008a40: 6046 494c 4554 5241 4e53 4645 5260 6020  `FILETRANSFER`` 
+00008a50: 746f 2077 6f72 6b2e 0a20 2020 2020 2020  to work..       
+00008a60: 2052 6574 7572 6e73 2060 6054 7275 6560   Returns ``True`
+00008a70: 6020 6966 2063 7265 6174 696e 6720 6469  ` if creating di
+00008a80: 7265 6374 6f72 7920 7761 7320 7375 6363  rectory was succ
+00008a90: 6573 7366 756c 2e0a 0a20 2020 2020 2020  essful...       
+00008aa0: 203a 7061 7261 6d20 736f 7572 6365 5f70   :param source_p
+00008ab0: 6174 683a 2070 6174 6820 6f66 2066 696c  ath: path of fil
+00008ac0: 6520 6f6e 2074 6865 2063 6f6e 7472 6f6c  e on the control
+00008ad0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00008ae0: 7461 7267 6574 5f70 6174 683a 2070 6174  target_path: pat
+00008af0: 6820 6f66 2074 6172 6765 7420 6c6f 6361  h of target loca
+00008b00: 7469 6f6e 2077 6974 6820 6f72 2077 6974  tion with or wit
+00008b10: 686f 7574 2066 696c 656e 616d 650a 0a20  hout filename.. 
+00008b20: 2020 2020 2020 203a 7261 6973 6573 204c         :raises L
+00008b30: 5356 3253 7461 7465 4578 6365 7074 696f  SV2StateExceptio
+00008b40: 6e3a 2069 6620 7468 6520 7365 6c65 6374  n: if the select
+00008b50: 6564 2070 6174 6820 636f 756c 6420 6e6f  ed path could no
+00008b60: 7420 6265 2066 6f75 6e64 206f 720a 2020  t be found or.  
+00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2020 7468 6520 7061 7468 2069 7320 6e6f    the path is no
+00008ba0: 7420 6163 6365 7373 6962 6c65 0a20 2020  t accessible.   
+00008bb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00008bc0: 2073 6f75 7263 655f 7061 7468 203d 2073   source_path = s
+00008bd0: 6f75 7263 655f 7061 7468 2e72 6570 6c61  ource_path.repla
+00008be0: 6365 2822 2f22 2c20 6c63 2e50 4154 485f  ce("/", lc.PATH_
+00008bf0: 5345 5029 0a20 2020 2020 2020 2074 6172  SEP).        tar
+00008c00: 6765 745f 7061 7468 203d 2074 6172 6765  get_path = targe
+00008c10: 745f 7061 7468 2e72 6570 6c61 6365 2822  t_path.replace("
+00008c20: 2f22 2c20 6c63 2e50 4154 485f 5345 5029  /", lc.PATH_SEP)
+00008c30: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00008c40: 2073 656c 662e 6c6f 6769 6e28 6c63 2e4c   self.login(lc.L
+00008c50: 6f67 696e 2e46 494c 4554 5241 4e53 4645  ogin.FILETRANSFE
+00008c60: 5229 3a0a 2020 2020 2020 2020 2020 2020  R):.            
+00008c70: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
+00008c80: 6e69 6e67 2822 636f 756c 6420 6e6f 7420  ning("could not 
+00008c90: 6c6f 6720 696e 2061 7320 7573 6572 2046  log in as user F
+00008ca0: 494c 4522 290a 2020 2020 2020 2020 2020  ILE").          
+00008cb0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00008cc0: 2020 2020 2020 2020 6966 206c 632e 5041          if lc.PA
+00008cd0: 5448 5f53 4550 2069 6e20 736f 7572 6365  TH_SEP in source
+00008ce0: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
+00008cf0: 2020 2073 6f75 7263 655f 6669 6c65 5f6e     source_file_n
+00008d00: 616d 6520 3d20 736f 7572 6365 5f70 6174  ame = source_pat
+00008d10: 682e 7370 6c69 7428 6c63 2e50 4154 485f  h.split(lc.PATH_
+00008d20: 5345 5029 5b2d 315d 0a20 2020 2020 2020  SEP)[-1].       
+00008d30: 2020 2020 2073 6f75 7263 655f 6469 7265       source_dire
+00008d40: 6374 6f72 7920 3d20 736f 7572 6365 5f70  ctory = source_p
+00008d50: 6174 682e 7273 7472 6970 2873 6f75 7263  ath.rstrip(sourc
+00008d60: 655f 6669 6c65 5f6e 616d 6529 0a20 2020  e_file_name).   
+00008d70: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00008d80: 7365 6c66 2e63 6861 6e67 655f 6469 7265  self.change_dire
+00008d90: 6374 6f72 7928 7265 6d6f 7465 5f64 6972  ctory(remote_dir
+00008da0: 6563 746f 7279 3d73 6f75 7263 655f 6469  ectory=source_di
+00008db0: 7265 6374 6f72 7929 3a0a 2020 2020 2020  rectory):.      
+00008dc0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00008dd0: 4c53 5632 5374 6174 6545 7863 6570 7469  LSV2StateExcepti
+00008de0: 6f6e 2822 636f 756c 6420 6e6f 7420 6f70  on("could not op
+00008df0: 656e 2074 6865 2073 6f75 7263 6520 6469  en the source di
+00008e00: 7265 6374 6f72 7922 290a 2020 2020 2020  rectory").      
+00008e10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008e20: 2020 2020 736f 7572 6365 5f66 696c 655f      source_file_
+00008e30: 6e61 6d65 203d 2073 6f75 7263 655f 7061  name = source_pa
+00008e40: 7468 0a20 2020 2020 2020 2020 2020 2073  th.            s
+00008e50: 6f75 7263 655f 6469 7265 6374 6f72 7920  ource_directory 
+00008e60: 3d20 222e 220a 0a20 2020 2020 2020 2069  = "."..        i
+00008e70: 6620 7461 7267 6574 5f70 6174 682e 656e  f target_path.en
+00008e80: 6473 7769 7468 286c 632e 5041 5448 5f53  dswith(lc.PATH_S
+00008e90: 4550 293a 0a20 2020 2020 2020 2020 2020  EP):.           
+00008ea0: 2074 6172 6765 745f 7061 7468 202b 3d20   target_path += 
+00008eb0: 736f 7572 6365 5f66 696c 655f 6e61 6d65  source_file_name
+00008ec0: 0a0a 2020 2020 2020 2020 7061 796c 6f61  ..        payloa
+00008ed0: 6420 3d20 6c6d 2e75 7374 725f 746f 5f62  d = lm.ustr_to_b
+00008ee0: 6128 736f 7572 6365 5f66 696c 655f 6e61  a(source_file_na
+00008ef0: 6d65 290a 2020 2020 2020 2020 7061 796c  me).        payl
+00008f00: 6f61 642e 6578 7465 6e64 286c 6d2e 7573  oad.extend(lm.us
+00008f10: 7472 5f74 6f5f 6261 2874 6172 6765 745f  tr_to_ba(target_
+00008f20: 7061 7468 2929 0a0a 2020 2020 2020 2020  path))..        
+00008f30: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
+00008f40: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
+00008f50: 2270 7265 7061 7265 2074 6f20 6d6f 7665  "prepare to move
+00008f60: 2066 696c 6520 2573 2066 726f 6d20 2573   file %s from %s
+00008f70: 2074 6f20 2573 222c 0a20 2020 2020 2020   to %s",.       
+00008f80: 2020 2020 2073 6f75 7263 655f 6669 6c65       source_file
+00008f90: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+00008fa0: 2020 2073 6f75 7263 655f 6469 7265 6374     source_direct
+00008fb0: 6f72 792c 0a20 2020 2020 2020 2020 2020  ory,.           
+00008fc0: 2074 6172 6765 745f 7061 7468 2c0a 2020   target_path,.  
+00008fd0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008fe0: 6966 2073 656c 662e 5f73 656e 645f 7265  if self._send_re
+00008ff0: 6369 7665 286c 632e 434d 442e 435f 4652  cive(lc.CMD.C_FR
+00009000: 2c20 7061 796c 6f61 642c 206c 632e 5253  , payload, lc.RS
+00009010: 502e 545f 4f4b 293a 0a20 2020 2020 2020  P.T_OK):.       
+00009020: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+00009030: 722e 6465 6275 6728 2273 7563 6365 7373  r.debug("success
+00009040: 6675 6c6c 7920 6d6f 7665 6420 6669 6c65  fully moved file
+00009050: 2025 7322 2c20 736f 7572 6365 5f70 6174   %s", source_pat
+00009060: 6829 0a20 2020 2020 2020 2020 2020 2072  h).            r
+00009070: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00009080: 2020 2020 6966 2073 656c 662e 6c61 7374      if self.last
+00009090: 5f65 7272 6f72 2e65 5f63 6f64 6520 3d3d  _error.e_code ==
+000090a0: 206c 632e 4c53 5632 5374 6174 7573 436f   lc.LSV2StatusCo
+000090b0: 6465 2e54 5f45 525f 4649 4c45 5f45 5849  de.T_ER_FILE_EXI
+000090c0: 5354 533a 0a20 2020 2020 2020 2020 2020  STS:.           
+000090d0: 2073 656c 662e 5f6c 6f67 6765 722e 696e   self._logger.in
+000090e0: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
+000090f0: 2020 2020 2263 6f75 6c64 206e 6f74 206d      "could not m
+00009100: 6f76 6520 6669 6c65 2025 7320 746f 2025  ove file %s to %
+00009110: 7320 7369 6e63 6520 616c 7265 6164 7920  s since already 
+00009120: 6578 6973 7473 222c 0a20 2020 2020 2020  exists",.       
+00009130: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
+00009140: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+00009150: 2020 2020 2020 7461 7267 6574 5f70 6174        target_pat
+00009160: 682c 0a20 2020 2020 2020 2020 2020 2029  h,.            )
+00009170: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009180: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
+00009190: 2020 2069 6620 7365 6c66 2e6c 6173 745f     if self.last_
+000091a0: 6572 726f 722e 655f 636f 6465 203d 3d20  error.e_code == 
+000091b0: 6c63 2e4c 5356 3253 7461 7475 7343 6f64  lc.LSV2StatusCod
+000091c0: 652e 545f 4552 5f4e 4f5f 4649 4c45 3a0a  e.T_ER_NO_FILE:.
+000091d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000091e0: 2e5f 6c6f 6767 6572 2e69 6e66 6f28 0a20  ._logger.info(. 
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00009200: 636f 756c 6420 6e6f 7420 6d6f 7665 2066  could not move f
+00009210: 696c 6520 7369 6e63 6520 6569 7468 6572  ile since either
+00009220: 2073 6f75 7263 6520 6f72 2074 6172 6765   source or targe
+00009230: 7420 7061 7468 2064 6f65 7320 6e6f 7420  t path does not 
+00009240: 6578 6973 7422 2c0a 2020 2020 2020 2020  exist",.        
+00009250: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00009260: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00009270: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+00009280: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
+00009290: 2020 2020 2020 2020 2020 2261 6e20 6572            "an er
+000092a0: 726f 7220 6f63 6375 7272 6564 206d 6f76  ror occurred mov
+000092b0: 696e 6720 6669 6c65 2025 7320 746f 2025  ing file %s to %
+000092c0: 7322 2c20 736f 7572 6365 5f70 6174 682c  s", source_path,
+000092d0: 2074 6172 6765 745f 7061 7468 0a20 2020   target_path.   
+000092e0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+000092f0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00009300: 2064 6566 2073 656e 645f 6669 6c65 280a   def send_file(.
+00009310: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00009320: 2020 2020 2020 6c6f 6361 6c5f 7061 7468        local_path
+00009330: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
+00009340: 686c 6962 2e50 6174 685d 2c0a 2020 2020  hlib.Path],.    
+00009350: 2020 2020 7265 6d6f 7465 5f70 6174 683a      remote_path:
+00009360: 2073 7472 2c0a 2020 2020 2020 2020 6f76   str,.        ov
+00009370: 6572 7269 6465 5f66 696c 653a 2062 6f6f  erride_file: boo
+00009380: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+00009390: 2020 2062 696e 6172 795f 6d6f 6465 3a20     binary_mode: 
+000093a0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+000093b0: 2020 2920 2d3e 2062 6f6f 6c3a 0a20 2020    ) -> bool:.   
+000093c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000093d0: 2055 706c 6f61 6420 6120 6669 6c65 2074   Upload a file t
+000093e0: 6f20 636f 6e74 726f 6c0a 2020 2020 2020  o control.      
+000093f0: 2020 5265 7175 6972 6573 2061 6363 6573    Requires acces
+00009400: 7320 6c65 7665 6c20 6060 4649 4c45 5452  s level ``FILETR
+00009410: 414e 5346 4552 6060 2074 6f20 776f 726b  ANSFER`` to work
+00009420: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00009430: 7320 6060 5472 7565 6060 2069 6620 636f  s ``True`` if co
+00009440: 6d70 6c65 7465 6420 7375 6363 6573 7366  mpleted successf
+00009450: 756c 6c79 2e0a 0a20 2020 2020 2020 203a  ully...        :
+00009460: 7061 7261 6d20 6c6f 6361 6c5f 7061 7468  param local_path
+00009470: 3a20 7061 7468 206f 6620 6669 6c65 2074  : path of file t
+00009480: 6f20 6265 2073 656e 7420 746f 2074 6865  o be sent to the
+00009490: 2063 6f6e 7472 6f6c 0a20 2020 2020 2020   control.       
+000094a0: 203a 7061 7261 6d20 7265 6d6f 7465 5f70   :param remote_p
+000094b0: 6174 683a 2070 6174 6820 7769 7468 206f  ath: path with o
+000094c0: 7220 7769 7468 6f75 7420 7468 6520 6669  r without the fi
+000094d0: 6c65 206e 616d 6520 6f6e 2074 6865 2063  le name on the c
+000094e0: 6f6e 7472 6f6c 0a20 2020 2020 2020 203a  ontrol.        :
+000094f0: 7061 7261 6d20 6f76 6572 7269 6465 5f66  param override_f
+00009500: 696c 653a 2066 6c61 6720 6966 2066 696c  ile: flag if fil
+00009510: 6520 7368 6f75 6c64 2062 6520 7265 706c  e should be repl
+00009520: 6163 6564 2069 6620 6974 2061 6c72 6561  aced if it alrea
+00009530: 6479 2065 7869 7374 730a 2020 2020 2020  dy exists.      
+00009540: 2020 3a70 6172 616d 2062 696e 6172 795f    :param binary_
+00009550: 6d6f 6465 3a20 666c 6167 2069 6620 6269  mode: flag if bi
+00009560: 6e61 7279 2074 7261 6e73 6665 7220 6d6f  nary transfer mo
+00009570: 6465 2073 686f 756c 6420 6265 2075 7365  de should be use
+00009580: 642c 2069 6620 6e6f 7420 7365 7420 7468  d, if not set th
+00009590: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000095a0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000095b0: 6c65 206e 616d 6520 6973 2063 6865 636b  le name is check
+000095c0: 6564 2066 6f72 206b 6e6f 776e 2062 696e  ed for known bin
+000095d0: 6172 7920 6669 6c65 2074 7970 650a 0a20  ary file type.. 
+000095e0: 2020 2020 2020 203a 7261 6973 6573 204c         :raises L
+000095f0: 5356 3253 7461 7465 4578 6365 7074 696f  SV2StateExceptio
+00009600: 6e3a 2069 6620 6c6f 6361 6c20 6669 6c65  n: if local file
+00009610: 2063 6f75 6c64 206e 6f74 2062 6520 6f70   could not be op
+00009620: 656e 6564 2c0a 2020 2020 2020 2020 2020  ened,.          
+00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009640: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00009650: 6174 696f 6e20 6469 7265 6374 6f72 7920  ation directory 
+00009660: 636f 756c 6420 6e6f 7420 6265 2061 6363  could not be acc
+00009670: 6573 7365 6420 6f72 0a20 2020 2020 2020  essed or.       
+00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009690: 2020 2020 2020 2020 2020 2020 2064 6573               des
+000096a0: 7469 6e61 7469 6f6e 2066 696c 6520 636f  tination file co
+000096b0: 756c 6420 6e6f 7420 6265 2064 656c 6574  uld not be delet
+000096c0: 6564 0a20 2020 2020 2020 2022 2222 0a20  ed.        """. 
+000096d0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+000096e0: 6c66 2e6c 6f67 696e 286c 632e 4c6f 6769  lf.login(lc.Logi
+000096f0: 6e2e 4649 4c45 5452 414e 5346 4552 293a  n.FILETRANSFER):
+00009700: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009710: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
+00009720: 6728 2263 6f75 6c64 206e 6f74 206c 6f67  g("could not log
+00009730: 2069 6e20 6173 2075 7365 7220 4649 4c45   in as user FILE
+00009740: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00009750: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00009760: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00009770: 6365 286c 6f63 616c 5f70 6174 682c 2028  ce(local_path, (
+00009780: 7374 722c 2929 3a0a 2020 2020 2020 2020  str,)):.        
+00009790: 2020 2020 6c6f 6361 6c5f 6669 6c65 203d      local_file =
+000097a0: 2070 6174 686c 6962 2e50 6174 6828 6c6f   pathlib.Path(lo
+000097b0: 6361 6c5f 7061 7468 290a 2020 2020 2020  cal_path).      
+000097c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000097d0: 2020 2020 6c6f 6361 6c5f 6669 6c65 203d      local_file =
+000097e0: 206c 6f63 616c 5f70 6174 680a 0a20 2020   local_path..   
+000097f0: 2020 2020 2069 6620 6e6f 7420 6c6f 6361       if not loca
+00009800: 6c5f 6669 6c65 2e69 735f 6669 6c65 2829  l_file.is_file()
+00009810: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009820: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
+00009830: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00009840: 2020 2020 2274 6865 2073 7570 706c 6965      "the supplie
+00009850: 6420 7061 7468 2025 7320 6469 6420 6e6f  d path %s did no
+00009860: 7420 7265 736f 6c76 6520 746f 2061 2066  t resolve to a f
+00009870: 696c 6522 2c20 6c6f 6361 6c5f 6669 6c65  ile", local_file
+00009880: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00009890: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000098a0: 204c 5356 3253 7461 7465 4578 6365 7074   LSV2StateExcept
+000098b0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+000098c0: 2020 2020 2022 6c6f 6361 6c20 6669 6c65       "local file
+000098d0: 2064 6f65 7320 6e6f 7420 6578 6973 7421   does not exist!
+000098e0: 207b 7d22 2e66 6f72 6d61 7428 6c6f 6361   {}".format(loca
+000098f0: 6c5f 6669 6c65 2929 0a0a 2020 2020 2020  l_file))..      
+00009900: 2020 7265 6d6f 7465 5f70 6174 6820 3d20    remote_path = 
+00009910: 7265 6d6f 7465 5f70 6174 682e 7265 706c  remote_path.repl
+00009920: 6163 6528 222f 222c 206c 632e 5041 5448  ace("/", lc.PATH
+00009930: 5f53 4550 290a 0a20 2020 2020 2020 2069  _SEP)..        i
+00009940: 6620 6c63 2e50 4154 485f 5345 5020 696e  f lc.PATH_SEP in
+00009950: 2072 656d 6f74 655f 7061 7468 3a0a 2020   remote_path:.  
+00009960: 2020 2020 2020 2020 2020 6966 2072 656d            if rem
+00009970: 6f74 655f 7061 7468 2e65 6e64 7377 6974  ote_path.endswit
+00009980: 6828 6c63 2e50 4154 485f 5345 5029 3a20  h(lc.PATH_SEP): 
+00009990: 2023 206e 6f20 6669 6c65 6e61 6d65 2067   # no filename g
+000099a0: 6976 656e 0a20 2020 2020 2020 2020 2020  iven.           
+000099b0: 2020 2020 2072 656d 6f74 655f 6669 6c65       remote_file
+000099c0: 5f6e 616d 6520 3d20 6c6f 6361 6c5f 6669  _name = local_fi
+000099d0: 6c65 2e6e 616d 650a 2020 2020 2020 2020  le.name.        
+000099e0: 2020 2020 2020 2020 7265 6d6f 7465 5f64          remote_d
+000099f0: 6972 6563 746f 7279 203d 2072 656d 6f74  irectory = remot
+00009a00: 655f 7061 7468 0a20 2020 2020 2020 2020  e_path.         
+00009a10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00009a20: 2020 2020 2020 2020 2072 656d 6f74 655f           remote_
+00009a30: 6669 6c65 5f6e 616d 6520 3d20 7265 6d6f  file_name = remo
+00009a40: 7465 5f70 6174 682e 7370 6c69 7428 6c63  te_path.split(lc
+00009a50: 2e50 4154 485f 5345 5029 5b2d 315d 0a20  .PATH_SEP)[-1]. 
+00009a60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009a70: 656d 6f74 655f 6469 7265 6374 6f72 7920  emote_directory 
+00009a80: 3d20 7265 6d6f 7465 5f70 6174 682e 7273  = remote_path.rs
+00009a90: 7472 6970 2872 656d 6f74 655f 6669 6c65  trip(remote_file
+00009aa0: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
+00009ab0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00009ac0: 6c66 2e63 6861 6e67 655f 6469 7265 6374  lf.change_direct
+00009ad0: 6f72 7928 7265 6d6f 7465 5f64 6972 6563  ory(remote_direc
+00009ae0: 746f 7279 3d72 656d 6f74 655f 6469 7265  tory=remote_dire
+00009af0: 6374 6f72 7929 3a0a 2020 2020 2020 2020  ctory):.        
+00009b00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00009b10: 6520 4c53 5632 5374 6174 6545 7863 6570  e LSV2StateExcep
+00009b20: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00009b40: 6f75 6c64 206e 6f74 206f 7065 6e20 7468  ould not open th
+00009b50: 6520 6465 7374 696e 6174 696f 6e20 6469  e destination di
+00009b60: 7265 6374 6f72 7920 7b7d 222e 666f 726d  rectory {}".form
+00009b70: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b90: 7265 6d6f 7465 5f64 6972 6563 746f 7279  remote_directory
+00009ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009bb0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00009bc0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00009bd0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00009be0: 2020 2020 2020 2020 2020 2072 656d 6f74             remot
+00009bf0: 655f 6669 6c65 5f6e 616d 6520 3d20 7265  e_file_name = re
+00009c00: 6d6f 7465 5f70 6174 680a 2020 2020 2020  mote_path.      
+00009c10: 2020 2020 2020 7265 6d6f 7465 5f64 6972        remote_dir
+00009c20: 6563 746f 7279 203d 2073 656c 662e 6469  ectory = self.di
+00009c30: 7265 6374 6f72 795f 696e 666f 2829 2e70  rectory_info().p
+00009c40: 6174 6820 2023 2067 6574 2070 7764 0a20  ath  # get pwd. 
+00009c50: 2020 2020 2020 2072 656d 6f74 655f 6469         remote_di
+00009c60: 7265 6374 6f72 7920 3d20 7265 6d6f 7465  rectory = remote
+00009c70: 5f64 6972 6563 746f 7279 2e72 7374 7269  _directory.rstri
+00009c80: 7028 6c63 2e50 4154 485f 5345 5029 0a0a  p(lc.PATH_SEP)..
+00009c90: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00009ca0: 656c 662e 6469 7265 6374 6f72 795f 696e  elf.directory_in
+00009cb0: 666f 2872 656d 6f74 655f 6469 7265 6374  fo(remote_direct
+00009cc0: 6f72 7929 3a0a 2020 2020 2020 2020 2020  ory):.          
+00009cd0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e64    self._logger.d
+00009ce0: 6562 7567 280a 2020 2020 2020 2020 2020  ebug(.          
+00009cf0: 2020 2020 2020 2272 656d 6f74 6520 7061        "remote pa
+00009d00: 7468 2064 6f65 7320 6e6f 7420 6578 6973  th does not exis
+00009d10: 742c 2063 7265 6174 6520 6469 7265 6374  t, create direct
+00009d20: 6f72 7928 7329 2229 0a20 2020 2020 2020  ory(s)").       
+00009d30: 2020 2020 2073 656c 662e 6d61 6b65 5f64       self.make_d
+00009d40: 6972 6563 746f 7279 2872 656d 6f74 655f  irectory(remote_
+00009d50: 6469 7265 6374 6f72 7929 0a0a 2020 2020  directory)..    
+00009d60: 2020 2020 7265 6d6f 7465 5f69 6e66 6f20      remote_info 
+00009d70: 3d20 7365 6c66 2e66 696c 655f 696e 666f  = self.file_info
+00009d80: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+00009d90: 6d6f 7465 5f64 6972 6563 746f 7279 202b  mote_directory +
+00009da0: 206c 632e 5041 5448 5f53 4550 202b 2072   lc.PATH_SEP + r
+00009db0: 656d 6f74 655f 6669 6c65 5f6e 616d 6529  emote_file_name)
+00009dc0: 0a0a 2020 2020 2020 2020 6966 2072 656d  ..        if rem
+00009dd0: 6f74 655f 696e 666f 3a0a 2020 2020 2020  ote_info:.      
+00009de0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+00009df0: 6572 2e64 6562 7567 2822 7265 6d6f 7465  er.debug("remote
+00009e00: 2070 6174 6820 6578 6973 7473 2061 6e64   path exists and
+00009e10: 2070 6f69 6e74 7320 746f 2066 696c 6527   points to file'
+00009e20: 7322 290a 2020 2020 2020 2020 2020 2020  s").            
+00009e30: 6966 206f 7665 7272 6964 655f 6669 6c65  if override_file
+00009e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009e50: 2020 6966 206e 6f74 2073 656c 662e 6465    if not self.de
+00009e60: 6c65 7465 5f66 696c 6528 0a20 2020 2020  lete_file(.     
+00009e70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009e80: 656d 6f74 655f 6469 7265 6374 6f72 7920  emote_directory 
+00009e90: 2b20 6c63 2e50 4154 485f 5345 5020 2b20  + lc.PATH_SEP + 
+00009ea0: 7265 6d6f 7465 5f66 696c 655f 6e61 6d65  remote_file_name
 00009eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ec0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00009ed0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00009ee0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00009ef0: 6f67 6765 722e 7761 726e 696e 6728 2272  ogger.warning("r
-00009f00: 656d 6f74 6520 6669 6c65 2061 6c72 6561  emote file alrea
-00009f10: 6479 2065 7869 7374 732c 206f 7665 7272  dy exists, overr
-00009f20: 6964 6520 7761 7320 6e6f 7420 7365 7422  ide was not set"
-00009f30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009f40: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00009f50: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00009f60: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-00009f70: 2020 2020 2020 2020 2272 6561 6479 2074          "ready t
-00009f80: 6f20 7365 6e64 2066 696c 6520 6672 6f6d  o send file from
-00009f90: 2025 7320 746f 2025 7322 2c0a 2020 2020   %s to %s",.    
-00009fa0: 2020 2020 2020 2020 6c6f 6361 6c5f 6669          local_fi
-00009fb0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
-00009fc0: 7265 6d6f 7465 5f64 6972 6563 746f 7279  remote_directory
-00009fd0: 202b 206c 632e 5041 5448 5f53 4550 202b   + lc.PATH_SEP +
-00009fe0: 2072 656d 6f74 655f 6669 6c65 5f6e 616d   remote_file_nam
-00009ff0: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
-0000a000: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-0000a010: 6c6d 2e75 7374 725f 746f 5f62 6128 7265  lm.ustr_to_ba(re
-0000a020: 6d6f 7465 5f64 6972 6563 746f 7279 202b  mote_directory +
-0000a030: 206c 632e 5041 5448 5f53 4550 202b 2072   lc.PATH_SEP + r
-0000a040: 656d 6f74 655f 6669 6c65 5f6e 616d 6529  emote_file_name)
-0000a050: 0a20 2020 2020 2020 2069 6620 6269 6e61  .        if bina
-0000a060: 7279 5f6d 6f64 6520 6f72 206c 6d2e 6973  ry_mode or lm.is
-0000a070: 5f66 696c 655f 6269 6e61 7279 286c 6f63  _file_binary(loc
-0000a080: 616c 5f70 6174 6829 3a0a 2020 2020 2020  al_path):.      
-0000a090: 2020 2020 2020 7061 796c 6f61 642e 6170        payload.ap
-0000a0a0: 7065 6e64 286c 632e 4d4f 4445 5f42 494e  pend(lc.MODE_BIN
-0000a0b0: 4152 5929 0a20 2020 2020 2020 2020 2020  ARY).           
-0000a0c0: 2073 656c 662e 5f6c 6f67 6765 722e 6465   self._logger.de
-0000a0d0: 6275 6728 2273 656c 6563 7469 6e67 2062  bug("selecting b
-0000a0e0: 696e 6172 7920 7472 616e 7366 6572 206d  inary transfer m
-0000a0f0: 6f64 6522 290a 2020 2020 2020 2020 656c  ode").        el
-0000a100: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000a110: 7061 796c 6f61 642e 6170 7065 6e64 286c  payload.append(l
-0000a120: 632e 4d4f 4445 5f4e 4f4e 5f42 494e 290a  c.MODE_NON_BIN).
-0000a130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a140: 2e5f 6c6f 6767 6572 2e64 6562 7567 2822  ._logger.debug("
-0000a150: 7365 6c65 6374 696e 6720 6e6f 6e20 6269  selecting non bi
-0000a160: 6e61 7279 2074 7261 6e73 6665 7220 6d6f  nary transfer mo
-0000a170: 6465 2229 0a0a 2020 2020 2020 2020 7365  de")..        se
-0000a180: 6c66 2e5f 6c6c 636f 6d2e 7465 6c65 6772  lf._llcom.telegr
-0000a190: 616d 280a 2020 2020 2020 2020 2020 2020  am(.            
-0000a1a0: 6c63 2e43 4d44 2e43 5f46 4c2c 0a20 2020  lc.CMD.C_FL,.   
-0000a1b0: 2020 2020 2020 2020 2070 6179 6c6f 6164           payload
-0000a1c0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000a1d0: 2020 2020 2069 6620 7365 6c66 2e5f 6c6c       if self._ll
-0000a1e0: 636f 6d2e 6c61 7374 5f72 6573 706f 6e73  com.last_respons
-0000a1f0: 6520 696e 206c 632e 5253 502e 545f 4f4b  e in lc.RSP.T_OK
-0000a200: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-0000a210: 7468 206c 6f63 616c 5f66 696c 652e 6f70  th local_file.op
-0000a220: 656e 2822 7262 2229 2061 7320 696e 7075  en("rb") as inpu
-0000a230: 745f 6275 6666 6572 3a0a 2020 2020 2020  t_buffer:.      
-0000a240: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-0000a250: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
-0000a260: 2020 2020 2020 2020 2020 2320 7573 6520            # use 
-0000a270: 6375 7272 656e 7420 6275 6666 6572 2073  current buffer s
-0000a280: 697a 6520 6275 7420 7265 6475 6365 2062  ize but reduce b
-0000a290: 7920 3130 2074 6f20 6d61 6b65 2073 7572  y 10 to make sur
-0000a2a0: 6520 6974 2066 6974 7320 746f 6765 7468  e it fits togeth
-0000a2b0: 6572 2077 6974 6820 636f 6d6d 616e 6420  er with command 
-0000a2c0: 616e 6420 7369 7a65 0a20 2020 2020 2020  and size.       
-0000a2d0: 2020 2020 2020 2020 2020 2020 2062 7566               buf
-0000a2e0: 6665 7220 3d20 6279 7465 6172 7261 7928  fer = bytearray(
-0000a2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a300: 2020 2020 2020 2020 2069 6e70 7574 5f62           input_b
-0000a310: 7566 6665 722e 7265 6164 2873 656c 662e  uffer.read(self.
-0000a320: 5f6c 6c63 6f6d 2e62 7566 6665 725f 7369  _llcom.buffer_si
-0000a330: 7a65 202d 2038 202d 2032 290a 2020 2020  ze - 8 - 2).    
-0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a350: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a360: 2020 2020 2020 6966 206e 6f74 2062 7566        if not buf
-0000a370: 6665 723a 0a20 2020 2020 2020 2020 2020  fer:.           
-0000a380: 2020 2020 2020 2020 2020 2020 2023 2066               # f
-0000a390: 696e 6973 6865 6420 7265 6164 696e 6720  inished reading 
-0000a3a0: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
-0000a3b0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-0000a3c0: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
-0000a3d0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6c          self._ll
-0000a3e0: 636f 6d2e 7465 6c65 6772 616d 280a 2020  com.telegram(.  
-0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a400: 2020 2020 2020 6c63 2e52 5350 2e53 5f46        lc.RSP.S_F
-0000a410: 4c2c 0a20 2020 2020 2020 2020 2020 2020  L,.             
-0000a420: 2020 2020 2020 2020 2020 2062 7566 6665             buffe
-0000a430: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000a440: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000a450: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a460: 7365 6c66 2e5f 6c6c 636f 6d2e 6c61 7374  self._llcom.last
-0000a470: 5f72 6573 706f 6e73 6520 696e 206c 632e  _response in lc.
-0000a480: 5253 502e 545f 4f4b 3a0a 2020 2020 2020  RSP.T_OK:.      
+00009ec0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00009ed0: 2020 2020 2020 2020 7261 6973 6520 4c53          raise LS
+00009ee0: 5632 5374 6174 6545 7863 6570 7469 6f6e  V2StateException
+00009ef0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00009f00: 2020 2020 2020 2020 2020 2273 6f6d 6574            "somet
+00009f10: 6869 6e67 2077 656e 7420 7772 6f6e 6720  hing went wrong 
+00009f20: 7768 696c 6520 6465 6c65 7469 6e67 2066  while deleting f
+00009f30: 696c 6520 7b7d 222e 666f 726d 6174 280a  ile {}".format(.
+00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f50: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
+00009f60: 7465 5f64 6972 6563 746f 7279 202b 206c  te_directory + l
+00009f70: 632e 5041 5448 5f53 4550 202b 2072 656d  c.PATH_SEP + rem
+00009f80: 6f74 655f 6669 6c65 5f6e 616d 650a 2020  ote_file_name.  
+00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fa0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00009fb0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00009fc0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fe0: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
+00009ff0: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
+0000a000: 2020 2020 2020 2020 2020 2272 656d 6f74            "remot
+0000a010: 6520 6669 6c65 2061 6c72 6561 6479 2065  e file already e
+0000a020: 7869 7374 732c 206f 7665 7272 6964 6520  xists, override 
+0000a030: 7761 7320 6e6f 7420 7365 7422 290a 2020  was not set").  
+0000a040: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000a050: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+0000a060: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+0000a070: 2e64 6562 7567 280a 2020 2020 2020 2020  .debug(.        
+0000a080: 2020 2020 2272 6561 6479 2074 6f20 7365      "ready to se
+0000a090: 6e64 2066 696c 6520 6672 6f6d 2025 7320  nd file from %s 
+0000a0a0: 746f 2025 7322 2c0a 2020 2020 2020 2020  to %s",.        
+0000a0b0: 2020 2020 6c6f 6361 6c5f 6669 6c65 2c0a      local_file,.
+0000a0c0: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
+0000a0d0: 7465 5f64 6972 6563 746f 7279 202b 206c  te_directory + l
+0000a0e0: 632e 5041 5448 5f53 4550 202b 2072 656d  c.PATH_SEP + rem
+0000a0f0: 6f74 655f 6669 6c65 5f6e 616d 652c 0a20  ote_file_name,. 
+0000a100: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000a110: 2020 7061 796c 6f61 6420 3d20 6c6d 2e75    payload = lm.u
+0000a120: 7374 725f 746f 5f62 6128 0a20 2020 2020  str_to_ba(.     
+0000a130: 2020 2020 2020 2072 656d 6f74 655f 6469         remote_di
+0000a140: 7265 6374 6f72 7920 2b20 6c63 2e50 4154  rectory + lc.PAT
+0000a150: 485f 5345 5020 2b20 7265 6d6f 7465 5f66  H_SEP + remote_f
+0000a160: 696c 655f 6e61 6d65 290a 2020 2020 2020  ile_name).      
+0000a170: 2020 6966 2062 696e 6172 795f 6d6f 6465    if binary_mode
+0000a180: 206f 7220 6c6d 2e69 735f 6669 6c65 5f62   or lm.is_file_b
+0000a190: 696e 6172 7928 6c6f 6361 6c5f 7061 7468  inary(local_path
+0000a1a0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+0000a1b0: 6179 6c6f 6164 2e61 7070 656e 6428 6c63  ayload.append(lc
+0000a1c0: 2e4d 4f44 455f 4249 4e41 5259 290a 2020  .MODE_BINARY).  
+0000a1d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a1e0: 6c6f 6767 6572 2e64 6562 7567 2822 7365  logger.debug("se
+0000a1f0: 6c65 6374 696e 6720 6269 6e61 7279 2074  lecting binary t
+0000a200: 7261 6e73 6665 7220 6d6f 6465 2229 0a20  ransfer mode"). 
+0000a210: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a220: 2020 2020 2020 2020 2070 6179 6c6f 6164           payload
+0000a230: 2e61 7070 656e 6428 6c63 2e4d 4f44 455f  .append(lc.MODE_
+0000a240: 4e4f 4e5f 4249 4e29 0a20 2020 2020 2020  NON_BIN).       
+0000a250: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+0000a260: 722e 6465 6275 6728 2273 656c 6563 7469  r.debug("selecti
+0000a270: 6e67 206e 6f6e 2062 696e 6172 7920 7472  ng non binary tr
+0000a280: 616e 7366 6572 206d 6f64 6522 290a 0a20  ansfer mode").. 
+0000a290: 2020 2020 2020 2073 656c 662e 5f6c 6c63         self._llc
+0000a2a0: 6f6d 2e74 656c 6567 7261 6d28 0a20 2020  om.telegram(.   
+0000a2b0: 2020 2020 2020 2020 206c 632e 434d 442e           lc.CMD.
+0000a2c0: 435f 464c 2c0a 2020 2020 2020 2020 2020  C_FL,.          
+0000a2d0: 2020 7061 796c 6f61 642c 0a20 2020 2020    payload,.     
+0000a2e0: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+0000a2f0: 2073 656c 662e 5f6c 6c63 6f6d 2e6c 6173   self._llcom.las
+0000a300: 745f 7265 7370 6f6e 7365 2069 6e20 6c63  t_response in lc
+0000a310: 2e52 5350 2e54 5f4f 4b3a 0a20 2020 2020  .RSP.T_OK:.     
+0000a320: 2020 2020 2020 2077 6974 6820 6c6f 6361         with loca
+0000a330: 6c5f 6669 6c65 2e6f 7065 6e28 2272 6222  l_file.open("rb"
+0000a340: 2920 6173 2069 6e70 7574 5f62 7566 6665  ) as input_buffe
+0000a350: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0000a360: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
+0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a380: 2020 2023 2075 7365 2063 7572 7265 6e74     # use current
+0000a390: 2062 7566 6665 7220 7369 7a65 2062 7574   buffer size but
+0000a3a0: 2072 6564 7563 6520 6279 2031 3020 746f   reduce by 10 to
+0000a3b0: 206d 616b 6520 7375 7265 2069 7420 6669   make sure it fi
+0000a3c0: 7473 2074 6f67 6574 6865 7220 7769 7468  ts together with
+0000a3d0: 2063 6f6d 6d61 6e64 2061 6e64 2073 697a   command and siz
+0000a3e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000a3f0: 2020 2020 2020 6275 6666 6572 203d 2062        buffer = b
+0000a400: 7974 6561 7272 6179 280a 2020 2020 2020  ytearray(.      
+0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a420: 2020 696e 7075 745f 6275 6666 6572 2e72    input_buffer.r
+0000a430: 6561 6428 7365 6c66 2e5f 6c6c 636f 6d2e  ead(self._llcom.
+0000a440: 6275 6666 6572 5f73 697a 6520 2d20 3820  buffer_size - 8 
+0000a450: 2d20 3229 0a20 2020 2020 2020 2020 2020  - 2).           
+0000a460: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000a470: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a480: 6620 6e6f 7420 6275 6666 6572 3a0a 2020  f not buffer:.  
 0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
-0000a4b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000a4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a4d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000a4e0: 2e5f 6c6c 636f 6d2e 6c61 7374 5f72 6573  ._llcom.last_res
-0000a4f0: 706f 6e73 6520 3d3d 206c 632e 5253 502e  ponse == lc.RSP.
-0000a500: 545f 4552 3a0a 2020 2020 2020 2020 2020  T_ER:.          
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e69    self._logger.i
-0000a530: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 2022 636f 6e74 726f 6c20 7265       "control re
-0000a560: 7475 726e 6564 2065 7272 6f72 2027 2573  turned error '%s
-0000a570: 2720 7768 6963 6820 7472 616e 736c 6174  ' which translat
-0000a580: 6573 2074 6f20 2725 7327 222c 0a20 2020  es to '%s'",.   
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a5b0: 662e 6c61 7374 5f65 7272 6f72 2c0a 2020  f.last_error,.  
+0000a4a0: 2020 2020 2020 2320 6669 6e69 7368 6564        # finished
+0000a4b0: 2072 6561 6469 6e67 2066 696c 650a 2020   reading file.  
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4d0: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
+0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4f0: 2073 656c 662e 5f6c 6c63 6f6d 2e74 656c   self._llcom.tel
+0000a500: 6567 7261 6d28 0a20 2020 2020 2020 2020  egram(.         
+0000a510: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000a520: 632e 5253 502e 535f 464c 2c0a 2020 2020  c.RSP.S_FL,.    
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a540: 2020 2020 6275 6666 6572 2c0a 2020 2020      buffer,.    
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a570: 2020 2020 2020 6966 2073 656c 662e 5f6c        if self._l
+0000a580: 6c63 6f6d 2e6c 6173 745f 7265 7370 6f6e  lcom.last_respon
+0000a590: 7365 2069 6e20 6c63 2e52 5350 2e54 5f4f  se in lc.RSP.T_O
+0000a5a0: 4b3a 0a20 2020 2020 2020 2020 2020 2020  K:.             
+0000a5b0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
 0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
-0000a5e0: 2e67 6574 5f65 7272 6f72 5f74 6578 7428  .get_error_text(
-0000a5f0: 7365 6c66 2e6c 6173 745f 6572 726f 7229  self.last_error)
-0000a600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a610: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000a5d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 6966 2073 656c 662e 5f6c 6c63 6f6d    if self._llcom
+0000a600: 2e6c 6173 745f 7265 7370 6f6e 7365 203d  .last_response =
+0000a610: 3d20 6c63 2e52 5350 2e54 5f45 523a 0a20  = lc.RSP.T_ER:. 
 0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a650: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000a660: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
-0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a690: 2263 6f75 6c64 206e 6f74 2073 656e 6420  "could not send 
-0000a6a0: 6461 7461 2c20 7265 6365 6976 6564 2075  data, received u
-0000a6b0: 6e65 7870 6563 7465 6420 7265 7370 6f6e  nexpected respon
-0000a6c0: 7365 2027 2573 2722 2c0a 2020 2020 2020  se '%s'",.      
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000a6f0: 6c6c 636f 6d2e 6c61 7374 5f72 6573 706f  llcom.last_respo
-0000a700: 6e73 652c 0a20 2020 2020 2020 2020 2020  nse,.           
-0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a720: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000a730: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a740: 6e20 4661 6c73 650a 0a20 2020 2020 2020  n False..       
-0000a750: 2020 2020 2023 2073 6967 6e61 6c20 7468       # signal th
-0000a760: 6174 206e 6f20 6d6f 7265 2064 6174 6120  at no more data 
-0000a770: 6973 2062 6569 6e67 2073 656e 740a 2020  is being sent.  
-0000a780: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000a790: 662e 5f73 6563 7572 655f 6669 6c65 5f73  f._secure_file_s
-0000a7a0: 656e 643a 0a20 2020 2020 2020 2020 2020  end:.           
-0000a7b0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0000a7c0: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
-0000a7d0: 2e52 5350 2e54 5f46 442c 204e 6f6e 652c  .RSP.T_FD, None,
-0000a7e0: 206c 632e 5253 502e 545f 4f4b 293a 0a20   lc.RSP.T_OK):. 
+0000a630: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a640: 5f6c 6f67 6765 722e 696e 666f 280a 2020  _logger.info(.  
+0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+0000a670: 6f6e 7472 6f6c 2072 6574 7572 6e65 6420  ontrol returned 
+0000a680: 6572 726f 7220 2725 7327 2077 6869 6368  error '%s' which
+0000a690: 2074 7261 6e73 6c61 7465 7320 746f 2027   translates to '
+0000a6a0: 2573 2722 2c0a 2020 2020 2020 2020 2020  %s'",.          
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 2020 2020 7365 6c66 2e6c 6173 745f        self.last_
+0000a6d0: 6572 726f 722c 0a20 2020 2020 2020 2020  error,.         
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6f0: 2020 2020 2020 206c 742e 6765 745f 6572         lt.get_er
+0000a700: 726f 725f 7465 7874 2873 656c 662e 6c61  ror_text(self.la
+0000a710: 7374 5f65 7272 6f72 292c 0a20 2020 2020  st_error),.     
+0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a730: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a750: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a770: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0000a780: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7a0: 2020 2020 2020 2020 2022 636f 756c 6420           "could 
+0000a7b0: 6e6f 7420 7365 6e64 2064 6174 612c 2072  not send data, r
+0000a7c0: 6563 6569 7665 6420 756e 6578 7065 6374  eceived unexpect
+0000a7d0: 6564 2072 6573 706f 6e73 6520 2725 7327  ed response '%s'
+0000a7e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
 0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a800: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
-0000a810: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+0000a800: 2020 2073 656c 662e 5f6c 6c63 6f6d 2e6c     self._llcom.l
+0000a810: 6173 745f 7265 7370 6f6e 7365 2c0a 2020  ast_response,.  
 0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a830: 2022 636f 756c 6420 6e6f 7420 7365 6e64   "could not send
-0000a840: 2065 6e64 206f 6620 7472 616e 736d 6973   end of transmis
-0000a850: 7369 6f6e 2074 656c 6567 7261 6d2c 2067  sion telegram, g
-0000a860: 6f74 2072 6573 706f 6e73 6520 2725 7327  ot response '%s'
-0000a870: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000a880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a890: 5f6c 6c63 6f6d 2e6c 6173 745f 7265 7370  _llcom.last_resp
-0000a8a0: 6f6e 7365 2c0a 2020 2020 2020 2020 2020  onse,.          
-0000a8b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8d0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-0000a8e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a900: 6620 6e6f 7420 7365 6c66 2e5f 7365 6e64  f not self._send
-0000a910: 5f72 6563 6976 6528 6c63 2e52 5350 2e54  _recive(lc.RSP.T
-0000a920: 5f46 442c 204e 6f6e 652c 206c 632e 5253  _FD, None, lc.RS
-0000a930: 502e 4e4f 4e45 293a 0a20 2020 2020 2020  P.NONE):.       
-0000a940: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a950: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
-0000a960: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-0000a970: 2020 2020 2020 2020 2020 2022 636f 756c             "coul
-0000a980: 6420 6e6f 7420 7365 6e64 2065 6e64 206f  d not send end o
-0000a990: 6620 7472 616e 736d 6973 7369 6f6e 2074  f transmission t
-0000a9a0: 656c 6567 7261 6d2c 2067 6f74 2072 6573  elegram, got res
-0000a9b0: 706f 6e73 6520 2725 7327 222c 0a20 2020  ponse '%s'",.   
+0000a830: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a850: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0000a860: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000a870: 7369 676e 616c 2074 6861 7420 6e6f 206d  signal that no m
+0000a880: 6f72 6520 6461 7461 2069 7320 6265 696e  ore data is bein
+0000a890: 6720 7365 6e74 0a20 2020 2020 2020 2020  g sent.         
+0000a8a0: 2020 2069 6620 7365 6c66 2e5f 7365 6375     if self._secu
+0000a8b0: 7265 5f66 696c 655f 7365 6e64 3a0a 2020  re_file_send:.  
+0000a8c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000a8d0: 206e 6f74 2073 656c 662e 5f73 656e 645f   not self._send_
+0000a8e0: 7265 6369 7665 286c 632e 5253 502e 545f  recive(lc.RSP.T_
+0000a8f0: 4644 2c20 4e6f 6e65 2c20 6c63 2e52 5350  FD, None, lc.RSP
+0000a900: 2e54 5f4f 4b29 3a0a 2020 2020 2020 2020  .T_OK):.        
+0000a910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a920: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
+0000a930: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a940: 2020 2020 2020 2020 2020 2263 6f75 6c64            "could
+0000a950: 206e 6f74 2073 656e 6420 656e 6420 6f66   not send end of
+0000a960: 2074 7261 6e73 6d69 7373 696f 6e20 7465   transmission te
+0000a970: 6c65 6772 616d 2c20 676f 7420 7265 7370  legram, got resp
+0000a980: 6f6e 7365 2027 2573 2722 2c0a 2020 2020  onse '%s'",.    
+0000a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9a0: 2020 2020 7365 6c66 2e5f 6c6c 636f 6d2e      self._llcom.
+0000a9b0: 6c61 7374 5f72 6573 706f 6e73 652c 0a20  last_response,. 
 0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9d0: 2020 2020 2073 656c 662e 5f6c 6c63 6f6d       self._llcom
-0000a9e0: 2e6c 6173 745f 7265 7370 6f6e 7365 2c0a  .last_response,.
-0000a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000aa10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000aa20: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-0000aa30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000aa40: 2020 6966 2073 656c 662e 5f6c 6c63 6f6d    if self._llcom
-0000aa50: 2e6c 6173 745f 7265 7370 6f6e 7365 2069  .last_response i
-0000aa60: 7320 6c63 2e52 5350 2e54 5f45 523a 0a20  s lc.RSP.T_ER:. 
-0000aa70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000aa80: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
-0000aa90: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
-0000aaa0: 2020 2020 2020 2020 2022 6572 726f 7220           "error 
-0000aab0: 7265 6365 6976 6564 2c20 2573 2027 2573  received, %s '%s
-0000aac0: 2722 2c0a 2020 2020 2020 2020 2020 2020  '",.            
-0000aad0: 2020 2020 2020 2020 7365 6c66 2e6c 6173          self.las
-0000aae0: 745f 6572 726f 722c 0a20 2020 2020 2020  t_error,.       
-0000aaf0: 2020 2020 2020 2020 2020 2020 206c 742e               lt.
-0000ab00: 6765 745f 6572 726f 725f 7465 7874 2873  get_error_text(s
-0000ab10: 656c 662e 6c61 7374 5f65 7272 6f72 292c  elf.last_error),
-0000ab20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab30: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-0000ab40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000ab50: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-0000ab60: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
-0000ab70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000ab80: 636f 756c 6420 6e6f 7420 7365 6e64 2066  could not send f
-0000ab90: 696c 6520 7769 7468 2065 7272 6f72 2025  ile with error %
-0000aba0: 7322 2c20 7365 6c66 2e5f 6c6c 636f 6d2e  s", self._llcom.
-0000abb0: 6c61 7374 5f72 6573 706f 6e73 650a 2020  last_response.  
-0000abc0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000abd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000abe0: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-0000abf0: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-0000ac00: 2020 2064 6566 2072 6563 6976 655f 6669     def recive_fi
-0000ac10: 6c65 280a 2020 2020 2020 2020 7365 6c66  le(.        self
-0000ac20: 2c0a 2020 2020 2020 2020 7265 6d6f 7465  ,.        remote
-0000ac30: 5f70 6174 683a 2073 7472 2c0a 2020 2020  _path: str,.    
-0000ac40: 2020 2020 6c6f 6361 6c5f 7061 7468 3a20      local_path: 
-0000ac50: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-0000ac60: 6962 2e50 6174 685d 2c0a 2020 2020 2020  ib.Path],.      
-0000ac70: 2020 6f76 6572 7269 6465 5f66 696c 653a    override_file:
-0000ac80: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-0000ac90: 2020 2020 2020 2062 696e 6172 795f 6d6f         binary_mo
-0000aca0: 6465 3a20 626f 6f6c 203d 2046 616c 7365  de: bool = False
-0000acb0: 2c0a 2020 2020 2920 2d3e 2062 6f6f 6c3a  ,.    ) -> bool:
-0000acc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000acd0: 2020 2020 2044 6f77 6e6c 6f61 6420 6120       Download a 
-0000ace0: 6669 6c65 2066 726f 6d20 636f 6e74 726f  file from contro
-0000acf0: 6c2e 0a20 2020 2020 2020 2052 6571 7569  l..        Requi
-0000ad00: 7265 7320 6163 6365 7373 206c 6576 656c  res access level
-0000ad10: 2060 6046 494c 4554 5241 4e53 4645 5260   ``FILETRANSFER`
-0000ad20: 6020 746f 2077 6f72 6b2e 0a20 2020 2020  ` to work..     
-0000ad30: 2020 2052 6574 7572 6e73 2060 6054 7275     Returns ``Tru
-0000ad40: 6560 6020 6966 2063 6f6d 706c 6574 6564  e`` if completed
-0000ad50: 2073 7563 6365 7373 6675 6c6c 792e 0a0a   successfully...
-0000ad60: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
-0000ad70: 656d 6f74 655f 7061 7468 3a20 7061 7468  emote_path: path
-0000ad80: 206f 6620 6669 6c65 206f 6e20 7468 6520   of file on the 
-0000ad90: 636f 6e74 726f 6c0a 2020 2020 2020 2020  control.        
-0000ada0: 3a70 6172 616d 206c 6f63 616c 5f70 6174  :param local_pat
-0000adb0: 683a 206c 6f63 616c 2070 6174 6820 6f66  h: local path of
-0000adc0: 2064 6573 7469 6e61 7469 6f6e 2077 6974   destination wit
-0000add0: 6820 6f72 2077 6974 686f 7574 2066 696c  h or without fil
-0000ade0: 6520 6e61 6d65 0a20 2020 2020 2020 203a  e name.        :
-0000adf0: 7061 7261 6d20 6f76 6572 7269 6465 5f66  param override_f
-0000ae00: 696c 653a 2066 6c61 6720 6966 2066 696c  ile: flag if fil
-0000ae10: 6520 7368 6f75 6c64 2062 6520 7265 706c  e should be repl
-0000ae20: 6163 6564 2069 6620 6974 2061 6c72 6561  aced if it alrea
-0000ae30: 6479 2065 7869 7374 730a 2020 2020 2020  dy exists.      
-0000ae40: 2020 3a70 6172 616d 2062 696e 6172 795f    :param binary_
-0000ae50: 6d6f 6465 3a20 666c 6167 2069 6620 6269  mode: flag if bi
-0000ae60: 6e61 7279 2074 7261 6e73 6665 7220 6d6f  nary transfer mo
-0000ae70: 6465 2073 686f 756c 6420 6265 2075 7365  de should be use
-0000ae80: 642c 2069 6620 6e6f 7420 7365 7420 7468  d, if not set th
-0000ae90: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000aea0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000aeb0: 6c65 206e 616d 6520 6973 2063 6865 636b  le name is check
-0000aec0: 6564 2066 6f72 206b 6e6f 776e 2062 696e  ed for known bin
-0000aed0: 6172 7920 6669 6c65 2074 7970 650a 2020  ary file type.  
-0000aee0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000aef0: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
-0000af00: 6769 6e28 6c63 2e4c 6f67 696e 2e46 494c  gin(lc.Login.FIL
-0000af10: 4554 5241 4e53 4645 5229 3a0a 2020 2020  ETRANSFER):.    
-0000af20: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0000af30: 6767 6572 2e77 6172 6e69 6e67 2822 636f  gger.warning("co
-0000af40: 756c 6420 6e6f 7420 6c6f 6720 696e 2061  uld not log in a
-0000af50: 7320 7573 6572 2046 494c 4522 290a 2020  s user FILE").  
-0000af60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000af70: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-0000af80: 6966 2069 7369 6e73 7461 6e63 6528 6c6f  if isinstance(lo
-0000af90: 6361 6c5f 7061 7468 2c20 2873 7472 2c29  cal_path, (str,)
-0000afa0: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
-0000afb0: 6f63 616c 5f66 696c 6520 3d20 7061 7468  ocal_file = path
-0000afc0: 6c69 622e 5061 7468 286c 6f63 616c 5f70  lib.Path(local_p
-0000afd0: 6174 6829 0a20 2020 2020 2020 2065 6c73  ath).        els
-0000afe0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-0000aff0: 6f63 616c 5f66 696c 6520 3d20 6c6f 6361  ocal_file = loca
-0000b000: 6c5f 7061 7468 0a0a 2020 2020 2020 2020  l_path..        
-0000b010: 7265 6d6f 7465 5f70 6174 6820 3d20 7265  remote_path = re
-0000b020: 6d6f 7465 5f70 6174 682e 7265 706c 6163  mote_path.replac
-0000b030: 6528 222f 222c 206c 632e 5041 5448 5f53  e("/", lc.PATH_S
-0000b040: 4550 290a 2020 2020 2020 2020 7265 6d6f  EP).        remo
-0000b050: 7465 5f66 696c 655f 696e 666f 203d 2073  te_file_info = s
-0000b060: 656c 662e 6669 6c65 5f69 6e66 6f28 7265  elf.file_info(re
-0000b070: 6d6f 7465 5f70 6174 6829 0a20 2020 2020  mote_path).     
-0000b080: 2020 2069 6620 6e6f 7420 7265 6d6f 7465     if not remote
-0000b090: 5f66 696c 655f 696e 666f 3a0a 2020 2020  _file_info:.    
-0000b0a0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0000b0b0: 6767 6572 2e77 6172 6e69 6e67 2822 7265  gger.warning("re
-0000b0c0: 6d6f 7465 2066 696c 6520 646f 6573 206e  mote file does n
-0000b0d0: 6f74 2065 7869 7374 3a20 2573 222c 2072  ot exist: %s", r
-0000b0e0: 656d 6f74 655f 7061 7468 290a 2020 2020  emote_path).    
-0000b0f0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0000b100: 616c 7365 0a0a 2020 2020 2020 2020 6966  alse..        if
-0000b110: 206c 6f63 616c 5f66 696c 652e 6973 5f64   local_file.is_d
-0000b120: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
-0000b130: 2020 6c6f 6361 6c5f 6669 6c65 2e6a 6f69    local_file.joi
-0000b140: 6e70 6174 6828 7265 6d6f 7465 5f70 6174  npath(remote_pat
-0000b150: 682e 7370 6c69 7428 222f 2229 5b2d 315d  h.split("/")[-1]
-0000b160: 290a 2020 2020 2020 2020 656c 6966 206c  ).        elif l
-0000b170: 6f63 616c 5f66 696c 652e 6973 5f66 696c  ocal_file.is_fil
-0000b180: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
-0000b190: 2023 2073 656c 662e 5f6c 6f67 6765 722e   # self._logger.
-0000b1a0: 6465 6275 6728 226c 6f63 616c 2070 6174  debug("local pat
-0000b1b0: 6820 6578 6973 7473 2061 6e64 2070 6f69  h exists and poi
-0000b1c0: 6e74 7320 746f 2066 696c 6522 290a 2020  nts to file").  
-0000b1d0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000b1e0: 206f 7665 7272 6964 655f 6669 6c65 3a0a   override_file:.
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b200: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-0000b210: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
-0000b220: 2020 2020 2020 2020 2020 226c 6f63 616c            "local
-0000b230: 2066 696c 6520 616c 7265 6164 7920 6578   file already ex
-0000b240: 6973 7473 2061 6e64 206f 7665 7272 6964  ists and overrid
-0000b250: 6520 7761 7320 6e6f 7420 7365 742e 206e  e was not set. n
-0000b260: 6f74 6869 6e67 2074 6f20 646f 220a 2020  othing to do".  
-0000b270: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-0000b2a0: 2020 2020 2020 2020 206c 6f63 616c 5f66           local_f
-0000b2b0: 696c 652e 756e 6c69 6e6b 2829 0a0a 2020  ile.unlink()..  
-0000b2c0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-0000b2d0: 6572 2e64 6562 7567 2822 6c6f 6164 696e  er.debug("loadin
-0000b2e0: 6720 6669 6c65 2066 726f 6d20 2573 2074  g file from %s t
-0000b2f0: 6f20 2573 222c 2072 656d 6f74 655f 7061  o %s", remote_pa
-0000b300: 7468 2c20 6c6f 6361 6c5f 6669 6c65 290a  th, local_file).
-0000b310: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000b320: 203d 206c 6d2e 7573 7472 5f74 6f5f 6261   = lm.ustr_to_ba
-0000b330: 2872 656d 6f74 655f 7061 7468 290a 0a20  (remote_path).. 
-0000b340: 2020 2020 2020 2069 6620 6269 6e61 7279         if binary
-0000b350: 5f6d 6f64 6520 6f72 206c 6d2e 6973 5f66  _mode or lm.is_f
-0000b360: 696c 655f 6269 6e61 7279 2872 656d 6f74  ile_binary(remot
-0000b370: 655f 7061 7468 293a 0a20 2020 2020 2020  e_path):.       
-0000b380: 2020 2020 2070 6179 6c6f 6164 2e61 7070       payload.app
-0000b390: 656e 6428 6c63 2e4d 4f44 455f 4249 4e41  end(lc.MODE_BINA
-0000b3a0: 5259 2920 2023 2066 6f72 6365 2062 696e  RY)  # force bin
-0000b3b0: 6172 7920 7472 616e 7366 6572 0a20 2020  ary transfer.   
-0000b3c0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0000b3d0: 6f67 6765 722e 6465 6275 6728 2275 7369  ogger.debug("usi
-0000b3e0: 6e67 2062 696e 6172 7920 7472 616e 7366  ng binary transf
-0000b3f0: 6572 206d 6f64 6522 290a 2020 2020 2020  er mode").      
-0000b400: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000b410: 2020 2020 7061 796c 6f61 642e 6170 7065      payload.appe
-0000b420: 6e64 286c 632e 4d4f 4445 5f4e 4f4e 5f42  nd(lc.MODE_NON_B
-0000b430: 494e 290a 2020 2020 2020 2020 2020 2020  IN).            
-0000b440: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
-0000b450: 7567 2822 7573 696e 6720 6e6f 6e20 6269  ug("using non bi
-0000b460: 6e61 7279 2074 7261 6e73 6665 7220 6d6f  nary transfer mo
-0000b470: 6465 2229 0a0a 2020 2020 2020 2020 636f  de")..        co
-0000b480: 6e74 656e 7420 3d20 7365 6c66 2e5f 6c6c  ntent = self._ll
-0000b490: 636f 6d2e 7465 6c65 6772 616d 280a 2020  com.telegram(.  
-0000b4a0: 2020 2020 2020 2020 2020 6c63 2e43 4d44            lc.CMD
-0000b4b0: 2e52 5f46 4c2c 0a20 2020 2020 2020 2020  .R_FL,.         
-0000b4c0: 2020 2070 6179 6c6f 6164 2c0a 2020 2020     payload,.    
-0000b4d0: 2020 2020 290a 0a20 2020 2020 2020 2077      )..        w
-0000b4e0: 6974 6820 6c6f 6361 6c5f 6669 6c65 2e6f  ith local_file.o
-0000b4f0: 7065 6e28 2277 6222 2920 6173 206f 7574  pen("wb") as out
-0000b500: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-0000b510: 2020 2069 6620 7365 6c66 2e5f 6c6c 636f     if self._llco
-0000b520: 6d2e 6c61 7374 5f72 6573 706f 6e73 6520  m.last_response 
-0000b530: 696e 206c 632e 5253 502e 535f 464c 3a0a  in lc.RSP.S_FL:.
-0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 6966 2062 696e 6172 795f 6d6f 6465 3a0a  if binary_mode:.
-0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b570: 2020 2020 6f75 745f 6669 6c65 2e77 7269      out_file.wri
-0000b580: 7465 2863 6f6e 7465 6e74 290a 2020 2020  te(content).    
-0000b590: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b5a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b5b0: 2020 2020 2020 6f75 745f 6669 6c65 2e77        out_file.w
-0000b5c0: 7269 7465 2863 6f6e 7465 6e74 2e72 6570  rite(content.rep
-0000b5d0: 6c61 6365 2862 225c 7830 3022 2c20 6222  lace(b"\x00", b"
-0000b5e0: 5c72 5c6e 2229 290a 2020 2020 2020 2020  \r\n")).        
-0000b5f0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0000b600: 6767 6572 2e64 6562 7567 2822 7265 6365  gger.debug("rece
-0000b610: 6976 6564 2066 6972 7374 2062 6c6f 636b  ived first block
-0000b620: 206f 6620 6669 6c65 2066 696c 6520 2573   of file file %s
-0000b630: 222c 2072 656d 6f74 655f 7061 7468 290a  ", remote_path).
-0000b640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b650: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
-0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b670: 2063 6f6e 7465 6e74 203d 2073 656c 662e   content = self.
-0000b680: 5f6c 6c63 6f6d 2e74 656c 6567 7261 6d28  _llcom.telegram(
-0000b690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b6a0: 2020 2020 2020 2020 206c 632e 5253 502e           lc.RSP.
-0000b6b0: 545f 4f4b 2c0a 2020 2020 2020 2020 2020  T_OK,.          
-0000b6c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6e0: 6966 2073 656c 662e 5f6c 6c63 6f6d 2e6c  if self._llcom.l
-0000b6f0: 6173 745f 7265 7370 6f6e 7365 2069 6e20  ast_response in 
-0000b700: 6c63 2e52 5350 2e53 5f46 4c3a 0a20 2020  lc.RSP.S_FL:.   
-0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b720: 2020 2020 2069 6620 6269 6e61 7279 5f6d       if binary_m
-0000b730: 6f64 653a 0a20 2020 2020 2020 2020 2020  ode:.           
+0000a9d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000a9e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a9f0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+0000aa00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000aa10: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0000aa20: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
+0000aa30: 286c 632e 5253 502e 545f 4644 2c20 4e6f  (lc.RSP.T_FD, No
+0000aa40: 6e65 2c20 6c63 2e52 5350 2e4e 4f4e 4529  ne, lc.RSP.NONE)
+0000aa50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000aa60: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+0000aa70: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
+0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa90: 2020 2020 2263 6f75 6c64 206e 6f74 2073      "could not s
+0000aaa0: 656e 6420 656e 6420 6f66 2074 7261 6e73  end end of trans
+0000aab0: 6d69 7373 696f 6e20 7465 6c65 6772 616d  mission telegram
+0000aac0: 2c20 676f 7420 7265 7370 6f6e 7365 2027  , got response '
+0000aad0: 2573 2722 2c0a 2020 2020 2020 2020 2020  %s'",.          
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000aaf0: 6c66 2e5f 6c6c 636f 6d2e 6c61 7374 5f72  lf._llcom.last_r
+0000ab00: 6573 706f 6e73 652c 0a20 2020 2020 2020  esponse,.       
+0000ab10: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab30: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0000ab40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000ab50: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000ab60: 6c66 2e5f 6c6c 636f 6d2e 6c61 7374 5f72  lf._llcom.last_r
+0000ab70: 6573 706f 6e73 6520 6973 206c 632e 5253  esponse is lc.RS
+0000ab80: 502e 545f 4552 3a0a 2020 2020 2020 2020  P.T_ER:.        
+0000ab90: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+0000aba0: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 2265 7272 6f72 2072 6563 6569 7665    "error receive
+0000abd0: 642c 2025 7320 2725 7327 222c 0a20 2020  d, %s '%s'",.   
+0000abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abf0: 2073 656c 662e 6c61 7374 5f65 7272 6f72   self.last_error
+0000ac00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ac10: 2020 2020 2020 6c74 2e67 6574 5f65 7272        lt.get_err
+0000ac20: 6f72 5f74 6578 7428 7365 6c66 2e6c 6173  or_text(self.las
+0000ac30: 745f 6572 726f 7229 2c0a 2020 2020 2020  t_error),.      
+0000ac40: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000ac50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ac60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ac70: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
+0000ac80: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000ac90: 2020 2020 2020 2020 2263 6f75 6c64 206e          "could n
+0000aca0: 6f74 2073 656e 6420 6669 6c65 2077 6974  ot send file wit
+0000acb0: 6820 6572 726f 7220 2573 222c 2073 656c  h error %s", sel
+0000acc0: 662e 5f6c 6c63 6f6d 2e6c 6173 745f 7265  f._llcom.last_re
+0000acd0: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
+0000ace0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000acf0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+0000ad00: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+0000ad10: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
+0000ad20: 7265 6369 7665 5f66 696c 6528 0a20 2020  recive_file(.   
+0000ad30: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000ad40: 2020 2072 656d 6f74 655f 7061 7468 3a20     remote_path: 
+0000ad50: 7374 722c 0a20 2020 2020 2020 206c 6f63  str,.        loc
+0000ad60: 616c 5f70 6174 683a 2055 6e69 6f6e 5b73  al_path: Union[s
+0000ad70: 7472 2c20 7061 7468 6c69 622e 5061 7468  tr, pathlib.Path
+0000ad80: 5d2c 0a20 2020 2020 2020 206f 7665 7272  ],.        overr
+0000ad90: 6964 655f 6669 6c65 3a20 626f 6f6c 203d  ide_file: bool =
+0000ada0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+0000adb0: 6269 6e61 7279 5f6d 6f64 653a 2062 6f6f  binary_mode: boo
+0000adc0: 6c20 3d20 4661 6c73 652c 0a20 2020 2029  l = False,.    )
+0000add0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+0000ade0: 2020 2222 220a 2020 2020 2020 2020 446f    """.        Do
+0000adf0: 776e 6c6f 6164 2061 2066 696c 6520 6672  wnload a file fr
+0000ae00: 6f6d 2063 6f6e 7472 6f6c 2e0a 2020 2020  om control..    
+0000ae10: 2020 2020 5265 7175 6972 6573 2061 6363      Requires acc
+0000ae20: 6573 7320 6c65 7665 6c20 6060 4649 4c45  ess level ``FILE
+0000ae30: 5452 414e 5346 4552 6060 2074 6f20 776f  TRANSFER`` to wo
+0000ae40: 726b 2e0a 2020 2020 2020 2020 5265 7475  rk..        Retu
+0000ae50: 726e 7320 6060 5472 7565 6060 2069 6620  rns ``True`` if 
+0000ae60: 636f 6d70 6c65 7465 6420 7375 6363 6573  completed succes
+0000ae70: 7366 756c 6c79 2e0a 0a20 2020 2020 2020  sfully...       
+0000ae80: 203a 7061 7261 6d20 7265 6d6f 7465 5f70   :param remote_p
+0000ae90: 6174 683a 2070 6174 6820 6f66 2066 696c  ath: path of fil
+0000aea0: 6520 6f6e 2074 6865 2063 6f6e 7472 6f6c  e on the control
+0000aeb0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000aec0: 6c6f 6361 6c5f 7061 7468 3a20 6c6f 6361  local_path: loca
+0000aed0: 6c20 7061 7468 206f 6620 6465 7374 696e  l path of destin
+0000aee0: 6174 696f 6e20 7769 7468 206f 7220 7769  ation with or wi
+0000aef0: 7468 6f75 7420 6669 6c65 206e 616d 650a  thout file name.
+0000af00: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+0000af10: 7665 7272 6964 655f 6669 6c65 3a20 666c  verride_file: fl
+0000af20: 6167 2069 6620 6669 6c65 2073 686f 756c  ag if file shoul
+0000af30: 6420 6265 2072 6570 6c61 6365 6420 6966  d be replaced if
+0000af40: 2069 7420 616c 7265 6164 7920 6578 6973   it already exis
+0000af50: 7473 0a20 2020 2020 2020 203a 7061 7261  ts.        :para
+0000af60: 6d20 6269 6e61 7279 5f6d 6f64 653a 2066  m binary_mode: f
+0000af70: 6c61 6720 6966 2062 696e 6172 7920 7472  lag if binary tr
+0000af80: 616e 7366 6572 206d 6f64 6520 7368 6f75  ansfer mode shou
+0000af90: 6c64 2062 6520 7573 6564 2c20 6966 206e  ld be used, if n
+0000afa0: 6f74 2073 6574 2074 6865 0a20 2020 2020  ot set the.     
+0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afc0: 2020 2020 2020 2066 696c 6520 6e61 6d65         file name
+0000afd0: 2069 7320 6368 6563 6b65 6420 666f 7220   is checked for 
+0000afe0: 6b6e 6f77 6e20 6269 6e61 7279 2066 696c  known binary fil
+0000aff0: 6520 7479 7065 0a20 2020 2020 2020 2022  e type.        "
+0000b000: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+0000b010: 7420 7365 6c66 2e6c 6f67 696e 286c 632e  t self.login(lc.
+0000b020: 4c6f 6769 6e2e 4649 4c45 5452 414e 5346  Login.FILETRANSF
+0000b030: 4552 293a 0a20 2020 2020 2020 2020 2020  ER):.           
+0000b040: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
+0000b050: 726e 696e 6728 2263 6f75 6c64 206e 6f74  rning("could not
+0000b060: 206c 6f67 2069 6e20 6173 2075 7365 7220   log in as user 
+0000b070: 4649 4c45 2229 0a20 2020 2020 2020 2020  FILE").         
+0000b080: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0000b090: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+0000b0a0: 7374 616e 6365 286c 6f63 616c 5f70 6174  stance(local_pat
+0000b0b0: 682c 2028 7374 722c 2929 3a0a 2020 2020  h, (str,)):.    
+0000b0c0: 2020 2020 2020 2020 6c6f 6361 6c5f 6669          local_fi
+0000b0d0: 6c65 203d 2070 6174 686c 6962 2e50 6174  le = pathlib.Pat
+0000b0e0: 6828 6c6f 6361 6c5f 7061 7468 290a 2020  h(local_path).  
+0000b0f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000b100: 2020 2020 2020 2020 6c6f 6361 6c5f 6669          local_fi
+0000b110: 6c65 203d 206c 6f63 616c 5f70 6174 680a  le = local_path.
+0000b120: 0a20 2020 2020 2020 2072 656d 6f74 655f  .        remote_
+0000b130: 7061 7468 203d 2072 656d 6f74 655f 7061  path = remote_pa
+0000b140: 7468 2e72 6570 6c61 6365 2822 2f22 2c20  th.replace("/", 
+0000b150: 6c63 2e50 4154 485f 5345 5029 0a20 2020  lc.PATH_SEP).   
+0000b160: 2020 2020 2072 656d 6f74 655f 6669 6c65       remote_file
+0000b170: 5f69 6e66 6f20 3d20 7365 6c66 2e66 696c  _info = self.fil
+0000b180: 655f 696e 666f 2872 656d 6f74 655f 7061  e_info(remote_pa
+0000b190: 7468 290a 2020 2020 2020 2020 6966 206e  th).        if n
+0000b1a0: 6f74 2072 656d 6f74 655f 6669 6c65 5f69  ot remote_file_i
+0000b1b0: 6e66 6f3a 0a20 2020 2020 2020 2020 2020  nfo:.           
+0000b1c0: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
+0000b1d0: 726e 696e 6728 2272 656d 6f74 6520 6669  rning("remote fi
+0000b1e0: 6c65 2064 6f65 7320 6e6f 7420 6578 6973  le does not exis
+0000b1f0: 743a 2025 7322 2c20 7265 6d6f 7465 5f70  t: %s", remote_p
+0000b200: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+0000b210: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+0000b220: 2020 2020 2020 2069 6620 6c6f 6361 6c5f         if local_
+0000b230: 6669 6c65 2e69 735f 6469 7228 293a 0a20  file.is_dir():. 
+0000b240: 2020 2020 2020 2020 2020 206c 6f63 616c             local
+0000b250: 5f66 696c 652e 6a6f 696e 7061 7468 2872  _file.joinpath(r
+0000b260: 656d 6f74 655f 7061 7468 2e73 706c 6974  emote_path.split
+0000b270: 2822 2f22 295b 2d31 5d29 0a20 2020 2020  ("/")[-1]).     
+0000b280: 2020 2065 6c69 6620 6c6f 6361 6c5f 6669     elif local_fi
+0000b290: 6c65 2e69 735f 6669 6c65 2829 3a0a 2020  le.is_file():.  
+0000b2a0: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+0000b2b0: 2e5f 6c6f 6767 6572 2e64 6562 7567 2822  ._logger.debug("
+0000b2c0: 6c6f 6361 6c20 7061 7468 2065 7869 7374  local path exist
+0000b2d0: 7320 616e 6420 706f 696e 7473 2074 6f20  s and points to 
+0000b2e0: 6669 6c65 2229 0a20 2020 2020 2020 2020  file").         
+0000b2f0: 2020 2069 6620 6e6f 7420 6f76 6572 7269     if not overri
+0000b300: 6465 5f66 696c 653a 0a20 2020 2020 2020  de_file:.       
+0000b310: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+0000b320: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2022 6c6f 6361 6c20 6669 6c65 2061     "local file a
+0000b350: 6c72 6561 6479 2065 7869 7374 7320 616e  lready exists an
+0000b360: 6420 6f76 6572 7269 6465 2077 6173 206e  d override was n
+0000b370: 6f74 2073 6574 2e20 6e6f 7468 696e 6720  ot set. nothing 
+0000b380: 746f 2064 6f22 0a20 2020 2020 2020 2020  to do".         
+0000b390: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000b3a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000b3b0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+0000b3c0: 2020 6c6f 6361 6c5f 6669 6c65 2e75 6e6c    local_file.unl
+0000b3d0: 696e 6b28 290a 0a20 2020 2020 2020 2073  ink()..        s
+0000b3e0: 656c 662e 5f6c 6f67 6765 722e 6465 6275  elf._logger.debu
+0000b3f0: 6728 226c 6f61 6469 6e67 2066 696c 6520  g("loading file 
+0000b400: 6672 6f6d 2025 7320 746f 2025 7322 2c0a  from %s to %s",.
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 2020 2020 2020 2020 2020 2072 656d 6f74             remot
+0000b430: 655f 7061 7468 2c20 6c6f 6361 6c5f 6669  e_path, local_fi
+0000b440: 6c65 290a 0a20 2020 2020 2020 2070 6179  le)..        pay
+0000b450: 6c6f 6164 203d 206c 6d2e 7573 7472 5f74  load = lm.ustr_t
+0000b460: 6f5f 6261 2872 656d 6f74 655f 7061 7468  o_ba(remote_path
+0000b470: 290a 0a20 2020 2020 2020 2069 6620 6269  )..        if bi
+0000b480: 6e61 7279 5f6d 6f64 6520 6f72 206c 6d2e  nary_mode or lm.
+0000b490: 6973 5f66 696c 655f 6269 6e61 7279 2872  is_file_binary(r
+0000b4a0: 656d 6f74 655f 7061 7468 293a 0a20 2020  emote_path):.   
+0000b4b0: 2020 2020 2020 2020 2070 6179 6c6f 6164           payload
+0000b4c0: 2e61 7070 656e 6428 6c63 2e4d 4f44 455f  .append(lc.MODE_
+0000b4d0: 4249 4e41 5259 2920 2023 2066 6f72 6365  BINARY)  # force
+0000b4e0: 2062 696e 6172 7920 7472 616e 7366 6572   binary transfer
+0000b4f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000b500: 662e 5f6c 6f67 6765 722e 6465 6275 6728  f._logger.debug(
+0000b510: 2275 7369 6e67 2062 696e 6172 7920 7472  "using binary tr
+0000b520: 616e 7366 6572 206d 6f64 6522 290a 2020  ansfer mode").  
+0000b530: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000b540: 2020 2020 2020 2020 7061 796c 6f61 642e          payload.
+0000b550: 6170 7065 6e64 286c 632e 4d4f 4445 5f4e  append(lc.MODE_N
+0000b560: 4f4e 5f42 494e 290a 2020 2020 2020 2020  ON_BIN).        
+0000b570: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+0000b580: 2e64 6562 7567 2822 7573 696e 6720 6e6f  .debug("using no
+0000b590: 6e20 6269 6e61 7279 2074 7261 6e73 6665  n binary transfe
+0000b5a0: 7220 6d6f 6465 2229 0a0a 2020 2020 2020  r mode")..      
+0000b5b0: 2020 636f 6e74 656e 7420 3d20 7365 6c66    content = self
+0000b5c0: 2e5f 6c6c 636f 6d2e 7465 6c65 6772 616d  ._llcom.telegram
+0000b5d0: 280a 2020 2020 2020 2020 2020 2020 6c63  (.            lc
+0000b5e0: 2e43 4d44 2e52 5f46 4c2c 0a20 2020 2020  .CMD.R_FL,.     
+0000b5f0: 2020 2020 2020 2070 6179 6c6f 6164 2c0a         payload,.
+0000b600: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000b610: 2020 2077 6974 6820 6c6f 6361 6c5f 6669     with local_fi
+0000b620: 6c65 2e6f 7065 6e28 2277 6222 2920 6173  le.open("wb") as
+0000b630: 206f 7574 5f66 696c 653a 0a20 2020 2020   out_file:.     
+0000b640: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000b650: 6c6c 636f 6d2e 6c61 7374 5f72 6573 706f  llcom.last_respo
+0000b660: 6e73 6520 696e 206c 632e 5253 502e 535f  nse in lc.RSP.S_
+0000b670: 464c 3a0a 2020 2020 2020 2020 2020 2020  FL:.            
+0000b680: 2020 2020 6966 2062 696e 6172 795f 6d6f      if binary_mo
+0000b690: 6465 3a0a 2020 2020 2020 2020 2020 2020  de:.            
+0000b6a0: 2020 2020 2020 2020 6f75 745f 6669 6c65          out_file
+0000b6b0: 2e77 7269 7465 2863 6f6e 7465 6e74 290a  .write(content).
+0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b6e0: 2020 2020 2020 2020 2020 6f75 745f 6669            out_fi
+0000b6f0: 6c65 2e77 7269 7465 2863 6f6e 7465 6e74  le.write(content
+0000b700: 2e72 6570 6c61 6365 2862 225c 7830 3022  .replace(b"\x00"
+0000b710: 2c20 6222 5c72 5c6e 2229 290a 2020 2020  , b"\r\n")).    
+0000b720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b730: 2e5f 6c6f 6767 6572 2e64 6562 7567 280a  ._logger.debug(.
 0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 206f 7574 5f66 696c 652e 7772 6974 6528   out_file.write(
-0000b760: 636f 6e74 656e 7429 0a20 2020 2020 2020  content).       
-0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 2020 206f 7574 5f66 696c 652e 7772 6974     out_file.writ
-0000b7b0: 6528 636f 6e74 656e 742e 7265 706c 6163  e(content.replac
-0000b7c0: 6528 6222 5c78 3030 222c 2062 225c 725c  e(b"\x00", b"\r\
-0000b7d0: 6e22 2929 0a20 2020 2020 2020 2020 2020  n")).           
-0000b7e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b7f0: 662e 5f6c 6f67 6765 722e 6465 6275 6728  f._logger.debug(
-0000b800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b810: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-0000b820: 6365 6976 6564 2025 6420 6d6f 7265 2062  ceived %d more b
-0000b830: 7974 6573 2066 6f72 2066 696c 6522 2c20  ytes for file", 
-0000b840: 6c65 6e28 636f 6e74 656e 7429 0a20 2020  len(content).   
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000b870: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000b880: 7365 6c66 2e5f 6c6c 636f 6d2e 6c61 7374  self._llcom.last
-0000b890: 5f72 6573 706f 6e73 6520 696e 206c 632e  _response in lc.
-0000b8a0: 5253 502e 545f 4644 3a0a 2020 2020 2020  RSP.T_FD:.      
-0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e69    self._logger.i
-0000b8d0: 6e66 6f28 2266 696e 6973 6865 6420 6c6f  nfo("finished lo
-0000b8e0: 6164 696e 6720 6669 6c65 2229 0a20 2020  ading file").   
-0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b900: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-0000b910: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000b920: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000b930: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b940: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
-0000b950: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000b970: 736f 6d65 7468 696e 6720 7765 6e74 2077  something went w
-0000b980: 726f 6e67 2077 6869 6c65 2072 6563 6569  rong while recei
-0000b990: 7669 6e67 2066 696c 6520 6461 7461 2025  ving file data %
-0000b9a0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+0000b750: 2020 2020 2272 6563 6569 7665 6420 6669      "received fi
+0000b760: 7273 7420 626c 6f63 6b20 6f66 2066 696c  rst block of fil
+0000b770: 6520 6669 6c65 2025 7322 2c20 7265 6d6f  e file %s", remo
+0000b780: 7465 5f70 6174 6829 0a0a 2020 2020 2020  te_path)..      
+0000b790: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+0000b7a0: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
+0000b7b0: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
+0000b7c0: 7420 3d20 7365 6c66 2e5f 6c6c 636f 6d2e  t = self._llcom.
+0000b7d0: 7465 6c65 6772 616d 280a 2020 2020 2020  telegram(.      
+0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7f0: 2020 6c63 2e52 5350 2e54 5f4f 4b2c 0a20    lc.RSP.T_OK,. 
+0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b810: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000b820: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000b830: 2e5f 6c6c 636f 6d2e 6c61 7374 5f72 6573  ._llcom.last_res
+0000b840: 706f 6e73 6520 696e 206c 632e 5253 502e  ponse in lc.RSP.
+0000b850: 535f 464c 3a0a 2020 2020 2020 2020 2020  S_FL:.          
+0000b860: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000b870: 2062 696e 6172 795f 6d6f 6465 3a0a 2020   binary_mode:.  
+0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b890: 2020 2020 2020 2020 2020 6f75 745f 6669            out_fi
+0000b8a0: 6c65 2e77 7269 7465 2863 6f6e 7465 6e74  le.write(content
+0000b8b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b8c0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8e0: 2020 2020 2020 2020 2020 2020 6f75 745f              out_
+0000b8f0: 6669 6c65 2e77 7269 7465 2863 6f6e 7465  file.write(conte
+0000b900: 6e74 2e72 6570 6c61 6365 2862 225c 7830  nt.replace(b"\x0
+0000b910: 3022 2c20 6222 5c72 5c6e 2229 290a 2020  0", b"\r\n")).  
+0000b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b930: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+0000b940: 6572 2e64 6562 7567 280a 2020 2020 2020  er.debug(.      
+0000b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b960: 2020 2020 2020 2272 6563 6569 7665 6420        "received 
+0000b970: 2564 206d 6f72 6520 6279 7465 7320 666f  %d more bytes fo
+0000b980: 7220 6669 6c65 222c 206c 656e 2863 6f6e  r file", len(con
+0000b990: 7465 6e74 290a 2020 2020 2020 2020 2020  tent).          
+0000b9a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
 0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9c0: 7265 6d6f 7465 5f70 6174 682c 0a20 2020  remote_path,.   
-0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000ba00: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba20: 7365 6c66 2e5f 6c6c 636f 6d2e 6c61 7374  self._llcom.last
-0000ba30: 5f72 6573 706f 6e73 6520 6973 206c 632e  _response is lc.
-0000ba40: 5253 502e 545f 4552 0a20 2020 2020 2020  RSP.T_ER.       
-0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba60: 2020 2020 206f 7220 7365 6c66 2e5f 6c6c       or self._ll
-0000ba70: 636f 6d2e 6c61 7374 5f72 6573 706f 6e73  com.last_respons
-0000ba80: 6520 6973 206c 632e 5253 502e 545f 4244  e is lc.RSP.T_BD
-0000ba90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000baa0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0000bad0: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
-0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-0000bb00: 6e20 6572 726f 7220 6f63 6375 7272 6564  n error occurred
-0000bb10: 2077 6869 6c65 206c 6f61 6469 6e67 2074   while loading t
-0000bb20: 6865 2066 6972 7374 2062 6c6f 636b 206f  he first block o
-0000bb30: 6620 6461 7461 2025 7320 2725 7327 222c  f data %s '%s'",
-0000bb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b9c0: 2020 2020 656c 6966 2073 656c 662e 5f6c      elif self._l
+0000b9d0: 6c63 6f6d 2e6c 6173 745f 7265 7370 6f6e  lcom.last_respon
+0000b9e0: 7365 2069 6e20 6c63 2e52 5350 2e54 5f46  se in lc.RSP.T_F
+0000b9f0: 443a 0a20 2020 2020 2020 2020 2020 2020  D:.             
+0000ba00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ba10: 5f6c 6f67 6765 722e 696e 666f 2822 6669  _logger.info("fi
+0000ba20: 6e69 7368 6564 206c 6f61 6469 6e67 2066  nished loading f
+0000ba30: 696c 6522 290a 2020 2020 2020 2020 2020  ile").          
+0000ba40: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0000ba50: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+0000ba60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba80: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+0000ba90: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 2020 2020 2020 2020 2273 6f6d 6574 6869          "somethi
+0000bac0: 6e67 2077 656e 7420 7772 6f6e 6720 7768  ng went wrong wh
+0000bad0: 696c 6520 7265 6365 6976 696e 6720 6669  ile receiving fi
+0000bae0: 6c65 2064 6174 6120 2573 222c 0a20 2020  le data %s",.   
+0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb00: 2020 2020 2020 2020 2072 656d 6f74 655f           remote_
+0000bb10: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
 0000bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb60: 2073 656c 662e 6c61 7374 5f65 7272 6f72   self.last_error
-0000bb70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb90: 2020 6c74 2e67 6574 5f65 7272 6f72 5f74    lt.get_error_t
-0000bba0: 6578 7428 7365 6c66 2e6c 6173 745f 6572  ext(self.last_er
-0000bbb0: 726f 7229 2c0a 2020 2020 2020 2020 2020  ror),.          
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbd0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000bbe0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000bbf0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0000bc00: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000bc10: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 7365 6c66 2e5f 6c6c 636f 6d2e      self._llcom.
-0000bc40: 6c61 7374 5f72 6573 706f 6e73 6520 6973  last_response is
-0000bc50: 206c 632e 5253 502e 545f 4552 0a20 2020   lc.RSP.T_ER.   
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc70: 206f 7220 7365 6c66 2e5f 6c6c 636f 6d2e   or self._llcom.
-0000bc80: 6c61 7374 5f72 6573 706f 6e73 6520 6973  last_response is
-0000bc90: 206c 632e 5253 502e 545f 4244 0a20 2020   lc.RSP.T_BD.   
-0000bca0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcc0: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-0000bcd0: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
-0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcf0: 2020 2261 6e20 6572 726f 7220 6f63 6375    "an error occu
-0000bd00: 7272 6564 2077 6869 6c65 206c 6f61 6469  rred while loadi
-0000bd10: 6e67 2074 6865 2066 6972 7374 2062 6c6f  ng the first blo
-0000bd20: 636b 206f 6620 6461 7461 2066 6f72 2066  ck of data for f
-0000bd30: 696c 6520 2573 2c20 2573 2027 2573 2722  ile %s, %s '%s'"
-0000bd40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bd50: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
-0000bd60: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000bd80: 656c 662e 6c61 7374 5f65 7272 6f72 2c0a  elf.last_error,.
-0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bda0: 2020 2020 2020 2020 6c74 2e67 6574 5f65          lt.get_e
-0000bdb0: 7272 6f72 5f74 6578 7428 7365 6c66 2e6c  rror_text(self.l
-0000bdc0: 6173 745f 6572 726f 7229 2c0a 2020 2020  ast_error),.    
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bde0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000bdf0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000be00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000be10: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
-0000be20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000be30: 2020 2020 2020 2020 2020 2263 6f75 6c64            "could
-0000be40: 206e 6f74 206c 6f61 6420 6669 6c65 2077   not load file w
-0000be50: 6974 6820 6572 726f 7220 2573 222c 2073  ith error %s", s
-0000be60: 656c 662e 5f6c 6c63 6f6d 2e6c 6173 745f  elf._llcom.last_
-0000be70: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
-0000be80: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000be90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000bea0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-0000beb0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-0000bec0: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-0000bed0: 2020 2020 2272 6563 6569 7665 6420 2564      "received %d
-0000bee0: 2062 7974 6573 2074 7261 6e73 6665 7220   bytes transfer 
-0000bef0: 636f 6d70 6c65 7465 2066 6f72 2066 696c  complete for fil
-0000bf00: 6520 2573 2074 6f20 2573 222c 0a20 2020  e %s to %s",.   
-0000bf10: 2020 2020 2020 2020 206c 6f63 616c 5f66           local_f
-0000bf20: 696c 652e 7374 6174 2829 2e73 745f 7369  ile.stat().st_si
-0000bf30: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
-0000bf40: 7265 6d6f 7465 5f70 6174 682c 0a20 2020  remote_path,.   
-0000bf50: 2020 2020 2020 2020 206c 6f63 616c 5f66           local_f
-0000bf60: 696c 652c 0a20 2020 2020 2020 2029 0a0a  ile,.        )..
-0000bf70: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000bf80: 7275 650a 0a20 2020 2064 6566 2072 6561  rue..    def rea
-0000bf90: 645f 706c 635f 6d65 6d6f 7279 280a 2020  d_plc_memory(.  
-0000bfa0: 2020 2020 2020 7365 6c66 2c20 6669 7273        self, firs
-0000bfb0: 745f 656c 656d 656e 743a 2069 6e74 2c20  t_element: int, 
-0000bfc0: 6d65 6d5f 7479 7065 3a20 6c63 2e4d 656d  mem_type: lc.Mem
-0000bfd0: 6f72 7954 7970 652c 206e 756d 6265 725f  oryType, number_
-0000bfe0: 6f66 5f65 6c65 6d65 6e74 733a 2069 6e74  of_elements: int
-0000bff0: 203d 2031 0a20 2020 2029 202d 3e20 6c69   = 1.    ) -> li
-0000c000: 7374 3a0a 2020 2020 2020 2020 2222 220a  st:.        """.
-0000c010: 2020 2020 2020 2020 5265 6164 2064 6174          Read dat
-0000c020: 6120 6672 6f6d 2070 6c63 206d 656d 6f72  a from plc memor
-0000c030: 792e 0a20 2020 2020 2020 2052 6571 7569  y..        Requi
-0000c040: 7265 7320 6163 6365 7373 206c 6576 656c  res access level
-0000c050: 2060 6050 4c43 4445 4255 4760 6020 746f   ``PLCDEBUG`` to
-0000c060: 2077 6f72 6b2e 0a0a 2020 2020 2020 2020   work...        
-0000c070: 3a70 6172 616d 2066 6972 7374 5f65 6c65  :param first_ele
-0000c080: 6d65 6e74 3a20 7768 6963 6820 6d65 6d6f  ment: which memo
-0000c090: 7279 206c 6f63 6174 696f 6e20 7368 6f75  ry location shou
-0000c0a0: 6c64 2062 6520 7265 6164 2c20 7374 6172  ld be read, star
-0000c0b0: 7473 2061 7420 3020 7570 2074 6f20 7468  ts at 0 up to th
-0000c0c0: 6520 6d61 7820 6e75 6d62 6572 2066 6f72  e max number for
-0000c0d0: 2065 6163 6820 7479 7065 0a20 2020 2020   each type.     
-0000c0e0: 2020 203a 7061 7261 6d20 6d65 6d5f 7479     :param mem_ty
-0000c0f0: 7065 3a20 7768 6174 2064 6174 6174 7970  pe: what datatyp
-0000c100: 6520 746f 2072 6561 640a 2020 2020 2020  e to read.      
-0000c110: 2020 3a70 6172 616d 206e 756d 6265 725f    :param number_
-0000c120: 6f66 5f65 6c65 6d65 6e74 733a 2068 6f77  of_elements: how
-0000c130: 206d 616e 7920 656c 656d 656e 7473 2073   many elements s
-0000c140: 686f 756c 6420 6265 2072 6561 640a 0a20  hould be read.. 
-0000c150: 2020 2020 2020 203a 7261 6973 6573 204c         :raises L
-0000c160: 5356 3249 6e70 7574 4578 6365 7074 696f  SV2InputExceptio
-0000c170: 6e3a 2069 6620 756e 6b6e 6f77 6e73 206d  n: if unknowns m
-0000c180: 656d 6f72 7920 7479 7065 2069 7320 7265  emory type is re
-0000c190: 7175 6573 7465 6420 6f72 2069 6620 7468  quested or if th
-0000c1a0: 6520 746f 206d 616e 7920 656c 656d 656e  e to many elemen
-0000c1b0: 7473 2061 7265 2072 6571 7565 7374 6564  ts are requested
-0000c1c0: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
-0000c1d0: 204c 5356 3244 6174 6145 7863 6570 7469   LSV2DataExcepti
-0000c1e0: 6f6e 3a20 6966 206e 756d 6265 7220 6f66  on: if number of
-0000c1f0: 2072 6563 6569 7665 6420 7661 6c75 6573   received values
-0000c200: 2064 6f65 7320 6e6f 7420 6d61 7463 6820   does not match 
-0000c210: 7468 6520 6e75 6d62 6572 206f 6620 6578  the number of ex
-0000c220: 7065 6374 6564 0a20 2020 2020 2020 2022  pected.        "
-0000c230: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
-0000c240: 656c 662e 5f73 7973 5f70 6172 2e6c 7376  elf._sys_par.lsv
-0000c250: 325f 7665 7273 696f 6e20 213d 202d 313a  2_version != -1:
-0000c260: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c270: 662e 5f72 6561 645f 7061 7261 6d65 7465  f._read_paramete
-0000c280: 7273 2829 0a0a 2020 2020 2020 2020 6966  rs()..        if
-0000c290: 206e 6f74 2073 656c 662e 6c6f 6769 6e28   not self.login(
-0000c2a0: 6c6f 6769 6e3d 6c63 2e4c 6f67 696e 2e50  login=lc.Login.P
-0000c2b0: 4c43 4445 4255 4729 3a0a 2020 2020 2020  LCDEBUG):.      
-0000c2c0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-0000c2d0: 6572 2e77 6172 6e69 6e67 2822 636f 756c  er.warning("coul
-0000c2e0: 6420 6e6f 7420 6c6f 6720 696e 2061 7320  d not log in as 
-0000c2f0: 7573 6572 2050 4c43 4445 4255 4722 290a  user PLCDEBUG").
-0000c300: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c310: 726e 205b 5d0a 0a20 2020 2020 2020 2069  rn []..        i
-0000c320: 6620 6d65 6d5f 7479 7065 2069 7320 6c63  f mem_type is lc
-0000c330: 2e4d 656d 6f72 7954 7970 652e 4d41 524b  .MemoryType.MARK
-0000c340: 4552 3a0a 2020 2020 2020 2020 2020 2020  ER:.            
-0000c350: 7374 6172 745f 6164 6472 6573 7320 3d20  start_address = 
-0000c360: 7365 6c66 2e5f 7379 735f 7061 722e 6d61  self._sys_par.ma
-0000c370: 726b 6572 735f 7374 6172 745f 6164 6472  rkers_start_addr
-0000c380: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
-0000c390: 6d61 785f 656c 656d 656e 7320 3d20 7365  max_elemens = se
-0000c3a0: 6c66 2e5f 7379 735f 7061 722e 6e75 6d62  lf._sys_par.numb
-0000c3b0: 6572 5f6f 665f 6d61 726b 6572 730a 2020  er_of_markers.  
-0000c3c0: 2020 2020 2020 2020 2020 6d65 6d5f 6279            mem_by
-0000c3d0: 7465 5f63 6f75 6e74 203d 2031 0a20 2020  te_count = 1.   
-0000c3e0: 2020 2020 2020 2020 2075 6e70 6163 6b5f           unpack_
-0000c3f0: 7374 7269 6e67 203d 2022 213f 220a 2020  string = "!?".  
-0000c400: 2020 2020 2020 656c 6966 206d 656d 5f74        elif mem_t
-0000c410: 7970 6520 6973 206c 632e 4d65 6d6f 7279  ype is lc.Memory
-0000c420: 5479 7065 2e49 4e50 5554 3a0a 2020 2020  Type.INPUT:.    
-0000c430: 2020 2020 2020 2020 7374 6172 745f 6164          start_ad
-0000c440: 6472 6573 7320 3d20 7365 6c66 2e5f 7379  dress = self._sy
-0000c450: 735f 7061 722e 696e 7075 7473 5f73 7461  s_par.inputs_sta
-0000c460: 7274 5f61 6464 7265 7373 0a20 2020 2020  rt_address.     
-0000c470: 2020 2020 2020 206d 6178 5f65 6c65 6d65         max_eleme
-0000c480: 6e73 203d 2073 656c 662e 5f73 7973 5f70  ns = self._sys_p
-0000c490: 6172 2e6e 756d 6265 725f 6f66 5f69 6e70  ar.number_of_inp
-0000c4a0: 7574 730a 2020 2020 2020 2020 2020 2020  uts.            
-0000c4b0: 6d65 6d5f 6279 7465 5f63 6f75 6e74 203d  mem_byte_count =
-0000c4c0: 2031 0a20 2020 2020 2020 2020 2020 2075   1.            u
-0000c4d0: 6e70 6163 6b5f 7374 7269 6e67 203d 2022  npack_string = "
-0000c4e0: 213f 220a 2020 2020 2020 2020 656c 6966  !?".        elif
-0000c4f0: 206d 656d 5f74 7970 6520 6973 206c 632e   mem_type is lc.
-0000c500: 4d65 6d6f 7279 5479 7065 2e4f 5554 5055  MemoryType.OUTPU
-0000c510: 543a 0a20 2020 2020 2020 2020 2020 2073  T:.            s
-0000c520: 7461 7274 5f61 6464 7265 7373 203d 2073  tart_address = s
-0000c530: 656c 662e 5f73 7973 5f70 6172 2e6f 7574  elf._sys_par.out
-0000c540: 7075 7473 5f73 7461 7274 5f61 6464 7265  puts_start_addre
-0000c550: 7373 0a20 2020 2020 2020 2020 2020 206d  ss.            m
-0000c560: 6178 5f65 6c65 6d65 6e73 203d 2073 656c  ax_elemens = sel
-0000c570: 662e 5f73 7973 5f70 6172 2e6e 756d 6265  f._sys_par.numbe
-0000c580: 725f 6f66 5f6f 7574 7075 7473 0a20 2020  r_of_outputs.   
-0000c590: 2020 2020 2020 2020 206d 656d 5f62 7974           mem_byt
-0000c5a0: 655f 636f 756e 7420 3d20 310a 2020 2020  e_count = 1.    
-0000c5b0: 2020 2020 2020 2020 756e 7061 636b 5f73          unpack_s
-0000c5c0: 7472 696e 6720 3d20 2221 3f22 0a20 2020  tring = "!?".   
-0000c5d0: 2020 2020 2065 6c69 6620 6d65 6d5f 7479       elif mem_ty
-0000c5e0: 7065 2069 7320 6c63 2e4d 656d 6f72 7954  pe is lc.MemoryT
-0000c5f0: 7970 652e 434f 554e 5445 523a 0a20 2020  ype.COUNTER:.   
-0000c600: 2020 2020 2020 2020 2073 7461 7274 5f61           start_a
-0000c610: 6464 7265 7373 203d 2073 656c 662e 5f73  ddress = self._s
-0000c620: 7973 5f70 6172 2e63 6f75 6e74 6572 735f  ys_par.counters_
-0000c630: 7374 6172 745f 6164 6472 6573 730a 2020  start_address.  
-0000c640: 2020 2020 2020 2020 2020 6d61 785f 656c            max_el
-0000c650: 656d 656e 7320 3d20 7365 6c66 2e5f 7379  emens = self._sy
-0000c660: 735f 7061 722e 6e75 6d62 6572 5f6f 665f  s_par.number_of_
-0000c670: 636f 756e 7465 7273 0a20 2020 2020 2020  counters.       
-0000c680: 2020 2020 206d 656d 5f62 7974 655f 636f       mem_byte_co
-0000c690: 756e 7420 3d20 310a 2020 2020 2020 2020  unt = 1.        
-0000c6a0: 2020 2020 756e 7061 636b 5f73 7472 696e      unpack_strin
-0000c6b0: 6720 3d20 2221 3f22 0a20 2020 2020 2020  g = "!?".       
-0000c6c0: 2065 6c69 6620 6d65 6d5f 7479 7065 2069   elif mem_type i
-0000c6d0: 7320 6c63 2e4d 656d 6f72 7954 7970 652e  s lc.MemoryType.
-0000c6e0: 5449 4d45 523a 0a20 2020 2020 2020 2020  TIMER:.         
-0000c6f0: 2020 2073 7461 7274 5f61 6464 7265 7373     start_address
-0000c700: 203d 2073 656c 662e 5f73 7973 5f70 6172   = self._sys_par
-0000c710: 2e74 696d 6572 735f 7374 6172 745f 6164  .timers_start_ad
-0000c720: 6472 6573 730a 2020 2020 2020 2020 2020  dress.          
-0000c730: 2020 6d61 785f 656c 656d 656e 7320 3d20    max_elemens = 
-0000c740: 7365 6c66 2e5f 7379 735f 7061 722e 6e75  self._sys_par.nu
-0000c750: 6d62 6572 5f6f 665f 7469 6d65 7273 0a20  mber_of_timers. 
-0000c760: 2020 2020 2020 2020 2020 206d 656d 5f62             mem_b
-0000c770: 7974 655f 636f 756e 7420 3d20 310a 2020  yte_count = 1.  
-0000c780: 2020 2020 2020 2020 2020 756e 7061 636b            unpack
-0000c790: 5f73 7472 696e 6720 3d20 2221 3f22 0a20  _string = "!?". 
-0000c7a0: 2020 2020 2020 2065 6c69 6620 6d65 6d5f         elif mem_
-0000c7b0: 7479 7065 2069 7320 6c63 2e4d 656d 6f72  type is lc.Memor
-0000c7c0: 7954 7970 652e 4259 5445 3a0a 2020 2020  yType.BYTE:.    
-0000c7d0: 2020 2020 2020 2020 7374 6172 745f 6164          start_ad
-0000c7e0: 6472 6573 7320 3d20 7365 6c66 2e5f 7379  dress = self._sy
-0000c7f0: 735f 7061 722e 776f 7264 735f 7374 6172  s_par.words_star
-0000c800: 745f 6164 6472 6573 730a 2020 2020 2020  t_address.      
-0000c810: 2020 2020 2020 6d61 785f 656c 656d 656e        max_elemen
-0000c820: 7320 3d20 7365 6c66 2e5f 7379 735f 7061  s = self._sys_pa
-0000c830: 722e 6e75 6d62 6572 5f6f 665f 776f 7264  r.number_of_word
-0000c840: 7320 2a20 320a 2020 2020 2020 2020 2020  s * 2.          
-0000c850: 2020 6d65 6d5f 6279 7465 5f63 6f75 6e74    mem_byte_count
-0000c860: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
-0000c870: 2075 6e70 6163 6b5f 7374 7269 6e67 203d   unpack_string =
-0000c880: 2022 2142 220a 2020 2020 2020 2020 656c   "!B".        el
-0000c890: 6966 206d 656d 5f74 7970 6520 6973 206c  if mem_type is l
-0000c8a0: 632e 4d65 6d6f 7279 5479 7065 2e57 4f52  c.MemoryType.WOR
-0000c8b0: 443a 0a20 2020 2020 2020 2020 2020 2073  D:.            s
-0000c8c0: 7461 7274 5f61 6464 7265 7373 203d 2073  tart_address = s
-0000c8d0: 656c 662e 5f73 7973 5f70 6172 2e77 6f72  elf._sys_par.wor
-0000c8e0: 6473 5f73 7461 7274 5f61 6464 7265 7373  ds_start_address
-0000c8f0: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-0000c900: 5f65 6c65 6d65 6e73 203d 2073 656c 662e  _elemens = self.
-0000c910: 5f73 7973 5f70 6172 2e6e 756d 6265 725f  _sys_par.number_
-0000c920: 6f66 5f77 6f72 6473 0a20 2020 2020 2020  of_words.       
-0000c930: 2020 2020 206d 656d 5f62 7974 655f 636f       mem_byte_co
-0000c940: 756e 7420 3d20 320a 2020 2020 2020 2020  unt = 2.        
-0000c950: 2020 2020 756e 7061 636b 5f73 7472 696e      unpack_strin
-0000c960: 6720 3d20 223c 4822 0a20 2020 2020 2020  g = "<H".       
-0000c970: 2065 6c69 6620 6d65 6d5f 7479 7065 2069   elif mem_type i
-0000c980: 7320 6c63 2e4d 656d 6f72 7954 7970 652e  s lc.MemoryType.
-0000c990: 4457 4f52 443a 0a20 2020 2020 2020 2020  DWORD:.         
-0000c9a0: 2020 2073 7461 7274 5f61 6464 7265 7373     start_address
-0000c9b0: 203d 2073 656c 662e 5f73 7973 5f70 6172   = self._sys_par
-0000c9c0: 2e77 6f72 6473 5f73 7461 7274 5f61 6464  .words_start_add
-0000c9d0: 7265 7373 0a20 2020 2020 2020 2020 2020  ress.           
-0000c9e0: 206d 6178 5f65 6c65 6d65 6e73 203d 2073   max_elemens = s
-0000c9f0: 656c 662e 5f73 7973 5f70 6172 2e6e 756d  elf._sys_par.num
-0000ca00: 6265 725f 6f66 5f77 6f72 6473 202f 2034  ber_of_words / 4
-0000ca10: 0a20 2020 2020 2020 2020 2020 206d 656d  .            mem
-0000ca20: 5f62 7974 655f 636f 756e 7420 3d20 340a  _byte_count = 4.
-0000ca30: 2020 2020 2020 2020 2020 2020 756e 7061              unpa
-0000ca40: 636b 5f73 7472 696e 6720 3d20 223c 4c22  ck_string = "<L"
-0000ca50: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
-0000ca60: 6d5f 7479 7065 2069 7320 6c63 2e4d 656d  m_type is lc.Mem
-0000ca70: 6f72 7954 7970 652e 5354 5249 4e47 3a0a  oryType.STRING:.
-0000ca80: 2020 2020 2020 2020 2020 2020 7374 6172              star
-0000ca90: 745f 6164 6472 6573 7320 3d20 7365 6c66  t_address = self
-0000caa0: 2e5f 7379 735f 7061 722e 7374 7269 6e67  ._sys_par.string
-0000cab0: 735f 7374 6172 745f 6164 6472 6573 730a  s_start_address.
-0000cac0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-0000cad0: 656c 656d 656e 7320 3d20 7365 6c66 2e5f  elemens = self._
-0000cae0: 7379 735f 7061 722e 6e75 6d62 6572 5f6f  sys_par.number_o
-0000caf0: 665f 7374 7269 6e67 730a 2020 2020 2020  f_strings.      
-0000cb00: 2020 2020 2020 6d65 6d5f 6279 7465 5f63        mem_byte_c
-0000cb10: 6f75 6e74 203d 2073 656c 662e 5f73 7973  ount = self._sys
-0000cb20: 5f70 6172 2e6d 6178 5f73 7472 696e 675f  _par.max_string_
-0000cb30: 6c65 6e67 6874 0a20 2020 2020 2020 2020  lenght.         
-0000cb40: 2020 2075 6e70 6163 6b5f 7374 7269 6e67     unpack_string
-0000cb50: 203d 2022 7b7d 7322 2e66 6f72 6d61 7428   = "{}s".format(
-0000cb60: 6d65 6d5f 6279 7465 5f63 6f75 6e74 290a  mem_byte_count).
-0000cb70: 2020 2020 2020 2020 656c 6966 206d 656d          elif mem
-0000cb80: 5f74 7970 6520 6973 206c 632e 4d65 6d6f  _type is lc.Memo
-0000cb90: 7279 5479 7065 2e49 4e50 5554 5f57 4f52  ryType.INPUT_WOR
-0000cba0: 443a 0a20 2020 2020 2020 2020 2020 2073  D:.            s
-0000cbb0: 7461 7274 5f61 6464 7265 7373 203d 2073  tart_address = s
-0000cbc0: 656c 662e 5f73 7973 5f70 6172 2e69 6e70  elf._sys_par.inp
-0000cbd0: 7574 5f77 6f72 6473 5f73 7461 7274 5f61  ut_words_start_a
-0000cbe0: 6464 7265 7373 0a20 2020 2020 2020 2020  ddress.         
-0000cbf0: 2020 206d 6178 5f65 6c65 6d65 6e73 203d     max_elemens =
-0000cc00: 2073 656c 662e 5f73 7973 5f70 6172 2e6e   self._sys_par.n
-0000cc10: 756d 6265 725f 6f66 5f69 6e70 7574 5f77  umber_of_input_w
-0000cc20: 6f72 6473 0a20 2020 2020 2020 2020 2020  ords.           
-0000cc30: 206d 656d 5f62 7974 655f 636f 756e 7420   mem_byte_count 
-0000cc40: 3d20 320a 2020 2020 2020 2020 2020 2020  = 2.            
-0000cc50: 756e 7061 636b 5f73 7472 696e 6720 3d20  unpack_string = 
-0000cc60: 223c 4822 0a20 2020 2020 2020 2065 6c69  "<H".        eli
-0000cc70: 6620 6d65 6d5f 7479 7065 2069 7320 6c63  f mem_type is lc
-0000cc80: 2e4d 656d 6f72 7954 7970 652e 4f55 5450  .MemoryType.OUTP
-0000cc90: 5554 5f57 4f52 443a 0a20 2020 2020 2020  UT_WORD:.       
-0000cca0: 2020 2020 2073 7461 7274 5f61 6464 7265       start_addre
-0000ccb0: 7373 203d 2073 656c 662e 5f73 7973 5f70  ss = self._sys_p
-0000ccc0: 6172 2e6f 7574 7075 745f 776f 7264 735f  ar.output_words_
-0000ccd0: 7374 6172 745f 6164 6472 6573 730a 2020  start_address.  
-0000cce0: 2020 2020 2020 2020 2020 6d61 785f 656c            max_el
-0000ccf0: 656d 656e 7320 3d20 7365 6c66 2e5f 7379  emens = self._sy
-0000cd00: 735f 7061 722e 6e75 6d62 6572 5f6f 665f  s_par.number_of_
-0000cd10: 6f75 7470 7574 5f77 6f72 6473 0a20 2020  output_words.   
-0000cd20: 2020 2020 2020 2020 206d 656d 5f62 7974           mem_byt
-0000cd30: 655f 636f 756e 7420 3d20 320a 2020 2020  e_count = 2.    
-0000cd40: 2020 2020 2020 2020 756e 7061 636b 5f73          unpack_s
-0000cd50: 7472 696e 6720 3d20 223c 4822 0a20 2020  tring = "<H".   
-0000cd60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000cd70: 2020 2020 2020 2072 6169 7365 204c 5356         raise LSV
-0000cd80: 3249 6e70 7574 4578 6365 7074 696f 6e28  2InputException(
-0000cd90: 2275 6e6b 6e6f 776e 2061 6464 7265 7373  "unknown address
-0000cda0: 2074 7970 6522 290a 0a20 2020 2020 2020   type")..       
-0000cdb0: 2069 6620 2866 6972 7374 5f65 6c65 6d65   if (first_eleme
-0000cdc0: 6e74 202b 206e 756d 6265 725f 6f66 5f65  nt + number_of_e
-0000cdd0: 6c65 6d65 6e74 7329 203e 206d 6178 5f65  lements) > max_e
-0000cde0: 6c65 6d65 6e73 3a0a 2020 2020 2020 2020  lemens:.        
-0000cdf0: 2020 2020 7261 6973 6520 4c53 5632 496e      raise LSV2In
-0000ce00: 7075 7445 7863 6570 7469 6f6e 280a 2020  putException(.  
-0000ce10: 2020 2020 2020 2020 2020 2020 2020 2268                "h
-0000ce20: 6967 6865 7374 2061 6464 7265 7373 2069  ighest address i
-0000ce30: 7320 2564 2062 7574 2061 6464 7265 7373  s %d but address
-0000ce40: 206f 6620 6c61 7374 2072 6571 7565 7374   of last request
-0000ce50: 6564 2065 6c65 6d65 6e74 2069 7320 2564  ed element is %d
-0000ce60: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000ce70: 2020 2520 286d 6178 5f65 6c65 6d65 6e73    % (max_elemens
-0000ce80: 2c20 2866 6972 7374 5f65 6c65 6d65 6e74  , (first_element
-0000ce90: 202b 206e 756d 6265 725f 6f66 5f65 6c65   + number_of_ele
-0000cea0: 6d65 6e74 7329 290a 2020 2020 2020 2020  ments)).        
-0000ceb0: 2020 2020 290a 0a20 2020 2020 2020 2070      )..        p
-0000cec0: 6c63 5f76 616c 7565 7320 3d20 5b5d 0a0a  lc_values = []..
-0000ced0: 2020 2020 2020 2020 6966 206d 656d 5f74          if mem_t
-0000cee0: 7970 6520 6973 206c 632e 4d65 6d6f 7279  ype is lc.Memory
-0000cef0: 5479 7065 2e53 5452 494e 473a 0a20 2020  Type.STRING:.   
-0000cf00: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-0000cf10: 6e20 7261 6e67 6528 6e75 6d62 6572 5f6f  n range(number_o
-0000cf20: 665f 656c 656d 656e 7473 293a 0a20 2020  f_elements):.   
-0000cf30: 2020 2020 2020 2020 2020 2020 2061 6464               add
-0000cf40: 7265 7373 203d 2028 0a20 2020 2020 2020  ress = (.       
-0000cf50: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-0000cf60: 7274 5f61 6464 7265 7373 202b 2066 6972  rt_address + fir
-0000cf70: 7374 5f65 6c65 6d65 6e74 202a 206d 656d  st_element * mem
-0000cf80: 5f62 7974 655f 636f 756e 7420 2b20 6920  _byte_count + i 
-0000cf90: 2a20 6d65 6d5f 6279 7465 5f63 6f75 6e74  * mem_byte_count
-0000cfa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cfb0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0000cfc0: 2020 2020 7061 796c 6f61 6420 3d20 6279      payload = by
-0000cfd0: 7465 6172 7261 7928 290a 2020 2020 2020  tearray().      
-0000cfe0: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
-0000cff0: 642e 6578 7465 6e64 2873 7472 7563 742e  d.extend(struct.
-0000d000: 7061 636b 2822 214c 222c 2061 6464 7265  pack("!L", addre
-0000d010: 7373 2929 0a20 2020 2020 2020 2020 2020  ss)).           
-0000d020: 2020 2020 2070 6179 6c6f 6164 2e65 7874       payload.ext
-0000d030: 656e 6428 7374 7275 6374 2e70 6163 6b28  end(struct.pack(
-0000d040: 2221 4222 2c20 6d65 6d5f 6279 7465 5f63  "!B", mem_byte_c
-0000d050: 6f75 6e74 2929 0a20 2020 2020 2020 2020  ount)).         
-0000d060: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000d070: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
-0000d080: 6528 6c63 2e43 4d44 2e52 5f4d 422c 2070  e(lc.CMD.R_MB, p
-0000d090: 6179 6c6f 6164 2c20 6c63 2e52 5350 2e53  ayload, lc.RSP.S
-0000d0a0: 5f4d 4229 0a20 2020 2020 2020 2020 2020  _MB).           
-0000d0b0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000d0c0: 6365 2872 6573 756c 742c 2028 6279 7465  ce(result, (byte
-0000d0d0: 6172 7261 792c 2929 3a0a 2020 2020 2020  array,)):.      
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000d0f0: 6767 696e 672e 6465 6275 6728 0a20 2020  gging.debug(.   
-0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d110: 2020 2020 2022 7265 6164 2073 7472 696e       "read strin
-0000d120: 6720 2564 2077 6974 6820 6c65 6e67 7468  g %d with length
-0000d130: 2025 6422 2c0a 2020 2020 2020 2020 2020   %d",.          
-0000d140: 2020 2020 2020 2020 2020 2020 2020 2866                (f
-0000d150: 6972 7374 5f65 6c65 6d65 6e74 202b 2069  irst_element + i
-0000d160: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000d170: 2020 2020 2020 2020 2020 206c 656e 2872             len(r
-0000d180: 6573 756c 7429 2c0a 2020 2020 2020 2020  esult),.        
-0000d190: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1b0: 2020 2075 6e70 6163 6b5f 7374 7269 6e67     unpack_string
-0000d1c0: 203d 2022 7b7d 7322 2e66 6f72 6d61 7428   = "{}s".format(
-0000d1d0: 6c65 6e28 7265 7375 6c74 2929 0a0a 2020  len(result))..  
-0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1f0: 2020 706c 635f 7661 6c75 6573 2e61 7070    plc_values.app
-0000d200: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
-0000d210: 2020 2020 2020 2020 2020 2020 206c 6d2e               lm.
-0000d220: 6261 5f74 6f5f 7573 7472 2873 7472 7563  ba_to_ustr(struc
-0000d230: 742e 756e 7061 636b 2875 6e70 6163 6b5f  t.unpack(unpack_
-0000d240: 7374 7269 6e67 2c20 7265 7375 6c74 295b  string, result)[
-0000d250: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0000d260: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d270: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d290: 2020 2020 6c6f 6767 696e 672e 6572 726f      logging.erro
-0000d2a0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000d2b0: 2020 2020 2020 2020 2020 2022 6661 696c             "fail
-0000d2c0: 6564 2074 6f20 7265 6164 2073 7472 696e  ed to read strin
-0000d2d0: 6720 2564 2066 726f 6d20 6164 6472 6573  g %d from addres
-0000d2e0: 7320 2564 222c 0a20 2020 2020 2020 2020  s %d",.         
-0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000d300: 6669 7273 745f 656c 656d 656e 7420 2b20  first_element + 
-0000d310: 6929 2c0a 2020 2020 2020 2020 2020 2020  i),.            
-0000d320: 2020 2020 2020 2020 2020 2020 6164 6472              addr
-0000d330: 6573 732c 0a20 2020 2020 2020 2020 2020  ess,.           
-0000d340: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000d350: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d360: 6574 7572 6e20 5b5d 0a20 2020 2020 2020  eturn [].       
-0000d370: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d380: 2020 206d 6178 5f65 6c65 6d65 6e74 735f     max_elements_
-0000d390: 7065 725f 7472 616e 7366 6572 203d 206d  per_transfer = m
-0000d3a0: 6174 682e 666c 6f6f 7228 3235 3520 2f20  ath.floor(255 / 
-0000d3b0: 6d65 6d5f 6279 7465 5f63 6f75 6e74 290a  mem_byte_count).
-0000d3c0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-0000d3d0: 6772 6f75 7073 203d 206d 6174 682e 6365  groups = math.ce
-0000d3e0: 696c 286e 756d 6265 725f 6f66 5f65 6c65  il(number_of_ele
-0000d3f0: 6d65 6e74 7320 2f20 6d61 785f 656c 656d  ments / max_elem
-0000d400: 656e 7473 5f70 6572 5f74 7261 6e73 6665  ents_per_transfe
-0000d410: 7229 0a20 2020 2020 2020 2020 2020 206c  r).            l
-0000d420: 6f67 6769 6e67 2e64 6562 7567 280a 2020  ogging.debug(.  
-0000d430: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-0000d440: 656d 6f72 7920 7479 7065 2061 6c6c 6f77  emory type allow
-0000d450: 7320 2564 2065 6c65 6d65 6e74 7320 7065  s %d elements pe
-0000d460: 7220 7465 6c65 6772 616d 2c20 7370 6c69  r telegram, spli
-0000d470: 7420 7265 7175 6573 7420 696e 746f 2025  t request into %
-0000d480: 6420 6772 6f75 7028 7329 222c 0a20 2020  d group(s)",.   
-0000d490: 2020 2020 2020 2020 2020 2020 206d 6178               max
-0000d4a0: 5f65 6c65 6d65 6e74 735f 7065 725f 7472  _elements_per_tr
-0000d4b0: 616e 7366 6572 2c0a 2020 2020 2020 2020  ansfer,.        
-0000d4c0: 2020 2020 2020 2020 6e75 6d5f 6772 6f75          num_grou
-0000d4d0: 7073 2c0a 2020 2020 2020 2020 2020 2020  ps,.            
-0000d4e0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000d4f0: 6d61 696e 696e 675f 656c 656d 656e 7473  maining_elements
-0000d500: 203d 206e 756d 6265 725f 6f66 5f65 6c65   = number_of_ele
-0000d510: 6d65 6e74 730a 0a20 2020 2020 2020 2020  ments..         
-0000d520: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000d530: 6528 6e75 6d5f 6772 6f75 7073 293a 0a20  e(num_groups):. 
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d550: 6620 7265 6d61 696e 696e 675f 656c 656d  f remaining_elem
-0000d560: 656e 7473 203e 3d20 6d61 785f 656c 656d  ents >= max_elem
-0000d570: 656e 7473 5f70 6572 5f74 7261 6e73 6665  ents_per_transfe
-0000d580: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000d590: 2020 2020 2020 2065 6c65 6d65 6e74 735f         elements_
-0000d5a0: 696e 5f67 726f 7570 203d 206d 6178 5f65  in_group = max_e
-0000d5b0: 6c65 6d65 6e74 735f 7065 725f 7472 616e  lements_per_tran
-0000d5c0: 7366 6572 0a20 2020 2020 2020 2020 2020  sfer.           
-0000d5d0: 2020 2020 2020 2020 2072 656d 6169 6e69           remaini
-0000d5e0: 6e67 5f65 6c65 6d65 6e74 7320 2d3d 206d  ng_elements -= m
-0000d5f0: 6178 5f65 6c65 6d65 6e74 735f 7065 725f  ax_elements_per_
-0000d600: 7472 616e 7366 6572 0a20 2020 2020 2020  transfer.       
-0000d610: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d630: 2020 2065 6c65 6d65 6e74 735f 696e 5f67     elements_in_g
-0000d640: 726f 7570 203d 2072 656d 6169 6e69 6e67  roup = remaining
-0000d650: 5f65 6c65 6d65 6e74 730a 2020 2020 2020  _elements.      
-0000d660: 2020 2020 2020 2020 2020 6164 6472 6573            addres
-0000d670: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
-0000d680: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-0000d690: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-0000d6a0: 2020 2020 2020 2020 2020 2020 2b20 6669              + fi
-0000d6b0: 7273 745f 656c 656d 656e 7420 2a20 6d65  rst_element * me
-0000d6c0: 6d5f 6279 7465 5f63 6f75 6e74 0a20 2020  m_byte_count.   
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 202b 2069 202a 2065 6c65 6d65 6e74 735f   + i * elements_
-0000d6f0: 696e 5f67 726f 7570 202a 206d 656d 5f62  in_group * mem_b
-0000d700: 7974 655f 636f 756e 740a 2020 2020 2020  yte_count.      
-0000d710: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d720: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000d730: 696e 672e 6465 6275 6728 0a20 2020 2020  ing.debug(.     
-0000d740: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000d750: 6375 7272 656e 7420 7472 616e 7366 6572  current transfer
-0000d760: 2067 726f 7570 2025 6420 6861 7320 2564   group %d has %d
-0000d770: 2065 6c65 6d65 6e74 7322 2c20 692c 2065   elements", i, e
-0000d780: 6c65 6d65 6e74 735f 696e 5f67 726f 7570  lements_in_group
-0000d790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d7a0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0000d7b0: 2020 2020 7061 796c 6f61 6420 3d20 6279      payload = by
-0000d7c0: 7465 6172 7261 7928 290a 2020 2020 2020  tearray().      
-0000d7d0: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
-0000d7e0: 642e 6578 7465 6e64 2873 7472 7563 742e  d.extend(struct.
-0000d7f0: 7061 636b 2822 214c 222c 2061 6464 7265  pack("!L", addre
-0000d800: 7373 2929 0a20 2020 2020 2020 2020 2020  ss)).           
-0000d810: 2020 2020 2070 6179 6c6f 6164 2e65 7874       payload.ext
-0000d820: 656e 6428 7374 7275 6374 2e70 6163 6b28  end(struct.pack(
-0000d830: 2221 4222 2c20 656c 656d 656e 7473 5f69  "!B", elements_i
-0000d840: 6e5f 6772 6f75 7020 2a20 6d65 6d5f 6279  n_group * mem_by
-0000d850: 7465 5f63 6f75 6e74 2929 0a20 2020 2020  te_count)).     
-0000d860: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000d870: 7420 3d20 7365 6c66 2e5f 7365 6e64 5f72  t = self._send_r
-0000d880: 6563 6976 6528 6c63 2e43 4d44 2e52 5f4d  ecive(lc.CMD.R_M
-0000d890: 422c 2070 6179 6c6f 6164 2c20 6c63 2e52  B, payload, lc.R
-0000d8a0: 5350 2e53 5f4d 4229 0a20 2020 2020 2020  SP.S_MB).       
-0000d8b0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000d8c0: 7374 616e 6365 2872 6573 756c 742c 2028  stance(result, (
-0000d8d0: 6279 7465 6172 7261 792c 2929 3a0a 2020  bytearray,)):.  
-0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8f0: 2020 6c6f 6767 696e 672e 6465 6275 6728    logging.debug(
-0000d900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d910: 2020 2020 2020 2020 2022 7265 6164 2025           "read %
-0000d920: 6420 7661 6c75 6528 7329 2066 726f 6d20  d value(s) from 
-0000d930: 6164 6472 6573 7320 2564 222c 0a20 2020  address %d",.   
-0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d950: 2020 2020 2065 6c65 6d65 6e74 735f 696e       elements_in
-0000d960: 5f67 726f 7570 2c0a 2020 2020 2020 2020  _group,.        
-0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d980: 6669 7273 745f 656c 656d 656e 742c 0a20  first_element,. 
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000d9b0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0000d9c0: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
-0000d9d0: 6573 756c 7429 2c20 6d65 6d5f 6279 7465  esult), mem_byte
-0000d9e0: 5f63 6f75 6e74 293a 0a20 2020 2020 2020  _count):.       
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da00: 2070 6c63 5f76 616c 7565 732e 6170 7065   plc_values.appe
-0000da10: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 7374 7275 6374 2e75 6e70 6163 6b28 0a20  struct.unpack(. 
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0000da60: 6e70 6163 6b5f 7374 7269 6e67 2c20 7265  npack_string, re
-0000da70: 7375 6c74 5b6a 203a 206a 202b 206d 656d  sult[j : j + mem
-0000da80: 5f62 7974 655f 636f 756e 745d 0a20 2020  _byte_count].   
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2020 2020 2020 2020 2029 5b30 5d0a 2020           )[0].  
+0000bb60: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+0000bb70: 6c63 6f6d 2e6c 6173 745f 7265 7370 6f6e  lcom.last_respon
+0000bb80: 7365 2069 7320 6c63 2e52 5350 2e54 5f45  se is lc.RSP.T_E
+0000bb90: 520a 2020 2020 2020 2020 2020 2020 2020  R.              
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+0000bbb0: 2073 656c 662e 5f6c 6c63 6f6d 2e6c 6173   self._llcom.las
+0000bbc0: 745f 7265 7370 6f6e 7365 2069 7320 6c63  t_response is lc
+0000bbd0: 2e52 5350 2e54 5f42 440a 2020 2020 2020  .RSP.T_BD.      
+0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbf0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
+0000bc20: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc40: 2020 2020 2020 2022 616e 2065 7272 6f72         "an error
+0000bc50: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
+0000bc60: 6c6f 6164 696e 6720 7468 6520 6669 7273  loading the firs
+0000bc70: 7420 626c 6f63 6b20 6f66 2064 6174 6120  t block of data 
+0000bc80: 2573 2027 2573 2722 2c0a 2020 2020 2020  %s '%s'",.      
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0000bcb0: 6173 745f 6572 726f 722c 0a20 2020 2020  ast_error,.     
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcd0: 2020 2020 2020 2020 2020 206c 742e 6765             lt.ge
+0000bce0: 745f 6572 726f 725f 7465 7874 2873 656c  t_error_text(sel
+0000bcf0: 662e 6c61 7374 5f65 7272 6f72 292c 0a20  f.last_error),. 
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd30: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+0000bd40: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+0000bd50: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000bd60: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+0000bd70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000bd80: 662e 5f6c 6c63 6f6d 2e6c 6173 745f 7265  f._llcom.last_re
+0000bd90: 7370 6f6e 7365 2069 7320 6c63 2e52 5350  sponse is lc.RSP
+0000bda0: 2e54 5f45 520a 2020 2020 2020 2020 2020  .T_ER.          
+0000bdb0: 2020 2020 2020 2020 2020 6f72 2073 656c            or sel
+0000bdc0: 662e 5f6c 6c63 6f6d 2e6c 6173 745f 7265  f._llcom.last_re
+0000bdd0: 7370 6f6e 7365 2069 7320 6c63 2e52 5350  sponse is lc.RSP
+0000bde0: 2e54 5f42 440a 2020 2020 2020 2020 2020  .T_BD.          
+0000bdf0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0000be00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000be10: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
+0000be20: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+0000be30: 2020 2020 2020 2020 2020 2022 616e 2065             "an e
+0000be40: 7272 6f72 206f 6363 7572 7265 6420 7768  rror occurred wh
+0000be50: 696c 6520 6c6f 6164 696e 6720 7468 6520  ile loading the 
+0000be60: 6669 7273 7420 626c 6f63 6b20 6f66 2064  first block of d
+0000be70: 6174 6120 666f 7220 6669 6c65 2025 732c  ata for file %s,
+0000be80: 2025 7320 2725 7327 222c 0a20 2020 2020   %s '%s'",.     
+0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 2020 2072 656d 6f74 655f 7061 7468 2c0a     remote_path,.
+0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bec0: 2020 2020 2020 2020 7365 6c66 2e6c 6173          self.las
+0000bed0: 745f 6572 726f 722c 0a20 2020 2020 2020  t_error,.       
+0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bef0: 206c 742e 6765 745f 6572 726f 725f 7465   lt.get_error_te
+0000bf00: 7874 2873 656c 662e 6c61 7374 5f65 7272  xt(self.last_err
+0000bf10: 6f72 292c 0a20 2020 2020 2020 2020 2020  or),.           
+0000bf20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000bf30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000bf40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bf50: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+0000bf60: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
+0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf80: 2020 2022 636f 756c 6420 6e6f 7420 6c6f     "could not lo
+0000bf90: 6164 2066 696c 6520 7769 7468 2065 7272  ad file with err
+0000bfa0: 6f72 2025 7322 2c20 7365 6c66 2e5f 6c6c  or %s", self._ll
+0000bfb0: 636f 6d2e 6c61 7374 5f72 6573 706f 6e73  com.last_respons
+0000bfc0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000bfd0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000bfe0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0000bff0: 616c 7365 0a0a 2020 2020 2020 2020 7365  alse..        se
+0000c000: 6c66 2e5f 6c6f 6767 6572 2e69 6e66 6f28  lf._logger.info(
+0000c010: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+0000c020: 6365 6976 6564 2025 6420 6279 7465 7320  ceived %d bytes 
+0000c030: 7472 616e 7366 6572 2063 6f6d 706c 6574  transfer complet
+0000c040: 6520 666f 7220 6669 6c65 2025 7320 746f  e for file %s to
+0000c050: 2025 7322 2c0a 2020 2020 2020 2020 2020   %s",.          
+0000c060: 2020 6c6f 6361 6c5f 6669 6c65 2e73 7461    local_file.sta
+0000c070: 7428 292e 7374 5f73 697a 652c 0a20 2020  t().st_size,.   
+0000c080: 2020 2020 2020 2020 2072 656d 6f74 655f           remote_
+0000c090: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000c0a0: 2020 6c6f 6361 6c5f 6669 6c65 2c0a 2020    local_file,.  
+0000c0b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000c0c0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+0000c0d0: 2020 6465 6620 7265 6164 5f70 6c63 5f6d    def read_plc_m
+0000c0e0: 656d 6f72 7928 0a20 2020 2020 2020 2073  emory(.        s
+0000c0f0: 656c 662c 2066 6972 7374 5f65 6c65 6d65  elf, first_eleme
+0000c100: 6e74 3a20 696e 742c 206d 656d 5f74 7970  nt: int, mem_typ
+0000c110: 653a 206c 632e 4d65 6d6f 7279 5479 7065  e: lc.MemoryType
+0000c120: 2c20 6e75 6d62 6572 5f6f 665f 656c 656d  , number_of_elem
+0000c130: 656e 7473 3a20 696e 7420 3d20 310a 2020  ents: int = 1.  
+0000c140: 2020 2920 2d3e 206c 6973 743a 0a20 2020    ) -> list:.   
+0000c150: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c160: 2052 6561 6420 6461 7461 2066 726f 6d20   Read data from 
+0000c170: 706c 6320 6d65 6d6f 7279 2e0a 2020 2020  plc memory..    
+0000c180: 2020 2020 5265 7175 6972 6573 2061 6363      Requires acc
+0000c190: 6573 7320 6c65 7665 6c20 6060 504c 4344  ess level ``PLCD
+0000c1a0: 4542 5547 6060 2074 6f20 776f 726b 2e0a  EBUG`` to work..
+0000c1b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000c1c0: 6669 7273 745f 656c 656d 656e 743a 2077  first_element: w
+0000c1d0: 6869 6368 206d 656d 6f72 7920 6c6f 6361  hich memory loca
+0000c1e0: 7469 6f6e 2073 686f 756c 6420 6265 2072  tion should be r
+0000c1f0: 6561 642c 2073 7461 7274 7320 6174 2030  ead, starts at 0
+0000c200: 2075 7020 746f 2074 6865 206d 6178 206e   up to the max n
+0000c210: 756d 6265 7220 666f 7220 6561 6368 2074  umber for each t
+0000c220: 7970 650a 2020 2020 2020 2020 3a70 6172  ype.        :par
+0000c230: 616d 206d 656d 5f74 7970 653a 2077 6861  am mem_type: wha
+0000c240: 7420 6461 7461 7479 7065 2074 6f20 7265  t datatype to re
+0000c250: 6164 0a20 2020 2020 2020 203a 7061 7261  ad.        :para
+0000c260: 6d20 6e75 6d62 6572 5f6f 665f 656c 656d  m number_of_elem
+0000c270: 656e 7473 3a20 686f 7720 6d61 6e79 2065  ents: how many e
+0000c280: 6c65 6d65 6e74 7320 7368 6f75 6c64 2062  lements should b
+0000c290: 6520 7265 6164 0a0a 2020 2020 2020 2020  e read..        
+0000c2a0: 3a72 6169 7365 7320 4c53 5632 496e 7075  :raises LSV2Inpu
+0000c2b0: 7445 7863 6570 7469 6f6e 3a20 6966 2075  tException: if u
+0000c2c0: 6e6b 6e6f 776e 7320 6d65 6d6f 7279 2074  nknowns memory t
+0000c2d0: 7970 6520 6973 2072 6571 7565 7374 6564  ype is requested
+0000c2e0: 206f 7220 6966 2074 6865 2074 6f20 6d61   or if the to ma
+0000c2f0: 6e79 2065 6c65 6d65 6e74 7320 6172 6520  ny elements are 
+0000c300: 7265 7175 6573 7465 640a 2020 2020 2020  requested.      
+0000c310: 2020 3a72 6169 7365 7320 4c53 5632 4461    :raises LSV2Da
+0000c320: 7461 4578 6365 7074 696f 6e3a 2069 6620  taException: if 
+0000c330: 6e75 6d62 6572 206f 6620 7265 6365 6976  number of receiv
+0000c340: 6564 2076 616c 7565 7320 646f 6573 206e  ed values does n
+0000c350: 6f74 206d 6174 6368 2074 6865 206e 756d  ot match the num
+0000c360: 6265 7220 6f66 2065 7870 6563 7465 640a  ber of expected.
+0000c370: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0000c380: 2020 2020 2069 6620 7365 6c66 2e5f 7379       if self._sy
+0000c390: 735f 7061 722e 6c73 7632 5f76 6572 7369  s_par.lsv2_versi
+0000c3a0: 6f6e 2021 3d20 2d31 3a0a 2020 2020 2020  on != -1:.      
+0000c3b0: 2020 2020 2020 7365 6c66 2e5f 7265 6164        self._read
+0000c3c0: 5f70 6172 616d 6574 6572 7328 290a 0a20  _parameters().. 
+0000c3d0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000c3e0: 6c66 2e6c 6f67 696e 286c 6f67 696e 3d6c  lf.login(login=l
+0000c3f0: 632e 4c6f 6769 6e2e 504c 4344 4542 5547  c.Login.PLCDEBUG
+0000c400: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000c410: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
+0000c420: 696e 6728 2263 6f75 6c64 206e 6f74 206c  ing("could not l
+0000c430: 6f67 2069 6e20 6173 2075 7365 7220 504c  og in as user PL
+0000c440: 4344 4542 5547 2229 0a20 2020 2020 2020  CDEBUG").       
+0000c450: 2020 2020 2072 6574 7572 6e20 5b5d 0a0a       return []..
+0000c460: 2020 2020 2020 2020 6966 206d 656d 5f74          if mem_t
+0000c470: 7970 6520 6973 206c 632e 4d65 6d6f 7279  ype is lc.Memory
+0000c480: 5479 7065 2e4d 4152 4b45 523a 0a20 2020  Type.MARKER:.   
+0000c490: 2020 2020 2020 2020 2073 7461 7274 5f61           start_a
+0000c4a0: 6464 7265 7373 203d 2073 656c 662e 5f73  ddress = self._s
+0000c4b0: 7973 5f70 6172 2e6d 6172 6b65 7273 5f73  ys_par.markers_s
+0000c4c0: 7461 7274 5f61 6464 7265 7373 0a20 2020  tart_address.   
+0000c4d0: 2020 2020 2020 2020 206d 6178 5f65 6c65           max_ele
+0000c4e0: 6d65 6e74 7320 3d20 7365 6c66 2e5f 7379  ments = self._sy
+0000c4f0: 735f 7061 722e 6e75 6d62 6572 5f6f 665f  s_par.number_of_
+0000c500: 6d61 726b 6572 730a 2020 2020 2020 2020  markers.        
+0000c510: 2020 2020 6d65 6d5f 6279 7465 5f63 6f75      mem_byte_cou
+0000c520: 6e74 203d 2031 0a20 2020 2020 2020 2020  nt = 1.         
+0000c530: 2020 2075 6e70 6163 6b5f 7374 7269 6e67     unpack_string
+0000c540: 203d 2022 213f 220a 2020 2020 2020 2020   = "!?".        
+0000c550: 656c 6966 206d 656d 5f74 7970 6520 6973  elif mem_type is
+0000c560: 206c 632e 4d65 6d6f 7279 5479 7065 2e49   lc.MemoryType.I
+0000c570: 4e50 5554 3a0a 2020 2020 2020 2020 2020  NPUT:.          
+0000c580: 2020 7374 6172 745f 6164 6472 6573 7320    start_address 
+0000c590: 3d20 7365 6c66 2e5f 7379 735f 7061 722e  = self._sys_par.
+0000c5a0: 696e 7075 7473 5f73 7461 7274 5f61 6464  inputs_start_add
+0000c5b0: 7265 7373 0a20 2020 2020 2020 2020 2020  ress.           
+0000c5c0: 206d 6178 5f65 6c65 6d65 6e74 7320 3d20   max_elements = 
+0000c5d0: 7365 6c66 2e5f 7379 735f 7061 722e 6e75  self._sys_par.nu
+0000c5e0: 6d62 6572 5f6f 665f 696e 7075 7473 0a20  mber_of_inputs. 
+0000c5f0: 2020 2020 2020 2020 2020 206d 656d 5f62             mem_b
+0000c600: 7974 655f 636f 756e 7420 3d20 310a 2020  yte_count = 1.  
+0000c610: 2020 2020 2020 2020 2020 756e 7061 636b            unpack
+0000c620: 5f73 7472 696e 6720 3d20 2221 3f22 0a20  _string = "!?". 
+0000c630: 2020 2020 2020 2065 6c69 6620 6d65 6d5f         elif mem_
+0000c640: 7479 7065 2069 7320 6c63 2e4d 656d 6f72  type is lc.Memor
+0000c650: 7954 7970 652e 4f55 5450 5554 3a0a 2020  yType.OUTPUT:.  
+0000c660: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0000c670: 6164 6472 6573 7320 3d20 7365 6c66 2e5f  address = self._
+0000c680: 7379 735f 7061 722e 6f75 7470 7574 735f  sys_par.outputs_
+0000c690: 7374 6172 745f 6164 6472 6573 730a 2020  start_address.  
+0000c6a0: 2020 2020 2020 2020 2020 6d61 785f 656c            max_el
+0000c6b0: 656d 656e 7473 203d 2073 656c 662e 5f73  ements = self._s
+0000c6c0: 7973 5f70 6172 2e6e 756d 6265 725f 6f66  ys_par.number_of
+0000c6d0: 5f6f 7574 7075 7473 0a20 2020 2020 2020  _outputs.       
+0000c6e0: 2020 2020 206d 656d 5f62 7974 655f 636f       mem_byte_co
+0000c6f0: 756e 7420 3d20 310a 2020 2020 2020 2020  unt = 1.        
+0000c700: 2020 2020 756e 7061 636b 5f73 7472 696e      unpack_strin
+0000c710: 6720 3d20 2221 3f22 0a20 2020 2020 2020  g = "!?".       
+0000c720: 2065 6c69 6620 6d65 6d5f 7479 7065 2069   elif mem_type i
+0000c730: 7320 6c63 2e4d 656d 6f72 7954 7970 652e  s lc.MemoryType.
+0000c740: 434f 554e 5445 523a 0a20 2020 2020 2020  COUNTER:.       
+0000c750: 2020 2020 2073 7461 7274 5f61 6464 7265       start_addre
+0000c760: 7373 203d 2073 656c 662e 5f73 7973 5f70  ss = self._sys_p
+0000c770: 6172 2e63 6f75 6e74 6572 735f 7374 6172  ar.counters_star
+0000c780: 745f 6164 6472 6573 730a 2020 2020 2020  t_address.      
+0000c790: 2020 2020 2020 6d61 785f 656c 656d 656e        max_elemen
+0000c7a0: 7473 203d 2073 656c 662e 5f73 7973 5f70  ts = self._sys_p
+0000c7b0: 6172 2e6e 756d 6265 725f 6f66 5f63 6f75  ar.number_of_cou
+0000c7c0: 6e74 6572 730a 2020 2020 2020 2020 2020  nters.          
+0000c7d0: 2020 6d65 6d5f 6279 7465 5f63 6f75 6e74    mem_byte_count
+0000c7e0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+0000c7f0: 2075 6e70 6163 6b5f 7374 7269 6e67 203d   unpack_string =
+0000c800: 2022 213f 220a 2020 2020 2020 2020 656c   "!?".        el
+0000c810: 6966 206d 656d 5f74 7970 6520 6973 206c  if mem_type is l
+0000c820: 632e 4d65 6d6f 7279 5479 7065 2e54 494d  c.MemoryType.TIM
+0000c830: 4552 3a0a 2020 2020 2020 2020 2020 2020  ER:.            
+0000c840: 7374 6172 745f 6164 6472 6573 7320 3d20  start_address = 
+0000c850: 7365 6c66 2e5f 7379 735f 7061 722e 7469  self._sys_par.ti
+0000c860: 6d65 7273 5f73 7461 7274 5f61 6464 7265  mers_start_addre
+0000c870: 7373 0a20 2020 2020 2020 2020 2020 206d  ss.            m
+0000c880: 6178 5f65 6c65 6d65 6e74 7320 3d20 7365  ax_elements = se
+0000c890: 6c66 2e5f 7379 735f 7061 722e 6e75 6d62  lf._sys_par.numb
+0000c8a0: 6572 5f6f 665f 7469 6d65 7273 0a20 2020  er_of_timers.   
+0000c8b0: 2020 2020 2020 2020 206d 656d 5f62 7974           mem_byt
+0000c8c0: 655f 636f 756e 7420 3d20 310a 2020 2020  e_count = 1.    
+0000c8d0: 2020 2020 2020 2020 756e 7061 636b 5f73          unpack_s
+0000c8e0: 7472 696e 6720 3d20 2221 3f22 0a20 2020  tring = "!?".   
+0000c8f0: 2020 2020 2065 6c69 6620 6d65 6d5f 7479       elif mem_ty
+0000c900: 7065 2069 7320 6c63 2e4d 656d 6f72 7954  pe is lc.MemoryT
+0000c910: 7970 652e 4259 5445 3a0a 2020 2020 2020  ype.BYTE:.      
+0000c920: 2020 2020 2020 7374 6172 745f 6164 6472        start_addr
+0000c930: 6573 7320 3d20 7365 6c66 2e5f 7379 735f  ess = self._sys_
+0000c940: 7061 722e 776f 7264 735f 7374 6172 745f  par.words_start_
+0000c950: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
+0000c960: 2020 2020 6d61 785f 656c 656d 656e 7473      max_elements
+0000c970: 203d 2073 656c 662e 5f73 7973 5f70 6172   = self._sys_par
+0000c980: 2e6e 756d 6265 725f 6f66 5f77 6f72 6473  .number_of_words
+0000c990: 202a 2032 0a20 2020 2020 2020 2020 2020   * 2.           
+0000c9a0: 206d 656d 5f62 7974 655f 636f 756e 7420   mem_byte_count 
+0000c9b0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+0000c9c0: 756e 7061 636b 5f73 7472 696e 6720 3d20  unpack_string = 
+0000c9d0: 223c 6222 0a20 2020 2020 2020 2065 6c69  "<b".        eli
+0000c9e0: 6620 6d65 6d5f 7479 7065 2069 7320 6c63  f mem_type is lc
+0000c9f0: 2e4d 656d 6f72 7954 7970 652e 574f 5244  .MemoryType.WORD
+0000ca00: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
+0000ca10: 6172 745f 6164 6472 6573 7320 3d20 7365  art_address = se
+0000ca20: 6c66 2e5f 7379 735f 7061 722e 776f 7264  lf._sys_par.word
+0000ca30: 735f 7374 6172 745f 6164 6472 6573 730a  s_start_address.
+0000ca40: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0000ca50: 656c 656d 656e 7473 203d 2073 656c 662e  elements = self.
+0000ca60: 5f73 7973 5f70 6172 2e6e 756d 6265 725f  _sys_par.number_
+0000ca70: 6f66 5f77 6f72 6473 0a20 2020 2020 2020  of_words.       
+0000ca80: 2020 2020 206d 656d 5f62 7974 655f 636f       mem_byte_co
+0000ca90: 756e 7420 3d20 320a 2020 2020 2020 2020  unt = 2.        
+0000caa0: 2020 2020 756e 7061 636b 5f73 7472 696e      unpack_strin
+0000cab0: 6720 3d20 223c 6822 0a20 2020 2020 2020  g = "<h".       
+0000cac0: 2065 6c69 6620 6d65 6d5f 7479 7065 2069   elif mem_type i
+0000cad0: 7320 6c63 2e4d 656d 6f72 7954 7970 652e  s lc.MemoryType.
+0000cae0: 4457 4f52 443a 0a20 2020 2020 2020 2020  DWORD:.         
+0000caf0: 2020 2073 7461 7274 5f61 6464 7265 7373     start_address
+0000cb00: 203d 2073 656c 662e 5f73 7973 5f70 6172   = self._sys_par
+0000cb10: 2e77 6f72 6473 5f73 7461 7274 5f61 6464  .words_start_add
+0000cb20: 7265 7373 0a20 2020 2020 2020 2020 2020  ress.           
+0000cb30: 206d 6178 5f65 6c65 6d65 6e74 7320 3d20   max_elements = 
+0000cb40: 7365 6c66 2e5f 7379 735f 7061 722e 6e75  self._sys_par.nu
+0000cb50: 6d62 6572 5f6f 665f 776f 7264 7320 2f20  mber_of_words / 
+0000cb60: 340a 2020 2020 2020 2020 2020 2020 6d65  4.            me
+0000cb70: 6d5f 6279 7465 5f63 6f75 6e74 203d 2034  m_byte_count = 4
+0000cb80: 0a20 2020 2020 2020 2020 2020 2075 6e70  .            unp
+0000cb90: 6163 6b5f 7374 7269 6e67 203d 2022 3c6c  ack_string = "<l
+0000cba0: 220a 2020 2020 2020 2020 656c 6966 206d  ".        elif m
+0000cbb0: 656d 5f74 7970 6520 6973 206c 632e 4d65  em_type is lc.Me
+0000cbc0: 6d6f 7279 5479 7065 2e53 5452 494e 473a  moryType.STRING:
+0000cbd0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+0000cbe0: 7274 5f61 6464 7265 7373 203d 2073 656c  rt_address = sel
+0000cbf0: 662e 5f73 7973 5f70 6172 2e73 7472 696e  f._sys_par.strin
+0000cc00: 6773 5f73 7461 7274 5f61 6464 7265 7373  gs_start_address
+0000cc10: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000cc20: 5f65 6c65 6d65 6e74 7320 3d20 7365 6c66  _elements = self
+0000cc30: 2e5f 7379 735f 7061 722e 6e75 6d62 6572  ._sys_par.number
+0000cc40: 5f6f 665f 7374 7269 6e67 730a 2020 2020  _of_strings.    
+0000cc50: 2020 2020 2020 2020 6d65 6d5f 6279 7465          mem_byte
+0000cc60: 5f63 6f75 6e74 203d 2073 656c 662e 5f73  _count = self._s
+0000cc70: 7973 5f70 6172 2e6d 6178 5f73 7472 696e  ys_par.max_strin
+0000cc80: 675f 6c65 6e67 6874 0a20 2020 2020 2020  g_lenght.       
+0000cc90: 2020 2020 2075 6e70 6163 6b5f 7374 7269       unpack_stri
+0000cca0: 6e67 203d 2022 7b7d 7322 2e66 6f72 6d61  ng = "{}s".forma
+0000ccb0: 7428 6d65 6d5f 6279 7465 5f63 6f75 6e74  t(mem_byte_count
+0000ccc0: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
+0000ccd0: 656d 5f74 7970 6520 6973 206c 632e 4d65  em_type is lc.Me
+0000cce0: 6d6f 7279 5479 7065 2e49 4e50 5554 5f57  moryType.INPUT_W
+0000ccf0: 4f52 443a 0a20 2020 2020 2020 2020 2020  ORD:.           
+0000cd00: 2073 7461 7274 5f61 6464 7265 7373 203d   start_address =
+0000cd10: 2073 656c 662e 5f73 7973 5f70 6172 2e69   self._sys_par.i
+0000cd20: 6e70 7574 5f77 6f72 6473 5f73 7461 7274  nput_words_start
+0000cd30: 5f61 6464 7265 7373 0a20 2020 2020 2020  _address.       
+0000cd40: 2020 2020 206d 6178 5f65 6c65 6d65 6e74       max_element
+0000cd50: 7320 3d20 7365 6c66 2e5f 7379 735f 7061  s = self._sys_pa
+0000cd60: 722e 6e75 6d62 6572 5f6f 665f 696e 7075  r.number_of_inpu
+0000cd70: 745f 776f 7264 730a 2020 2020 2020 2020  t_words.        
+0000cd80: 2020 2020 6d65 6d5f 6279 7465 5f63 6f75      mem_byte_cou
+0000cd90: 6e74 203d 2032 0a20 2020 2020 2020 2020  nt = 2.         
+0000cda0: 2020 2075 6e70 6163 6b5f 7374 7269 6e67     unpack_string
+0000cdb0: 203d 2022 3c48 220a 2020 2020 2020 2020   = "<H".        
+0000cdc0: 656c 6966 206d 656d 5f74 7970 6520 6973  elif mem_type is
+0000cdd0: 206c 632e 4d65 6d6f 7279 5479 7065 2e4f   lc.MemoryType.O
+0000cde0: 5554 5055 545f 574f 5244 3a0a 2020 2020  UTPUT_WORD:.    
+0000cdf0: 2020 2020 2020 2020 7374 6172 745f 6164          start_ad
+0000ce00: 6472 6573 7320 3d20 7365 6c66 2e5f 7379  dress = self._sy
+0000ce10: 735f 7061 722e 6f75 7470 7574 5f77 6f72  s_par.output_wor
+0000ce20: 6473 5f73 7461 7274 5f61 6464 7265 7373  ds_start_address
+0000ce30: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000ce40: 5f65 6c65 6d65 6e74 7320 3d20 7365 6c66  _elements = self
+0000ce50: 2e5f 7379 735f 7061 722e 6e75 6d62 6572  ._sys_par.number
+0000ce60: 5f6f 665f 6f75 7470 7574 5f77 6f72 6473  _of_output_words
+0000ce70: 0a20 2020 2020 2020 2020 2020 206d 656d  .            mem
+0000ce80: 5f62 7974 655f 636f 756e 7420 3d20 320a  _byte_count = 2.
+0000ce90: 2020 2020 2020 2020 2020 2020 756e 7061              unpa
+0000cea0: 636b 5f73 7472 696e 6720 3d20 223c 4822  ck_string = "<H"
+0000ceb0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000cec0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000ced0: 204c 5356 3249 6e70 7574 4578 6365 7074   LSV2InputExcept
+0000cee0: 696f 6e28 2275 6e6b 6e6f 776e 2061 6464  ion("unknown add
+0000cef0: 7265 7373 2074 7970 6522 290a 0a20 2020  ress type")..   
+0000cf00: 2020 2020 2069 6620 2866 6972 7374 5f65       if (first_e
+0000cf10: 6c65 6d65 6e74 202b 206e 756d 6265 725f  lement + number_
+0000cf20: 6f66 5f65 6c65 6d65 6e74 7329 203e 206d  of_elements) > m
+0000cf30: 6178 5f65 6c65 6d65 6e74 733a 0a20 2020  ax_elements:.   
+0000cf40: 2020 2020 2020 2020 2072 6169 7365 204c           raise L
+0000cf50: 5356 3249 6e70 7574 4578 6365 7074 696f  SV2InputExceptio
+0000cf60: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000cf70: 2020 2022 6869 6768 6573 7420 6164 6472     "highest addr
+0000cf80: 6573 7320 6973 2025 6420 6275 7420 6164  ess is %d but ad
+0000cf90: 6472 6573 7320 6f66 206c 6173 7420 7265  dress of last re
+0000cfa0: 7175 6573 7465 6420 656c 656d 656e 7420  quested element 
+0000cfb0: 6973 2025 6422 0a20 2020 2020 2020 2020  is %d".         
+0000cfc0: 2020 2020 2020 2025 2028 6d61 785f 656c         % (max_el
+0000cfd0: 656d 656e 7473 2c20 2866 6972 7374 5f65  ements, (first_e
+0000cfe0: 6c65 6d65 6e74 202b 206e 756d 6265 725f  lement + number_
+0000cff0: 6f66 5f65 6c65 6d65 6e74 7329 290a 2020  of_elements)).  
+0000d000: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000d010: 2020 2020 2070 6c63 5f76 616c 7565 7320       plc_values 
+0000d020: 3d20 5b5d 0a0a 2020 2020 2020 2020 6966  = []..        if
+0000d030: 206d 656d 5f74 7970 6520 6973 206c 632e   mem_type is lc.
+0000d040: 4d65 6d6f 7279 5479 7065 2e53 5452 494e  MemoryType.STRIN
+0000d050: 473a 0a20 2020 2020 2020 2020 2020 2066  G:.            f
+0000d060: 6f72 2069 2069 6e20 7261 6e67 6528 6e75  or i in range(nu
+0000d070: 6d62 6572 5f6f 665f 656c 656d 656e 7473  mber_of_elements
+0000d080: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000d090: 2020 2061 6464 7265 7373 203d 2028 0a20     address = (. 
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 2073 7461 7274 5f61 6464 7265 7373     start_address
+0000d0c0: 202b 2066 6972 7374 5f65 6c65 6d65 6e74   + first_element
+0000d0d0: 202a 206d 656d 5f62 7974 655f 636f 756e   * mem_byte_coun
+0000d0e0: 7420 2b20 6920 2a20 6d65 6d5f 6279 7465  t + i * mem_byte
+0000d0f0: 5f63 6f75 6e74 0a20 2020 2020 2020 2020  _count.         
+0000d100: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000d110: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
+0000d120: 6420 3d20 6279 7465 6172 7261 7928 290a  d = bytearray().
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 7061 796c 6f61 642e 6578 7465 6e64 2873  payload.extend(s
+0000d150: 7472 7563 742e 7061 636b 2822 214c 222c  truct.pack("!L",
+0000d160: 2061 6464 7265 7373 2929 0a20 2020 2020   address)).     
+0000d170: 2020 2020 2020 2020 2020 2070 6179 6c6f             paylo
+0000d180: 6164 2e65 7874 656e 6428 7374 7275 6374  ad.extend(struct
+0000d190: 2e70 6163 6b28 2221 4222 2c20 6d65 6d5f  .pack("!B", mem_
+0000d1a0: 6279 7465 5f63 6f75 6e74 2929 0a20 2020  byte_count)).   
+0000d1b0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0000d1c0: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
+0000d1d0: 5f72 6563 6976 6528 6c63 2e43 4d44 2e52  _recive(lc.CMD.R
+0000d1e0: 5f4d 422c 2070 6179 6c6f 6164 2c20 6c63  _MB, payload, lc
+0000d1f0: 2e52 5350 2e53 5f4d 4229 0a20 2020 2020  .RSP.S_MB).     
+0000d200: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000d210: 696e 7374 616e 6365 2872 6573 756c 742c  instance(result,
+0000d220: 2028 6279 7465 6172 7261 792c 2929 3a0a   (bytearray,)):.
+0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d240: 2020 2020 6c6f 6767 696e 672e 6465 6275      logging.debu
+0000d250: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+0000d260: 2020 2020 2020 2020 2020 2022 7265 6164             "read
+0000d270: 2073 7472 696e 6720 2564 2077 6974 6820   string %d with 
+0000d280: 6c65 6e67 7468 2025 6422 2c0a 2020 2020  length %d",.    
+0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 2020 2020 2866 6972 7374 5f65 6c65 6d65      (first_eleme
+0000d2b0: 6e74 202b 2069 292c 0a20 2020 2020 2020  nt + i),.       
+0000d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2d0: 206c 656e 2872 6573 756c 7429 2c0a 2020   len(result),.  
+0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2f0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0000d300: 2020 2020 2020 2020 2075 6e70 6163 6b5f           unpack_
+0000d310: 7374 7269 6e67 203d 2022 7b7d 7322 2e66  string = "{}s".f
+0000d320: 6f72 6d61 7428 6c65 6e28 7265 7375 6c74  ormat(len(result
+0000d330: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+0000d340: 2020 2020 2020 2020 706c 635f 7661 6c75          plc_valu
+0000d350: 6573 2e61 7070 656e 6428 0a20 2020 2020  es.append(.     
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d370: 2020 206c 6d2e 6261 5f74 6f5f 7573 7472     lm.ba_to_ustr
+0000d380: 2873 7472 7563 742e 756e 7061 636b 2875  (struct.unpack(u
+0000d390: 6e70 6163 6b5f 7374 7269 6e67 2c20 7265  npack_string, re
+0000d3a0: 7375 6c74 295b 305d 290a 2020 2020 2020  sult)[0]).      
+0000d3b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000d3e0: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+0000d3f0: 672e 6572 726f 7228 0a20 2020 2020 2020  g.error(.       
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d410: 2022 6661 696c 6564 2074 6f20 7265 6164   "failed to read
+0000d420: 2073 7472 696e 6720 2564 2066 726f 6d20   string %d from 
+0000d430: 6164 6472 6573 7320 2564 222c 0a20 2020  address %d",.   
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 2020 2020 2028 6669 7273 745f 656c 656d       (first_elem
+0000d460: 656e 7420 2b20 6929 2c0a 2020 2020 2020  ent + i),.      
+0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d480: 2020 6164 6472 6573 732c 0a20 2020 2020    address,.     
+0000d490: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000d4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d4b0: 2020 2020 2072 6574 7572 6e20 5b5d 0a20       return []. 
+0000d4c0: 2020 2020 2020 2065 6c73 653a 0a0a 2020         else:..  
+0000d4d0: 2020 2020 2020 2020 2020 6d61 785f 656c            max_el
+0000d4e0: 656d 656e 7473 5f70 6572 5f74 7261 6e73  ements_per_trans
+0000d4f0: 6665 7220 3d20 6d61 7468 2e66 6c6f 6f72  fer = math.floor
+0000d500: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000d510: 2020 3235 3520 2f20 6d65 6d5f 6279 7465    255 / mem_byte
+0000d520: 5f63 6f75 6e74 2920 2d20 3120 2023 2073  _count) - 1  # s
+0000d530: 7562 7472 6163 7420 3120 666f 7220 7361  ubtract 1 for sa
+0000d540: 6665 7479 0a20 2020 2020 2020 2020 2020  fety.           
+0000d550: 206e 756d 5f67 726f 7570 7320 3d20 6d61   num_groups = ma
+0000d560: 7468 2e63 6569 6c28 0a20 2020 2020 2020  th.ceil(.       
+0000d570: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+0000d580: 6f66 5f65 6c65 6d65 6e74 7320 2f20 6d61  of_elements / ma
+0000d590: 785f 656c 656d 656e 7473 5f70 6572 5f74  x_elements_per_t
+0000d5a0: 7261 6e73 6665 7229 0a20 2020 2020 2020  ransfer).       
+0000d5b0: 2020 2020 206c 6f67 6769 6e67 2e64 6562       logging.deb
+0000d5c0: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
+0000d5d0: 2020 2020 226d 656d 6f72 7920 7479 7065      "memory type
+0000d5e0: 2061 6c6c 6f77 7320 2564 2065 6c65 6d65   allows %d eleme
+0000d5f0: 6e74 7320 7065 7220 7465 6c65 6772 616d  nts per telegram
+0000d600: 2c20 7370 6c69 7420 7265 7175 6573 7420  , split request 
+0000d610: 696e 746f 2025 6420 6772 6f75 7028 7329  into %d group(s)
+0000d620: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000d630: 2020 206d 6178 5f65 6c65 6d65 6e74 735f     max_elements_
+0000d640: 7065 725f 7472 616e 7366 6572 2c0a 2020  per_transfer,.  
+0000d650: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+0000d660: 6d5f 6772 6f75 7073 2c0a 2020 2020 2020  m_groups,.      
+0000d670: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000d680: 2020 2020 2072 656d 6169 6e69 6e67 5f65       remaining_e
+0000d690: 6c65 6d65 6e74 7320 3d20 6e75 6d62 6572  lements = number
+0000d6a0: 5f6f 665f 656c 656d 656e 7473 0a20 2020  _of_elements.   
+0000d6b0: 2020 2020 2020 2020 2066 6972 7374 5f65           first_e
+0000d6c0: 6c65 6d65 6e74 5f69 6e5f 6772 6f75 7020  lement_in_group 
+0000d6d0: 3d20 6669 7273 745f 656c 656d 656e 740a  = first_element.
+0000d6e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000d6f0: 2069 2069 6e20 7261 6e67 6528 6e75 6d5f   i in range(num_
+0000d700: 6772 6f75 7073 293a 0a0a 2020 2020 2020  groups):..      
+0000d710: 2020 2020 2020 2020 2020 2320 6465 7465            # dete
+0000d720: 726d 696e 6520 6e75 6d62 6572 206f 6620  rmine number of 
+0000d730: 656c 656d 656e 7473 2066 6f72 2074 6869  elements for thi
+0000d740: 7320 6772 6f75 700a 2020 2020 2020 2020  s group.        
+0000d750: 2020 2020 2020 2020 6966 2072 656d 6169          if remai
+0000d760: 6e69 6e67 5f65 6c65 6d65 6e74 7320 3e20  ning_elements > 
+0000d770: 6d61 785f 656c 656d 656e 7473 5f70 6572  max_elements_per
+0000d780: 5f74 7261 6e73 6665 723a 0a20 2020 2020  _transfer:.     
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000d7a0: 6c65 6d65 6e74 735f 696e 5f67 726f 7570  lements_in_group
+0000d7b0: 203d 206d 6178 5f65 6c65 6d65 6e74 735f   = max_elements_
+0000d7c0: 7065 725f 7472 616e 7366 6572 0a20 2020  per_transfer.   
+0000d7d0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000d7e0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000d7f0: 2020 2020 2020 2065 6c65 6d65 6e74 735f         elements_
+0000d800: 696e 5f67 726f 7570 203d 2072 656d 6169  in_group = remai
+0000d810: 6e69 6e67 5f65 6c65 6d65 6e74 730a 0a20  ning_elements.. 
+0000d820: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000d830: 6464 7265 7373 203d 2073 7461 7274 5f61  ddress = start_a
+0000d840: 6464 7265 7373 202b 2066 6972 7374 5f65  ddress + first_e
+0000d850: 6c65 6d65 6e74 5f69 6e5f 6772 6f75 7020  lement_in_group 
+0000d860: 2a20 6d65 6d5f 6279 7465 5f63 6f75 6e74  * mem_byte_count
+0000d870: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d880: 2020 6c6f 6767 696e 672e 6465 6275 6728    logging.debug(
+0000d890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d8a0: 2020 2020 2022 6375 7272 656e 7420 7472       "current tr
+0000d8b0: 616e 7366 6572 2067 726f 7570 2025 6420  ansfer group %d 
+0000d8c0: 6861 7320 2564 2065 6c65 6d65 6e74 7322  has %d elements"
+0000d8d0: 2c20 692c 2065 6c65 6d65 6e74 735f 696e  , i, elements_in
+0000d8e0: 5f67 726f 7570 0a20 2020 2020 2020 2020  _group.         
+0000d8f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000d900: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
+0000d910: 6420 3d20 6279 7465 6172 7261 7928 290a  d = bytearray().
+0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d930: 7061 796c 6f61 642e 6578 7465 6e64 2873  payload.extend(s
+0000d940: 7472 7563 742e 7061 636b 2822 214c 222c  truct.pack("!L",
+0000d950: 2061 6464 7265 7373 2929 0a20 2020 2020   address)).     
+0000d960: 2020 2020 2020 2020 2020 2070 6179 6c6f             paylo
+0000d970: 6164 2e65 7874 656e 6428 7374 7275 6374  ad.extend(struct
+0000d980: 2e70 6163 6b28 0a20 2020 2020 2020 2020  .pack(.         
+0000d990: 2020 2020 2020 2020 2020 2022 2142 222c             "!B",
+0000d9a0: 2065 6c65 6d65 6e74 735f 696e 5f67 726f   elements_in_gro
+0000d9b0: 7570 202a 206d 656d 5f62 7974 655f 636f  up * mem_byte_co
+0000d9c0: 756e 7429 290a 2020 2020 2020 2020 2020  unt)).          
+0000d9d0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0000d9e0: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
+0000d9f0: 286c 632e 434d 442e 525f 4d42 2c20 7061  (lc.CMD.R_MB, pa
+0000da00: 796c 6f61 642c 206c 632e 5253 502e 535f  yload, lc.RSP.S_
+0000da10: 4d42 290a 2020 2020 2020 2020 2020 2020  MB).            
+0000da20: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000da30: 6528 7265 7375 6c74 2c20 2862 7974 6561  e(result, (bytea
+0000da40: 7272 6179 2c29 293a 0a20 2020 2020 2020  rray,)):.       
+0000da50: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000da60: 6769 6e67 2e64 6562 7567 280a 2020 2020  ging.debug(.    
+0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da80: 2020 2020 2272 6561 6420 2564 2076 616c      "read %d val
+0000da90: 7565 2873 2920 6672 6f6d 2061 6464 7265  ue(s) from addre
+0000daa0: 7373 2025 6422 2c0a 2020 2020 2020 2020  ss %d",.        
 0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dac0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000dad0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daf0: 2020 6c6f 6767 696e 672e 6572 726f 7228    logging.error(
-0000db00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000db10: 2020 2020 2020 2020 2022 6661 696c 6564           "failed
-0000db20: 2074 6f20 7265 6164 2076 616c 7565 2066   to read value f
-0000db30: 726f 6d20 6164 6472 6573 7320 2564 222c  rom address %d",
-0000db40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000db50: 2020 2020 2020 2020 2073 7461 7274 5f61           start_a
-0000db60: 6464 7265 7373 202b 2066 6972 7374 5f65  ddress + first_e
-0000db70: 6c65 6d65 6e74 2c0a 2020 2020 2020 2020  lement,.        
-0000db80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000dac0: 656c 656d 656e 7473 5f69 6e5f 6772 6f75  elements_in_grou
+0000dad0: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+0000dae0: 2020 2020 2020 2020 2020 2066 6972 7374             first
+0000daf0: 5f65 6c65 6d65 6e74 5f69 6e5f 6772 6f75  _element_in_grou
+0000db00: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+0000db10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000db20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000db30: 206a 2069 6e20 7261 6e67 6528 302c 206c   j in range(0, l
+0000db40: 656e 2872 6573 756c 7429 2c20 6d65 6d5f  en(result), mem_
+0000db50: 6279 7465 5f63 6f75 6e74 293a 0a20 2020  byte_count):.   
+0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db70: 2020 2020 2070 6c63 5f76 616c 7565 732e       plc_values.
+0000db80: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
 0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dba0: 2020 7265 7475 726e 205b 5d0a 2020 2020    return [].    
-0000dbb0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-0000dbc0: 6465 6275 6728 2272 6561 6420 6120 746f  debug("read a to
-0000dbd0: 7461 6c20 6f66 2025 6420 7661 6c75 6528  tal of %d value(
-0000dbe0: 7329 222c 206c 656e 2870 6c63 5f76 616c  s)", len(plc_val
-0000dbf0: 7565 7329 290a 2020 2020 2020 2020 6966  ues)).        if
-0000dc00: 206c 656e 2870 6c63 5f76 616c 7565 7329   len(plc_values)
-0000dc10: 2021 3d20 6e75 6d62 6572 5f6f 665f 656c   != number_of_el
-0000dc20: 656d 656e 7473 3a0a 2020 2020 2020 2020  ements:.        
-0000dc30: 2020 2020 7261 6973 6520 4c53 5632 4461      raise LSV2Da
-0000dc40: 7461 4578 6365 7074 696f 6e28 0a20 2020  taException(.   
-0000dc50: 2020 2020 2020 2020 2020 2020 2022 6e75               "nu
-0000dc60: 6d62 6572 206f 6620 7265 6365 6976 6564  mber of received
-0000dc70: 2076 616c 7565 7320 2564 2069 7320 6e6f   values %d is no
-0000dc80: 7420 6571 7561 6c20 746f 206e 756d 6265  t equal to numbe
-0000dc90: 7220 6f66 2072 6571 7565 7374 6564 2025  r of requested %
-0000dca0: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
-0000dcb0: 2020 2025 2028 6c65 6e28 706c 635f 7661     % (len(plc_va
-0000dcc0: 6c75 6573 292c 206e 756d 6265 725f 6f66  lues), number_of
-0000dcd0: 5f65 6c65 6d65 6e74 7329 0a20 2020 2020  _elements).     
-0000dce0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000dcf0: 2072 6574 7572 6e20 706c 635f 7661 6c75   return plc_valu
-0000dd00: 6573 0a0a 2020 2020 6465 6620 7365 745f  es..    def set_
-0000dd10: 6b65 7962 6f61 7264 5f61 6363 6573 7328  keyboard_access(
-0000dd20: 7365 6c66 2c20 756e 6c6f 636b 6564 3a20  self, unlocked: 
-0000dd30: 626f 6f6c 2920 2d3e 2062 6f6f 6c3a 0a20  bool) -> bool:. 
-0000dd40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000dd50: 2020 2045 6e61 626c 6520 6f72 2064 6973     Enable or dis
-0000dd60: 6162 6c65 2074 6865 206b 6579 626f 6172  able the keyboar
-0000dd70: 6420 6f6e 2074 6865 2063 6f6e 7472 6f6c  d on the control
-0000dd80: 2e0a 2020 2020 2020 2020 5265 7175 6972  ..        Requir
-0000dd90: 6573 2061 6363 6573 7320 6c65 7665 6c20  es access level 
-0000dda0: 6060 4d4f 4e49 544f 5260 6020 746f 2077  ``MONITOR`` to w
-0000ddb0: 6f72 6b2e 0a20 2020 2020 2020 2052 6574  ork..        Ret
-0000ddc0: 7572 6e73 2060 6054 7275 6560 6020 6966  urns ``True`` if
-0000ddd0: 2063 6f6d 706c 6574 6564 2073 7563 6365   completed succe
-0000dde0: 7373 6675 6c6c 792e 0a0a 2020 2020 2020  ssfully...      
-0000ddf0: 2020 3a70 6172 616d 2075 6e6c 6f63 6b65    :param unlocke
-0000de00: 643a 2069 6620 6060 5472 7565 6060 2075  d: if ``True`` u
-0000de10: 6e6c 6f63 6b73 2074 6865 206b 6579 626f  nlocks the keybo
-0000de20: 6172 6420 736f 2069 7420 6361 6e20 6265  ard so it can be
-0000de30: 2075 7365 642e 2049 6620 6060 4661 6c73   used. If ``Fals
-0000de40: 6560 602c 2069 6e70 7574 2069 7320 7365  e``, input is se
-0000de50: 7420 746f 206c 6f63 6b65 640a 2020 2020  t to locked.    
-0000de60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000de70: 6966 2073 656c 662e 7665 7273 696f 6e73  if self.versions
-0000de80: 2e69 735f 746e 6337 2829 3a0a 2020 2020  .is_tnc7():.    
-0000de90: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0000dea0: 6767 6572 2e77 6172 6e69 6e67 2822 7468  gger.warning("th
-0000deb0: 6973 2066 756e 6374 696f 6e20 6d69 6768  is function migh
-0000dec0: 7420 6e6f 7420 6265 2073 7570 706f 7274  t not be support
-0000ded0: 6564 206f 6e20 544e 4337 2229 0a0a 2020  ed on TNC7")..  
-0000dee0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000def0: 662e 6c6f 6769 6e28 6c63 2e4c 6f67 696e  f.login(lc.Login
-0000df00: 2e4d 4f4e 4954 4f52 293a 0a20 2020 2020  .MONITOR):.     
-0000df10: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-0000df20: 6765 722e 7761 726e 696e 6728 2263 6c6f  ger.warning("clo
-0000df30: 756c 6420 6e6f 7420 6c6f 6720 696e 2061  uld not log in a
-0000df40: 7320 7573 6572 204d 4f4e 4954 4f52 2229  s user MONITOR")
-0000df50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000df60: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
-0000df70: 2020 2070 6179 6c6f 6164 203d 2062 7974     payload = byt
-0000df80: 6561 7272 6179 2829 0a20 2020 2020 2020  earray().       
-0000df90: 2069 6620 756e 6c6f 636b 6564 3a0a 2020   if unlocked:.  
-0000dfa0: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
-0000dfb0: 642e 6578 7465 6e64 2873 7472 7563 742e  d.extend(struct.
-0000dfc0: 7061 636b 2822 2142 222c 2030 7830 3029  pack("!B", 0x00)
-0000dfd0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000dfe0: 2020 2020 2020 2020 2020 2020 7061 796c              payl
-0000dff0: 6f61 642e 6578 7465 6e64 2873 7472 7563  oad.extend(struc
-0000e000: 742e 7061 636b 2822 2142 222c 2030 7830  t.pack("!B", 0x0
-0000e010: 3129 290a 0a20 2020 2020 2020 2072 6573  1))..        res
-0000e020: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
-0000e030: 5f72 6563 6976 6528 6c63 2e43 4d44 2e43  _recive(lc.CMD.C
-0000e040: 5f4c 4b2c 2070 6179 6c6f 6164 2c20 6c63  _LK, payload, lc
-0000e050: 2e52 5350 2e54 5f4f 4b29 0a20 2020 2020  .RSP.T_OK).     
-0000e060: 2020 2069 6620 7265 7375 6c74 3a0a 2020     if result:.  
-0000e070: 2020 2020 2020 2020 2020 6966 2075 6e6c            if unl
-0000e080: 6f63 6b65 643a 0a20 2020 2020 2020 2020  ocked:.         
-0000e090: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-0000e0a0: 6765 722e 6465 6275 6728 2263 6f6d 6d61  ger.debug("comma
-0000e0b0: 6e64 2074 6f20 756e 6c6f 636b 206b 6579  nd to unlock key
-0000e0c0: 626f 6172 6420 7761 7320 7375 6363 6573  board was succes
-0000e0d0: 7366 756c 2229 0a20 2020 2020 2020 2020  sful").         
-0000e0e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e0f0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0000e100: 6f67 6765 722e 6465 6275 6728 2263 6f6d  ogger.debug("com
-0000e110: 6d61 6e64 2074 6f20 6c6f 636b 206b 6579  mand to lock key
-0000e120: 626f 6172 6420 7761 7320 7375 6363 6573  board was succes
-0000e130: 7366 756c 2229 0a20 2020 2020 2020 2020  sful").         
-0000e140: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-0000e150: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-0000e160: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
-0000e170: 2020 2020 2020 2020 2022 616e 2065 7272           "an err
-0000e180: 6f72 206f 6363 7572 7265 6420 6368 616e  or occurred chan
-0000e190: 6769 6e67 2074 6865 2073 7461 7465 206f  ging the state o
-0000e1a0: 6620 7468 6520 6b65 7962 6f61 7264 206c  f the keyboard l
-0000e1b0: 6f63 6b22 0a20 2020 2020 2020 2029 0a20  ock".        ). 
-0000e1c0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0000e1d0: 6c73 650a 0a20 2020 2064 6566 2067 6574  lse..    def get
-0000e1e0: 5f6d 6163 6869 6e65 5f70 6172 616d 6574  _machine_paramet
-0000e1f0: 6572 2873 656c 662c 206e 616d 653a 2073  er(self, name: s
-0000e200: 7472 2920 2d3e 2073 7472 3a0a 2020 2020  tr) -> str:.    
-0000e210: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000e220: 5265 6164 206d 6163 6869 6e65 2070 6172  Read machine par
-0000e230: 616d 6574 6572 2066 726f 6d20 636f 6e74  ameter from cont
-0000e240: 726f 6c2e 0a20 2020 2020 2020 2052 6571  rol..        Req
-0000e250: 7569 7265 7320 6163 6365 7373 206c 6576  uires access lev
-0000e260: 656c 2060 6049 4e53 5045 4354 6060 206c  el ``INSPECT`` l
-0000e270: 6576 656c 2074 6f20 776f 726b 2e0a 0a20  evel to work... 
-0000e280: 2020 2020 2020 203a 7061 7261 6d20 6e61         :param na
-0000e290: 6d65 3a20 6e61 6d65 206f 6620 7468 6520  me: name of the 
-0000e2a0: 6d61 6368 696e 6520 7061 7261 6d65 7465  machine paramete
-0000e2b0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-0000e2c0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000e2d0: 6c66 2e6c 6f67 696e 286c 632e 4c6f 6769  lf.login(lc.Logi
-0000e2e0: 6e2e 494e 5350 4543 5429 3a0a 2020 2020  n.INSPECT):.    
-0000e2f0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0000e300: 6767 6572 2e77 6172 6e69 6e67 2822 636c  gger.warning("cl
-0000e310: 6f75 6c64 206e 6f74 206c 6f67 2069 6e20  ould not log in 
-0000e320: 6173 2075 7365 7220 494e 5350 4543 5422  as user INSPECT"
-0000e330: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000e340: 7475 726e 2022 220a 0a20 2020 2020 2020  turn ""..       
-0000e350: 2069 6620 6973 696e 7374 616e 6365 286e   if isinstance(n
-0000e360: 616d 652c 2028 696e 742c 2929 3a0a 2020  ame, (int,)):.  
-0000e370: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
-0000e380: 2073 7472 286e 616d 6529 0a0a 2020 2020   str(name)..    
-0000e390: 2020 2020 7061 796c 6f61 6420 3d20 6c6d      payload = lm
-0000e3a0: 2e75 7374 725f 746f 5f62 6128 6e61 6d65  .ustr_to_ba(name
-0000e3b0: 290a 0a20 2020 2020 2020 2072 6573 756c  )..        resul
-0000e3c0: 7420 3d20 7365 6c66 2e5f 7365 6e64 5f72  t = self._send_r
-0000e3d0: 6563 6976 6528 6c63 2e43 4d44 2e52 5f4d  ecive(lc.CMD.R_M
-0000e3e0: 432c 2070 6179 6c6f 6164 2c20 6c63 2e52  C, payload, lc.R
-0000e3f0: 5350 2e53 5f4d 4329 0a20 2020 2020 2020  SP.S_MC).       
-0000e400: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-0000e410: 6573 756c 742c 2028 6279 7465 6172 7261  esult, (bytearra
-0000e420: 792c 2929 2061 6e64 206c 656e 2872 6573  y,)) and len(res
-0000e430: 756c 7429 203e 2030 3a0a 2020 2020 2020  ult) > 0:.      
-0000e440: 2020 2020 2020 7661 6c75 6520 3d20 6c6d        value = lm
-0000e450: 2e62 615f 746f 5f75 7374 7228 7265 7375  .ba_to_ustr(resu
-0000e460: 6c74 290a 2020 2020 2020 2020 2020 2020  lt).            
-0000e470: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
-0000e480: 7567 2822 6d61 6368 696e 6520 7061 7261  ug("machine para
-0000e490: 6d65 7465 7220 2573 2068 6173 2076 616c  meter %s has val
-0000e4a0: 7565 2025 7322 2c20 6e61 6d65 2c20 7661  ue %s", name, va
-0000e4b0: 6c75 6529 0a20 2020 2020 2020 2020 2020  lue).           
-0000e4c0: 2072 6574 7572 6e20 7661 6c75 650a 0a20   return value.. 
-0000e4d0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-0000e4e0: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
-0000e4f0: 2020 2020 2020 2020 2022 616e 2065 7272           "an err
-0000e500: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
-0000e510: 6520 7265 6164 696e 6720 6d61 6368 696e  e reading machin
-0000e520: 6520 7061 7261 6d65 7465 7220 2573 222c  e parameter %s",
-0000e530: 206e 616d 650a 2020 2020 2020 2020 290a   name.        ).
-0000e540: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-0000e550: 220a 0a20 2020 2064 6566 2073 6574 5f6d  "..    def set_m
-0000e560: 6163 6869 6e65 5f70 6172 616d 6574 6572  achine_parameter
-0000e570: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0000e580: 6e61 6d65 3a20 7374 722c 2076 616c 7565  name: str, value
-0000e590: 3a20 7374 722c 2073 6166 655f 746f 5f64  : str, safe_to_d
-0000e5a0: 6973 6b3a 2062 6f6f 6c20 3d20 4661 6c73  isk: bool = Fals
-0000e5b0: 650a 2020 2020 2920 2d3e 2062 6f6f 6c3a  e.    ) -> bool:
-0000e5c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000e5d0: 2020 2020 2053 6574 206d 6163 6869 6e65       Set machine
-0000e5e0: 2070 6172 616d 6574 6572 206f 6e20 636f   parameter on co
-0000e5f0: 6e74 726f 6c2e 2057 7269 7469 6e67 2061  ntrol. Writing a
-0000e600: 2070 6172 616d 6574 6572 2074 616b 6573   parameter takes
-0000e610: 2073 6f6d 6520 7469 6d65 2c20 6d61 6b65   some time, make
-0000e620: 2073 7572 6520 746f 2073 6574 2074 696d   sure to set tim
-0000e630: 656f 7574 0a20 2020 2020 2020 2073 7566  eout.        suf
-0000e640: 6669 6369 656e 746c 7920 6869 6768 210a  ficiently high!.
-0000e650: 2020 2020 2020 2020 5265 7175 6972 6573          Requires
-0000e660: 2061 6363 6573 7320 6060 504c 4344 4542   access ``PLCDEB
-0000e670: 5547 6060 206c 6576 656c 2074 6f20 776f  UG`` level to wo
-0000e680: 726b 2e0a 2020 2020 2020 2020 5265 7475  rk..        Retu
-0000e690: 726e 7320 6060 5472 7565 6060 2069 6620  rns ``True`` if 
-0000e6a0: 636f 6d70 6c65 7465 6420 7375 6363 6573  completed succes
-0000e6b0: 7366 756c 6c79 2e0a 0a20 2020 2020 2020  sfully...       
-0000e6c0: 203a 7061 7261 6d20 6e61 6d65 3a20 6e61   :param name: na
-0000e6d0: 6d65 206f 6620 7468 6520 6d61 6368 696e  me of the machin
-0000e6e0: 6520 7061 7261 6d65 7465 722e 2046 6f72  e parameter. For
-0000e6f0: 2069 544e 4320 7468 6520 7061 7261 6d65   iTNC the parame
-0000e700: 7465 7220 6e75 6d62 6572 2068 6173 6520  ter number hase 
-0000e710: 746f 2062 6520 636f 6e76 6572 7465 6420  to be converted 
-0000e720: 746f 2073 7472 696e 670a 2020 2020 2020  to string.      
-0000e730: 2020 3a70 6172 616d 2076 616c 7565 3a20    :param value: 
-0000e740: 6e65 7720 7661 6c75 6520 6f66 2074 6865  new value of the
-0000e750: 206d 6163 6869 6e65 2070 6172 616d 6574   machine paramet
-0000e760: 6572 2e20 5468 6572 6520 6973 206e 6f20  er. There is no 
-0000e770: 7479 7065 2063 6865 636b 696e 672c 2069  type checking, i
-0000e780: 6620 7468 6520 7661 6c75 6520 6361 6e20  f the value can 
-0000e790: 6e6f 7420 6265 0a20 2020 2020 2020 2020  not be.         
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000e7b0: 6f6e 7665 7274 6564 2062 7920 7468 6520  onverted by the 
-0000e7c0: 636f 6e74 726f 6c20 616e 2065 7272 6f72  control an error
-0000e7d0: 2077 696c 6c20 6265 2073 656e 742e 0a20   will be sent.. 
-0000e7e0: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-0000e7f0: 6665 5f74 6f5f 6469 736b 3a20 4966 2054  fe_to_disk: If T
-0000e800: 7275 6520 7468 6520 6e65 7720 7661 6c75  rue the new valu
-0000e810: 6520 7769 6c6c 2062 6520 7772 6974 7465  e will be writte
-0000e820: 6e20 746f 2074 6865 2068 6172 6464 6973  n to the harddis
-0000e830: 6b20 616e 6420 7374 6179 2070 6572 6d61  k and stay perma
-0000e840: 6e65 6e74 2e0a 2020 2020 2020 2020 2020  nent..          
-0000e850: 2020 2020 2020 2020 2020 2020 2020 4966                If
-0000e860: 2046 616c 7365 2028 6465 6661 756c 7429   False (default)
-0000e870: 2074 6865 2076 616c 7565 2077 696c 6c20   the value will 
-0000e880: 6f6e 6c79 2062 6520 6176 6169 6c61 626c  only be availabl
-0000e890: 6520 756e 7469 6c20 7468 6520 6e65 7874  e until the next
-0000e8a0: 2072 6562 6f6f 742e 0a20 2020 2020 2020   reboot..       
-0000e8b0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0000e8c0: 6e6f 7420 7365 6c66 2e6c 6f67 696e 286c  not self.login(l
-0000e8d0: 632e 4c6f 6769 6e2e 504c 4344 4542 5547  c.Login.PLCDEBUG
-0000e8e0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000e8f0: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
-0000e900: 696e 6728 2263 6c6f 756c 6420 6e6f 7420  ing("clould not 
-0000e910: 6c6f 6720 696e 2061 7320 7573 6572 2050  log in as user P
-0000e920: 4c43 4445 4255 4722 290a 2020 2020 2020  LCDEBUG").      
-0000e930: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000e940: 7365 0a0a 2020 2020 2020 2020 7061 796c  se..        payl
-0000e950: 6f61 6420 3d20 6279 7465 6172 7261 7928  oad = bytearray(
-0000e960: 290a 2020 2020 2020 2020 6966 2073 6166  ).        if saf
-0000e970: 655f 746f 5f64 6973 6b3a 0a20 2020 2020  e_to_disk:.     
-0000e980: 2020 2020 2020 2070 6179 6c6f 6164 2e65         payload.e
-0000e990: 7874 656e 6428 7374 7275 6374 2e70 6163  xtend(struct.pac
-0000e9a0: 6b28 2221 4c22 2c20 3078 3030 2929 0a20  k("!L", 0x00)). 
-0000e9b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000e9c0: 2020 2020 2020 2020 2070 6179 6c6f 6164           payload
-0000e9d0: 2e65 7874 656e 6428 7374 7275 6374 2e70  .extend(struct.p
-0000e9e0: 6163 6b28 2221 4c22 2c20 3078 3031 2929  ack("!L", 0x01))
-0000e9f0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000ea00: 2e65 7874 656e 6428 6c6d 2e75 7374 725f  .extend(lm.ustr_
-0000ea10: 746f 5f62 6128 6e61 6d65 2929 0a20 2020  to_ba(name)).   
-0000ea20: 2020 2020 2070 6179 6c6f 6164 2e65 7874       payload.ext
-0000ea30: 656e 6428 6c6d 2e75 7374 725f 746f 5f62  end(lm.ustr_to_b
-0000ea40: 6128 7661 6c75 6529 290a 0a20 2020 2020  a(value))..     
-0000ea50: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0000ea60: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
-0000ea70: 2e43 4d44 2e43 5f4d 432c 2070 6179 6c6f  .CMD.C_MC, paylo
-0000ea80: 6164 2c20 6c63 2e52 5350 2e54 5f4f 4b29  ad, lc.RSP.T_OK)
-0000ea90: 0a20 2020 2020 2020 2069 6620 7265 7375  .        if resu
-0000eaa0: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
-0000eab0: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
-0000eac0: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
-0000ead0: 2020 2020 2273 6574 7469 6e67 206f 6620      "setting of 
-0000eae0: 6d61 6368 696e 6520 7061 7261 6d65 7465  machine paramete
-0000eaf0: 7220 2573 2074 6f20 7661 6c75 6520 2573  r %s to value %s
-0000eb00: 2077 6173 2073 7563 6365 7373 6675 6c22   was successful"
-0000eb10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000eb20: 2020 6e61 6d65 2c0a 2020 2020 2020 2020    name,.        
-0000eb30: 2020 2020 2020 2020 7661 6c75 652c 0a20          value,. 
-0000eb40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000eb50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000eb60: 5472 7565 0a0a 2020 2020 2020 2020 7365  True..        se
-0000eb70: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
-0000eb80: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-0000eb90: 2261 6e20 6572 726f 7220 6f63 6375 7272  "an error occurr
-0000eba0: 6564 2077 6869 6c65 2073 6574 7469 6e67  ed while setting
-0000ebb0: 206d 6163 6869 6e65 2070 6172 616d 6574   machine paramet
-0000ebc0: 6572 2025 7320 746f 2076 616c 7565 2025  er %s to value %
-0000ebd0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-0000ebe0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0000ebf0: 2020 7661 6c75 652c 0a20 2020 2020 2020    value,.       
-0000ec00: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0000ec10: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-0000ec20: 2073 656e 645f 6b65 795f 636f 6465 2873   send_key_code(s
-0000ec30: 656c 662c 206b 6579 5f63 6f64 653a 2055  elf, key_code: U
-0000ec40: 6e69 6f6e 5b6c 632e 4b65 7943 6f64 652c  nion[lc.KeyCode,
-0000ec50: 206c 632e 4f6c 644b 6579 436f 6465 5d29   lc.OldKeyCode])
-0000ec60: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000ec70: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-0000ec80: 6e64 206b 6579 2063 6f64 6520 746f 2063  nd key code to c
-0000ec90: 6f6e 7472 6f6c 2e20 4265 6861 7665 7320  ontrol. Behaves 
-0000eca0: 6173 2069 6620 7468 6520 6173 736f 6369  as if the associ
-0000ecb0: 6174 6564 206b 6579 2077 6173 2070 7265  ated key was pre
-0000ecc0: 7373 6564 206f 6e20 7468 6520 6b65 7962  ssed on the keyb
-0000ecd0: 6f61 7264 2e0a 2020 2020 2020 2020 5265  oard..        Re
-0000ece0: 7175 6972 6573 2061 6363 6573 7320 6060  quires access ``
-0000ecf0: 4d4f 4e49 544f 5260 6020 6c65 7665 6c20  MONITOR`` level 
-0000ed00: 746f 2077 6f72 6b2e 0a20 2020 2020 2020  to work..       
-0000ed10: 2054 6f20 776f 726b 2063 6f72 7265 6374   To work correct
-0000ed20: 6c79 2079 6f75 2066 6972 7374 2068 6176  ly you first hav
-0000ed30: 6520 746f 206c 6f63 6b20 7468 6520 6b65  e to lock the ke
-0000ed40: 7962 6f61 7264 2061 6e64 2075 6e6c 6f63  yboard and unloc
-0000ed50: 6b20 6974 2061 6674 6572 7761 7264 7321  k it afterwards!
-0000ed60: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
-0000ed70: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-0000ed80: 6e0a 0a20 2020 2020 2020 2020 2020 2073  n..            s
-0000ed90: 6574 5f6b 6579 626f 6172 645f 6163 6365  et_keyboard_acce
-0000eda0: 7373 2846 616c 7365 290a 2020 2020 2020  ss(False).      
-0000edb0: 2020 2020 2020 7365 6e64 5f6b 6579 5f63        send_key_c
-0000edc0: 6f64 6528 4b65 7943 6f64 652e 4345 290a  ode(KeyCode.CE).
-0000edd0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-0000ede0: 6b65 7962 6f61 7264 5f61 6363 6573 7328  keyboard_access(
-0000edf0: 5472 7565 290a 0a20 2020 2020 2020 2052  True)..        R
-0000ee00: 6574 7572 6e73 2060 6054 7275 6560 6020  eturns ``True`` 
-0000ee10: 6966 2063 6f6d 706c 6574 6564 2073 7563  if completed suc
-0000ee20: 6365 7373 6675 6c6c 792e 0a0a 2020 2020  cessfully...    
-0000ee30: 2020 2020 3a70 6172 616d 206b 6579 5f63      :param key_c
-0000ee40: 6f64 653a 2063 6f64 6520 6e75 6d62 6572  ode: code number
-0000ee50: 206f 6620 7468 6520 6b65 7962 6f61 7264   of the keyboard
-0000ee60: 206b 6579 0a20 2020 2020 2020 2022 2222   key.        """
-0000ee70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000ee80: 2e76 6572 7369 6f6e 732e 6973 5f74 6e63  .versions.is_tnc
-0000ee90: 3728 293a 0a20 2020 2020 2020 2020 2020  7():.           
-0000eea0: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
-0000eeb0: 726e 696e 6728 2274 6869 7320 6675 6e63  rning("this func
-0000eec0: 7469 6f6e 206d 6967 6874 206e 6f74 2062  tion might not b
-0000eed0: 6520 7375 7070 6f72 7465 6420 6f6e 2054  e supported on T
-0000eee0: 4e43 3722 290a 0a20 2020 2020 2020 2069  NC7")..        i
-0000eef0: 6620 6e6f 7420 7365 6c66 2e6c 6f67 696e  f not self.login
-0000ef00: 286c 632e 4c6f 6769 6e2e 4d4f 4e49 544f  (lc.Login.MONITO
-0000ef10: 5229 3a0a 2020 2020 2020 2020 2020 2020  R):.            
-0000ef20: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-0000ef30: 6e69 6e67 2822 636c 6f75 6c64 206e 6f74  ning("clould not
-0000ef40: 206c 6f67 2069 6e20 6173 2075 7365 7220   log in as user 
-0000ef50: 4d4f 4e49 544f 5222 290a 2020 2020 2020  MONITOR").      
-0000ef60: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000ef70: 7365 0a0a 2020 2020 2020 2020 7061 796c  se..        payl
-0000ef80: 6f61 6420 3d20 6279 7465 6172 7261 7928  oad = bytearray(
-0000ef90: 290a 2020 2020 2020 2020 7061 796c 6f61  ).        payloa
-0000efa0: 642e 6578 7465 6e64 2873 7472 7563 742e  d.extend(struct.
-0000efb0: 7061 636b 2822 2148 222c 206b 6579 5f63  pack("!H", key_c
-0000efc0: 6f64 6529 290a 0a20 2020 2020 2020 2072  ode))..        r
-0000efd0: 6573 756c 7420 3d20 7365 6c66 2e5f 7365  esult = self._se
-0000efe0: 6e64 5f72 6563 6976 6528 6c63 2e43 4d44  nd_recive(lc.CMD
-0000eff0: 2e43 5f45 4b2c 2070 6179 6c6f 6164 2c20  .C_EK, payload, 
-0000f000: 6c63 2e52 5350 2e54 5f4f 4b29 0a20 2020  lc.RSP.T_OK).   
-0000f010: 2020 2020 2069 6620 7265 7375 6c74 3a0a       if result:.
-0000f020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f030: 2e5f 6c6f 6767 6572 2e64 6562 7567 2822  ._logger.debug("
-0000f040: 7365 6e64 696e 6720 7468 6520 6b65 7920  sending the key 
-0000f050: 636f 6465 2025 6420 7761 7320 7375 6363  code %d was succ
-0000f060: 6573 7366 756c 222c 206b 6579 5f63 6f64  essful", key_cod
-0000f070: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
-0000f080: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-0000f090: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-0000f0a0: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
-0000f0b0: 2020 2020 2020 2261 6e20 6572 726f 7220        "an error 
-0000f0c0: 6f63 6375 7272 6564 2077 6869 6c65 2073  occurred while s
-0000f0d0: 656e 6469 6e67 2074 6865 206b 6579 2063  ending the key c
-0000f0e0: 6f64 6520 2564 222c 206b 6579 5f63 6f64  ode %d", key_cod
-0000f0f0: 650a 2020 2020 2020 2020 290a 2020 2020  e.        ).    
-0000f100: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0000f110: 0a0a 2020 2020 6465 6620 7370 696e 646c  ..    def spindl
-0000f120: 655f 746f 6f6c 5f73 7461 7475 7328 7365  e_tool_status(se
-0000f130: 6c66 2920 2d3e 2055 6e69 6f6e 5b6c 642e  lf) -> Union[ld.
-0000f140: 546f 6f6c 496e 666f 726d 6174 696f 6e2c  ToolInformation,
-0000f150: 204e 6f6e 655d 3a0a 2020 2020 2020 2020   None]:.        
-0000f160: 2222 220a 2020 2020 2020 2020 4765 7420  """.        Get 
-0000f170: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
-0000f180: 7420 7468 6520 746f 6f6c 2063 7572 7265  t the tool curre
-0000f190: 6e74 6c79 2069 6e20 7468 6520 7370 696e  ntly in the spin
-0000f1a0: 646c 650a 2020 2020 2020 2020 5265 7175  dle.        Requ
-0000f1b0: 6972 6573 2061 6363 6573 7320 6c65 7665  ires access leve
-0000f1c0: 6c20 6060 444e 4360 6020 746f 2077 6f72  l ``DNC`` to wor
-0000f1d0: 6b2e 0a20 2020 2020 2020 2022 2222 0a20  k..        """. 
-0000f1e0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000f1f0: 6c66 2e6c 6f67 696e 286c 632e 4c6f 6769  lf.login(lc.Logi
-0000f200: 6e2e 444e 4329 3a0a 2020 2020 2020 2020  n.DNC):.        
-0000f210: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-0000f220: 2e77 6172 6e69 6e67 2822 636c 6f75 6c64  .warning("clould
-0000f230: 206e 6f74 206c 6f67 2069 6e20 6173 2075   not log in as u
-0000f240: 7365 7220 444e 4322 290a 2020 2020 2020  ser DNC").      
-0000f250: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0000f260: 650a 0a20 2020 2020 2020 2070 6179 6c6f  e..        paylo
-0000f270: 6164 203d 2062 7974 6561 7272 6179 2829  ad = bytearray()
-0000f280: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000f290: 2e65 7874 656e 6428 7374 7275 6374 2e70  .extend(struct.p
-0000f2a0: 6163 6b28 2221 4822 2c20 6c63 2e50 6172  ack("!H", lc.Par
-0000f2b0: 5252 492e 4355 5252 454e 545f 544f 4f4c  RRI.CURRENT_TOOL
-0000f2c0: 2929 0a0a 2020 2020 2020 2020 7265 7375  ))..        resu
-0000f2d0: 6c74 203d 2073 656c 662e 5f73 656e 645f  lt = self._send_
-0000f2e0: 7265 6369 7665 286c 632e 434d 442e 525f  recive(lc.CMD.R_
-0000f2f0: 5249 2c20 7061 796c 6f61 642c 206c 632e  RI, payload, lc.
-0000f300: 5253 502e 535f 5249 290a 2020 2020 2020  RSP.S_RI).      
-0000f310: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000f320: 7265 7375 6c74 2c20 2862 7974 6561 7272  result, (bytearr
-0000f330: 6179 2c29 2920 616e 6420 6c65 6e28 7265  ay,)) and len(re
-0000f340: 7375 6c74 2920 3e20 303a 0a20 2020 2020  sult) > 0:.     
-0000f350: 2020 2020 2020 2074 6f6f 6c5f 696e 666f         tool_info
-0000f360: 203d 206c 6d2e 6465 636f 6465 5f74 6f6f   = lm.decode_too
-0000f370: 6c5f 696e 666f 2872 6573 756c 7429 0a20  l_info(result). 
-0000f380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f390: 5f6c 6f67 6765 722e 6465 6275 6728 2273  _logger.debug("s
-0000f3a0: 7563 6365 7373 6675 6c6c 7920 7265 6164  uccessfully read
-0000f3b0: 2069 6e66 6f20 6f6e 2063 7572 7265 6e74   info on current
-0000f3c0: 2074 6f6f 6c3a 2025 7322 2c20 746f 6f6c   tool: %s", tool
-0000f3d0: 5f69 6e66 6f29 0a20 2020 2020 2020 2020  _info).         
-0000f3e0: 2020 2072 6574 7572 6e20 746f 6f6c 5f69     return tool_i
-0000f3f0: 6e66 6f0a 2020 2020 2020 2020 7365 6c66  nfo.        self
-0000f400: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
-0000f410: 280a 2020 2020 2020 2020 2020 2020 2261  (.            "a
-0000f420: 6e20 6572 726f 7220 6f63 6375 7272 6564  n error occurred
-0000f430: 2077 6869 6c65 2071 7565 7279 696e 6720   while querying 
-0000f440: 6375 7272 656e 7420 746f 6f6c 2069 6e66  current tool inf
-0000f450: 6f72 6d61 7469 6f6e 2e20 5468 6973 2064  ormation. This d
-0000f460: 6f65 7320 6e6f 7420 776f 726b 2066 6f72  oes not work for
-0000f470: 2061 6c6c 2063 6f6e 7472 6f6c 2074 7970   all control typ
-0000f480: 6573 220a 2020 2020 2020 2020 290a 2020  es".        ).  
-0000f490: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0000f4a0: 650a 0a20 2020 2064 6566 206f 7665 7272  e..    def overr
-0000f4b0: 6964 655f 7374 6174 6528 7365 6c66 2920  ide_state(self) 
-0000f4c0: 2d3e 2055 6e69 6f6e 5b6c 642e 4f76 6572  -> Union[ld.Over
-0000f4d0: 7269 6465 5374 6174 652c 204e 6f6e 655d  rideState, None]
-0000f4e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000f4f0: 2020 2020 2020 4765 7420 696e 666f 726d        Get inform
-0000f500: 6174 696f 6e20 6162 6f75 7420 7468 6520  ation about the 
-0000f510: 6f76 6572 7269 6465 2069 6e66 6f2e 0a20  override info.. 
-0000f520: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
-0000f530: 6163 6365 7373 206c 6576 656c 2060 6044  access level ``D
-0000f540: 4e43 6060 2074 6f20 776f 726b 2e0a 2020  NC`` to work..  
-0000f550: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000f560: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
-0000f570: 6769 6e28 6c63 2e4c 6f67 696e 2e44 4e43  gin(lc.Login.DNC
-0000f580: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000f590: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
-0000f5a0: 696e 6728 2263 6c6f 756c 6420 6e6f 7420  ing("clould not 
-0000f5b0: 6c6f 6720 696e 2061 7320 7573 6572 2044  log in as user D
-0000f5c0: 4e43 2229 0a20 2020 2020 2020 2020 2020  NC").           
-0000f5d0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-0000f5e0: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-0000f5f0: 6279 7465 6172 7261 7928 290a 2020 2020  bytearray().    
-0000f600: 2020 2020 7061 796c 6f61 642e 6578 7465      payload.exte
-0000f610: 6e64 2873 7472 7563 742e 7061 636b 2822  nd(struct.pack("
-0000f620: 2148 222c 206c 632e 5061 7252 5249 2e4f  !H", lc.ParRRI.O
-0000f630: 5645 5252 4944 4529 290a 0a20 2020 2020  VERRIDE))..     
-0000f640: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0000f650: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
-0000f660: 2e43 4d44 2e52 5f52 492c 2070 6179 6c6f  .CMD.R_RI, paylo
-0000f670: 6164 2c20 6c63 2e52 5350 2e53 5f52 4929  ad, lc.RSP.S_RI)
-0000f680: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000f690: 7374 616e 6365 2872 6573 756c 742c 2028  stance(result, (
-0000f6a0: 6279 7465 6172 7261 792c 2929 2061 6e64  bytearray,)) and
-0000f6b0: 206c 656e 2872 6573 756c 7429 203e 2030   len(result) > 0
-0000f6c0: 3a0a 2020 2020 2020 2020 2020 2020 6f76  :.            ov
-0000f6d0: 6572 7269 6465 5f69 6e66 6f20 3d20 6c6d  erride_info = lm
-0000f6e0: 2e64 6563 6f64 655f 6f76 6572 7269 6465  .decode_override
-0000f6f0: 5f73 7461 7465 2872 6573 756c 7429 0a20  _state(result). 
-0000f700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f710: 5f6c 6f67 6765 722e 6465 6275 6728 2273  _logger.debug("s
-0000f720: 7563 6365 7373 6675 6c6c 7920 7265 6164  uccessfully read
-0000f730: 206f 7665 7272 6964 6520 696e 666f 3a20   override info: 
-0000f740: 2573 222c 206f 7665 7272 6964 655f 696e  %s", override_in
-0000f750: 666f 290a 2020 2020 2020 2020 2020 2020  fo).            
-0000f760: 7265 7475 726e 206f 7665 7272 6964 655f  return override_
-0000f770: 696e 666f 0a20 2020 2020 2020 2073 656c  info.        sel
-0000f780: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
-0000f790: 6728 0a20 2020 2020 2020 2020 2020 2022  g(.            "
-0000f7a0: 616e 2065 7272 6f72 206f 6363 7572 7265  an error occurre
-0000f7b0: 6420 7768 696c 6520 7175 6572 7969 6e67  d while querying
-0000f7c0: 2063 7572 7265 6e74 206f 7665 7272 6964   current overrid
-0000f7d0: 6520 696e 666f 726d 6174 696f 6e2e 2054  e information. T
-0000f7e0: 6869 7320 646f 6573 206e 6f74 2077 6f72  his does not wor
-0000f7f0: 6b20 666f 7220 616c 6c20 636f 6e74 726f  k for all contro
-0000f800: 6c20 7479 7065 7322 0a20 2020 2020 2020  l types".       
-0000f810: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0000f820: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-0000f830: 6765 745f 6572 726f 725f 6d65 7373 6167  get_error_messag
-0000f840: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
-0000f850: 5b6c 642e 4e43 4572 726f 724d 6573 7361  [ld.NCErrorMessa
-0000f860: 6765 5d3a 0a20 2020 2020 2020 2022 2222  ge]:.        """
-0000f870: 0a20 2020 2020 2020 2047 6574 2069 6e66  .        Get inf
-0000f880: 6f72 6d61 7469 6f6e 2061 626f 7574 2074  ormation about t
-0000f890: 6865 2066 6972 7374 206f 7220 6e65 7874  he first or next
-0000f8a0: 2065 7272 6f72 2064 6973 706c 6179 6564   error displayed
-0000f8b0: 206f 6e20 7468 6520 636f 6e74 726f 6c0a   on the control.
-0000f8c0: 2020 2020 2020 2020 5265 7175 6972 6573          Requires
-0000f8d0: 2061 6363 6573 7320 6c65 7665 6c20 6060   access level ``
-0000f8e0: 444e 4360 6020 746f 2077 6f72 6b2e 0a20  DNC`` to work.. 
-0000f8f0: 2020 2020 2020 2052 6574 7572 6e73 2065         Returns e
-0000f900: 7272 6f72 206c 6973 7420 6f66 2065 7272  rror list of err
-0000f910: 6f72 206d 6573 7361 6765 730a 2020 2020  or messages.    
-0000f920: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f930: 6d65 7373 6167 6573 203d 205b 5d0a 2020  messages = [].  
-0000f940: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000f950: 662e 6c6f 6769 6e28 6c63 2e4c 6f67 696e  f.login(lc.Login
-0000f960: 2e44 4e43 293a 0a20 2020 2020 2020 2020  .DNC):.         
-0000f970: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
-0000f980: 7761 726e 696e 6728 2263 6c6f 756c 6420  warning("clould 
-0000f990: 6e6f 7420 6c6f 6720 696e 2061 7320 7573  not log in as us
-0000f9a0: 6572 2044 4e43 2229 0a20 2020 2020 2020  er DNC").       
-0000f9b0: 2020 2020 2072 6574 7572 6e20 5b5d 0a0a       return []..
-0000f9c0: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
-0000f9d0: 3d20 6279 7465 6172 7261 7928 290a 2020  = bytearray().  
-0000f9e0: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
-0000f9f0: 7465 6e64 2873 7472 7563 742e 7061 636b  tend(struct.pack
-0000fa00: 2822 2148 222c 206c 632e 5061 7252 5249  ("!H", lc.ParRRI
-0000fa10: 2e46 4952 5354 5f45 5252 4f52 2929 0a0a  .FIRST_ERROR))..
-0000fa20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000fa30: 2073 656c 662e 5f73 656e 645f 7265 6369   self._send_reci
-0000fa40: 7665 286c 632e 434d 442e 525f 5249 2c20  ve(lc.CMD.R_RI, 
-0000fa50: 7061 796c 6f61 642c 206c 632e 5253 502e  payload, lc.RSP.
-0000fa60: 535f 5249 290a 2020 2020 2020 2020 6966  S_RI).        if
-0000fa70: 2069 7369 6e73 7461 6e63 6528 7265 7375   isinstance(resu
-0000fa80: 6c74 2c20 2862 7974 6561 7272 6179 2c29  lt, (bytearray,)
-0000fa90: 2920 616e 6420 6c65 6e28 7265 7375 6c74  ) and len(result
-0000faa0: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
-0000fab0: 2020 206d 6573 7361 6765 732e 6170 7065     messages.appe
-0000fac0: 6e64 286c 6d2e 6465 636f 6465 5f65 7272  nd(lm.decode_err
-0000fad0: 6f72 5f6d 6573 7361 6765 2872 6573 756c  or_message(resul
-0000fae0: 7429 290a 2020 2020 2020 2020 2020 2020  t)).            
-0000faf0: 7061 796c 6f61 6420 3d20 6279 7465 6172  payload = bytear
-0000fb00: 7261 7928 290a 2020 2020 2020 2020 2020  ray().          
-0000fb10: 2020 7061 796c 6f61 642e 6578 7465 6e64    payload.extend
-0000fb20: 2873 7472 7563 742e 7061 636b 2822 2148  (struct.pack("!H
-0000fb30: 222c 206c 632e 5061 7252 5249 2e4e 4558  ", lc.ParRRI.NEX
-0000fb40: 545f 4552 524f 5229 290a 2020 2020 2020  T_ERROR)).      
-0000fb50: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-0000fb60: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
-0000fb70: 286c 632e 434d 442e 525f 5249 2c20 7061  (lc.CMD.R_RI, pa
-0000fb80: 796c 6f61 642c 206c 632e 5253 502e 535f  yload, lc.RSP.S_
-0000fb90: 5249 290a 2020 2020 2020 2020 2020 2020  RI).            
-0000fba0: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
-0000fbb0: 7567 2822 7375 6363 6573 7366 756c 6c79  ug("successfully
-0000fbc0: 2072 6561 6420 6669 7273 7420 6572 726f   read first erro
-0000fbd0: 7220 6275 7420 6675 7274 6865 7220 6572  r but further er
-0000fbe0: 726f 7273 2229 0a0a 2020 2020 2020 2020  rors")..        
-0000fbf0: 2020 2020 7768 696c 6520 6973 696e 7374      while isinst
-0000fc00: 616e 6365 2872 6573 756c 742c 2028 6279  ance(result, (by
-0000fc10: 7465 6172 7261 792c 2929 3a0a 2020 2020  tearray,)):.    
-0000fc20: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-0000fc30: 6167 6573 2e61 7070 656e 6428 6c6d 2e64  ages.append(lm.d
-0000fc40: 6563 6f64 655f 6572 726f 725f 6d65 7373  ecode_error_mess
-0000fc50: 6167 6528 7265 7375 6c74 2929 0a20 2020  age(result)).   
-0000fc60: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000fc70: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
-0000fc80: 5f72 6563 6976 6528 6c63 2e43 4d44 2e52  _recive(lc.CMD.R
-0000fc90: 5f52 492c 2070 6179 6c6f 6164 2c20 6c63  _RI, payload, lc
-0000fca0: 2e52 5350 2e53 5f52 4929 0a0a 2020 2020  .RSP.S_RI)..    
-0000fcb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000fcc0: 6c61 7374 5f65 7272 6f72 2069 7320 6c63  last_error is lc
-0000fcd0: 2e4c 5356 3253 7461 7475 7343 6f64 652e  .LSV2StatusCode.
-0000fce0: 545f 4552 5f4e 4f5f 4e45 5854 5f45 5252  T_ER_NO_NEXT_ERR
-0000fcf0: 4f52 3a0a 2020 2020 2020 2020 2020 2020  OR:.            
-0000fd00: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-0000fd10: 2e64 6562 7567 2822 7375 6363 6573 7366  .debug("successf
-0000fd20: 756c 6c79 2072 6561 6420 616c 6c20 6572  ully read all er
-0000fd30: 726f 7273 2229 0a20 2020 2020 2020 2020  rors").         
-0000fd40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000fd50: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0000fd60: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
-0000fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd80: 2020 2022 616e 2065 7272 6f72 206f 6363     "an error occ
-0000fd90: 7572 7265 6420 7768 696c 6520 7175 6572  urred while quer
-0000fda0: 7969 6e67 2065 7272 6f72 2069 6e66 6f72  ying error infor
-0000fdb0: 6d61 7469 6f6e 2e22 0a20 2020 2020 2020  mation.".       
-0000fdc0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000fdd0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-0000fde0: 6573 7361 6765 730a 0a20 2020 2020 2020  essages..       
-0000fdf0: 2069 6620 7365 6c66 2e6c 6173 745f 6572   if self.last_er
-0000fe00: 726f 7220 6973 206c 632e 4c53 5632 5374  ror is lc.LSV2St
-0000fe10: 6174 7573 436f 6465 2e54 5f45 525f 4e4f  atusCode.T_ER_NO
-0000fe20: 5f4e 4558 545f 4552 524f 523a 0a20 2020  _NEXT_ERROR:.   
-0000fe30: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0000fe40: 6f67 6765 722e 6465 6275 6728 2273 7563  ogger.debug("suc
-0000fe50: 6365 7373 6675 6c6c 7920 7265 6164 2066  cessfully read f
-0000fe60: 6972 7374 2065 7272 6f72 2062 7574 206e  irst error but n
-0000fe70: 6f20 6572 726f 7220 6163 7469 7665 2229  o error active")
-0000fe80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000fe90: 7572 6e20 6d65 7373 6167 6573 0a0a 2020  urn messages..  
-0000fea0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-0000feb0: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
-0000fec0: 2020 2020 2020 2020 2261 6e20 6572 726f          "an erro
-0000fed0: 7220 6f63 6375 7272 6564 2077 6869 6c65  r occurred while
-0000fee0: 2071 7565 7279 696e 6720 6572 726f 7220   querying error 
-0000fef0: 696e 666f 726d 6174 696f 6e2e 2054 6869  information. Thi
-0000ff00: 7320 646f 6573 206e 6f74 2077 6f72 6b20  s does not work 
-0000ff10: 666f 7220 616c 6c20 636f 6e74 726f 6c20  for all control 
-0000ff20: 7479 7065 7322 0a20 2020 2020 2020 2029  types".        )
-0000ff30: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000ff40: 205b 5d0a 0a20 2020 2064 6566 205f 7761   []..    def _wa
-0000ff50: 6c6b 5f64 6972 2873 656c 662c 2064 6573  lk_dir(self, des
-0000ff60: 6365 6e64 3a20 626f 6f6c 203d 2054 7275  cend: bool = Tru
-0000ff70: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-0000ff80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ff90: 2020 2020 2068 656c 7065 7220 6675 6e63       helper func
-0000ffa0: 7469 6f6e 2074 6f20 7265 6375 7273 6976  tion to recursiv
-0000ffb0: 656c 7920 7365 6172 6368 2069 6e20 6469  ely search in di
-0000ffc0: 7265 6374 6f72 6965 7320 666f 7220 6669  rectories for fi
-0000ffd0: 6c65 732e 0a20 2020 2020 2020 2052 6571  les..        Req
-0000ffe0: 7569 7265 7320 6163 6365 7373 206c 6576  uires access lev
-0000fff0: 656c 2060 6046 494c 4554 5241 4e53 4645  el ``FILETRANSFE
-00010000: 5260 6020 746f 2077 6f72 6b2e 0a0a 2020  R`` to work...  
-00010010: 2020 2020 2020 3a70 6172 616d 2064 6573        :param des
-00010020: 6365 6e64 3a20 636f 6e74 726f 6c20 6966  cend: control if
-00010030: 2073 6561 7263 6820 7368 6f75 6c64 2072   search should r
-00010040: 756e 2072 6563 7572 7369 7665 6c79 0a20  un recursively. 
-00010050: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010060: 2020 2069 6620 6e6f 7420 7365 6c66 2e6c     if not self.l
-00010070: 6f67 696e 286c 632e 4c6f 6769 6e2e 4649  ogin(lc.Login.FI
-00010080: 4c45 5452 414e 5346 4552 293a 0a20 2020  LETRANSFER):.   
-00010090: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-000100a0: 6f67 6765 722e 7761 726e 696e 6728 2263  ogger.warning("c
-000100b0: 6c6f 756c 6420 6e6f 7420 6c6f 6720 696e  lould not log in
-000100c0: 2061 7320 7573 6572 2046 494c 4522 290a   as user FILE").
-000100d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000100e0: 726e 205b 5d0a 0a20 2020 2020 2020 2063  rn []..        c
-000100f0: 7572 7265 6e74 5f70 6174 6820 3d20 7365  urrent_path = se
-00010100: 6c66 2e64 6972 6563 746f 7279 5f69 6e66  lf.directory_inf
-00010110: 6f28 292e 7061 7468 0a20 2020 2020 2020  o().path.       
-00010120: 2063 6f6e 7465 6e74 203d 205b 5d0a 2020   content = [].  
-00010130: 2020 2020 2020 666f 7220 656e 7472 7920        for entry 
-00010140: 696e 2073 656c 662e 6469 7265 6374 6f72  in self.director
-00010150: 795f 636f 6e74 656e 7428 293a 0a20 2020  y_content():.   
-00010160: 2020 2020 2020 2020 2069 6620 656e 7472           if entr
-00010170: 792e 6e61 6d65 203d 3d20 222e 2220 6f72  y.name == "." or
-00010180: 2065 6e74 7279 2e6e 616d 6520 3d3d 2022   entry.name == "
-00010190: 2e2e 2220 6f72 2065 6e74 7279 2e6e 616d  .." or entry.nam
-000101a0: 652e 656e 6473 7769 7468 2822 3a22 293a  e.endswith(":"):
-000101b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101c0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-000101d0: 2020 2020 2020 6375 7272 656e 745f 6673        current_fs
-000101e0: 5f65 6c65 6d65 6e74 203d 2073 7472 2863  _element = str(c
-000101f0: 7572 7265 6e74 5f70 6174 6820 2b20 656e  urrent_path + en
-00010200: 7472 792e 6e61 6d65 292e 7265 706c 6163  try.name).replac
-00010210: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00010220: 2020 2022 2f22 2c20 6c63 2e50 4154 485f     "/", lc.PATH_
-00010230: 5345 500a 2020 2020 2020 2020 2020 2020  SEP.            
-00010240: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00010250: 2065 6e74 7279 2e69 735f 6469 7265 6374   entry.is_direct
-00010260: 6f72 7920 6973 2054 7275 6520 616e 6420  ory is True and 
-00010270: 6465 7363 656e 6420 6973 2054 7275 653a  descend is True:
-00010280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010290: 2069 6620 7365 6c66 2e63 6861 6e67 655f   if self.change_
-000102a0: 6469 7265 6374 6f72 7928 6375 7272 656e  directory(curren
-000102b0: 745f 6673 5f65 6c65 6d65 6e74 293a 0a20  t_fs_element):. 
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102d0: 2020 2063 6f6e 7465 6e74 2e65 7874 656e     content.exten
-000102e0: 6428 7365 6c66 2e5f 7761 6c6b 5f64 6972  d(self._walk_dir
-000102f0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-00010300: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00010310: 2020 2020 2020 636f 6e74 656e 742e 6170        content.ap
-00010320: 7065 6e64 2863 7572 7265 6e74 5f66 735f  pend(current_fs_
-00010330: 656c 656d 656e 7429 0a20 2020 2020 2020  element).       
-00010340: 2073 656c 662e 6368 616e 6765 5f64 6972   self.change_dir
-00010350: 6563 746f 7279 2863 7572 7265 6e74 5f70  ectory(current_p
-00010360: 6174 6829 0a20 2020 2020 2020 2072 6574  ath).        ret
-00010370: 7572 6e20 636f 6e74 656e 740a 0a20 2020  urn content..   
-00010380: 2064 6566 2067 6574 5f66 696c 655f 6c69   def get_file_li
-00010390: 7374 280a 2020 2020 2020 2020 7365 6c66  st(.        self
-000103a0: 2c20 7061 7468 3a20 7374 7220 3d20 2222  , path: str = ""
-000103b0: 2c20 6465 7363 656e 643a 2062 6f6f 6c20  , descend: bool 
-000103c0: 3d20 5472 7565 2c20 7061 7474 6572 6e3a  = True, pattern:
-000103d0: 2073 7472 203d 2022 220a 2020 2020 2920   str = "".    ) 
-000103e0: 2d3e 204c 6973 745b 7374 725d 3a0a 2020  -> List[str]:.  
-000103f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010400: 2020 4765 7420 6c69 7374 206f 6620 6669    Get list of fi
-00010410: 6c65 7320 696e 2064 6972 6563 746f 7279  les in directory
-00010420: 2073 7472 7563 7475 7265 2e0a 2020 2020   structure..    
-00010430: 2020 2020 5265 7175 6972 6573 2061 6363      Requires acc
-00010440: 6573 7320 6c65 7665 6c20 6060 4649 4c45  ess level ``FILE
-00010450: 5452 414e 5346 4552 6060 2074 6f20 776f  TRANSFER`` to wo
-00010460: 726b 2e0a 0a20 2020 2020 2020 203a 7061  rk...        :pa
-00010470: 7261 6d20 7061 7468 3a20 7061 7468 206f  ram path: path o
-00010480: 6620 7468 6520 6469 7265 6374 6f72 7920  f the directory 
-00010490: 7768 6572 6520 6669 6c65 7320 7368 6f75  where files shou
-000104a0: 6c64 2062 6520 7365 6172 6368 6564 2e20  ld be searched. 
-000104b0: 6966 204e 6f6e 6520 7468 616e 2074 6865  if None than the
-000104c0: 2063 7572 7265 6e74 2064 6972 6563 746f   current directo
-000104d0: 7279 2069 7320 7573 6564 0a20 2020 2020  ry is used.     
-000104e0: 2020 203a 7061 7261 6d20 6465 7363 656e     :param descen
-000104f0: 643a 2063 6f6e 7472 6f6c 2069 6620 7365  d: control if se
-00010500: 6172 6368 2073 686f 756c 6420 7275 6e20  arch should run 
-00010510: 7265 6375 7273 6976 656c 790a 2020 2020  recursively.    
-00010520: 2020 2020 3a70 6172 616d 2070 6174 7465      :param patte
-00010530: 726e 3a20 7265 6765 7820 7374 7269 6e67  rn: regex string
-00010540: 2074 6f20 6669 6c74 6572 2074 6865 2066   to filter the f
-00010550: 696c 6520 6e61 6d65 730a 2020 2020 2020  ile names.      
-00010560: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00010570: 206e 6f74 2073 656c 662e 6c6f 6769 6e28   not self.login(
-00010580: 6c63 2e4c 6f67 696e 2e46 494c 4554 5241  lc.Login.FILETRA
-00010590: 4e53 4645 5229 3a0a 2020 2020 2020 2020  NSFER):.        
-000105a0: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-000105b0: 2e77 6172 6e69 6e67 2822 636c 6f75 6c64  .warning("clould
-000105c0: 206e 6f74 206c 6f67 2069 6e20 6173 2075   not log in as u
-000105d0: 7365 7220 4649 4c45 2229 0a20 2020 2020  ser FILE").     
-000105e0: 2020 2020 2020 2072 6574 7572 6e20 5b5d         return []
-000105f0: 0a0a 2020 2020 2020 2020 6966 2070 6174  ..        if pat
-00010600: 6820 6973 206e 6f74 204e 6f6e 653a 0a20  h is not None:. 
-00010610: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00010620: 6c66 2e63 6861 6e67 655f 6469 7265 6374  lf.change_direct
-00010630: 6f72 7928 7061 7468 2920 6973 2046 616c  ory(path) is Fal
-00010640: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00010650: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
-00010660: 2e77 6172 6e69 6e67 2822 636f 756c 6420  .warning("could 
-00010670: 6e6f 7420 6368 616e 6765 2074 6f20 6469  not change to di
-00010680: 7265 6374 6f72 7922 290a 2020 2020 2020  rectory").      
-00010690: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000106a0: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
-000106b0: 6c65 6e28 7061 7474 6572 6e29 203d 3d20  len(pattern) == 
-000106c0: 303a 0a20 2020 2020 2020 2020 2020 2066  0:.            f
-000106d0: 696c 655f 6c69 7374 203d 2073 656c 662e  ile_list = self.
-000106e0: 5f77 616c 6b5f 6469 7228 6465 7363 656e  _walk_dir(descen
-000106f0: 6429 0a20 2020 2020 2020 2065 6c73 653a  d).        else:
-00010700: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00010710: 655f 6c69 7374 203d 205b 5d0a 2020 2020  e_list = [].    
-00010720: 2020 2020 2020 2020 666f 7220 656e 7472          for entr
-00010730: 7920 696e 2073 656c 662e 5f77 616c 6b5f  y in self._walk_
-00010740: 6469 7228 6465 7363 656e 6429 3a0a 2020  dir(descend):.  
-00010750: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00010760: 6c65 5f6e 616d 6520 3d20 656e 7472 792e  le_name = entry.
-00010770: 7370 6c69 7428 6c63 2e50 4154 485f 5345  split(lc.PATH_SE
-00010780: 5029 5b2d 315d 0a20 2020 2020 2020 2020  P)[-1].         
-00010790: 2020 2020 2020 2069 6620 7265 2e6d 6174         if re.mat
-000107a0: 6368 2870 6174 7465 726e 2c20 6669 6c65  ch(pattern, file
-000107b0: 5f6e 616d 6529 3a0a 2020 2020 2020 2020  _name):.        
-000107c0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-000107d0: 5f6c 6973 742e 6170 7065 6e64 2865 6e74  _list.append(ent
-000107e0: 7279 290a 2020 2020 2020 2020 7265 7475  ry).        retu
-000107f0: 726e 2066 696c 655f 6c69 7374 0a0a 2020  rn file_list..  
-00010800: 2020 6465 6620 7265 6164 5f64 6174 615f    def read_data_
-00010810: 7061 7468 2873 656c 662c 2070 6174 683a  path(self, path:
-00010820: 2073 7472 2920 2d3e 2055 6e69 6f6e 5b62   str) -> Union[b
-00010830: 6f6f 6c2c 2069 6e74 2c20 666c 6f61 742c  ool, int, float,
-00010840: 2073 7472 2c20 4e6f 6e65 5d3a 0a20 2020   str, None]:.   
-00010850: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010860: 2052 6561 6420 7661 6c75 6573 2066 726f   Read values fro
-00010870: 6d20 636f 6e74 726f 6c20 7669 6120 6461  m control via da
-00010880: 7461 2070 6174 682e 204f 6e6c 7920 776f  ta path. Only wo
-00010890: 726b 7320 6f6e 2069 544e 4320 636f 6e74  rks on iTNC cont
-000108a0: 726f 6c73 2e0a 2020 2020 2020 2020 466f  rols..        Fo
-000108b0: 7220 6561 7365 206f 6620 7573 652c 2074  r ease of use, t
-000108c0: 6865 2070 6174 6820 6973 2066 6f72 6d61  he path is forma
-000108d0: 7474 6564 2062 7920 7265 706c 6163 696e  tted by replacin
-000108e0: 6720 2f20 6279 205c 5c20 616e 6420 2220  g / by \\ and " 
-000108f0: 6279 2027 2e0a 2020 2020 2020 2020 5265  by '..        Re
-00010900: 7475 726e 7320 6461 7461 2076 616c 7565  turns data value
-00010910: 2072 6561 6420 6672 6f6d 2063 6f6e 7472   read from contr
-00010920: 6f6c 2066 6f72 6d61 7474 6564 2069 6e20  ol formatted in 
-00010930: 6e61 7469 7620 6461 7461 2074 7970 6520  nativ data type 
-00010940: 6f72 204e 6f6e 6520 6966 2072 6561 6469  or None if readi
-00010950: 6e67 0a20 2020 2020 2020 2077 6173 206e  ng.        was n
-00010960: 6f74 2073 7563 6365 7373 6675 6c2e 0a20  ot successful.. 
-00010970: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
-00010980: 6163 6365 7373 206c 6576 656c 2060 6044  access level ``D
-00010990: 4154 4160 6020 746f 2077 6f72 6b2e 0a0a  ATA`` to work...
-000109a0: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-000109b0: 6174 683a 2064 6174 6120 7061 7468 2066  ath: data path f
-000109c0: 726f 6d20 7768 6963 6820 746f 2072 6561  rom which to rea
-000109d0: 6420 7468 6520 7661 6c75 652e 0a0a 2020  d the value...  
-000109e0: 2020 2020 2020 3a72 6169 7365 7320 4c53        :raises LS
-000109f0: 5632 5072 6f74 6f63 6f6c 4578 6365 7074  V2ProtocolExcept
-00010a00: 696f 6e3a 2069 6620 6461 7461 2074 7970  ion: if data typ
-00010a10: 6520 636f 756c 6420 6e6f 7420 6265 2064  e could not be d
-00010a20: 6574 6572 6d69 656e 640a 2020 2020 2020  etermiend.      
-00010a30: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00010a40: 206e 6f74 2073 656c 662e 7665 7273 696f   not self.versio
-00010a50: 6e73 2e69 735f 6974 6e63 2829 3a0a 2020  ns.is_itnc():.  
-00010a60: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00010a70: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a90: 2252 6561 6469 6e67 2076 616c 7565 7320  "Reading values 
-00010aa0: 6672 6f6d 2064 6174 6120 7061 7468 2064  from data path d
-00010ab0: 6f65 7320 6e6f 7420 776f 726b 206f 6e20  oes not work on 
-00010ac0: 6e6f 6e20 6954 4e43 2063 6f6e 7472 6f6c  non iTNC control
-00010ad0: 7321 220a 2020 2020 2020 2020 2020 2020  s!".            
-00010ae0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00010af0: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
-00010b00: 2020 2070 6174 6820 3d20 7061 7468 2e72     path = path.r
-00010b10: 6570 6c61 6365 2822 2f22 2c20 6c63 2e50  eplace("/", lc.P
-00010b20: 4154 485f 5345 5029 2e72 6570 6c61 6365  ATH_SEP).replace
-00010b30: 2827 2227 2c20 2227 2229 0a0a 2020 2020  ('"', "'")..    
-00010b40: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00010b50: 6c6f 6769 6e28 6c63 2e4c 6f67 696e 2e44  login(lc.Login.D
-00010b60: 4154 4129 3a0a 2020 2020 2020 2020 2020  ATA):.          
-00010b70: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e77    self._logger.w
-00010b80: 6172 6e69 6e67 2822 636c 6f75 6c64 206e  arning("clould n
-00010b90: 6f74 206c 6f67 2069 6e20 6173 2075 7365  ot log in as use
-00010ba0: 7220 4441 5441 2229 0a20 2020 2020 2020  r DATA").       
-00010bb0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00010bc0: 0a0a 2020 2020 2020 2020 7061 796c 6f61  ..        payloa
-00010bd0: 6420 3d20 6279 7465 6172 7261 7928 290a  d = bytearray().
-00010be0: 2020 2020 2020 2020 7061 796c 6f61 642e          payload.
-00010bf0: 6578 7465 6e64 2862 225c 7830 3022 2920  extend(b"\x00") 
-00010c00: 2023 203c 2d20 3f3f 3f0a 2020 2020 2020   # <- ???.      
-00010c10: 2020 7061 796c 6f61 642e 6578 7465 6e64    payload.extend
-00010c20: 2862 225c 7830 3022 2920 2023 203c 2d20  (b"\x00")  # <- 
-00010c30: 3f3f 3f0a 2020 2020 2020 2020 7061 796c  ???.        payl
-00010c40: 6f61 642e 6578 7465 6e64 2862 225c 7830  oad.extend(b"\x0
-00010c50: 3022 2920 2023 203c 2d20 3f3f 3f0a 2020  0")  # <- ???.  
-00010c60: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
-00010c70: 7465 6e64 2862 225c 7830 3022 2920 2023  tend(b"\x00")  #
-00010c80: 203c 2d20 3f3f 3f0a 2020 2020 2020 2020   <- ???.        
-00010c90: 7061 796c 6f61 642e 6578 7465 6e64 286c  payload.extend(l
-00010ca0: 6d2e 7573 7472 5f74 6f5f 6261 2870 6174  m.ustr_to_ba(pat
-00010cb0: 6829 290a 0a20 2020 2020 2020 2072 6573  h))..        res
-00010cc0: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
-00010cd0: 5f72 6563 6976 6528 6c63 2e43 4d44 2e52  _recive(lc.CMD.R
-00010ce0: 5f44 502c 2070 6179 6c6f 6164 2c20 6c63  _DP, payload, lc
-00010cf0: 2e52 5350 2e53 5f44 5029 0a0a 2020 2020  .RSP.S_DP)..    
-00010d00: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00010d10: 6528 7265 7375 6c74 2c20 2862 7974 6561  e(result, (bytea
-00010d20: 7272 6179 2c29 2920 616e 6420 6c65 6e28  rray,)) and len(
-00010d30: 7265 7375 6c74 2920 3e20 303a 0a20 2020  result) > 0:.   
-00010d40: 2020 2020 2020 2020 2076 616c 7565 5f74           value_t
-00010d50: 7970 6520 3d20 7374 7275 6374 2e75 6e70  ype = struct.unp
-00010d60: 6163 6b28 2221 4c22 2c20 7265 7375 6c74  ack("!L", result
-00010d70: 5b30 3a34 5d29 5b30 5d0a 2020 2020 2020  [0:4])[0].      
-00010d80: 2020 2020 2020 6966 2076 616c 7565 5f74        if value_t
-00010d90: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
-00010da0: 2020 2020 2020 2020 2020 6461 7461 5f76            data_v
-00010db0: 616c 7565 203d 2073 7472 7563 742e 756e  alue = struct.un
-00010dc0: 7061 636b 2822 2168 222c 2072 6573 756c  pack("!h", resul
-00010dd0: 745b 343a 365d 295b 305d 0a20 2020 2020  t[4:6])[0].     
-00010de0: 2020 2020 2020 2065 6c69 6620 7661 6c75         elif valu
-00010df0: 655f 7479 7065 203d 3d20 333a 0a20 2020  e_type == 3:.   
-00010e00: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00010e10: 615f 7661 6c75 6520 3d20 7374 7275 6374  a_value = struct
-00010e20: 2e75 6e70 6163 6b28 2221 6c22 2c20 7265  .unpack("!l", re
-00010e30: 7375 6c74 5b34 3a38 5d29 5b30 5d0a 2020  sult[4:8])[0].  
-00010e40: 2020 2020 2020 2020 2020 656c 6966 2076            elif v
-00010e50: 616c 7565 5f74 7970 6520 3d3d 2035 3a0a  alue_type == 5:.
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e70: 6461 7461 5f76 616c 7565 203d 2073 7472  data_value = str
-00010e80: 7563 742e 756e 7061 636b 2822 3c64 222c  uct.unpack("<d",
-00010e90: 2072 6573 756c 745b 343a 3132 5d29 5b30   result[4:12])[0
-00010ea0: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-00010eb0: 6966 2076 616c 7565 5f74 7970 6520 3d3d  if value_type ==
-00010ec0: 2038 3a0a 2020 2020 2020 2020 2020 2020   8:.            
-00010ed0: 2020 2020 6461 7461 5f76 616c 7565 203d      data_value =
-00010ee0: 206c 6d2e 6261 5f74 6f5f 7573 7472 2872   lm.ba_to_ustr(r
-00010ef0: 6573 756c 745b 343a 5d29 0a20 2020 2020  esult[4:]).     
-00010f00: 2020 2020 2020 2065 6c69 6620 7661 6c75         elif valu
-00010f10: 655f 7479 7065 203d 3d20 3131 3a0a 2020  e_type == 11:.  
-00010f20: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00010f30: 7461 5f76 616c 7565 203d 2073 7472 7563  ta_value = struc
-00010f40: 742e 756e 7061 636b 2822 213f 222c 2072  t.unpack("!?", r
-00010f50: 6573 756c 745b 343a 355d 295b 305d 0a20  esult[4:5])[0]. 
-00010f60: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00010f70: 7661 6c75 655f 7479 7065 203d 3d20 3136  value_type == 16
-00010f80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010f90: 2020 6461 7461 5f76 616c 7565 203d 2073    data_value = s
-00010fa0: 7472 7563 742e 756e 7061 636b 2822 2162  truct.unpack("!b
-00010fb0: 222c 2072 6573 756c 745b 343a 355d 295b  ", result[4:5])[
-00010fc0: 305d 0a20 2020 2020 2020 2020 2020 2065  0].            e
-00010fd0: 6c69 6620 7661 6c75 655f 7479 7065 203d  lif value_type =
-00010fe0: 3d20 3137 3a0a 2020 2020 2020 2020 2020  = 17:.          
-00010ff0: 2020 2020 2020 6461 7461 5f76 616c 7565        data_value
-00011000: 203d 2073 7472 7563 742e 756e 7061 636b   = struct.unpack
-00011010: 2822 2142 222c 2072 6573 756c 745b 343a  ("!B", result[4:
-00011020: 355d 295b 305d 0a20 2020 2020 2020 2020  5])[0].         
-00011030: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00011040: 2020 2020 2020 2020 2072 6169 7365 204c           raise L
-00011050: 5356 3250 726f 746f 636f 6c45 7863 6570  SV2ProtocolExcep
-00011060: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00011070: 2020 2020 2020 2020 2020 2275 6e6b 6e6f            "unkno
-00011080: 776e 2072 6574 7572 6e20 7479 7065 3a20  wn return type: 
-00011090: 2564 2066 6f72 2025 7322 2025 2028 7661  %d for %s" % (va
-000110a0: 6c75 655f 7479 7065 2c20 7265 7375 6c74  lue_type, result
-000110b0: 5b34 3a5d 290a 2020 2020 2020 2020 2020  [4:]).          
-000110c0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000110d0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-000110e0: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-000110f0: 2020 2020 2020 2020 2273 7563 6365 7373          "success
-00011100: 6675 6c6c 7920 7265 6164 2064 6174 6120  fully read data 
-00011110: 7061 7468 3a20 2573 2061 6e64 2067 6f74  path: %s and got
-00011120: 2076 616c 7565 2027 2573 2722 2c20 7061   value '%s'", pa
-00011130: 7468 2c20 6461 7461 5f76 616c 7565 0a20  th, data_value. 
-00011140: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00011150: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011160: 6461 7461 5f76 616c 7565 0a20 2020 2020  data_value.     
-00011170: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
-00011180: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
-00011190: 2020 2020 2022 616e 2065 7272 6f72 206f       "an error o
-000111a0: 6363 7572 7265 6420 7768 696c 6520 7175  ccurred while qu
-000111b0: 6572 7969 6e67 2064 6174 6120 7061 7468  erying data path
-000111c0: 2027 2573 272e 2054 6869 7320 646f 6573   '%s'. This does
-000111d0: 206e 6f74 2077 6f72 6b20 666f 7220 616c   not work for al
-000111e0: 6c20 636f 6e74 726f 6c20 7479 7065 7322  l control types"
-000111f0: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-00011200: 7468 2c0a 2020 2020 2020 2020 290a 2020  th,.        ).  
-00011210: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00011220: 650a 0a20 2020 2064 6566 2061 7865 735f  e..    def axes_
-00011230: 6c6f 6361 7469 6f6e 2873 656c 6629 202d  location(self) -
-00011240: 3e20 556e 696f 6e5b 4469 6374 5b73 7472  > Union[Dict[str
-00011250: 2c20 666c 6f61 745d 2c20 4e6f 6e65 5d3a  , float], None]:
-00011260: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011270: 2020 2020 2052 6561 6420 6178 6573 206c       Read axes l
-00011280: 6f63 6174 696f 6e20 6672 6f6d 2063 6f6e  ocation from con
-00011290: 7472 6f6c 2e20 4e6f 7420 6675 6c6c 7920  trol. Not fully 
-000112a0: 646f 6375 6d65 6e74 6564 2c20 7661 6c75  documented, valu
-000112b0: 6520 6f66 2066 6972 7374 2062 7974 6520  e of first byte 
-000112c0: 756e 6b6e 6f77 6e2e 0a20 2020 2020 2020  unknown..       
-000112d0: 2052 6571 7569 7265 7320 6163 6365 7373   Requires access
-000112e0: 206c 6576 656c 2060 6044 4e43 6060 2074   level ``DNC`` t
-000112f0: 6f20 776f 726b 2e0a 2020 2020 2020 2020  o work..        
-00011300: 5265 7475 726e 7320 6060 4e6f 6e65 6060  Returns ``None``
-00011310: 2069 6620 6e6f 2064 6174 6120 7761 7320   if no data was 
-00011320: 7265 6365 6976 6564 206f 7220 6469 6374  received or dict
-00011330: 696f 6e61 7279 2077 6974 6820 6b65 7920  ionary with key 
-00011340: 3d20 6178 6973 206e 616d 652c 2076 616c  = axis name, val
-00011350: 7565 203d 2070 6f73 6974 696f 6e0a 0a20  ue = position.. 
-00011360: 2020 2020 2020 203a 7261 6973 6573 204c         :raises L
-00011370: 5356 3244 6174 6145 7863 6570 7469 6f6e  SV2DataException
-00011380: 3a20 4572 726f 7220 6475 7269 6e67 2070  : Error during p
-00011390: 6172 7369 6e67 206f 6620 6461 7461 2076  arsing of data v
-000113a0: 616c 7565 730a 2020 2020 2020 2020 2222  alues.        ""
-000113b0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-000113c0: 2073 656c 662e 6c6f 6769 6e28 6c63 2e4c   self.login(lc.L
-000113d0: 6f67 696e 2e44 4e43 293a 0a20 2020 2020  ogin.DNC):.     
-000113e0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-000113f0: 6765 722e 7761 726e 696e 6728 2263 6c6f  ger.warning("clo
-00011400: 756c 6420 6e6f 7420 6c6f 6720 696e 2061  uld not log in a
-00011410: 7320 7573 6572 2044 4e43 2229 0a20 2020  s user DNC").   
-00011420: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011430: 4e6f 6e65 0a0a 2020 2020 2020 2020 7061  None..        pa
-00011440: 796c 6f61 6420 3d20 6279 7465 6172 7261  yload = bytearra
-00011450: 7928 290a 2020 2020 2020 2020 7061 796c  y().        payl
-00011460: 6f61 642e 6578 7465 6e64 2873 7472 7563  oad.extend(struc
-00011470: 742e 7061 636b 2822 2148 222c 206c 632e  t.pack("!H", lc.
-00011480: 5061 7252 5249 2e41 5849 535f 4c4f 4341  ParRRI.AXIS_LOCA
-00011490: 5449 4f4e 2929 0a0a 2020 2020 2020 2020  TION))..        
-000114a0: 7265 7375 6c74 203d 2073 656c 662e 5f73  result = self._s
-000114b0: 656e 645f 7265 6369 7665 286c 632e 434d  end_recive(lc.CM
-000114c0: 442e 525f 5249 2c20 7061 796c 6f61 642c  D.R_RI, payload,
-000114d0: 206c 632e 5253 502e 535f 5249 290a 2020   lc.RSP.S_RI).  
-000114e0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000114f0: 6e63 6528 7265 7375 6c74 2c20 2862 7974  nce(result, (byt
-00011500: 6561 7272 6179 2c29 2920 616e 6420 6c65  earray,)) and le
-00011510: 6e28 7265 7375 6c74 2920 3e20 303a 0a20  n(result) > 0:. 
-00011520: 2020 2020 2020 2020 2020 2061 7865 735f             axes_
-00011530: 7661 6c75 6573 203d 206c 6d2e 6465 636f  values = lm.deco
-00011540: 6465 5f61 7869 735f 6c6f 6361 7469 6f6e  de_axis_location
-00011550: 2872 6573 756c 7429 0a20 2020 2020 2020  (result).       
-00011560: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
-00011570: 722e 696e 666f 2822 7375 6363 6573 7366  r.info("successf
-00011580: 756c 6c79 2072 6561 6420 6178 6573 2076  ully read axes v
-00011590: 616c 7565 733a 2025 7322 2c20 6178 6573  alues: %s", axes
-000115a0: 5f76 616c 7565 7329 0a20 2020 2020 2020  _values).       
-000115b0: 2020 2020 2072 6574 7572 6e20 6178 6573       return axes
-000115c0: 5f76 616c 7565 730a 0a20 2020 2020 2020  _values..       
-000115d0: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
-000115e0: 726e 696e 6728 2261 6e20 6572 726f 7220  rning("an error 
-000115f0: 6f63 6375 7272 6564 2077 6869 6c65 2071  occurred while q
-00011600: 7565 7279 696e 6720 6178 6573 2070 6f73  uerying axes pos
-00011610: 6974 696f 6e22 290a 2020 2020 2020 2020  ition").        
-00011620: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00011630: 2064 6566 2067 7261 625f 7363 7265 656e   def grab_screen
-00011640: 5f64 756d 7028 7365 6c66 2c20 696d 6167  _dump(self, imag
-00011650: 655f 7061 7468 3a20 7061 7468 6c69 622e  e_path: pathlib.
-00011660: 5061 7468 2920 2d3e 2062 6f6f 6c3a 0a20  Path) -> bool:. 
-00011670: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011680: 2020 2043 7265 6174 6520 7363 7265 656e     Create screen
-00011690: 5f64 756d 7020 6f66 2063 7572 7265 6e74  _dump of current
-000116a0: 2063 6f6e 7472 6f6c 2073 6372 6565 6e20   control screen 
-000116b0: 616e 6420 7361 7665 2069 7420 6173 2062  and save it as b
-000116c0: 6974 6d61 702e 0a20 2020 2020 2020 2052  itmap..        R
-000116d0: 6571 7569 7265 7320 6163 6365 7373 206c  equires access l
-000116e0: 6576 656c 2060 6044 4e43 6060 2074 6f20  evel ``DNC`` to 
-000116f0: 776f 726b 2e0a 2020 2020 2020 2020 5265  work..        Re
-00011700: 7475 726e 7320 6060 5472 7565 6060 2069  turns ``True`` i
-00011710: 6620 636f 6d70 6c65 7465 6420 7375 6363  f completed succ
-00011720: 6573 7366 756c 6c79 2e0a 0a20 2020 2020  essfully...     
-00011730: 2020 203a 7061 7261 6d20 696d 6167 655f     :param image_
-00011740: 7061 7468 3a20 7061 7468 206f 6620 626d  path: path of bm
-00011750: 7020 6669 6c65 2066 6f72 2073 6372 6565  p file for scree
-00011760: 6e64 756d 700a 2020 2020 2020 2020 2222  ndump.        ""
-00011770: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00011780: 2073 656c 662e 6c6f 6769 6e28 6c63 2e4c   self.login(lc.L
-00011790: 6f67 696e 2e46 494c 4554 5241 4e53 4645  ogin.FILETRANSFE
-000117a0: 5229 3a0a 2020 2020 2020 2020 2020 2020  R):.            
-000117b0: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-000117c0: 6e69 6e67 2822 636c 6f75 6c64 206e 6f74  ning("clould not
-000117d0: 206c 6f67 2069 6e20 6173 2075 7365 7220   log in as user 
-000117e0: 4649 4c45 2229 0a20 2020 2020 2020 2020  FILE").         
-000117f0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00011800: 0a20 2020 2020 2020 2074 656d 705f 6669  .        temp_fi
-00011810: 6c65 5f70 6174 6820 3d20 280a 2020 2020  le_path = (.    
-00011820: 2020 2020 2020 2020 6c63 2e44 7269 7665          lc.Drive
-00011830: 4e61 6d65 2e54 4e43 0a20 2020 2020 2020  Name.TNC.       
-00011840: 2020 2020 202b 206c 632e 5041 5448 5f53       + lc.PATH_S
-00011850: 4550 0a20 2020 2020 2020 2020 2020 202b  EP.            +
-00011860: 2022 7363 7265 656e 6475 6d70 5f22 0a20   "screendump_". 
-00011870: 2020 2020 2020 2020 2020 202b 2064 6174             + dat
-00011880: 6574 696d 652e 6e6f 7728 292e 7374 7266  etime.now().strf
-00011890: 7469 6d65 2822 2559 256d 2564 5f25 4825  time("%Y%m%d_%H%
-000118a0: 4d25 5322 290a 2020 2020 2020 2020 2020  M%S").          
-000118b0: 2020 2b20 222e 626d 7022 0a20 2020 2020    + ".bmp".     
-000118c0: 2020 2029 0a0a 2020 2020 2020 2020 7061     )..        pa
-000118d0: 796c 6f61 6420 3d20 6279 7465 6172 7261  yload = bytearra
-000118e0: 7928 7374 7275 6374 2e70 6163 6b28 2221  y(struct.pack("!
-000118f0: 4822 2c20 6c63 2e50 6172 4343 432e 5343  H", lc.ParCCC.SC
-00011900: 5245 454e 4455 4d50 2929 0a20 2020 2020  REENDUMP)).     
-00011910: 2020 2070 6179 6c6f 6164 2e65 7874 656e     payload.exten
-00011920: 6428 6c6d 2e75 7374 725f 746f 5f62 6128  d(lm.ustr_to_ba(
-00011930: 7465 6d70 5f66 696c 655f 7061 7468 2929  temp_file_path))
-00011940: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00011950: 203d 2073 656c 662e 5f73 656e 645f 7265   = self._send_re
-00011960: 6369 7665 286c 632e 434d 442e 435f 4343  cive(lc.CMD.C_CC
-00011970: 2c20 7061 796c 6f61 642c 206c 632e 5253  , payload, lc.RS
-00011980: 502e 545f 4f4b 290a 0a20 2020 2020 2020  P.T_OK)..       
-00011990: 2069 6620 6e6f 7420 2869 7369 6e73 7461   if not (isinsta
-000119a0: 6e63 6528 7265 7375 6c74 2c20 2862 6f6f  nce(result, (boo
-000119b0: 6c2c 2929 2061 6e64 2072 6573 756c 7420  l,)) and result 
-000119c0: 6973 2054 7275 6529 3a0a 2020 2020 2020  is True):.      
-000119d0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-000119e0: 6572 2e77 6172 6e69 6e67 2822 7363 7265  er.warning("scre
-000119f0: 656e 2064 756d 7020 7761 7320 6e6f 7420  en dump was not 
-00011a00: 6372 6561 7465 6422 290a 2020 2020 2020  created").      
-00011a10: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00011a20: 7365 0a0a 2020 2020 2020 2020 6966 206e  se..        if n
-00011a30: 6f74 2073 656c 662e 7265 6369 7665 5f66  ot self.recive_f
-00011a40: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
-00011a50: 2072 656d 6f74 655f 7061 7468 3d74 656d   remote_path=tem
-00011a60: 705f 6669 6c65 5f70 6174 682c 206c 6f63  p_file_path, loc
-00011a70: 616c 5f70 6174 683d 696d 6167 655f 7061  al_path=image_pa
-00011a80: 7468 2c20 6269 6e61 7279 5f6d 6f64 653d  th, binary_mode=
-00011a90: 5472 7565 0a20 2020 2020 2020 2029 3a0a  True.        ):.
-00011aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011ab0: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
-00011ac0: 2822 636f 756c 6420 6e6f 7420 646f 776e  ("could not down
-00011ad0: 6c6f 6164 2073 6372 6565 6e20 6475 6d70  load screen dump
-00011ae0: 2066 726f 6d20 636f 6e74 726f 6c22 290a   from control").
-00011af0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011b00: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-00011b10: 2020 6966 206e 6f74 2073 656c 662e 6465    if not self.de
-00011b20: 6c65 7465 5f66 696c 6528 7465 6d70 5f66  lete_file(temp_f
-00011b30: 696c 655f 7061 7468 293a 0a20 2020 2020  ile_path):.     
-00011b40: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-00011b50: 6765 722e 7761 726e 696e 6728 2263 6c6f  ger.warning("clo
-00011b60: 756c 6420 6e6f 7420 6465 6c65 7465 2074  uld not delete t
-00011b70: 656d 706f 7261 7279 2066 696c 6520 6f6e  emporary file on
-00011b80: 2063 6f6e 7472 6f6c 2229 0a20 2020 2020   control").     
-00011b90: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00011ba0: 6c73 650a 0a20 2020 2020 2020 2073 656c  lse..        sel
-00011bb0: 662e 5f6c 6f67 6765 722e 6465 6275 6728  f._logger.debug(
-00011bc0: 2273 7563 6365 7373 6675 6c6c 7920 7265  "successfully re
-00011bd0: 6365 6976 6564 2073 6372 6565 6e20 6475  ceived screen du
-00011be0: 6d70 2229 0a20 2020 2020 2020 2072 6574  mp").        ret
-00011bf0: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
-00011c00: 6620 6765 745f 7265 6d6f 7465 5f64 6174  f get_remote_dat
-00011c10: 6574 696d 6528 7365 6c66 2920 2d3e 2064  etime(self) -> d
-00011c20: 6174 6574 696d 653a 0a20 2020 2020 2020  atetime:.       
-00011c30: 2022 2222 0a20 2020 2020 2020 2052 6561   """.        Rea
-00011c40: 6420 6375 7272 656e 7420 7469 6d65 2061  d current time a
-00011c50: 6e64 2064 6174 6520 6672 6f6d 2063 6f6e  nd date from con
-00011c60: 7472 6f6c 0a20 2020 2020 2020 2022 2222  trol.        """
-00011c70: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00011c80: 7365 6c66 2e6c 6f67 696e 286c 632e 4c6f  self.login(lc.Lo
-00011c90: 6769 6e2e 4449 4147 293a 0a20 2020 2020  gin.DIAG):.     
-00011ca0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-00011cb0: 6765 722e 7761 726e 696e 6728 2263 6c6f  ger.warning("clo
-00011cc0: 756c 6420 6e6f 7420 6c6f 6720 696e 2061  uld not log in a
-00011cd0: 7320 7573 6572 2066 6f72 2044 4941 474e  s user for DIAGN
-00011ce0: 4f53 5449 4353 2066 756e 6374 696f 6e22  OSTICS function"
-00011cf0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00011d00: 7475 726e 2064 6174 6574 696d 652e 6672  turn datetime.fr
-00011d10: 6f6d 7469 6d65 7374 616d 7028 3029 0a0a  omtimestamp(0)..
-00011d20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00011d30: 2073 656c 662e 5f73 656e 645f 7265 6369   self._send_reci
-00011d40: 7665 286c 632e 434d 442e 525f 4454 2c20  ve(lc.CMD.R_DT, 
-00011d50: 4e6f 6e65 2c20 6c63 2e52 5350 2e53 5f44  None, lc.RSP.S_D
-00011d60: 5429 0a20 2020 2020 2020 2069 6620 6973  T).        if is
-00011d70: 696e 7374 616e 6365 2872 6573 756c 742c  instance(result,
-00011d80: 2028 6279 7465 6172 7261 792c 2929 2061   (bytearray,)) a
-00011d90: 6e64 206c 656e 2872 6573 756c 7429 203e  nd len(result) >
-00011da0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00011db0: 7473 203d 206c 6d2e 6465 636f 6465 5f74  ts = lm.decode_t
-00011dc0: 696d 6573 7461 6d70 2872 6573 756c 7429  imestamp(result)
-00011dd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00011de0: 662e 5f6c 6f67 6765 722e 6465 6275 6728  f._logger.debug(
-00011df0: 2254 696d 6520 6f6e 2043 6f6e 7472 6f6c  "Time on Control
-00011e00: 2069 7320 2573 222c 2074 732e 6973 6f66   is %s", ts.isof
-00011e10: 6f72 6d61 7428 2929 0a20 2020 2020 2020  ormat()).       
-00011e20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00011e30: 2020 2072 6169 7365 204c 5356 3250 726f     raise LSV2Pro
-00011e40: 746f 636f 6c45 7863 6570 7469 6f6e 280a  tocolException(.
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2273 6f6d 6574 6869 6e67 2077 656e 7420  "something went 
-00011e70: 7772 6f6e 6720 7768 696c 6520 7265 6164  wrong while read
-00011e80: 696e 6720 6375 7272 656e 7420 7469 6d65  ing current time
-00011e90: 2061 6e64 2064 6174 6522 0a20 2020 2020   and date".     
-00011ea0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00011eb0: 2072 6574 7572 6e20 7473 0a0a 2020 2020   return ts..    
-00011ec0: 6465 6620 7265 6164 5f73 636f 7065 5f73  def read_scope_s
-00011ed0: 6967 6e61 6c73 2873 656c 6629 202d 3e20  ignals(self) -> 
-00011ee0: 4c69 7374 5b6c 642e 5363 6f70 6553 6967  List[ld.ScopeSig
-00011ef0: 6e61 6c5d 3a0a 2020 2020 2020 2020 2222  nal]:.        ""
-00011f00: 220a 2020 2020 2020 2020 5265 6164 2061  ".        Read a
-00011f10: 7661 696c 6162 6c65 2073 636f 7065 2063  vailable scope c
-00011f20: 6861 6e6e 656c 7320 616e 6420 7369 676e  hannels and sign
-00011f30: 616c 732e 204f 6e6c 7920 776f 726b 7320  als. Only works 
-00011f40: 666f 7220 6954 4e43 2035 3330 2e0a 2020  for iTNC 530..  
-00011f50: 2020 2020 2020 5265 7175 6972 6573 2061        Requires a
-00011f60: 6363 6573 7320 6c65 7665 6c20 6060 5343  ccess level ``SC
-00011f70: 4f50 4560 6020 746f 2077 6f72 6b2e 0a20  OPE`` to work.. 
-00011f80: 2020 2020 2020 2072 6574 7572 6e73 206c         returns l
-00011f90: 6973 7420 6f66 203a 7079 3a63 6c61 7373  ist of :py:class
-00011fa0: 3a60 7e70 794c 5356 322e 4c53 5632 2e53  :`~pyLSV2.LSV2.S
-00011fb0: 636f 7065 5369 676e 616c 6020 666f 7220  copeSignal` for 
-00011fc0: 6561 6368 2073 6967 6e61 6c0a 2020 2020  each signal.    
-00011fd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011fe0: 6966 206e 6f74 2073 656c 662e 7665 7273  if not self.vers
-00011ff0: 696f 6e73 2e69 735f 6974 6e63 2829 3a0a  ions.is_itnc():.
-00012000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012010: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
-00012020: 2822 6f6e 6c79 2077 6f72 6b73 2066 6f72  ("only works for
-00012030: 2069 544e 4335 3330 2229 0a20 2020 2020   iTNC530").     
-00012040: 2020 2020 2020 2072 6574 7572 6e20 6c69         return li
-00012050: 7374 2829 0a0a 2020 2020 2020 2020 6966  st()..        if
-00012060: 206e 6f74 2073 656c 662e 6c6f 6769 6e28   not self.login(
-00012070: 6c63 2e4c 6f67 696e 2e53 434f 5045 293a  lc.Login.SCOPE):
-00012080: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012090: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
-000120a0: 6728 2263 6c6f 756c 6420 6e6f 7420 6c6f  g("clould not lo
-000120b0: 6720 696e 2061 7320 7573 6572 2066 6f72  g in as user for
-000120c0: 2073 636f 7065 2066 756e 6374 696f 6e22   scope function"
-000120d0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000120e0: 7475 726e 206c 6973 7428 290a 0a20 2020  turn list()..   
-000120f0: 2020 2020 2063 6861 6e6e 656c 5f6c 6973       channel_lis
-00012100: 7420 3d20 6c69 7374 2829 0a0a 2020 2020  t = list()..    
-00012110: 2020 2020 636f 6e74 656e 7420 3d20 7365      content = se
-00012120: 6c66 2e5f 6c6c 636f 6d2e 7465 6c65 6772  lf._llcom.telegr
-00012130: 616d 286c 632e 434d 442e 525f 4f43 290a  am(lc.CMD.R_OC).
-00012140: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00012150: 5f6c 6c63 6f6d 2e6c 6173 745f 7265 7370  _llcom.last_resp
-00012160: 6f6e 7365 2069 6e20 6c63 2e52 5350 2e53  onse in lc.RSP.S
-00012170: 5f4f 433a 0a20 2020 2020 2020 2020 2020  _OC:.           
-00012180: 2063 6861 6e6e 656c 5f6c 6973 742e 6578   channel_list.ex
-00012190: 7465 6e64 286c 6d73 2e64 6563 6f64 655f  tend(lms.decode_
-000121a0: 7369 676e 616c 5f64 6573 6372 6970 7469  signal_descripti
-000121b0: 6f6e 2863 6f6e 7465 6e74 2929 0a0a 2020  on(content))..  
-000121c0: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-000121d0: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
-000121e0: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-000121f0: 7365 6c66 2e5f 6c6c 636f 6d2e 7465 6c65  self._llcom.tele
-00012200: 6772 616d 286c 632e 5253 502e 545f 4f4b  gram(lc.RSP.T_OK
-00012210: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012220: 2020 2069 6620 7365 6c66 2e5f 6c6c 636f     if self._llco
-00012230: 6d2e 6c61 7374 5f72 6573 706f 6e73 6520  m.last_response 
-00012240: 696e 206c 632e 5253 502e 535f 4f43 3a0a  in lc.RSP.S_OC:.
-00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012260: 2020 2020 6368 616e 6e65 6c5f 6c69 7374      channel_list
-00012270: 2e65 7874 656e 6428 6c6d 732e 6465 636f  .extend(lms.deco
-00012280: 6465 5f73 6967 6e61 6c5f 6465 7363 7269  de_signal_descri
-00012290: 7074 696f 6e28 636f 6e74 656e 7429 290a  ption(content)).
-000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122b0: 656c 6966 2073 656c 662e 5f6c 6c63 6f6d  elif self._llcom
-000122c0: 2e6c 6173 745f 7265 7370 6f6e 7365 2069  .last_response i
-000122d0: 6e20 6c63 2e52 5350 2e54 5f46 443a 0a20  n lc.RSP.T_FD:. 
-000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122f0: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
-00012300: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
-00012310: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00012320: 696e 6973 6865 6420 6c6f 6164 696e 6720  inished loading 
-00012330: 616e 6420 7061 7273 696e 6720 6461 7461  and parsing data
-00012340: 2066 6f72 2061 6c6c 2073 636f 7065 2073   for all scope s
-00012350: 6967 6e61 6c73 220a 2020 2020 2020 2020  ignals".        
-00012360: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012380: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00012390: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123b0: 2020 7365 6c66 2e5f 6c6f 6767 6572 2e65    self._logger.e
-000123c0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-000123d0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000123e0: 6f6d 6574 6869 6e67 2077 656e 7420 7772  omething went wr
-000123f0: 6f6e 6720 7768 696c 6520 7265 6164 696e  ong while readin
-00012400: 6720 7363 6f70 6520 7369 676e 616c 220a  g scope signal".
-00012410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012420: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00012430: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00012440: 4c53 5632 5072 6f74 6f63 6f6c 4578 6365  LSV2ProtocolExce
-00012450: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
-00012460: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012470: 6469 6420 6e6f 7420 7265 6365 6976 6564  did not received
-00012480: 2065 7870 6563 7465 6420 7265 7370 6f6e   expected respon
-00012490: 7365 2077 6869 6c65 2072 6561 6469 6e67  se while reading
-000124a0: 2064 6174 6120 666f 7220 7363 6f70 6520   data for scope 
-000124b0: 7369 676e 616c 7322 0a20 2020 2020 2020  signals".       
-000124c0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-000124d0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-000124e0: 6861 6e6e 656c 5f6c 6973 740a 0a20 2020  hannel_list..   
-000124f0: 2064 6566 2072 6561 6c5f 7469 6d65 5f72   def real_time_r
-00012500: 6561 6469 6e67 7328 0a20 2020 2020 2020  eadings(.       
-00012510: 2073 656c 662c 2073 6967 6e61 6c5f 6c69   self, signal_li
-00012520: 7374 3a20 4c69 7374 5b6c 642e 5363 6f70  st: List[ld.Scop
-00012530: 6553 6967 6e61 6c5d 2c20 6475 7261 7469  eSignal], durati
-00012540: 6f6e 3a20 696e 742c 2069 6e74 6572 7661  on: int, interva
-00012550: 6c3a 2069 6e74 0a20 2020 2029 3a0a 2020  l: int.    ):.  
-00012560: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012570: 2020 5265 6164 2073 6967 6e61 6c20 7265    Read signal re
-00012580: 6164 696e 6773 2066 726f 6d20 636f 6e74  adings from cont
-00012590: 726f 6c20 696e 2072 6561 6c20 7469 6d65  rol in real time
-000125a0: 2e20 4f6e 6c79 2077 6f72 6b73 2066 6f72  . Only works for
-000125b0: 2069 544e 4320 3533 302e 0a20 2020 2020   iTNC 530..     
-000125c0: 2020 2042 6566 6f72 6520 7265 6164 696e     Before readin
-000125d0: 6720 6461 7461 2c20 7468 6520 7369 676e  g data, the sign
-000125e0: 616c 2064 6573 6372 6970 7469 6f6e 2069  al description i
-000125f0: 7320 7570 6461 7465 6420 7769 7468 2069  s updated with i
-00012600: 6e66 6f72 6d61 7469 6f6e 2072 6567 6172  nformation regar
-00012610: 6469 6e66 206f 6666 7365 7420 616e 6420  dinf offset and 
-00012620: 6661 6374 6f72 2e0a 2020 2020 2020 2020  factor..        
-00012630: 5265 7175 6972 6573 2061 6363 6573 7320  Requires access 
-00012640: 6c65 7665 6c20 6060 5343 4f50 4560 6020  level ``SCOPE`` 
-00012650: 746f 2077 6f72 6b2e 0a0a 2020 2020 2020  to work...      
-00012660: 2020 3a70 6172 616d 2073 6967 6e61 6c5f    :param signal_
-00012670: 6c69 7374 3a20 6c69 7374 206f 6620 3a70  list: list of :p
-00012680: 793a 636c 6173 733a 607e 7079 4c53 5632  y:class:`~pyLSV2
-00012690: 2e4c 5356 322e 5363 6f70 6553 6967 6e61  .LSV2.ScopeSigna
-000126a0: 6c60 2077 6869 6368 2073 686f 756c 6420  l` which should 
-000126b0: 6265 2072 6561 6420 6672 6f6d 2063 6f6e  be read from con
-000126c0: 7472 6f6c 0a20 2020 2020 2020 203a 7061  trol.        :pa
-000126d0: 7261 6d20 6475 7261 7469 6f6e 3a20 6e75  ram duration: nu
-000126e0: 6d62 6572 206f 6620 7365 636f 6e64 7320  mber of seconds 
-000126f0: 666f 7220 7768 6963 6820 6461 7461 2073  for which data s
-00012700: 686f 756c 6420 6265 2072 6561 640a 2020  hould be read.  
-00012710: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
-00012720: 6572 7661 6c3a 2069 6e74 6572 7661 6c20  erval: interval 
-00012730: 696e 20c2 b573 2062 6574 7765 656e 2072  in ..s between r
-00012740: 6561 6469 6e67 730a 0a20 2020 2020 2020  eadings..       
-00012750: 203a 7261 6973 6573 204c 5356 3250 726f   :raises LSV2Pro
-00012760: 746f 636f 6c45 7863 6570 7469 6f6e 3a0a  tocolException:.
-00012770: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012780: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00012790: 7665 7273 696f 6e73 2e69 735f 6974 6e63  versions.is_itnc
-000127a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000127b0: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-000127c0: 6e69 6e67 2822 6f6e 6c79 2077 6f72 6b73  ning("only works
-000127d0: 2066 6f72 2069 544e 4335 3330 2229 0a20   for iTNC530"). 
-000127e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000127f0: 6e20 6c69 7374 2829 0a0a 2020 2020 2020  n list()..      
-00012800: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
-00012810: 6769 6e28 6c63 2e4c 6f67 696e 2e53 434f  gin(lc.Login.SCO
-00012820: 5045 293a 0a20 2020 2020 2020 2020 2020  PE):.           
-00012830: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
-00012840: 726e 696e 6728 2263 6c6f 756c 6420 6e6f  rning("clould no
-00012850: 7420 6c6f 6720 696e 2061 7320 7573 6572  t log in as user
-00012860: 2066 6f72 2073 636f 7065 2066 756e 6374   for scope funct
-00012870: 696f 6e22 290a 2020 2020 2020 2020 2020  ion").          
-00012880: 2020 7265 7475 726e 206c 6973 7428 290a    return list().
-00012890: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
-000128a0: 6f67 6765 722e 6465 6275 6728 0a20 2020  ogger.debug(.   
-000128b0: 2020 2020 2020 2020 2022 7374 6172 7420           "start 
-000128c0: 7265 636f 6469 6e67 2025 6420 7265 6164  recoding %d read
-000128d0: 696e 6773 2077 6974 6820 696e 7465 7276  ings with interv
-000128e0: 616c 206f 6620 2564 20c2 b573 222c 0a20  al of %d ..s",. 
-000128f0: 2020 2020 2020 2020 2020 2064 7572 6174             durat
-00012900: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00012910: 2069 6e74 6572 7661 6c2c 0a20 2020 2020   interval,.     
-00012920: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-00012930: 7365 7420 696e 7465 7276 616c 2061 6e64  set interval and
-00012940: 2073 656c 6563 7420 7369 676e 616c 730a   select signals.
-00012950: 2020 2020 2020 2020 7061 796c 6f61 6420          payload 
-00012960: 3d20 6279 7465 6172 7261 7928 290a 2020  = bytearray().  
-00012970: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
-00012980: 7465 6e64 2873 7472 7563 742e 7061 636b  tend(struct.pack
-00012990: 2822 214c 222c 2069 6e74 6572 7661 6c29  ("!L", interval)
-000129a0: 290a 2020 2020 2020 2020 666f 7220 7369  ).        for si
-000129b0: 676e 616c 2069 6e20 7369 676e 616c 5f6c  gnal in signal_l
-000129c0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-000129d0: 2069 6620 696e 7465 7276 616c 206e 6f74   if interval not
-000129e0: 2069 6e20 5b36 3030 2c20 3330 3030 2c20   in [600, 3000, 
-000129f0: 3231 3030 305d 3a0a 2020 2020 2020 2020  21000]:.        
-00012a00: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00012a10: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 2020 2274 6865 2073 656c 6563 7465 6420    "the selected 
-00012a40: 696e 7465 7276 616c 2064 6f65 736e 2774  interval doesn't
-00012a50: 2066 6974 2066 6f72 2073 6967 6e61 6c73   fit for signals
-00012a60: 2072 6561 6469 6e67 7321 220a 2020 2020   readings!".    
-00012a70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00012a80: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00012a90: 6973 6520 4c53 5632 5072 6f74 6f63 6f6c  ise LSV2Protocol
-00012aa0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-00012ab0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012ac0: 7468 6520 7365 6c65 6374 6564 2069 6e74  the selected int
-00012ad0: 6572 7661 6c20 6d75 7374 2062 653a 2036  erval must be: 6
-00012ae0: 3030 206f 7220 3330 3030 206f 7220 3231  00 or 3000 or 21
-00012af0: 3030 3020 7573 220a 2020 2020 2020 2020  000 us".        
-00012b00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00012b10: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
-00012b20: 7465 6e64 2873 6967 6e61 6c2e 746f 5f62  tend(signal.to_b
-00012b30: 6128 2929 0a0a 2020 2020 2020 2020 7265  a())..        re
-00012b40: 7375 6c74 203d 2073 656c 662e 5f73 656e  sult = self._sen
-00012b50: 645f 7265 6369 7665 286c 632e 434d 442e  d_recive(lc.CMD.
-00012b60: 525f 4f50 2c20 7061 796c 6f61 642c 206c  R_OP, payload, l
-00012b70: 632e 5253 502e 535f 4f50 290a 2020 2020  c.RSP.S_OP).    
-00012b80: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00012b90: 6528 7265 7375 6c74 2c20 2862 7974 6561  e(result, (bytea
-00012ba0: 7272 6179 2c29 2920 616e 6420 6c65 6e28  rray,)) and len(
-00012bb0: 7265 7375 6c74 2920 3e20 303a 0a20 2020  result) > 0:.   
-00012bc0: 2020 2020 2020 2020 2073 6967 6e61 6c5f           signal_
-00012bd0: 6c69 7374 203d 206c 6d73 2e64 6563 6f64  list = lms.decod
-00012be0: 655f 7369 676e 616c 5f64 6574 6169 6c73  e_signal_details
-00012bf0: 2873 6967 6e61 6c5f 6c69 7374 2c20 7265  (signal_list, re
-00012c00: 7375 6c74 290a 2020 2020 2020 2020 656c  sult).        el
-00012c10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00012c20: 6966 2073 656c 662e 6c61 7374 5f65 7272  if self.last_err
-00012c30: 6f72 2e65 5f63 6f64 6520 3d3d 2038 353a  or.e_code == 85:
-00012c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c50: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
-00012c60: 726e 696e 6728 2274 6f6f 206d 616e 7920  rning("too many 
-00012c70: 7369 676e 616c 7320 7365 6c65 6374 6564  signals selected
-00012c80: 3a20 2564 222c 206c 656e 2873 6967 6e61  : %d", len(signa
-00012c90: 6c5f 6c69 7374 2929 0a20 2020 2020 2020  l_list)).       
-00012ca0: 2020 2020 2020 2020 2072 6169 7365 204c           raise L
-00012cb0: 5356 3250 726f 746f 636f 6c45 7863 6570  SV2ProtocolExcep
-00012cc0: 7469 6f6e 2822 746f 6f20 6d61 6e79 2073  tion("too many s
-00012cd0: 6967 6e61 6c73 2073 656c 6563 7465 643f  ignals selected?
-00012ce0: 3f3f 2229 0a20 2020 2020 2020 2020 2020  ??").           
-00012cf0: 2069 6620 7365 6c66 2e6c 6173 745f 6572   if self.last_er
-00012d00: 726f 722e 655f 636f 6465 203d 3d20 6c63  ror.e_code == lc
-00012d10: 2e4c 5356 3253 7461 7475 7343 6f64 652e  .LSV2StatusCode.
-00012d20: 545f 4552 5f4f 535a 495f 4348 5345 4c3a  T_ER_OSZI_CHSEL:
-00012d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d40: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
-00012d50: 726e 696e 6728 2245 7272 6f72 2073 6574  rning("Error set
-00012d60: 7469 6e67 2075 7020 7468 6520 6368 616e  ting up the chan
-00012d70: 6e65 6c73 2229 0a20 2020 2020 2020 2020  nels").         
-00012d80: 2020 2020 2020 2072 6169 7365 204c 5356         raise LSV
-00012d90: 3250 726f 746f 636f 6c45 7863 6570 7469  2ProtocolExcepti
-00012da0: 6f6e 2822 4572 726f 7220 7365 7474 696e  on("Error settin
-00012db0: 6720 7570 2074 6865 2063 6861 6e6e 656c  g up the channel
-00012dc0: 7322 290a 2020 2020 2020 2020 2020 2020  s").            
-00012dd0: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
-00012de0: 6e69 6e67 2822 4572 726f 7220 7768 696c  ning("Error whil
-00012df0: 6520 636f 6e66 6967 7572 696e 6720 696e  e configuring in
-00012e00: 7465 7276 616c 2061 6e64 2073 6967 6e61  terval and signa
-00012e10: 6c73 2229 0a20 2020 2020 2020 2020 2020  ls").           
-00012e20: 2072 6169 7365 204c 5356 3250 726f 746f   raise LSV2Proto
-00012e30: 636f 6c45 7863 6570 7469 6f6e 2822 4572  colException("Er
-00012e40: 726f 7220 7768 696c 6520 636f 6e66 6967  ror while config
-00012e50: 7572 696e 6720 696e 7465 7276 616c 2061  uring interval a
-00012e60: 6e64 2073 6967 6e61 6c73 2229 0a0a 2020  nd signals")..  
-00012e70: 2020 2020 2020 2320 7365 7475 7020 7472        # setup tr
-00012e80: 6967 6765 7220 616e 6420 7265 6164 2064  igger and read d
-00012e90: 6174 6120 6672 6f6d 2063 6f6e 7472 6f6c  ata from control
-00012ea0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00012eb0: 203d 2062 7974 6561 7272 6179 2829 0a20   = bytearray(). 
-00012ec0: 2020 2020 2020 2070 6179 6c6f 6164 2e65         payload.e
-00012ed0: 7874 656e 6428 7374 7275 6374 2e70 6163  xtend(struct.pac
-00012ee0: 6b28 2221 4822 2c20 3629 2920 2023 2074  k("!H", 6))  # t
-00012ef0: 7269 6767 6572 2063 6861 6e6e 656c 3f0a  rigger channel?.
-00012f00: 2020 2020 2020 2020 7061 796c 6f61 642e          payload.
-00012f10: 6578 7465 6e64 2873 7472 7563 742e 7061  extend(struct.pa
-00012f20: 636b 2822 2148 222c 2036 3535 3335 2929  ck("!H", 65535))
-00012f30: 2020 2320 7472 6967 6765 7220 6d6f 6465    # trigger mode
-00012f40: 3f0a 2020 2020 2020 2020 7061 796c 6f61  ?.        payloa
-00012f50: 642e 6578 7465 6e64 2873 7472 7563 742e  d.extend(struct.
-00012f60: 7061 636b 2822 214c 222c 2030 2929 2020  pack("!L", 0))  
-00012f70: 2320 7472 6967 6765 7220 6c65 7665 6c3f  # trigger level?
-00012f80: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00012f90: 2e65 7874 656e 6428 7374 7275 6374 2e70  .extend(struct.p
-00012fa0: 6163 6b28 2221 4c22 2c20 3029 2920 2023  ack("!L", 0))  #
-00012fb0: 2070 7265 2074 7269 6767 6572 3f0a 2020   pre trigger?.  
-00012fc0: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
-00012fd0: 7465 6e64 2873 7472 7563 742e 7061 636b  tend(struct.pack
-00012fe0: 2822 214c 222c 2069 6e74 6572 7661 6c29  ("!L", interval)
-00012ff0: 290a 0a20 2020 2020 2020 2073 7461 7274  )..        start
-00013000: 203d 2074 696d 652e 7469 6d65 2829 2020   = time.time()  
-00013010: 2320 7374 6172 7420 7469 6d65 720a 2020  # start timer.  
-00013020: 2020 2020 2020 7265 636f 7264 6564 5f64        recorded_d
-00013030: 6174 6120 3d20 6c69 7374 2829 0a20 2020  ata = list().   
-00013040: 2020 2020 2063 6f6e 7465 6e74 203d 2073       content = s
-00013050: 656c 662e 5f73 656e 645f 7265 6369 7665  elf._send_recive
-00013060: 286c 632e 434d 442e 525f 4f44 2c20 7061  (lc.CMD.R_OD, pa
-00013070: 796c 6f61 642c 206c 632e 5253 502e 535f  yload, lc.RSP.S_
-00013080: 4f44 290a 0a20 2020 2020 2020 2069 6620  OD)..        if 
-00013090: 6e6f 7420 6973 696e 7374 616e 6365 2863  not isinstance(c
-000130a0: 6f6e 7465 6e74 2c20 2862 7974 6561 7272  ontent, (bytearr
-000130b0: 6179 2c29 2920 6f72 206c 656e 2863 6f6e  ay,)) or len(con
-000130c0: 7465 6e74 2920 3c3d 2030 3a0a 2020 2020  tent) <= 0:.    
-000130d0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-000130e0: 6767 6572 2e65 7272 6f72 280a 2020 2020  gger.error(.    
-000130f0: 2020 2020 2020 2020 2020 2020 2273 6f6d              "som
-00013100: 6574 6869 6e67 2077 656e 7420 7772 6f6e  ething went wron
-00013110: 6720 7768 696c 6520 7265 6164 696e 6720  g while reading 
-00013120: 6669 7273 7420 6461 7461 2070 6163 6b61  first data packa
-00013130: 6765 2066 6f72 2073 6967 6e61 6c73 220a  ge for signals".
-00013140: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00013150: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00013160: 4c53 5632 5072 6f74 6f63 6f6c 4578 6365  LSV2ProtocolExce
-00013170: 7074 696f 6e28 2273 6f6d 6574 6869 6e67  ption("something
-00013180: 2077 656e 7420 7772 6f6e 6720 7768 696c   went wrong whil
-00013190: 6520 7265 6164 696e 6720 7363 6f70 6520  e reading scope 
-000131a0: 6461 7461 2229 0a0a 2020 2020 2020 2020  data")..        
-000131b0: 7265 636f 7264 6564 5f64 6174 612e 6170  recorded_data.ap
-000131c0: 7065 6e64 286c 6d73 2e64 6563 6f64 655f  pend(lms.decode_
-000131d0: 7363 6f70 655f 7265 6164 696e 6728 7369  scope_reading(si
-000131e0: 676e 616c 5f6c 6973 742c 2063 6f6e 7465  gnal_list, conte
-000131f0: 6e74 2929 0a20 2020 2020 2020 2065 6e64  nt)).        end
-00013200: 203d 2074 696d 652e 7469 6d65 2829 0a20   = time.time(). 
-00013210: 2020 2020 2020 2074 696d 6572 203d 2065         timer = e
-00013220: 6e64 202d 2073 7461 7274 0a20 2020 2020  nd - start.     
-00013230: 2020 2077 6869 6c65 2074 696d 6572 203c     while timer <
-00013240: 2064 7572 6174 696f 6e3a 0a20 2020 2020   duration:.     
-00013250: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-00013260: 2073 656c 662e 5f6c 6c63 6f6d 2e74 656c   self._llcom.tel
-00013270: 6567 7261 6d28 6c63 2e52 5350 2e54 5f4f  egram(lc.RSP.T_O
-00013280: 4b29 0a20 2020 2020 2020 2020 2020 2069  K).            i
-00013290: 6620 7365 6c66 2e5f 6c6c 636f 6d2e 6c61  f self._llcom.la
-000132a0: 7374 5f72 6573 706f 6e73 6520 696e 206c  st_response in l
-000132b0: 632e 5253 502e 535f 4f44 3a0a 2020 2020  c.RSP.S_OD:.    
-000132c0: 2020 2020 2020 2020 2020 2020 7265 636f              reco
-000132d0: 7264 6564 5f64 6174 612e 6170 7065 6e64  rded_data.append
-000132e0: 286c 6d73 2e64 6563 6f64 655f 7363 6f70  (lms.decode_scop
-000132f0: 655f 7265 6164 696e 6728 7369 676e 616c  e_reading(signal
-00013300: 5f6c 6973 742c 2063 6f6e 7465 6e74 2929  _list, content))
-00013310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013320: 2079 6965 6c64 2072 6563 6f72 6465 645f   yield recorded_
-00013330: 6461 7461 5b30 5d0a 2020 2020 2020 2020  data[0].        
-00013340: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00013350: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00013360: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
-00013370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013380: 2020 2020 2273 6f6d 6574 6869 6e67 2077      "something w
-00013390: 656e 7420 7772 6f6e 6720 6475 7269 6e67  ent wrong during
-000133a0: 2070 6572 696f 6469 6361 6c6c 7920 7265   periodically re
-000133b0: 6164 696e 6720 7363 6f70 6520 6461 7461  ading scope data
-000133c0: 2c20 6162 6f72 7420 7265 6164 696e 6722  , abort reading"
-000133d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000133e0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000133f0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00013400: 2020 2020 2065 6e64 203d 2074 696d 652e       end = time.
-00013410: 7469 6d65 2829 0a20 2020 2020 2020 2020  time().         
-00013420: 2020 2074 696d 6572 203d 2065 6e64 202d     timer = end -
-00013430: 2073 7461 7274 0a20 2020 2020 2020 2020   start.         
-00013440: 2020 2072 6563 6f72 6465 645f 6461 7461     recorded_data
-00013450: 203d 206c 6973 7428 290a 0a20 2020 2020   = list()..     
-00013460: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
-00013470: 6465 6275 6728 2266 696e 6973 6865 6420  debug("finished 
-00013480: 7265 6164 696e 6720 7363 6f70 6520 6461  reading scope da
-00013490: 7461 2229 0a                             ta").
+0000dba0: 2020 2020 7374 7275 6374 2e75 6e70 6163      struct.unpac
+0000dbb0: 6b28 0a20 2020 2020 2020 2020 2020 2020  k(.             
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbd0: 2020 2075 6e70 6163 6b5f 7374 7269 6e67     unpack_string
+0000dbe0: 2c20 7265 7375 6c74 5b6a 3a20 6a20 2b20  , result[j: j + 
+0000dbf0: 6d65 6d5f 6279 7465 5f63 6f75 6e74 5d0a  mem_byte_count].
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc10: 2020 2020 2020 2020 2020 2020 295b 305d              )[0]
+0000dc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc30: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000dc40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000dc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc60: 2020 2020 206c 6f67 6769 6e67 2e65 7272       logging.err
+0000dc70: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000dc80: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
+0000dc90: 6c65 6420 746f 2072 6561 6420 7661 6c75  led to read valu
+0000dca0: 6520 6672 6f6d 2061 6464 7265 7373 2025  e from address %
+0000dcb0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0000dcc0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+0000dcd0: 745f 6164 6472 6573 7320 2b20 6669 7273  t_address + firs
+0000dce0: 745f 656c 656d 656e 745f 696e 5f67 726f  t_element_in_gro
+0000dcf0: 7570 2c0a 2020 2020 2020 2020 2020 2020  up,.            
+0000dd00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000dd20: 7475 726e 205b 5d0a 0a20 2020 2020 2020  turn []..       
+0000dd30: 2020 2020 2020 2020 2072 656d 6169 6e69           remaini
+0000dd40: 6e67 5f65 6c65 6d65 6e74 7320 2d3d 2065  ng_elements -= e
+0000dd50: 6c65 6d65 6e74 735f 696e 5f67 726f 7570  lements_in_group
+0000dd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd70: 2066 6972 7374 5f65 6c65 6d65 6e74 5f69   first_element_i
+0000dd80: 6e5f 6772 6f75 7020 2b3d 2066 6972 7374  n_group += first
+0000dd90: 5f65 6c65 6d65 6e74 5f69 6e5f 6772 6f75  _element_in_grou
+0000dda0: 7020 2b20 656c 656d 656e 7473 5f69 6e5f  p + elements_in_
+0000ddb0: 6772 6f75 700a 0a20 2020 2020 2020 2020  group..         
+0000ddc0: 2020 206c 6f67 6769 6e67 2e64 6562 7567     logging.debug
+0000ddd0: 2822 7265 6164 2061 2074 6f74 616c 206f  ("read a total o
+0000dde0: 6620 2564 2076 616c 7565 2873 2922 2c20  f %d value(s)", 
+0000ddf0: 6c65 6e28 706c 635f 7661 6c75 6573 2929  len(plc_values))
+0000de00: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0000de10: 706c 635f 7661 6c75 6573 2920 213d 206e  plc_values) != n
+0000de20: 756d 6265 725f 6f66 5f65 6c65 6d65 6e74  umber_of_element
+0000de30: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+0000de40: 6169 7365 204c 5356 3244 6174 6145 7863  aise LSV2DataExc
+0000de50: 6570 7469 6f6e 280a 2020 2020 2020 2020  eption(.        
+0000de60: 2020 2020 2020 2020 226e 756d 6265 7220          "number 
+0000de70: 6f66 2072 6563 6569 7665 6420 7661 6c75  of received valu
+0000de80: 6573 2025 6420 6973 206e 6f74 2065 7175  es %d is not equ
+0000de90: 616c 2074 6f20 6e75 6d62 6572 206f 6620  al to number of 
+0000dea0: 7265 7175 6573 7465 6420 2564 220a 2020  requested %d".  
+0000deb0: 2020 2020 2020 2020 2020 2020 2020 2520                % 
+0000dec0: 286c 656e 2870 6c63 5f76 616c 7565 7329  (len(plc_values)
+0000ded0: 2c20 6e75 6d62 6572 5f6f 665f 656c 656d  , number_of_elem
+0000dee0: 656e 7473 290a 2020 2020 2020 2020 2020  ents).          
+0000def0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0000df00: 726e 2070 6c63 5f76 616c 7565 730a 0a20  rn plc_values.. 
+0000df10: 2020 2064 6566 2073 6574 5f6b 6579 626f     def set_keybo
+0000df20: 6172 645f 6163 6365 7373 2873 656c 662c  ard_access(self,
+0000df30: 2075 6e6c 6f63 6b65 643a 2062 6f6f 6c29   unlocked: bool)
+0000df40: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+0000df50: 2020 2222 220a 2020 2020 2020 2020 456e    """.        En
+0000df60: 6162 6c65 206f 7220 6469 7361 626c 6520  able or disable 
+0000df70: 7468 6520 6b65 7962 6f61 7264 206f 6e20  the keyboard on 
+0000df80: 7468 6520 636f 6e74 726f 6c2e 0a20 2020  the control..   
+0000df90: 2020 2020 2052 6571 7569 7265 7320 6163       Requires ac
+0000dfa0: 6365 7373 206c 6576 656c 2060 604d 4f4e  cess level ``MON
+0000dfb0: 4954 4f52 6060 2074 6f20 776f 726b 2e0a  ITOR`` to work..
+0000dfc0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+0000dfd0: 6060 5472 7565 6060 2069 6620 636f 6d70  ``True`` if comp
+0000dfe0: 6c65 7465 6420 7375 6363 6573 7366 756c  leted successful
+0000dff0: 6c79 2e0a 0a20 2020 2020 2020 203a 7061  ly...        :pa
+0000e000: 7261 6d20 756e 6c6f 636b 6564 3a20 6966  ram unlocked: if
+0000e010: 2060 6054 7275 6560 6020 756e 6c6f 636b   ``True`` unlock
+0000e020: 7320 7468 6520 6b65 7962 6f61 7264 2073  s the keyboard s
+0000e030: 6f20 6974 2063 616e 2062 6520 7573 6564  o it can be used
+0000e040: 2e20 4966 2060 6046 616c 7365 6060 2c20  . If ``False``, 
+0000e050: 696e 7075 7420 6973 2073 6574 2074 6f20  input is set to 
+0000e060: 6c6f 636b 6564 0a20 2020 2020 2020 2022  locked.        "
+0000e070: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+0000e080: 6c66 2e76 6572 7369 6f6e 732e 6973 5f74  lf.versions.is_t
+0000e090: 6e63 3728 293a 0a20 2020 2020 2020 2020  nc7():.         
+0000e0a0: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0000e0b0: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+0000e0c0: 2020 2020 2020 2020 2022 7468 6973 2066           "this f
+0000e0d0: 756e 6374 696f 6e20 6d69 6768 7420 6e6f  unction might no
+0000e0e0: 7420 6265 2073 7570 706f 7274 6564 206f  t be supported o
+0000e0f0: 6e20 544e 4337 2229 0a0a 2020 2020 2020  n TNC7")..      
+0000e100: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
+0000e110: 6769 6e28 6c63 2e4c 6f67 696e 2e4d 4f4e  gin(lc.Login.MON
+0000e120: 4954 4f52 293a 0a20 2020 2020 2020 2020  ITOR):.         
+0000e130: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0000e140: 7761 726e 696e 6728 2263 6c6f 756c 6420  warning("clould 
+0000e150: 6e6f 7420 6c6f 6720 696e 2061 7320 7573  not log in as us
+0000e160: 6572 204d 4f4e 4954 4f52 2229 0a20 2020  er MONITOR").   
+0000e170: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e180: 4661 6c73 650a 0a20 2020 2020 2020 2070  False..        p
+0000e190: 6179 6c6f 6164 203d 2062 7974 6561 7272  ayload = bytearr
+0000e1a0: 6179 2829 0a20 2020 2020 2020 2069 6620  ay().        if 
+0000e1b0: 756e 6c6f 636b 6564 3a0a 2020 2020 2020  unlocked:.      
+0000e1c0: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
+0000e1d0: 7465 6e64 2873 7472 7563 742e 7061 636b  tend(struct.pack
+0000e1e0: 2822 2142 222c 2030 7830 3029 290a 2020  ("!B", 0x00)).  
+0000e1f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000e200: 2020 2020 2020 2020 7061 796c 6f61 642e          payload.
+0000e210: 6578 7465 6e64 2873 7472 7563 742e 7061  extend(struct.pa
+0000e220: 636b 2822 2142 222c 2030 7830 3129 290a  ck("!B", 0x01)).
+0000e230: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000e240: 3d20 7365 6c66 2e5f 7365 6e64 5f72 6563  = self._send_rec
+0000e250: 6976 6528 6c63 2e43 4d44 2e43 5f4c 4b2c  ive(lc.CMD.C_LK,
+0000e260: 2070 6179 6c6f 6164 2c20 6c63 2e52 5350   payload, lc.RSP
+0000e270: 2e54 5f4f 4b29 0a20 2020 2020 2020 2069  .T_OK).        i
+0000e280: 6620 7265 7375 6c74 3a0a 2020 2020 2020  f result:.      
+0000e290: 2020 2020 2020 6966 2075 6e6c 6f63 6b65        if unlocke
+0000e2a0: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+0000e2b0: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0000e2c0: 6465 6275 6728 2263 6f6d 6d61 6e64 2074  debug("command t
+0000e2d0: 6f20 756e 6c6f 636b 206b 6579 626f 6172  o unlock keyboar
+0000e2e0: 6420 7761 7320 7375 6363 6573 7366 756c  d was successful
+0000e2f0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+0000e300: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000e310: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+0000e320: 722e 6465 6275 6728 2263 6f6d 6d61 6e64  r.debug("command
+0000e330: 2074 6f20 6c6f 636b 206b 6579 626f 6172   to lock keyboar
+0000e340: 6420 7761 7320 7375 6363 6573 7366 756c  d was successful
+0000e350: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+0000e360: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+0000e370: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0000e380: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+0000e390: 2020 2020 2022 616e 2065 7272 6f72 206f       "an error o
+0000e3a0: 6363 7572 7265 6420 6368 616e 6769 6e67  ccurred changing
+0000e3b0: 2074 6865 2073 7461 7465 206f 6620 7468   the state of th
+0000e3c0: 6520 6b65 7962 6f61 7264 206c 6f63 6b22  e keyboard lock"
+0000e3d0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000e3e0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0000e3f0: 0a20 2020 2064 6566 2067 6574 5f6d 6163  .    def get_mac
+0000e400: 6869 6e65 5f70 6172 616d 6574 6572 2873  hine_parameter(s
+0000e410: 656c 662c 206e 616d 653a 2073 7472 2920  elf, name: str) 
+0000e420: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+0000e430: 2222 220a 2020 2020 2020 2020 5265 6164  """.        Read
+0000e440: 206d 6163 6869 6e65 2070 6172 616d 6574   machine paramet
+0000e450: 6572 2066 726f 6d20 636f 6e74 726f 6c2e  er from control.
+0000e460: 0a20 2020 2020 2020 2052 6571 7569 7265  .        Require
+0000e470: 7320 6163 6365 7373 206c 6576 656c 2060  s access level `
+0000e480: 6049 4e53 5045 4354 6060 206c 6576 656c  `INSPECT`` level
+0000e490: 2074 6f20 776f 726b 2e0a 0a20 2020 2020   to work...     
+0000e4a0: 2020 203a 7061 7261 6d20 6e61 6d65 3a20     :param name: 
+0000e4b0: 6e61 6d65 206f 6620 7468 6520 6d61 6368  name of the mach
+0000e4c0: 696e 6520 7061 7261 6d65 7465 722e 0a20  ine parameter.. 
+0000e4d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000e4e0: 2020 2069 6620 6e6f 7420 7365 6c66 2e6c     if not self.l
+0000e4f0: 6f67 696e 286c 632e 4c6f 6769 6e2e 494e  ogin(lc.Login.IN
+0000e500: 5350 4543 5429 3a0a 2020 2020 2020 2020  SPECT):.        
+0000e510: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+0000e520: 2e77 6172 6e69 6e67 2822 636c 6f75 6c64  .warning("clould
+0000e530: 206e 6f74 206c 6f67 2069 6e20 6173 2075   not log in as u
+0000e540: 7365 7220 494e 5350 4543 5422 290a 2020  ser INSPECT").  
+0000e550: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e560: 2022 220a 0a20 2020 2020 2020 2069 6620   ""..        if 
+0000e570: 6973 696e 7374 616e 6365 286e 616d 652c  isinstance(name,
+0000e580: 2028 696e 742c 2929 3a0a 2020 2020 2020   (int,)):.      
+0000e590: 2020 2020 2020 6e61 6d65 203d 2073 7472        name = str
+0000e5a0: 286e 616d 6529 0a0a 2020 2020 2020 2020  (name)..        
+0000e5b0: 7061 796c 6f61 6420 3d20 6c6d 2e75 7374  payload = lm.ust
+0000e5c0: 725f 746f 5f62 6128 6e61 6d65 290a 0a20  r_to_ba(name).. 
+0000e5d0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000e5e0: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
+0000e5f0: 6528 6c63 2e43 4d44 2e52 5f4d 432c 2070  e(lc.CMD.R_MC, p
+0000e600: 6179 6c6f 6164 2c20 6c63 2e52 5350 2e53  ayload, lc.RSP.S
+0000e610: 5f4d 4329 0a20 2020 2020 2020 2069 6620  _MC).        if 
+0000e620: 6973 696e 7374 616e 6365 2872 6573 756c  isinstance(resul
+0000e630: 742c 2028 6279 7465 6172 7261 792c 2929  t, (bytearray,))
+0000e640: 2061 6e64 206c 656e 2872 6573 756c 7429   and len(result)
+0000e650: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+0000e660: 2020 7661 6c75 6520 3d20 6c6d 2e62 615f    value = lm.ba_
+0000e670: 746f 5f75 7374 7228 7265 7375 6c74 290a  to_ustr(result).
+0000e680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e690: 2e5f 6c6f 6767 6572 2e64 6562 7567 280a  ._logger.debug(.
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6b0: 226d 6163 6869 6e65 2070 6172 616d 6574  "machine paramet
+0000e6c0: 6572 2025 7320 6861 7320 7661 6c75 6520  er %s has value 
+0000e6d0: 2573 222c 206e 616d 652c 2076 616c 7565  %s", name, value
+0000e6e0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000e6f0: 7475 726e 2076 616c 7565 0a0a 2020 2020  turn value..    
+0000e700: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+0000e710: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+0000e720: 2020 2020 2020 2261 6e20 6572 726f 7220        "an error 
+0000e730: 6f63 6375 7272 6564 2077 6869 6c65 2072  occurred while r
+0000e740: 6561 6469 6e67 206d 6163 6869 6e65 2070  eading machine p
+0000e750: 6172 616d 6574 6572 2025 7322 2c20 6e61  arameter %s", na
+0000e760: 6d65 0a20 2020 2020 2020 2029 0a20 2020  me.        ).   
+0000e770: 2020 2020 2072 6574 7572 6e20 2222 0a0a       return ""..
+0000e780: 2020 2020 6465 6620 7365 745f 6d61 6368      def set_mach
+0000e790: 696e 655f 7061 7261 6d65 7465 7228 0a20  ine_parameter(. 
+0000e7a0: 2020 2020 2020 2073 656c 662c 206e 616d         self, nam
+0000e7b0: 653a 2073 7472 2c20 7661 6c75 653a 2073  e: str, value: s
+0000e7c0: 7472 2c20 7361 6665 5f74 6f5f 6469 736b  tr, safe_to_disk
+0000e7d0: 3a20 626f 6f6c 203d 2046 616c 7365 0a20  : bool = False. 
+0000e7e0: 2020 2029 202d 3e20 626f 6f6c 3a0a 2020     ) -> bool:.  
+0000e7f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e800: 2020 5365 7420 6d61 6368 696e 6520 7061    Set machine pa
+0000e810: 7261 6d65 7465 7220 6f6e 2063 6f6e 7472  rameter on contr
+0000e820: 6f6c 2e20 5772 6974 696e 6720 6120 7061  ol. Writing a pa
+0000e830: 7261 6d65 7465 7220 7461 6b65 7320 736f  rameter takes so
+0000e840: 6d65 2074 696d 652c 206d 616b 6520 7375  me time, make su
+0000e850: 7265 2074 6f20 7365 7420 7469 6d65 6f75  re to set timeou
+0000e860: 740a 2020 2020 2020 2020 7375 6666 6963  t.        suffic
+0000e870: 6965 6e74 6c79 2068 6967 6821 0a20 2020  iently high!.   
+0000e880: 2020 2020 2052 6571 7569 7265 7320 6163       Requires ac
+0000e890: 6365 7373 2060 6050 4c43 4445 4255 4760  cess ``PLCDEBUG`
+0000e8a0: 6020 6c65 7665 6c20 746f 2077 6f72 6b2e  ` level to work.
+0000e8b0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000e8c0: 2060 6054 7275 6560 6020 6966 2063 6f6d   ``True`` if com
+0000e8d0: 706c 6574 6564 2073 7563 6365 7373 6675  pleted successfu
+0000e8e0: 6c6c 792e 0a0a 2020 2020 2020 2020 3a70  lly...        :p
+0000e8f0: 6172 616d 206e 616d 653a 206e 616d 6520  aram name: name 
+0000e900: 6f66 2074 6865 206d 6163 6869 6e65 2070  of the machine p
+0000e910: 6172 616d 6574 6572 2e20 466f 7220 6954  arameter. For iT
+0000e920: 4e43 2074 6865 2070 6172 616d 6574 6572  NC the parameter
+0000e930: 206e 756d 6265 7220 6861 7365 2074 6f20   number hase to 
+0000e940: 6265 2063 6f6e 7665 7274 6564 2074 6f20  be converted to 
+0000e950: 7374 7269 6e67 0a20 2020 2020 2020 203a  string.        :
+0000e960: 7061 7261 6d20 7661 6c75 653a 206e 6577  param value: new
+0000e970: 2076 616c 7565 206f 6620 7468 6520 6d61   value of the ma
+0000e980: 6368 696e 6520 7061 7261 6d65 7465 722e  chine parameter.
+0000e990: 2054 6865 7265 2069 7320 6e6f 2074 7970   There is no typ
+0000e9a0: 6520 6368 6563 6b69 6e67 2c20 6966 2074  e checking, if t
+0000e9b0: 6865 2076 616c 7565 2063 616e 206e 6f74  he value can not
+0000e9c0: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+0000e9d0: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
+0000e9e0: 6572 7465 6420 6279 2074 6865 2063 6f6e  erted by the con
+0000e9f0: 7472 6f6c 2061 6e20 6572 726f 7220 7769  trol an error wi
+0000ea00: 6c6c 2062 6520 7365 6e74 2e0a 2020 2020  ll be sent..    
+0000ea10: 2020 2020 3a70 6172 616d 2073 6166 655f      :param safe_
+0000ea20: 746f 5f64 6973 6b3a 2049 6620 5472 7565  to_disk: If True
+0000ea30: 2074 6865 206e 6577 2076 616c 7565 2077   the new value w
+0000ea40: 696c 6c20 6265 2077 7269 7474 656e 2074  ill be written t
+0000ea50: 6f20 7468 6520 6861 7264 6469 736b 2061  o the harddisk a
+0000ea60: 6e64 2073 7461 7920 7065 726d 616e 656e  nd stay permanen
+0000ea70: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
+0000ea80: 2020 2020 2020 2020 2020 2049 6620 4661             If Fa
+0000ea90: 6c73 6520 2864 6566 6175 6c74 2920 7468  lse (default) th
+0000eaa0: 6520 7661 6c75 6520 7769 6c6c 206f 6e6c  e value will onl
+0000eab0: 7920 6265 2061 7661 696c 6162 6c65 2075  y be available u
+0000eac0: 6e74 696c 2074 6865 206e 6578 7420 7265  ntil the next re
+0000ead0: 626f 6f74 2e0a 2020 2020 2020 2020 2222  boot..        ""
+0000eae0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000eaf0: 2073 656c 662e 6c6f 6769 6e28 6c63 2e4c   self.login(lc.L
+0000eb00: 6f67 696e 2e50 4c43 4445 4255 4729 3a0a  ogin.PLCDEBUG):.
+0000eb10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000eb20: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
+0000eb30: 2822 636c 6f75 6c64 206e 6f74 206c 6f67  ("clould not log
+0000eb40: 2069 6e20 6173 2075 7365 7220 504c 4344   in as user PLCD
+0000eb50: 4542 5547 2229 0a20 2020 2020 2020 2020  EBUG").         
+0000eb60: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0000eb70: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+0000eb80: 203d 2062 7974 6561 7272 6179 2829 0a20   = bytearray(). 
+0000eb90: 2020 2020 2020 2069 6620 7361 6665 5f74         if safe_t
+0000eba0: 6f5f 6469 736b 3a0a 2020 2020 2020 2020  o_disk:.        
+0000ebb0: 2020 2020 7061 796c 6f61 642e 6578 7465      payload.exte
+0000ebc0: 6e64 2873 7472 7563 742e 7061 636b 2822  nd(struct.pack("
+0000ebd0: 214c 222c 2030 7830 3029 290a 2020 2020  !L", 0x00)).    
+0000ebe0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ebf0: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
+0000ec00: 7465 6e64 2873 7472 7563 742e 7061 636b  tend(struct.pack
+0000ec10: 2822 214c 222c 2030 7830 3129 290a 2020  ("!L", 0x01)).  
+0000ec20: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
+0000ec30: 7465 6e64 286c 6d2e 7573 7472 5f74 6f5f  tend(lm.ustr_to_
+0000ec40: 6261 286e 616d 6529 290a 2020 2020 2020  ba(name)).      
+0000ec50: 2020 7061 796c 6f61 642e 6578 7465 6e64    payload.extend
+0000ec60: 286c 6d2e 7573 7472 5f74 6f5f 6261 2876  (lm.ustr_to_ba(v
+0000ec70: 616c 7565 2929 0a0a 2020 2020 2020 2020  alue))..        
+0000ec80: 7265 7375 6c74 203d 2073 656c 662e 5f73  result = self._s
+0000ec90: 656e 645f 7265 6369 7665 286c 632e 434d  end_recive(lc.CM
+0000eca0: 442e 435f 4d43 2c20 7061 796c 6f61 642c  D.C_MC, payload,
+0000ecb0: 206c 632e 5253 502e 545f 4f4b 290a 2020   lc.RSP.T_OK).  
+0000ecc0: 2020 2020 2020 6966 2072 6573 756c 743a        if result:
+0000ecd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ece0: 662e 5f6c 6f67 6765 722e 6465 6275 6728  f._logger.debug(
+0000ecf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ed00: 2022 7365 7474 696e 6720 6f66 206d 6163   "setting of mac
+0000ed10: 6869 6e65 2070 6172 616d 6574 6572 2025  hine parameter %
+0000ed20: 7320 746f 2076 616c 7565 2025 7320 7761  s to value %s wa
+0000ed30: 7320 7375 6363 6573 7366 756c 222c 0a20  s successful",. 
+0000ed40: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000ed50: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0000ed60: 2020 2020 2076 616c 7565 2c0a 2020 2020       value,.    
+0000ed70: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000ed80: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000ed90: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+0000eda0: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
+0000edb0: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
+0000edc0: 2065 7272 6f72 206f 6363 7572 7265 6420   error occurred 
+0000edd0: 7768 696c 6520 7365 7474 696e 6720 6d61  while setting ma
+0000ede0: 6368 696e 6520 7061 7261 6d65 7465 7220  chine parameter 
+0000edf0: 2573 2074 6f20 7661 6c75 6520 2573 222c  %s to value %s",
+0000ee00: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+0000ee10: 652c 0a20 2020 2020 2020 2020 2020 2076  e,.            v
+0000ee20: 616c 7565 2c0a 2020 2020 2020 2020 290a  alue,.        ).
+0000ee30: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0000ee40: 616c 7365 0a0a 2020 2020 6465 6620 7365  alse..    def se
+0000ee50: 6e64 5f6b 6579 5f63 6f64 6528 7365 6c66  nd_key_code(self
+0000ee60: 2c20 6b65 795f 636f 6465 3a20 556e 696f  , key_code: Unio
+0000ee70: 6e5b 6c63 2e4b 6579 436f 6465 2c20 6c63  n[lc.KeyCode, lc
+0000ee80: 2e4f 6c64 4b65 7943 6f64 655d 2920 2d3e  .OldKeyCode]) ->
+0000ee90: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+0000eea0: 2222 0a20 2020 2020 2020 2053 656e 6420  "".        Send 
+0000eeb0: 6b65 7920 636f 6465 2074 6f20 636f 6e74  key code to cont
+0000eec0: 726f 6c2e 2042 6568 6176 6573 2061 7320  rol. Behaves as 
+0000eed0: 6966 2074 6865 2061 7373 6f63 6961 7465  if the associate
+0000eee0: 6420 6b65 7920 7761 7320 7072 6573 7365  d key was presse
+0000eef0: 6420 6f6e 2074 6865 206b 6579 626f 6172  d on the keyboar
+0000ef00: 642e 0a20 2020 2020 2020 2052 6571 7569  d..        Requi
+0000ef10: 7265 7320 6163 6365 7373 2060 604d 4f4e  res access ``MON
+0000ef20: 4954 4f52 6060 206c 6576 656c 2074 6f20  ITOR`` level to 
+0000ef30: 776f 726b 2e0a 2020 2020 2020 2020 546f  work..        To
+0000ef40: 2077 6f72 6b20 636f 7272 6563 746c 7920   work correctly 
+0000ef50: 796f 7520 6669 7273 7420 6861 7665 2074  you first have t
+0000ef60: 6f20 6c6f 636b 2074 6865 206b 6579 626f  o lock the keybo
+0000ef70: 6172 6420 616e 6420 756e 6c6f 636b 2069  ard and unlock i
+0000ef80: 7420 6166 7465 7277 6172 6473 213a 0a0a  t afterwards!:..
+0000ef90: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+0000efa0: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+0000efb0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+0000efc0: 6b65 7962 6f61 7264 5f61 6363 6573 7328  keyboard_access(
+0000efd0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+0000efe0: 2020 2073 656e 645f 6b65 795f 636f 6465     send_key_code
+0000eff0: 284b 6579 436f 6465 2e43 4529 0a20 2020  (KeyCode.CE).   
+0000f000: 2020 2020 2020 2020 2073 6574 5f6b 6579           set_key
+0000f010: 626f 6172 645f 6163 6365 7373 2854 7275  board_access(Tru
+0000f020: 6529 0a0a 2020 2020 2020 2020 5265 7475  e)..        Retu
+0000f030: 726e 7320 6060 5472 7565 6060 2069 6620  rns ``True`` if 
+0000f040: 636f 6d70 6c65 7465 6420 7375 6363 6573  completed succes
+0000f050: 7366 756c 6c79 2e0a 0a20 2020 2020 2020  sfully...       
+0000f060: 203a 7061 7261 6d20 6b65 795f 636f 6465   :param key_code
+0000f070: 3a20 636f 6465 206e 756d 6265 7220 6f66  : code number of
+0000f080: 2074 6865 206b 6579 626f 6172 6420 6b65   the keyboard ke
+0000f090: 790a 2020 2020 2020 2020 2222 220a 2020  y.        """.  
+0000f0a0: 2020 2020 2020 6966 2073 656c 662e 7665        if self.ve
+0000f0b0: 7273 696f 6e73 2e69 735f 746e 6337 2829  rsions.is_tnc7()
+0000f0c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f0d0: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
+0000f0e0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000f0f0: 2020 2020 2274 6869 7320 6675 6e63 7469      "this functi
+0000f100: 6f6e 206d 6967 6874 206e 6f74 2062 6520  on might not be 
+0000f110: 7375 7070 6f72 7465 6420 6f6e 2054 4e43  supported on TNC
+0000f120: 3722 290a 0a20 2020 2020 2020 2069 6620  7")..        if 
+0000f130: 6e6f 7420 7365 6c66 2e6c 6f67 696e 286c  not self.login(l
+0000f140: 632e 4c6f 6769 6e2e 4d4f 4e49 544f 5229  c.Login.MONITOR)
+0000f150: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f160: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
+0000f170: 6e67 2822 636c 6f75 6c64 206e 6f74 206c  ng("clould not l
+0000f180: 6f67 2069 6e20 6173 2075 7365 7220 4d4f  og in as user MO
+0000f190: 4e49 544f 5222 290a 2020 2020 2020 2020  NITOR").        
+0000f1a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0000f1b0: 0a0a 2020 2020 2020 2020 7061 796c 6f61  ..        payloa
+0000f1c0: 6420 3d20 6279 7465 6172 7261 7928 290a  d = bytearray().
+0000f1d0: 2020 2020 2020 2020 7061 796c 6f61 642e          payload.
+0000f1e0: 6578 7465 6e64 2873 7472 7563 742e 7061  extend(struct.pa
+0000f1f0: 636b 2822 2148 222c 206b 6579 5f63 6f64  ck("!H", key_cod
+0000f200: 6529 290a 0a20 2020 2020 2020 2072 6573  e))..        res
+0000f210: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
+0000f220: 5f72 6563 6976 6528 6c63 2e43 4d44 2e43  _recive(lc.CMD.C
+0000f230: 5f45 4b2c 2070 6179 6c6f 6164 2c20 6c63  _EK, payload, lc
+0000f240: 2e52 5350 2e54 5f4f 4b29 0a20 2020 2020  .RSP.T_OK).     
+0000f250: 2020 2069 6620 7265 7375 6c74 3a0a 2020     if result:.  
+0000f260: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000f270: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
+0000f280: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+0000f290: 656e 6469 6e67 2074 6865 206b 6579 2063  ending the key c
+0000f2a0: 6f64 6520 2564 2077 6173 2073 7563 6365  ode %d was succe
+0000f2b0: 7373 6675 6c22 2c20 6b65 795f 636f 6465  ssful", key_code
+0000f2c0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000f2d0: 7475 726e 2054 7275 650a 0a20 2020 2020  turn True..     
+0000f2e0: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0000f2f0: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+0000f300: 2020 2020 2022 616e 2065 7272 6f72 206f       "an error o
+0000f310: 6363 7572 7265 6420 7768 696c 6520 7365  ccurred while se
+0000f320: 6e64 696e 6720 7468 6520 6b65 7920 636f  nding the key co
+0000f330: 6465 2025 6422 2c20 6b65 795f 636f 6465  de %d", key_code
+0000f340: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000f350: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0000f360: 0a20 2020 2064 6566 2073 7069 6e64 6c65  .    def spindle
+0000f370: 5f74 6f6f 6c5f 7374 6174 7573 2873 656c  _tool_status(sel
+0000f380: 6629 202d 3e20 556e 696f 6e5b 6c64 2e54  f) -> Union[ld.T
+0000f390: 6f6f 6c49 6e66 6f72 6d61 7469 6f6e 2c20  oolInformation, 
+0000f3a0: 4e6f 6e65 5d3a 0a20 2020 2020 2020 2022  None]:.        "
+0000f3b0: 2222 0a20 2020 2020 2020 2047 6574 2069  "".        Get i
+0000f3c0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+0000f3d0: 2074 6865 2074 6f6f 6c20 6375 7272 656e   the tool curren
+0000f3e0: 746c 7920 696e 2074 6865 2073 7069 6e64  tly in the spind
+0000f3f0: 6c65 0a20 2020 2020 2020 2052 6571 7569  le.        Requi
+0000f400: 7265 7320 6163 6365 7373 206c 6576 656c  res access level
+0000f410: 2060 6044 4e43 6060 2074 6f20 776f 726b   ``DNC`` to work
+0000f420: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000f430: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0000f440: 662e 6c6f 6769 6e28 6c63 2e4c 6f67 696e  f.login(lc.Login
+0000f450: 2e44 4e43 293a 0a20 2020 2020 2020 2020  .DNC):.         
+0000f460: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0000f470: 7761 726e 696e 6728 2263 6c6f 756c 6420  warning("clould 
+0000f480: 6e6f 7420 6c6f 6720 696e 2061 7320 7573  not log in as us
+0000f490: 6572 2044 4e43 2229 0a20 2020 2020 2020  er DNC").       
+0000f4a0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+0000f4b0: 0a0a 2020 2020 2020 2020 7061 796c 6f61  ..        payloa
+0000f4c0: 6420 3d20 6279 7465 6172 7261 7928 290a  d = bytearray().
+0000f4d0: 2020 2020 2020 2020 7061 796c 6f61 642e          payload.
+0000f4e0: 6578 7465 6e64 2873 7472 7563 742e 7061  extend(struct.pa
+0000f4f0: 636b 2822 2148 222c 206c 632e 5061 7252  ck("!H", lc.ParR
+0000f500: 5249 2e43 5552 5245 4e54 5f54 4f4f 4c29  RI.CURRENT_TOOL)
+0000f510: 290a 0a20 2020 2020 2020 2072 6573 756c  )..        resul
+0000f520: 7420 3d20 7365 6c66 2e5f 7365 6e64 5f72  t = self._send_r
+0000f530: 6563 6976 6528 6c63 2e43 4d44 2e52 5f52  ecive(lc.CMD.R_R
+0000f540: 492c 2070 6179 6c6f 6164 2c20 6c63 2e52  I, payload, lc.R
+0000f550: 5350 2e53 5f52 4929 0a20 2020 2020 2020  SP.S_RI).       
+0000f560: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+0000f570: 6573 756c 742c 2028 6279 7465 6172 7261  esult, (bytearra
+0000f580: 792c 2929 2061 6e64 206c 656e 2872 6573  y,)) and len(res
+0000f590: 756c 7429 203e 2030 3a0a 2020 2020 2020  ult) > 0:.      
+0000f5a0: 2020 2020 2020 746f 6f6c 5f69 6e66 6f20        tool_info 
+0000f5b0: 3d20 6c6d 2e64 6563 6f64 655f 746f 6f6c  = lm.decode_tool
+0000f5c0: 5f69 6e66 6f28 7265 7375 6c74 290a 2020  _info(result).  
+0000f5d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000f5e0: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
+0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+0000f600: 7563 6365 7373 6675 6c6c 7920 7265 6164  uccessfully read
+0000f610: 2069 6e66 6f20 6f6e 2063 7572 7265 6e74   info on current
+0000f620: 2074 6f6f 6c3a 2025 7322 2c20 746f 6f6c   tool: %s", tool
+0000f630: 5f69 6e66 6f29 0a20 2020 2020 2020 2020  _info).         
+0000f640: 2020 2072 6574 7572 6e20 746f 6f6c 5f69     return tool_i
+0000f650: 6e66 6f0a 2020 2020 2020 2020 7365 6c66  nfo.        self
+0000f660: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
+0000f670: 280a 2020 2020 2020 2020 2020 2020 2261  (.            "a
+0000f680: 6e20 6572 726f 7220 6f63 6375 7272 6564  n error occurred
+0000f690: 2077 6869 6c65 2071 7565 7279 696e 6720   while querying 
+0000f6a0: 6375 7272 656e 7420 746f 6f6c 2069 6e66  current tool inf
+0000f6b0: 6f72 6d61 7469 6f6e 2e20 5468 6973 2064  ormation. This d
+0000f6c0: 6f65 7320 6e6f 7420 776f 726b 2066 6f72  oes not work for
+0000f6d0: 2061 6c6c 2063 6f6e 7472 6f6c 2074 7970   all control typ
+0000f6e0: 6573 220a 2020 2020 2020 2020 290a 2020  es".        ).  
+0000f6f0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+0000f700: 650a 0a20 2020 2064 6566 206f 7665 7272  e..    def overr
+0000f710: 6964 655f 7374 6174 6528 7365 6c66 2920  ide_state(self) 
+0000f720: 2d3e 2055 6e69 6f6e 5b6c 642e 4f76 6572  -> Union[ld.Over
+0000f730: 7269 6465 5374 6174 652c 204e 6f6e 655d  rideState, None]
+0000f740: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f750: 2020 2020 2020 4765 7420 696e 666f 726d        Get inform
+0000f760: 6174 696f 6e20 6162 6f75 7420 7468 6520  ation about the 
+0000f770: 6f76 6572 7269 6465 2069 6e66 6f2e 0a20  override info.. 
+0000f780: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
+0000f790: 6163 6365 7373 206c 6576 656c 2060 6044  access level ``D
+0000f7a0: 4e43 6060 2074 6f20 776f 726b 2e0a 2020  NC`` to work..  
+0000f7b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f7c0: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
+0000f7d0: 6769 6e28 6c63 2e4c 6f67 696e 2e44 4e43  gin(lc.Login.DNC
+0000f7e0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000f7f0: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
+0000f800: 696e 6728 2263 6c6f 756c 6420 6e6f 7420  ing("clould not 
+0000f810: 6c6f 6720 696e 2061 7320 7573 6572 2044  log in as user D
+0000f820: 4e43 2229 0a20 2020 2020 2020 2020 2020  NC").           
+0000f830: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+0000f840: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
+0000f850: 6279 7465 6172 7261 7928 290a 2020 2020  bytearray().    
+0000f860: 2020 2020 7061 796c 6f61 642e 6578 7465      payload.exte
+0000f870: 6e64 2873 7472 7563 742e 7061 636b 2822  nd(struct.pack("
+0000f880: 2148 222c 206c 632e 5061 7252 5249 2e4f  !H", lc.ParRRI.O
+0000f890: 5645 5252 4944 4529 290a 0a20 2020 2020  VERRIDE))..     
+0000f8a0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+0000f8b0: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
+0000f8c0: 2e43 4d44 2e52 5f52 492c 2070 6179 6c6f  .CMD.R_RI, paylo
+0000f8d0: 6164 2c20 6c63 2e52 5350 2e53 5f52 4929  ad, lc.RSP.S_RI)
+0000f8e0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+0000f8f0: 7374 616e 6365 2872 6573 756c 742c 2028  stance(result, (
+0000f900: 6279 7465 6172 7261 792c 2929 2061 6e64  bytearray,)) and
+0000f910: 206c 656e 2872 6573 756c 7429 203e 2030   len(result) > 0
+0000f920: 3a0a 2020 2020 2020 2020 2020 2020 6f76  :.            ov
+0000f930: 6572 7269 6465 5f69 6e66 6f20 3d20 6c6d  erride_info = lm
+0000f940: 2e64 6563 6f64 655f 6f76 6572 7269 6465  .decode_override
+0000f950: 5f73 7461 7465 2872 6573 756c 7429 0a20  _state(result). 
+0000f960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f970: 5f6c 6f67 6765 722e 6465 6275 6728 0a20  _logger.debug(. 
+0000f980: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000f990: 7375 6363 6573 7366 756c 6c79 2072 6561  successfully rea
+0000f9a0: 6420 6f76 6572 7269 6465 2069 6e66 6f3a  d override info:
+0000f9b0: 2025 7322 2c20 6f76 6572 7269 6465 5f69   %s", override_i
+0000f9c0: 6e66 6f29 0a20 2020 2020 2020 2020 2020  nfo).           
+0000f9d0: 2072 6574 7572 6e20 6f76 6572 7269 6465   return override
+0000f9e0: 5f69 6e66 6f0a 2020 2020 2020 2020 7365  _info.        se
+0000f9f0: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
+0000fa00: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000fa10: 2261 6e20 6572 726f 7220 6f63 6375 7272  "an error occurr
+0000fa20: 6564 2077 6869 6c65 2071 7565 7279 696e  ed while queryin
+0000fa30: 6720 6375 7272 656e 7420 6f76 6572 7269  g current overri
+0000fa40: 6465 2069 6e66 6f72 6d61 7469 6f6e 2e20  de information. 
+0000fa50: 5468 6973 2064 6f65 7320 6e6f 7420 776f  This does not wo
+0000fa60: 726b 2066 6f72 2061 6c6c 2063 6f6e 7472  rk for all contr
+0000fa70: 6f6c 2074 7970 6573 220a 2020 2020 2020  ol types".      
+0000fa80: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0000fa90: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
+0000faa0: 2067 6574 5f65 7272 6f72 5f6d 6573 7361   get_error_messa
+0000fab0: 6765 7328 7365 6c66 2920 2d3e 204c 6973  ges(self) -> Lis
+0000fac0: 745b 6c64 2e4e 4345 7272 6f72 4d65 7373  t[ld.NCErrorMess
+0000fad0: 6167 655d 3a0a 2020 2020 2020 2020 2222  age]:.        ""
+0000fae0: 220a 2020 2020 2020 2020 4765 7420 696e  ".        Get in
+0000faf0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+0000fb00: 7468 6520 6669 7273 7420 6f72 206e 6578  the first or nex
+0000fb10: 7420 6572 726f 7220 6469 7370 6c61 7965  t error displaye
+0000fb20: 6420 6f6e 2074 6865 2063 6f6e 7472 6f6c  d on the control
+0000fb30: 0a20 2020 2020 2020 2052 6571 7569 7265  .        Require
+0000fb40: 7320 6163 6365 7373 206c 6576 656c 2060  s access level `
+0000fb50: 6044 4e43 6060 2074 6f20 776f 726b 2e0a  `DNC`` to work..
+0000fb60: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+0000fb70: 6572 726f 7220 6c69 7374 206f 6620 6572  error list of er
+0000fb80: 726f 7220 6d65 7373 6167 6573 0a20 2020  ror messages.   
+0000fb90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000fba0: 206d 6573 7361 6765 7320 3d20 5b5d 0a20   messages = []. 
+0000fbb0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000fbc0: 6c66 2e6c 6f67 696e 286c 632e 4c6f 6769  lf.login(lc.Logi
+0000fbd0: 6e2e 444e 4329 3a0a 2020 2020 2020 2020  n.DNC):.        
+0000fbe0: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+0000fbf0: 2e77 6172 6e69 6e67 2822 636c 6f75 6c64  .warning("clould
+0000fc00: 206e 6f74 206c 6f67 2069 6e20 6173 2075   not log in as u
+0000fc10: 7365 7220 444e 4322 290a 2020 2020 2020  ser DNC").      
+0000fc20: 2020 2020 2020 7265 7475 726e 205b 5d0a        return [].
+0000fc30: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+0000fc40: 203d 2062 7974 6561 7272 6179 2829 0a20   = bytearray(). 
+0000fc50: 2020 2020 2020 2070 6179 6c6f 6164 2e65         payload.e
+0000fc60: 7874 656e 6428 7374 7275 6374 2e70 6163  xtend(struct.pac
+0000fc70: 6b28 2221 4822 2c20 6c63 2e50 6172 5252  k("!H", lc.ParRR
+0000fc80: 492e 4649 5253 545f 4552 524f 5229 290a  I.FIRST_ERROR)).
+0000fc90: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000fca0: 3d20 7365 6c66 2e5f 7365 6e64 5f72 6563  = self._send_rec
+0000fcb0: 6976 6528 6c63 2e43 4d44 2e52 5f52 492c  ive(lc.CMD.R_RI,
+0000fcc0: 2070 6179 6c6f 6164 2c20 6c63 2e52 5350   payload, lc.RSP
+0000fcd0: 2e53 5f52 4929 0a20 2020 2020 2020 2069  .S_RI).        i
+0000fce0: 6620 6973 696e 7374 616e 6365 2872 6573  f isinstance(res
+0000fcf0: 756c 742c 2028 6279 7465 6172 7261 792c  ult, (bytearray,
+0000fd00: 2929 2061 6e64 206c 656e 2872 6573 756c  )) and len(resul
+0000fd10: 7429 203e 2030 3a0a 2020 2020 2020 2020  t) > 0:.        
+0000fd20: 2020 2020 6d65 7373 6167 6573 2e61 7070      messages.app
+0000fd30: 656e 6428 6c6d 2e64 6563 6f64 655f 6572  end(lm.decode_er
+0000fd40: 726f 725f 6d65 7373 6167 6528 7265 7375  ror_message(resu
+0000fd50: 6c74 2929 0a20 2020 2020 2020 2020 2020  lt)).           
+0000fd60: 2070 6179 6c6f 6164 203d 2062 7974 6561   payload = bytea
+0000fd70: 7272 6179 2829 0a20 2020 2020 2020 2020  rray().         
+0000fd80: 2020 2070 6179 6c6f 6164 2e65 7874 656e     payload.exten
+0000fd90: 6428 7374 7275 6374 2e70 6163 6b28 2221  d(struct.pack("!
+0000fda0: 4822 2c20 6c63 2e50 6172 5252 492e 4e45  H", lc.ParRRI.NE
+0000fdb0: 5854 5f45 5252 4f52 2929 0a20 2020 2020  XT_ERROR)).     
+0000fdc0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000fdd0: 7365 6c66 2e5f 7365 6e64 5f72 6563 6976  self._send_reciv
+0000fde0: 6528 6c63 2e43 4d44 2e52 5f52 492c 2070  e(lc.CMD.R_RI, p
+0000fdf0: 6179 6c6f 6164 2c20 6c63 2e52 5350 2e53  ayload, lc.RSP.S
+0000fe00: 5f52 4929 0a20 2020 2020 2020 2020 2020  _RI).           
+0000fe10: 2073 656c 662e 5f6c 6f67 6765 722e 6465   self._logger.de
+0000fe20: 6275 6728 0a20 2020 2020 2020 2020 2020  bug(.           
+0000fe30: 2020 2020 2022 7375 6363 6573 7366 756c       "successful
+0000fe40: 6c79 2072 6561 6420 6669 7273 7420 6572  ly read first er
+0000fe50: 726f 7220 6275 7420 6675 7274 6865 7220  ror but further 
+0000fe60: 6572 726f 7273 2229 0a0a 2020 2020 2020  errors")..      
+0000fe70: 2020 2020 2020 7768 696c 6520 6973 696e        while isin
+0000fe80: 7374 616e 6365 2872 6573 756c 742c 2028  stance(result, (
+0000fe90: 6279 7465 6172 7261 792c 2929 3a0a 2020  bytearray,)):.  
+0000fea0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000feb0: 7373 6167 6573 2e61 7070 656e 6428 6c6d  ssages.append(lm
+0000fec0: 2e64 6563 6f64 655f 6572 726f 725f 6d65  .decode_error_me
+0000fed0: 7373 6167 6528 7265 7375 6c74 2929 0a20  ssage(result)). 
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000fef0: 6573 756c 7420 3d20 7365 6c66 2e5f 7365  esult = self._se
+0000ff00: 6e64 5f72 6563 6976 6528 6c63 2e43 4d44  nd_recive(lc.CMD
+0000ff10: 2e52 5f52 492c 2070 6179 6c6f 6164 2c20  .R_RI, payload, 
+0000ff20: 6c63 2e52 5350 2e53 5f52 4929 0a0a 2020  lc.RSP.S_RI)..  
+0000ff30: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000ff40: 662e 6c61 7374 5f65 7272 6f72 2069 7320  f.last_error is 
+0000ff50: 6c63 2e4c 5356 3253 7461 7475 7343 6f64  lc.LSV2StatusCod
+0000ff60: 652e 545f 4552 5f4e 4f5f 4e45 5854 5f45  e.T_ER_NO_NEXT_E
+0000ff70: 5252 4f52 3a0a 2020 2020 2020 2020 2020  RROR:.          
+0000ff80: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+0000ff90: 6572 2e64 6562 7567 2822 7375 6363 6573  er.debug("succes
+0000ffa0: 7366 756c 6c79 2072 6561 6420 616c 6c20  sfully read all 
+0000ffb0: 6572 726f 7273 2229 0a20 2020 2020 2020  errors").       
+0000ffc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000ffd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ffe0: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
+0000fff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010000: 2020 2020 2022 616e 2065 7272 6f72 206f       "an error o
+00010010: 6363 7572 7265 6420 7768 696c 6520 7175  ccurred while qu
+00010020: 6572 7969 6e67 2065 7272 6f72 2069 6e66  erying error inf
+00010030: 6f72 6d61 7469 6f6e 2e22 0a20 2020 2020  ormation.".     
+00010040: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00010050: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010060: 206d 6573 7361 6765 730a 0a20 2020 2020   messages..     
+00010070: 2020 2069 6620 7365 6c66 2e6c 6173 745f     if self.last_
+00010080: 6572 726f 7220 6973 206c 632e 4c53 5632  error is lc.LSV2
+00010090: 5374 6174 7573 436f 6465 2e54 5f45 525f  StatusCode.T_ER_
+000100a0: 4e4f 5f4e 4558 545f 4552 524f 523a 0a20  NO_NEXT_ERROR:. 
+000100b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000100c0: 5f6c 6f67 6765 722e 6465 6275 6728 0a20  _logger.debug(. 
+000100d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000100e0: 7375 6363 6573 7366 756c 6c79 2072 6561  successfully rea
+000100f0: 6420 6669 7273 7420 6572 726f 7220 6275  d first error bu
+00010100: 7420 6e6f 2065 7272 6f72 2061 6374 6976  t no error activ
+00010110: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
+00010120: 7265 7475 726e 206d 6573 7361 6765 730a  return messages.
+00010130: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
+00010140: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
+00010150: 2020 2020 2020 2020 2020 2022 616e 2065             "an e
+00010160: 7272 6f72 206f 6363 7572 7265 6420 7768  rror occurred wh
+00010170: 696c 6520 7175 6572 7969 6e67 2065 7272  ile querying err
+00010180: 6f72 2069 6e66 6f72 6d61 7469 6f6e 2e20  or information. 
+00010190: 5468 6973 2064 6f65 7320 6e6f 7420 776f  This does not wo
+000101a0: 726b 2066 6f72 2061 6c6c 2063 6f6e 7472  rk for all contr
+000101b0: 6f6c 2074 7970 6573 220a 2020 2020 2020  ol types".      
+000101c0: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+000101d0: 7572 6e20 5b5d 0a0a 2020 2020 6465 6620  urn []..    def 
+000101e0: 5f77 616c 6b5f 6469 7228 7365 6c66 2c20  _walk_dir(self, 
+000101f0: 6465 7363 656e 643a 2062 6f6f 6c20 3d20  descend: bool = 
+00010200: 5472 7565 2920 2d3e 204c 6973 745b 7374  True) -> List[st
+00010210: 725d 3a0a 2020 2020 2020 2020 2222 220a  r]:.        """.
+00010220: 2020 2020 2020 2020 6865 6c70 6572 2066          helper f
+00010230: 756e 6374 696f 6e20 746f 2072 6563 7572  unction to recur
+00010240: 7369 7665 6c79 2073 6561 7263 6820 696e  sively search in
+00010250: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
+00010260: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
+00010270: 5265 7175 6972 6573 2061 6363 6573 7320  Requires access 
+00010280: 6c65 7665 6c20 6060 4649 4c45 5452 414e  level ``FILETRAN
+00010290: 5346 4552 6060 2074 6f20 776f 726b 2e0a  SFER`` to work..
+000102a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000102b0: 6465 7363 656e 643a 2063 6f6e 7472 6f6c  descend: control
+000102c0: 2069 6620 7365 6172 6368 2073 686f 756c   if search shoul
+000102d0: 6420 7275 6e20 7265 6375 7273 6976 656c  d run recursivel
+000102e0: 790a 2020 2020 2020 2020 2222 220a 2020  y.        """.  
+000102f0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00010300: 662e 6c6f 6769 6e28 6c63 2e4c 6f67 696e  f.login(lc.Login
+00010310: 2e46 494c 4554 5241 4e53 4645 5229 3a0a  .FILETRANSFER):.
+00010320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010330: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
+00010340: 2822 636c 6f75 6c64 206e 6f74 206c 6f67  ("clould not log
+00010350: 2069 6e20 6173 2075 7365 7220 4649 4c45   in as user FILE
+00010360: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00010370: 6574 7572 6e20 5b5d 0a0a 2020 2020 2020  eturn []..      
+00010380: 2020 6375 7272 656e 745f 7061 7468 203d    current_path =
+00010390: 2073 656c 662e 6469 7265 6374 6f72 795f   self.directory_
+000103a0: 696e 666f 2829 2e70 6174 680a 2020 2020  info().path.    
+000103b0: 2020 2020 636f 6e74 656e 7420 3d20 5b5d      content = []
+000103c0: 0a20 2020 2020 2020 2066 6f72 2065 6e74  .        for ent
+000103d0: 7279 2069 6e20 7365 6c66 2e64 6972 6563  ry in self.direc
+000103e0: 746f 7279 5f63 6f6e 7465 6e74 2829 3a0a  tory_content():.
+000103f0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00010400: 6e74 7279 2e6e 616d 6520 3d3d 2022 2e22  ntry.name == "."
+00010410: 206f 7220 656e 7472 792e 6e61 6d65 203d   or entry.name =
+00010420: 3d20 222e 2e22 206f 7220 656e 7472 792e  = ".." or entry.
+00010430: 6e61 6d65 2e65 6e64 7377 6974 6828 223a  name.endswith(":
+00010440: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00010450: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00010460: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00010470: 5f66 735f 656c 656d 656e 7420 3d20 7374  _fs_element = st
+00010480: 7228 6375 7272 656e 745f 7061 7468 202b  r(current_path +
+00010490: 2065 6e74 7279 2e6e 616d 6529 2e72 6570   entry.name).rep
+000104a0: 6c61 6365 280a 2020 2020 2020 2020 2020  lace(.          
+000104b0: 2020 2020 2020 222f 222c 206c 632e 5041        "/", lc.PA
+000104c0: 5448 5f53 4550 0a20 2020 2020 2020 2020  TH_SEP.         
+000104d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000104e0: 2069 6620 656e 7472 792e 6973 5f64 6972   if entry.is_dir
+000104f0: 6563 746f 7279 2069 7320 5472 7565 2061  ectory is True a
+00010500: 6e64 2064 6573 6365 6e64 2069 7320 5472  nd descend is Tr
+00010510: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00010520: 2020 2020 6966 2073 656c 662e 6368 616e      if self.chan
+00010530: 6765 5f64 6972 6563 746f 7279 2863 7572  ge_directory(cur
+00010540: 7265 6e74 5f66 735f 656c 656d 656e 7429  rent_fs_element)
+00010550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010560: 2020 2020 2020 636f 6e74 656e 742e 6578        content.ex
+00010570: 7465 6e64 2873 656c 662e 5f77 616c 6b5f  tend(self._walk_
+00010580: 6469 7228 2929 0a20 2020 2020 2020 2020  dir()).         
+00010590: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000105a0: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+000105b0: 2e61 7070 656e 6428 6375 7272 656e 745f  .append(current_
+000105c0: 6673 5f65 6c65 6d65 6e74 290a 2020 2020  fs_element).    
+000105d0: 2020 2020 7365 6c66 2e63 6861 6e67 655f      self.change_
+000105e0: 6469 7265 6374 6f72 7928 6375 7272 656e  directory(curren
+000105f0: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
+00010600: 7265 7475 726e 2063 6f6e 7465 6e74 0a0a  return content..
+00010610: 2020 2020 6465 6620 6765 745f 6669 6c65      def get_file
+00010620: 5f6c 6973 7428 0a20 2020 2020 2020 2073  _list(.        s
+00010630: 656c 662c 2070 6174 683a 2073 7472 203d  elf, path: str =
+00010640: 2022 222c 2064 6573 6365 6e64 3a20 626f   "", descend: bo
+00010650: 6f6c 203d 2054 7275 652c 2070 6174 7465  ol = True, patte
+00010660: 726e 3a20 7374 7220 3d20 2222 0a20 2020  rn: str = "".   
+00010670: 2029 202d 3e20 4c69 7374 5b73 7472 5d3a   ) -> List[str]:
+00010680: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010690: 2020 2020 2047 6574 206c 6973 7420 6f66       Get list of
+000106a0: 2066 696c 6573 2069 6e20 6469 7265 6374   files in direct
+000106b0: 6f72 7920 7374 7275 6374 7572 652e 0a20  ory structure.. 
+000106c0: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
+000106d0: 6163 6365 7373 206c 6576 656c 2060 6046  access level ``F
+000106e0: 494c 4554 5241 4e53 4645 5260 6020 746f  ILETRANSFER`` to
+000106f0: 2077 6f72 6b2e 0a0a 2020 2020 2020 2020   work...        
+00010700: 3a70 6172 616d 2070 6174 683a 2070 6174  :param path: pat
+00010710: 6820 6f66 2074 6865 2064 6972 6563 746f  h of the directo
+00010720: 7279 2077 6865 7265 2066 696c 6573 2073  ry where files s
+00010730: 686f 756c 6420 6265 2073 6561 7263 6865  hould be searche
+00010740: 642e 2069 6620 4e6f 6e65 2074 6861 6e20  d. if None than 
+00010750: 7468 6520 6375 7272 656e 7420 6469 7265  the current dire
+00010760: 6374 6f72 7920 6973 2075 7365 640a 2020  ctory is used.  
+00010770: 2020 2020 2020 3a70 6172 616d 2064 6573        :param des
+00010780: 6365 6e64 3a20 636f 6e74 726f 6c20 6966  cend: control if
+00010790: 2073 6561 7263 6820 7368 6f75 6c64 2072   search should r
+000107a0: 756e 2072 6563 7572 7369 7665 6c79 0a20  un recursively. 
+000107b0: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
+000107c0: 7474 6572 6e3a 2072 6567 6578 2073 7472  ttern: regex str
+000107d0: 696e 6720 746f 2066 696c 7465 7220 7468  ing to filter th
+000107e0: 6520 6669 6c65 206e 616d 6573 0a20 2020  e file names.   
+000107f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00010800: 2069 6620 6e6f 7420 7365 6c66 2e6c 6f67   if not self.log
+00010810: 696e 286c 632e 4c6f 6769 6e2e 4649 4c45  in(lc.Login.FILE
+00010820: 5452 414e 5346 4552 293a 0a20 2020 2020  TRANSFER):.     
+00010830: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+00010840: 6765 722e 7761 726e 696e 6728 2263 6c6f  ger.warning("clo
+00010850: 756c 6420 6e6f 7420 6c6f 6720 696e 2061  uld not log in a
+00010860: 7320 7573 6572 2046 494c 4522 290a 2020  s user FILE").  
+00010870: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010880: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
+00010890: 7061 7468 2069 7320 6e6f 7420 4e6f 6e65  path is not None
+000108a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000108b0: 2073 656c 662e 6368 616e 6765 5f64 6972   self.change_dir
+000108c0: 6563 746f 7279 2870 6174 6829 2069 7320  ectory(path) is 
+000108d0: 4661 6c73 653a 0a20 2020 2020 2020 2020  False:.         
+000108e0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+000108f0: 6765 722e 7761 726e 696e 6728 2263 6f75  ger.warning("cou
+00010900: 6c64 206e 6f74 2063 6861 6e67 6520 746f  ld not change to
+00010910: 2064 6972 6563 746f 7279 2229 0a20 2020   directory").   
+00010920: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010930: 7572 6e20 5b5d 0a0a 2020 2020 2020 2020  urn []..        
+00010940: 6966 206c 656e 2870 6174 7465 726e 2920  if len(pattern) 
+00010950: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00010960: 2020 6669 6c65 5f6c 6973 7420 3d20 7365    file_list = se
+00010970: 6c66 2e5f 7761 6c6b 5f64 6972 2864 6573  lf._walk_dir(des
+00010980: 6365 6e64 290a 2020 2020 2020 2020 656c  cend).        el
+00010990: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000109a0: 6669 6c65 5f6c 6973 7420 3d20 5b5d 0a20  file_list = []. 
+000109b0: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
+000109c0: 6e74 7279 2069 6e20 7365 6c66 2e5f 7761  ntry in self._wa
+000109d0: 6c6b 5f64 6972 2864 6573 6365 6e64 293a  lk_dir(descend):
+000109e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000109f0: 2066 696c 655f 6e61 6d65 203d 2065 6e74   file_name = ent
+00010a00: 7279 2e73 706c 6974 286c 632e 5041 5448  ry.split(lc.PATH
+00010a10: 5f53 4550 295b 2d31 5d0a 2020 2020 2020  _SEP)[-1].      
+00010a20: 2020 2020 2020 2020 2020 6966 2072 652e            if re.
+00010a30: 6d61 7463 6828 7061 7474 6572 6e2c 2066  match(pattern, f
+00010a40: 696c 655f 6e61 6d65 293a 0a20 2020 2020  ile_name):.     
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010a60: 696c 655f 6c69 7374 2e61 7070 656e 6428  ile_list.append(
+00010a70: 656e 7472 7929 0a20 2020 2020 2020 2072  entry).        r
+00010a80: 6574 7572 6e20 6669 6c65 5f6c 6973 740a  eturn file_list.
+00010a90: 0a20 2020 2064 6566 2072 6561 645f 6461  .    def read_da
+00010aa0: 7461 5f70 6174 6828 7365 6c66 2c20 7061  ta_path(self, pa
+00010ab0: 7468 3a20 7374 7229 202d 3e20 556e 696f  th: str) -> Unio
+00010ac0: 6e5b 626f 6f6c 2c20 696e 742c 2066 6c6f  n[bool, int, flo
+00010ad0: 6174 2c20 7374 722c 204e 6f6e 655d 3a0a  at, str, None]:.
+00010ae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010af0: 2020 2020 5265 6164 2076 616c 7565 7320      Read values 
+00010b00: 6672 6f6d 2063 6f6e 7472 6f6c 2076 6961  from control via
+00010b10: 2064 6174 6120 7061 7468 2e20 4f6e 6c79   data path. Only
+00010b20: 2077 6f72 6b73 206f 6e20 6954 4e43 2063   works on iTNC c
+00010b30: 6f6e 7472 6f6c 732e 0a20 2020 2020 2020  ontrols..       
+00010b40: 2046 6f72 2065 6173 6520 6f66 2075 7365   For ease of use
+00010b50: 2c20 7468 6520 7061 7468 2069 7320 666f  , the path is fo
+00010b60: 726d 6174 7465 6420 6279 2072 6570 6c61  rmatted by repla
+00010b70: 6369 6e67 202f 2062 7920 5c5c 2061 6e64  cing / by \\ and
+00010b80: 2022 2062 7920 272e 0a20 2020 2020 2020   " by '..       
+00010b90: 2052 6574 7572 6e73 2064 6174 6120 7661   Returns data va
+00010ba0: 6c75 6520 7265 6164 2066 726f 6d20 636f  lue read from co
+00010bb0: 6e74 726f 6c20 666f 726d 6174 7465 6420  ntrol formatted 
+00010bc0: 696e 206e 6174 6976 2064 6174 6120 7479  in nativ data ty
+00010bd0: 7065 206f 7220 4e6f 6e65 2069 6620 7265  pe or None if re
+00010be0: 6164 696e 670a 2020 2020 2020 2020 7761  ading.        wa
+00010bf0: 7320 6e6f 7420 7375 6363 6573 7366 756c  s not successful
+00010c00: 2e0a 2020 2020 2020 2020 5265 7175 6972  ..        Requir
+00010c10: 6573 2061 6363 6573 7320 6c65 7665 6c20  es access level 
+00010c20: 6060 4441 5441 6060 2074 6f20 776f 726b  ``DATA`` to work
+00010c30: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00010c40: 6d20 7061 7468 3a20 6461 7461 2070 6174  m path: data pat
+00010c50: 6820 6672 6f6d 2077 6869 6368 2074 6f20  h from which to 
+00010c60: 7265 6164 2074 6865 2076 616c 7565 2e0a  read the value..
+00010c70: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+00010c80: 204c 5356 3250 726f 746f 636f 6c45 7863   LSV2ProtocolExc
+00010c90: 6570 7469 6f6e 3a20 6966 2064 6174 6120  eption: if data 
+00010ca0: 7479 7065 2063 6f75 6c64 206e 6f74 2062  type could not b
+00010cb0: 6520 6465 7465 726d 6965 6e64 0a20 2020  e determiend.   
+00010cc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00010cd0: 2069 6620 6e6f 7420 7365 6c66 2e76 6572   if not self.ver
+00010ce0: 7369 6f6e 732e 6973 5f69 746e 6328 293a  sions.is_itnc():
+00010cf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010d00: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
+00010d10: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+00010d20: 2020 2022 5265 6164 696e 6720 7661 6c75     "Reading valu
+00010d30: 6573 2066 726f 6d20 6461 7461 2070 6174  es from data pat
+00010d40: 6820 646f 6573 206e 6f74 2077 6f72 6b20  h does not work 
+00010d50: 6f6e 206e 6f6e 2069 544e 4320 636f 6e74  on non iTNC cont
+00010d60: 726f 6c73 2122 0a20 2020 2020 2020 2020  rols!".         
+00010d70: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00010d80: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00010d90: 2020 2020 2020 7061 7468 203d 2070 6174        path = pat
+00010da0: 682e 7265 706c 6163 6528 222f 222c 206c  h.replace("/", l
+00010db0: 632e 5041 5448 5f53 4550 292e 7265 706c  c.PATH_SEP).repl
+00010dc0: 6163 6528 2722 272c 2022 2722 290a 0a20  ace('"', "'").. 
+00010dd0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00010de0: 6c66 2e6c 6f67 696e 286c 632e 4c6f 6769  lf.login(lc.Logi
+00010df0: 6e2e 4441 5441 293a 0a20 2020 2020 2020  n.DATA):.       
+00010e00: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+00010e10: 722e 7761 726e 696e 6728 2263 6c6f 756c  r.warning("cloul
+00010e20: 6420 6e6f 7420 6c6f 6720 696e 2061 7320  d not log in as 
+00010e30: 7573 6572 2044 4154 4122 290a 2020 2020  user DATA").    
+00010e40: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00010e50: 6f6e 650a 0a20 2020 2020 2020 2070 6179  one..        pay
+00010e60: 6c6f 6164 203d 2062 7974 6561 7272 6179  load = bytearray
+00010e70: 2829 0a20 2020 2020 2020 2070 6179 6c6f  ().        paylo
+00010e80: 6164 2e65 7874 656e 6428 6222 5c78 3030  ad.extend(b"\x00
+00010e90: 2229 2020 2320 3c2d 203f 3f3f 0a20 2020  ")  # <- ???.   
+00010ea0: 2020 2020 2070 6179 6c6f 6164 2e65 7874       payload.ext
+00010eb0: 656e 6428 6222 5c78 3030 2229 2020 2320  end(b"\x00")  # 
+00010ec0: 3c2d 203f 3f3f 0a20 2020 2020 2020 2070  <- ???.        p
+00010ed0: 6179 6c6f 6164 2e65 7874 656e 6428 6222  ayload.extend(b"
+00010ee0: 5c78 3030 2229 2020 2320 3c2d 203f 3f3f  \x00")  # <- ???
+00010ef0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00010f00: 2e65 7874 656e 6428 6222 5c78 3030 2229  .extend(b"\x00")
+00010f10: 2020 2320 3c2d 203f 3f3f 0a20 2020 2020    # <- ???.     
+00010f20: 2020 2070 6179 6c6f 6164 2e65 7874 656e     payload.exten
+00010f30: 6428 6c6d 2e75 7374 725f 746f 5f62 6128  d(lm.ustr_to_ba(
+00010f40: 7061 7468 2929 0a0a 2020 2020 2020 2020  path))..        
+00010f50: 7265 7375 6c74 203d 2073 656c 662e 5f73  result = self._s
+00010f60: 656e 645f 7265 6369 7665 286c 632e 434d  end_recive(lc.CM
+00010f70: 442e 525f 4450 2c20 7061 796c 6f61 642c  D.R_DP, payload,
+00010f80: 206c 632e 5253 502e 535f 4450 290a 0a20   lc.RSP.S_DP).. 
+00010f90: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00010fa0: 616e 6365 2872 6573 756c 742c 2028 6279  ance(result, (by
+00010fb0: 7465 6172 7261 792c 2929 2061 6e64 206c  tearray,)) and l
+00010fc0: 656e 2872 6573 756c 7429 203e 2030 3a0a  en(result) > 0:.
+00010fd0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00010fe0: 655f 7479 7065 203d 2073 7472 7563 742e  e_type = struct.
+00010ff0: 756e 7061 636b 2822 214c 222c 2072 6573  unpack("!L", res
+00011000: 756c 745b 303a 345d 295b 305d 0a20 2020  ult[0:4])[0].   
+00011010: 2020 2020 2020 2020 2069 6620 7661 6c75           if valu
+00011020: 655f 7479 7065 203d 3d20 323a 0a20 2020  e_type == 2:.   
+00011030: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00011040: 615f 7661 6c75 6520 3d20 7374 7275 6374  a_value = struct
+00011050: 2e75 6e70 6163 6b28 2221 6822 2c20 7265  .unpack("!h", re
+00011060: 7375 6c74 5b34 3a36 5d29 5b30 5d0a 2020  sult[4:6])[0].  
+00011070: 2020 2020 2020 2020 2020 656c 6966 2076            elif v
+00011080: 616c 7565 5f74 7970 6520 3d3d 2033 3a0a  alue_type == 3:.
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 6461 7461 5f76 616c 7565 203d 2073 7472  data_value = str
+000110b0: 7563 742e 756e 7061 636b 2822 216c 222c  uct.unpack("!l",
+000110c0: 2072 6573 756c 745b 343a 385d 295b 305d   result[4:8])[0]
+000110d0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000110e0: 6620 7661 6c75 655f 7479 7065 203d 3d20  f value_type == 
+000110f0: 353a 0a20 2020 2020 2020 2020 2020 2020  5:.             
+00011100: 2020 2064 6174 615f 7661 6c75 6520 3d20     data_value = 
+00011110: 7374 7275 6374 2e75 6e70 6163 6b28 223c  struct.unpack("<
+00011120: 6422 2c20 7265 7375 6c74 5b34 3a31 325d  d", result[4:12]
+00011130: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
+00011140: 2065 6c69 6620 7661 6c75 655f 7479 7065   elif value_type
+00011150: 203d 3d20 383a 0a20 2020 2020 2020 2020   == 8:.         
+00011160: 2020 2020 2020 2064 6174 615f 7661 6c75         data_valu
+00011170: 6520 3d20 6c6d 2e62 615f 746f 5f75 7374  e = lm.ba_to_ust
+00011180: 7228 7265 7375 6c74 5b34 3a5d 290a 2020  r(result[4:]).  
+00011190: 2020 2020 2020 2020 2020 656c 6966 2076            elif v
+000111a0: 616c 7565 5f74 7970 6520 3d3d 2031 313a  alue_type == 11:
+000111b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111c0: 2064 6174 615f 7661 6c75 6520 3d20 7374   data_value = st
+000111d0: 7275 6374 2e75 6e70 6163 6b28 2221 3f22  ruct.unpack("!?"
+000111e0: 2c20 7265 7375 6c74 5b34 3a35 5d29 5b30  , result[4:5])[0
+000111f0: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+00011200: 6966 2076 616c 7565 5f74 7970 6520 3d3d  if value_type ==
+00011210: 2031 363a 0a20 2020 2020 2020 2020 2020   16:.           
+00011220: 2020 2020 2064 6174 615f 7661 6c75 6520       data_value 
+00011230: 3d20 7374 7275 6374 2e75 6e70 6163 6b28  = struct.unpack(
+00011240: 2221 6222 2c20 7265 7375 6c74 5b34 3a35  "!b", result[4:5
+00011250: 5d29 5b30 5d0a 2020 2020 2020 2020 2020  ])[0].          
+00011260: 2020 656c 6966 2076 616c 7565 5f74 7970    elif value_typ
+00011270: 6520 3d3d 2031 373a 0a20 2020 2020 2020  e == 17:.       
+00011280: 2020 2020 2020 2020 2064 6174 615f 7661           data_va
+00011290: 6c75 6520 3d20 7374 7275 6374 2e75 6e70  lue = struct.unp
+000112a0: 6163 6b28 2221 4222 2c20 7265 7375 6c74  ack("!B", result
+000112b0: 5b34 3a35 5d29 5b30 5d0a 2020 2020 2020  [4:5])[0].      
+000112c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000112d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000112e0: 6520 4c53 5632 5072 6f74 6f63 6f6c 4578  e LSV2ProtocolEx
+000112f0: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
+00011300: 2020 2020 2020 2020 2020 2020 2022 756e               "un
+00011310: 6b6e 6f77 6e20 7265 7475 726e 2074 7970  known return typ
+00011320: 653a 2025 6420 666f 7220 2573 2220 2520  e: %d for %s" % 
+00011330: 2876 616c 7565 5f74 7970 652c 2072 6573  (value_type, res
+00011340: 756c 745b 343a 5d29 0a20 2020 2020 2020  ult[4:]).       
+00011350: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00011360: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+00011370: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
+00011380: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
+00011390: 6573 7366 756c 6c79 2072 6561 6420 6461  essfully read da
+000113a0: 7461 2070 6174 683a 2025 7320 616e 6420  ta path: %s and 
+000113b0: 676f 7420 7661 6c75 6520 2725 7327 222c  got value '%s'",
+000113c0: 2070 6174 682c 2064 6174 615f 7661 6c75   path, data_valu
+000113d0: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
+000113e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000113f0: 726e 2064 6174 615f 7661 6c75 650a 2020  rn data_value.  
+00011400: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+00011410: 6c61 7374 5f65 7272 6f72 2e65 5f63 6f64  last_error.e_cod
+00011420: 6520 3d3d 206c 632e 4c53 5632 5374 6174  e == lc.LSV2Stat
+00011430: 7573 436f 6465 2e54 5f45 525f 5752 4f4e  usCode.T_ER_WRON
+00011440: 475f 5041 5241 3a0a 2020 2020 2020 2020  G_PARA:.        
+00011450: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+00011460: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+00011470: 2020 2020 2020 2020 2020 2274 6865 2061            "the a
+00011480: 7267 756d 656e 7420 2725 7327 2069 7320  rgument '%s' is 
+00011490: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+000114a0: 2074 6869 7320 636f 6e74 726f 6c22 2c20   this control", 
+000114b0: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+000114c0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+000114d0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+000114e0: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
+000114f0: 2020 2020 2020 2020 2261 6e20 6572 726f          "an erro
+00011500: 7220 6f63 6375 7272 6564 2077 6869 6c65  r occurred while
+00011510: 2071 7565 7279 696e 6720 6461 7461 2070   querying data p
+00011520: 6174 6820 2725 7327 2e20 4572 726f 7220  ath '%s'. Error 
+00011530: 636f 6465 2077 6173 2025 6422 2c0a 2020  code was %d",.  
+00011540: 2020 2020 2020 2020 2020 7061 7468 2c20            path, 
+00011550: 7365 6c66 2e6c 6173 745f 6572 726f 722e  self.last_error.
+00011560: 655f 636f 6465 0a20 2020 2020 2020 2029  e_code.        )
+00011570: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011580: 4e6f 6e65 0a0a 2020 2020 6465 6620 6178  None..    def ax
+00011590: 6573 5f6c 6f63 6174 696f 6e28 7365 6c66  es_location(self
+000115a0: 2920 2d3e 2055 6e69 6f6e 5b44 6963 745b  ) -> Union[Dict[
+000115b0: 7374 722c 2066 6c6f 6174 5d2c 204e 6f6e  str, float], Non
+000115c0: 655d 3a0a 2020 2020 2020 2020 2222 220a  e]:.        """.
+000115d0: 2020 2020 2020 2020 5265 6164 2061 7865          Read axe
+000115e0: 7320 6c6f 6361 7469 6f6e 2066 726f 6d20  s location from 
+000115f0: 636f 6e74 726f 6c2e 204e 6f74 2066 756c  control. Not ful
+00011600: 6c79 2064 6f63 756d 656e 7465 642c 2076  ly documented, v
+00011610: 616c 7565 206f 6620 6669 7273 7420 6279  alue of first by
+00011620: 7465 2075 6e6b 6e6f 776e 2e0a 2020 2020  te unknown..    
+00011630: 2020 2020 5265 7175 6972 6573 2061 6363      Requires acc
+00011640: 6573 7320 6c65 7665 6c20 6060 444e 4360  ess level ``DNC`
+00011650: 6020 746f 2077 6f72 6b2e 0a20 2020 2020  ` to work..     
+00011660: 2020 2052 6574 7572 6e73 2060 604e 6f6e     Returns ``Non
+00011670: 6560 6020 6966 206e 6f20 6461 7461 2077  e`` if no data w
+00011680: 6173 2072 6563 6569 7665 6420 6f72 2064  as received or d
+00011690: 6963 7469 6f6e 6172 7920 7769 7468 206b  ictionary with k
+000116a0: 6579 203d 2061 7869 7320 6e61 6d65 2c20  ey = axis name, 
+000116b0: 7661 6c75 6520 3d20 706f 7369 7469 6f6e  value = position
+000116c0: 0a0a 2020 2020 2020 2020 3a72 6169 7365  ..        :raise
+000116d0: 7320 4c53 5632 4461 7461 4578 6365 7074  s LSV2DataExcept
+000116e0: 696f 6e3a 2045 7272 6f72 2064 7572 696e  ion: Error durin
+000116f0: 6720 7061 7273 696e 6720 6f66 2064 6174  g parsing of dat
+00011700: 6120 7661 6c75 6573 0a20 2020 2020 2020  a values.       
+00011710: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00011720: 6e6f 7420 7365 6c66 2e6c 6f67 696e 286c  not self.login(l
+00011730: 632e 4c6f 6769 6e2e 444e 4329 3a0a 2020  c.Login.DNC):.  
+00011740: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00011750: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+00011760: 636c 6f75 6c64 206e 6f74 206c 6f67 2069  clould not log i
+00011770: 6e20 6173 2075 7365 7220 444e 4322 290a  n as user DNC").
+00011780: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011790: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
+000117a0: 2070 6179 6c6f 6164 203d 2062 7974 6561   payload = bytea
+000117b0: 7272 6179 2829 0a20 2020 2020 2020 2070  rray().        p
+000117c0: 6179 6c6f 6164 2e65 7874 656e 6428 7374  ayload.extend(st
+000117d0: 7275 6374 2e70 6163 6b28 2221 4822 2c20  ruct.pack("!H", 
+000117e0: 6c63 2e50 6172 5252 492e 4158 4953 5f4c  lc.ParRRI.AXIS_L
+000117f0: 4f43 4154 494f 4e29 290a 0a20 2020 2020  OCATION))..     
+00011800: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+00011810: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
+00011820: 2e43 4d44 2e52 5f52 492c 2070 6179 6c6f  .CMD.R_RI, paylo
+00011830: 6164 2c20 6c63 2e52 5350 2e53 5f52 4929  ad, lc.RSP.S_RI)
+00011840: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00011850: 7374 616e 6365 2872 6573 756c 742c 2028  stance(result, (
+00011860: 6279 7465 6172 7261 792c 2929 2061 6e64  bytearray,)) and
+00011870: 206c 656e 2872 6573 756c 7429 203e 2030   len(result) > 0
+00011880: 3a0a 2020 2020 2020 2020 2020 2020 6178  :.            ax
+00011890: 6573 5f76 616c 7565 7320 3d20 6c6d 2e64  es_values = lm.d
+000118a0: 6563 6f64 655f 6178 6973 5f6c 6f63 6174  ecode_axis_locat
+000118b0: 696f 6e28 7265 7375 6c74 290a 2020 2020  ion(result).    
+000118c0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+000118d0: 6767 6572 2e69 6e66 6f28 2273 7563 6365  gger.info("succe
+000118e0: 7373 6675 6c6c 7920 7265 6164 2061 7865  ssfully read axe
+000118f0: 7320 7661 6c75 6573 3a20 2573 222c 2061  s values: %s", a
+00011900: 7865 735f 7661 6c75 6573 290a 2020 2020  xes_values).    
+00011910: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00011920: 7865 735f 7661 6c75 6573 0a0a 2020 2020  xes_values..    
+00011930: 2020 2020 7365 6c66 2e5f 6c6f 6767 6572      self._logger
+00011940: 2e77 6172 6e69 6e67 2822 616e 2065 7272  .warning("an err
+00011950: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
+00011960: 6520 7175 6572 7969 6e67 2061 7865 7320  e querying axes 
+00011970: 706f 7369 7469 6f6e 2229 0a20 2020 2020  position").     
+00011980: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00011990: 2020 2020 6465 6620 6772 6162 5f73 6372      def grab_scr
+000119a0: 6565 6e5f 6475 6d70 2873 656c 662c 2069  een_dump(self, i
+000119b0: 6d61 6765 5f70 6174 683a 2070 6174 686c  mage_path: pathl
+000119c0: 6962 2e50 6174 6829 202d 3e20 626f 6f6c  ib.Path) -> bool
+000119d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000119e0: 2020 2020 2020 4372 6561 7465 2073 6372        Create scr
+000119f0: 6565 6e5f 6475 6d70 206f 6620 6375 7272  een_dump of curr
+00011a00: 656e 7420 636f 6e74 726f 6c20 7363 7265  ent control scre
+00011a10: 656e 2061 6e64 2073 6176 6520 6974 2061  en and save it a
+00011a20: 7320 6269 746d 6170 2e0a 2020 2020 2020  s bitmap..      
+00011a30: 2020 5265 7175 6972 6573 2061 6363 6573    Requires acces
+00011a40: 7320 6c65 7665 6c20 6060 444e 4360 6020  s level ``DNC`` 
+00011a50: 746f 2077 6f72 6b2e 0a20 2020 2020 2020  to work..       
+00011a60: 2052 6574 7572 6e73 2060 6054 7275 6560   Returns ``True`
+00011a70: 6020 6966 2063 6f6d 706c 6574 6564 2073  ` if completed s
+00011a80: 7563 6365 7373 6675 6c6c 792e 0a0a 2020  uccessfully...  
+00011a90: 2020 2020 2020 3a70 6172 616d 2069 6d61        :param ima
+00011aa0: 6765 5f70 6174 683a 2070 6174 6820 6f66  ge_path: path of
+00011ab0: 2062 6d70 2066 696c 6520 666f 7220 7363   bmp file for sc
+00011ac0: 7265 656e 6475 6d70 0a20 2020 2020 2020  reendump.       
+00011ad0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00011ae0: 6e6f 7420 7365 6c66 2e6c 6f67 696e 286c  not self.login(l
+00011af0: 632e 4c6f 6769 6e2e 4649 4c45 5452 414e  c.Login.FILETRAN
+00011b00: 5346 4552 293a 0a20 2020 2020 2020 2020  SFER):.         
+00011b10: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+00011b20: 7761 726e 696e 6728 2263 6c6f 756c 6420  warning("clould 
+00011b30: 6e6f 7420 6c6f 6720 696e 2061 7320 7573  not log in as us
+00011b40: 6572 2046 494c 4522 290a 2020 2020 2020  er FILE").      
+00011b50: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00011b60: 7365 0a0a 2020 2020 2020 2020 7465 6d70  se..        temp
+00011b70: 5f66 696c 655f 7061 7468 203d 2028 0a20  _file_path = (. 
+00011b80: 2020 2020 2020 2020 2020 206c 632e 4472             lc.Dr
+00011b90: 6976 654e 616d 652e 544e 430a 2020 2020  iveName.TNC.    
+00011ba0: 2020 2020 2020 2020 2b20 6c63 2e50 4154          + lc.PAT
+00011bb0: 485f 5345 500a 2020 2020 2020 2020 2020  H_SEP.          
+00011bc0: 2020 2b20 2273 6372 6565 6e64 756d 705f    + "screendump_
+00011bd0: 220a 2020 2020 2020 2020 2020 2020 2b20  ".            + 
+00011be0: 6461 7465 7469 6d65 2e6e 6f77 2829 2e73  datetime.now().s
+00011bf0: 7472 6674 696d 6528 2225 5925 6d25 645f  trftime("%Y%m%d_
+00011c00: 2548 254d 2553 2229 0a20 2020 2020 2020  %H%M%S").       
+00011c10: 2020 2020 202b 2022 2e62 6d70 220a 2020       + ".bmp".  
+00011c20: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00011c30: 2070 6179 6c6f 6164 203d 2062 7974 6561   payload = bytea
+00011c40: 7272 6179 2873 7472 7563 742e 7061 636b  rray(struct.pack
+00011c50: 2822 2148 222c 206c 632e 5061 7243 4343  ("!H", lc.ParCCC
+00011c60: 2e53 4352 4545 4e44 554d 5029 290a 2020  .SCREENDUMP)).  
+00011c70: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
+00011c80: 7465 6e64 286c 6d2e 7573 7472 5f74 6f5f  tend(lm.ustr_to_
+00011c90: 6261 2874 656d 705f 6669 6c65 5f70 6174  ba(temp_file_pat
+00011ca0: 6829 290a 0a20 2020 2020 2020 2072 6573  h))..        res
+00011cb0: 756c 7420 3d20 7365 6c66 2e5f 7365 6e64  ult = self._send
+00011cc0: 5f72 6563 6976 6528 6c63 2e43 4d44 2e43  _recive(lc.CMD.C
+00011cd0: 5f43 432c 2070 6179 6c6f 6164 2c20 6c63  _CC, payload, lc
+00011ce0: 2e52 5350 2e54 5f4f 4b29 0a0a 2020 2020  .RSP.T_OK)..    
+00011cf0: 2020 2020 6966 206e 6f74 2028 6973 696e      if not (isin
+00011d00: 7374 616e 6365 2872 6573 756c 742c 2028  stance(result, (
+00011d10: 626f 6f6c 2c29 2920 616e 6420 7265 7375  bool,)) and resu
+00011d20: 6c74 2069 7320 5472 7565 293a 0a20 2020  lt is True):.   
+00011d30: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+00011d40: 6f67 6765 722e 7761 726e 696e 6728 2273  ogger.warning("s
+00011d50: 6372 6565 6e20 6475 6d70 2077 6173 206e  creen dump was n
+00011d60: 6f74 2063 7265 6174 6564 2229 0a20 2020  ot created").   
+00011d70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011d80: 4661 6c73 650a 0a20 2020 2020 2020 2069  False..        i
+00011d90: 6620 6e6f 7420 7365 6c66 2e72 6563 6976  f not self.reciv
+00011da0: 655f 6669 6c65 280a 2020 2020 2020 2020  e_file(.        
+00011db0: 2020 2020 7265 6d6f 7465 5f70 6174 683d      remote_path=
+00011dc0: 7465 6d70 5f66 696c 655f 7061 7468 2c20  temp_file_path, 
+00011dd0: 6c6f 6361 6c5f 7061 7468 3d69 6d61 6765  local_path=image
+00011de0: 5f70 6174 682c 2062 696e 6172 795f 6d6f  _path, binary_mo
+00011df0: 6465 3d54 7275 650a 2020 2020 2020 2020  de=True.        
+00011e00: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00011e10: 656c 662e 5f6c 6f67 6765 722e 7761 726e  elf._logger.warn
+00011e20: 696e 6728 2263 6f75 6c64 206e 6f74 2064  ing("could not d
+00011e30: 6f77 6e6c 6f61 6420 7363 7265 656e 2064  ownload screen d
+00011e40: 756d 7020 6672 6f6d 2063 6f6e 7472 6f6c  ump from control
+00011e50: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00011e60: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00011e70: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00011e80: 2e64 656c 6574 655f 6669 6c65 2874 656d  .delete_file(tem
+00011e90: 705f 6669 6c65 5f70 6174 6829 3a0a 2020  p_file_path):.  
+00011ea0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00011eb0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+00011ec0: 636c 6f75 6c64 206e 6f74 2064 656c 6574  clould not delet
+00011ed0: 6520 7465 6d70 6f72 6172 7920 6669 6c65  e temporary file
+00011ee0: 206f 6e20 636f 6e74 726f 6c22 290a 2020   on control").  
+00011ef0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011f00: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+00011f10: 7365 6c66 2e5f 6c6f 6767 6572 2e64 6562  self._logger.deb
+00011f20: 7567 2822 7375 6363 6573 7366 756c 6c79  ug("successfully
+00011f30: 2072 6563 6569 7665 6420 7363 7265 656e   received screen
+00011f40: 2064 756d 7022 290a 2020 2020 2020 2020   dump").        
+00011f50: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00011f60: 2064 6566 2067 6574 5f72 656d 6f74 655f   def get_remote_
+00011f70: 6461 7465 7469 6d65 2873 656c 6629 202d  datetime(self) -
+00011f80: 3e20 6461 7465 7469 6d65 3a0a 2020 2020  > datetime:.    
+00011f90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011fa0: 5265 6164 2063 7572 7265 6e74 2074 696d  Read current tim
+00011fb0: 6520 616e 6420 6461 7465 2066 726f 6d20  e and date from 
+00011fc0: 636f 6e74 726f 6c0a 2020 2020 2020 2020  control.        
+00011fd0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+00011fe0: 6f74 2073 656c 662e 6c6f 6769 6e28 6c63  ot self.login(lc
+00011ff0: 2e4c 6f67 696e 2e44 4941 4729 3a0a 2020  .Login.DIAG):.  
+00012000: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00012010: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
+00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012030: 2263 6c6f 756c 6420 6e6f 7420 6c6f 6720  "clould not log 
+00012040: 696e 2061 7320 7573 6572 2066 6f72 2044  in as user for D
+00012050: 4941 474e 4f53 5449 4353 2066 756e 6374  IAGNOSTICS funct
+00012060: 696f 6e22 290a 2020 2020 2020 2020 2020  ion").          
+00012070: 2020 7265 7475 726e 2064 6174 6574 696d    return datetim
+00012080: 652e 6672 6f6d 7469 6d65 7374 616d 7028  e.fromtimestamp(
+00012090: 3029 0a0a 2020 2020 2020 2020 7265 7375  0)..        resu
+000120a0: 6c74 203d 2073 656c 662e 5f73 656e 645f  lt = self._send_
+000120b0: 7265 6369 7665 286c 632e 434d 442e 525f  recive(lc.CMD.R_
+000120c0: 4454 2c20 4e6f 6e65 2c20 6c63 2e52 5350  DT, None, lc.RSP
+000120d0: 2e53 5f44 5429 0a20 2020 2020 2020 2069  .S_DT).        i
+000120e0: 6620 6973 696e 7374 616e 6365 2872 6573  f isinstance(res
+000120f0: 756c 742c 2028 6279 7465 6172 7261 792c  ult, (bytearray,
+00012100: 2929 2061 6e64 206c 656e 2872 6573 756c  )) and len(resul
+00012110: 7429 203e 2030 3a0a 2020 2020 2020 2020  t) > 0:.        
+00012120: 2020 2020 7473 203d 206c 6d2e 6465 636f      ts = lm.deco
+00012130: 6465 5f74 696d 6573 7461 6d70 2872 6573  de_timestamp(res
+00012140: 756c 7429 0a20 2020 2020 2020 2020 2020  ult).           
+00012150: 2073 656c 662e 5f6c 6f67 6765 722e 6465   self._logger.de
+00012160: 6275 6728 2254 696d 6520 6f6e 2043 6f6e  bug("Time on Con
+00012170: 7472 6f6c 2069 7320 2573 222c 2074 732e  trol is %s", ts.
+00012180: 6973 6f66 6f72 6d61 7428 2929 0a20 2020  isoformat()).   
+00012190: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000121a0: 2020 2020 2020 2072 6169 7365 204c 5356         raise LSV
+000121b0: 3250 726f 746f 636f 6c45 7863 6570 7469  2ProtocolExcepti
+000121c0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000121d0: 2020 2020 2273 6f6d 6574 6869 6e67 2077      "something w
+000121e0: 656e 7420 7772 6f6e 6720 7768 696c 6520  ent wrong while 
+000121f0: 7265 6164 696e 6720 6375 7272 656e 7420  reading current 
+00012200: 7469 6d65 2061 6e64 2064 6174 6522 0a20  time and date". 
+00012210: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00012220: 2020 2020 2072 6574 7572 6e20 7473 0a0a       return ts..
+00012230: 2020 2020 6465 6620 7265 6164 5f73 636f      def read_sco
+00012240: 7065 5f73 6967 6e61 6c73 2873 656c 6629  pe_signals(self)
+00012250: 202d 3e20 4c69 7374 5b6c 642e 5363 6f70   -> List[ld.Scop
+00012260: 6553 6967 6e61 6c5d 3a0a 2020 2020 2020  eSignal]:.      
+00012270: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+00012280: 6164 2061 7661 696c 6162 6c65 2073 636f  ad available sco
+00012290: 7065 2063 6861 6e6e 656c 7320 616e 6420  pe channels and 
+000122a0: 7369 676e 616c 732e 204f 6e6c 7920 776f  signals. Only wo
+000122b0: 726b 7320 666f 7220 6954 4e43 2035 3330  rks for iTNC 530
+000122c0: 2e0a 2020 2020 2020 2020 5265 7175 6972  ..        Requir
+000122d0: 6573 2061 6363 6573 7320 6c65 7665 6c20  es access level 
+000122e0: 6060 5343 4f50 4560 6020 746f 2077 6f72  ``SCOPE`` to wor
+000122f0: 6b2e 0a20 2020 2020 2020 2072 6574 7572  k..        retur
+00012300: 6e73 206c 6973 7420 6f66 203a 7079 3a63  ns list of :py:c
+00012310: 6c61 7373 3a60 7e70 794c 5356 322e 4c53  lass:`~pyLSV2.LS
+00012320: 5632 2e53 636f 7065 5369 676e 616c 6020  V2.ScopeSignal` 
+00012330: 666f 7220 6561 6368 2073 6967 6e61 6c0a  for each signal.
+00012340: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012350: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00012360: 7665 7273 696f 6e73 2e69 735f 6974 6e63  versions.is_itnc
+00012370: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00012380: 7365 6c66 2e5f 6c6f 6767 6572 2e77 6172  self._logger.war
+00012390: 6e69 6e67 2822 6f6e 6c79 2077 6f72 6b73  ning("only works
+000123a0: 2066 6f72 2069 544e 4335 3330 2229 0a20   for iTNC530"). 
+000123b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000123c0: 6e20 6c69 7374 2829 0a0a 2020 2020 2020  n list()..      
+000123d0: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
+000123e0: 6769 6e28 6c63 2e4c 6f67 696e 2e53 434f  gin(lc.Login.SCO
+000123f0: 5045 293a 0a20 2020 2020 2020 2020 2020  PE):.           
+00012400: 2073 656c 662e 5f6c 6f67 6765 722e 7761   self._logger.wa
+00012410: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+00012420: 2020 2020 2020 2022 636c 6f75 6c64 206e         "clould n
+00012430: 6f74 206c 6f67 2069 6e20 6173 2075 7365  ot log in as use
+00012440: 7220 666f 7220 7363 6f70 6520 6675 6e63  r for scope func
+00012450: 7469 6f6e 2229 0a20 2020 2020 2020 2020  tion").         
+00012460: 2020 2072 6574 7572 6e20 6c69 7374 2829     return list()
+00012470: 0a0a 2020 2020 2020 2020 6368 616e 6e65  ..        channe
+00012480: 6c5f 6c69 7374 203d 206c 6973 7428 290a  l_list = list().
+00012490: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
+000124a0: 203d 2073 656c 662e 5f6c 6c63 6f6d 2e74   = self._llcom.t
+000124b0: 656c 6567 7261 6d28 6c63 2e43 4d44 2e52  elegram(lc.CMD.R
+000124c0: 5f4f 4329 0a20 2020 2020 2020 2069 6620  _OC).        if 
+000124d0: 7365 6c66 2e5f 6c6c 636f 6d2e 6c61 7374  self._llcom.last
+000124e0: 5f72 6573 706f 6e73 6520 696e 206c 632e  _response in lc.
+000124f0: 5253 502e 535f 4f43 3a0a 2020 2020 2020  RSP.S_OC:.      
+00012500: 2020 2020 2020 6368 616e 6e65 6c5f 6c69        channel_li
+00012510: 7374 2e65 7874 656e 6428 6c6d 732e 6465  st.extend(lms.de
+00012520: 636f 6465 5f73 6967 6e61 6c5f 6465 7363  code_signal_desc
+00012530: 7269 7074 696f 6e28 636f 6e74 656e 7429  ription(content)
+00012540: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00012550: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
+00012560: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00012570: 6e74 203d 2073 656c 662e 5f6c 6c63 6f6d  nt = self._llcom
+00012580: 2e74 656c 6567 7261 6d28 6c63 2e52 5350  .telegram(lc.RSP
+00012590: 2e54 5f4f 4b29 0a0a 2020 2020 2020 2020  .T_OK)..        
+000125a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000125b0: 5f6c 6c63 6f6d 2e6c 6173 745f 7265 7370  _llcom.last_resp
+000125c0: 6f6e 7365 2069 6e20 6c63 2e52 5350 2e53  onse in lc.RSP.S
+000125d0: 5f4f 433a 0a20 2020 2020 2020 2020 2020  _OC:.           
+000125e0: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
+000125f0: 5f6c 6973 742e 6578 7465 6e64 286c 6d73  _list.extend(lms
+00012600: 2e64 6563 6f64 655f 7369 676e 616c 5f64  .decode_signal_d
+00012610: 6573 6372 6970 7469 6f6e 2863 6f6e 7465  escription(conte
+00012620: 6e74 2929 0a20 2020 2020 2020 2020 2020  nt)).           
+00012630: 2020 2020 2065 6c69 6620 7365 6c66 2e5f       elif self._
+00012640: 6c6c 636f 6d2e 6c61 7374 5f72 6573 706f  llcom.last_respo
+00012650: 6e73 6520 696e 206c 632e 5253 502e 545f  nse in lc.RSP.T_
+00012660: 4644 3a0a 2020 2020 2020 2020 2020 2020  FD:.            
+00012670: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+00012680: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
+00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126a0: 2020 2022 6669 6e69 7368 6564 206c 6f61     "finished loa
+000126b0: 6469 6e67 2061 6e64 2070 6172 7369 6e67  ding and parsing
+000126c0: 2064 6174 6120 666f 7220 616c 6c20 7363   data for all sc
+000126d0: 6f70 6520 7369 676e 616c 7322 0a20 2020  ope signals".   
+000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126f0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00012700: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00012710: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00012720: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00012730: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+00012740: 6765 722e 6572 726f 7228 0a20 2020 2020  ger.error(.     
+00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012760: 2020 2022 736f 6d65 7468 696e 6720 7765     "something we
+00012770: 6e74 2077 726f 6e67 2077 6869 6c65 2072  nt wrong while r
+00012780: 6561 6469 6e67 2073 636f 7065 2073 6967  eading scope sig
+00012790: 6e61 6c22 0a20 2020 2020 2020 2020 2020  nal".           
+000127a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000127b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000127c0: 6169 7365 204c 5356 3250 726f 746f 636f  aise LSV2Protoco
+000127d0: 6c45 7863 6570 7469 6f6e 280a 2020 2020  lException(.    
+000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127f0: 2020 2020 2264 6964 206e 6f74 2072 6563      "did not rec
+00012800: 6569 7665 6420 6578 7065 6374 6564 2072  eived expected r
+00012810: 6573 706f 6e73 6520 7768 696c 6520 7265  esponse while re
+00012820: 6164 696e 6720 6461 7461 2066 6f72 2073  ading data for s
+00012830: 636f 7065 2073 6967 6e61 6c73 220a 2020  cope signals".  
+00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012850: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00012860: 7572 6e20 6368 616e 6e65 6c5f 6c69 7374  urn channel_list
+00012870: 0a0a 2020 2020 6465 6620 7265 616c 5f74  ..    def real_t
+00012880: 696d 655f 7265 6164 696e 6773 280a 2020  ime_readings(.  
+00012890: 2020 2020 2020 7365 6c66 2c20 7369 676e        self, sign
+000128a0: 616c 5f6c 6973 743a 204c 6973 745b 6c64  al_list: List[ld
+000128b0: 2e53 636f 7065 5369 676e 616c 5d2c 2064  .ScopeSignal], d
+000128c0: 7572 6174 696f 6e3a 2069 6e74 2c20 696e  uration: int, in
+000128d0: 7465 7276 616c 3a20 696e 740a 2020 2020  terval: int.    
+000128e0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000128f0: 2020 2020 2020 2052 6561 6420 7369 676e         Read sign
+00012900: 616c 2072 6561 6469 6e67 7320 6672 6f6d  al readings from
+00012910: 2063 6f6e 7472 6f6c 2069 6e20 7265 616c   control in real
+00012920: 2074 696d 652e 204f 6e6c 7920 776f 726b   time. Only work
+00012930: 7320 666f 7220 6954 4e43 2035 3330 2e0a  s for iTNC 530..
+00012940: 2020 2020 2020 2020 4265 666f 7265 2072          Before r
+00012950: 6561 6469 6e67 2064 6174 612c 2074 6865  eading data, the
+00012960: 2073 6967 6e61 6c20 6465 7363 7269 7074   signal descript
+00012970: 696f 6e20 6973 2075 7064 6174 6564 2077  ion is updated w
+00012980: 6974 6820 696e 666f 726d 6174 696f 6e20  ith information 
+00012990: 7265 6761 7264 696e 6620 6f66 6673 6574  regardinf offset
+000129a0: 2061 6e64 2066 6163 746f 722e 0a20 2020   and factor..   
+000129b0: 2020 2020 2052 6571 7569 7265 7320 6163       Requires ac
+000129c0: 6365 7373 206c 6576 656c 2060 6053 434f  cess level ``SCO
+000129d0: 5045 6060 2074 6f20 776f 726b 2e0a 0a20  PE`` to work... 
+000129e0: 2020 2020 2020 203a 7061 7261 6d20 7369         :param si
+000129f0: 676e 616c 5f6c 6973 743a 206c 6973 7420  gnal_list: list 
+00012a00: 6f66 203a 7079 3a63 6c61 7373 3a60 7e70  of :py:class:`~p
+00012a10: 794c 5356 322e 4c53 5632 2e53 636f 7065  yLSV2.LSV2.Scope
+00012a20: 5369 676e 616c 6020 7768 6963 6820 7368  Signal` which sh
+00012a30: 6f75 6c64 2062 6520 7265 6164 2066 726f  ould be read fro
+00012a40: 6d20 636f 6e74 726f 6c0a 2020 2020 2020  m control.      
+00012a50: 2020 3a70 6172 616d 2064 7572 6174 696f    :param duratio
+00012a60: 6e3a 206e 756d 6265 7220 6f66 2073 6563  n: number of sec
+00012a70: 6f6e 6473 2066 6f72 2077 6869 6368 2064  onds for which d
+00012a80: 6174 6120 7368 6f75 6c64 2062 6520 7265  ata should be re
+00012a90: 6164 0a20 2020 2020 2020 203a 7061 7261  ad.        :para
+00012aa0: 6d20 696e 7465 7276 616c 3a20 696e 7465  m interval: inte
+00012ab0: 7276 616c 2069 6e20 c2b5 7320 6265 7477  rval in ..s betw
+00012ac0: 6565 6e20 7265 6164 696e 6773 0a0a 2020  een readings..  
+00012ad0: 2020 2020 2020 3a72 6169 7365 7320 4c53        :raises LS
+00012ae0: 5632 5072 6f74 6f63 6f6c 4578 6365 7074  V2ProtocolExcept
+00012af0: 696f 6e3a 0a20 2020 2020 2020 2022 2222  ion:.        """
+00012b00: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00012b10: 7365 6c66 2e76 6572 7369 6f6e 732e 6973  self.versions.is
+00012b20: 5f69 746e 6328 293a 0a20 2020 2020 2020  _itnc():.       
+00012b30: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+00012b40: 722e 7761 726e 696e 6728 226f 6e6c 7920  r.warning("only 
+00012b50: 776f 726b 7320 666f 7220 6954 4e43 3533  works for iTNC53
+00012b60: 3022 290a 2020 2020 2020 2020 2020 2020  0").            
+00012b70: 7265 7475 726e 206c 6973 7428 290a 0a20  return list().. 
+00012b80: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00012b90: 6c66 2e6c 6f67 696e 286c 632e 4c6f 6769  lf.login(lc.Logi
+00012ba0: 6e2e 5343 4f50 4529 3a0a 2020 2020 2020  n.SCOPE):.      
+00012bb0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+00012bc0: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
+00012bd0: 2020 2020 2020 2020 2020 2020 2263 6c6f              "clo
+00012be0: 756c 6420 6e6f 7420 6c6f 6720 696e 2061  uld not log in a
+00012bf0: 7320 7573 6572 2066 6f72 2073 636f 7065  s user for scope
+00012c00: 2066 756e 6374 696f 6e22 290a 2020 2020   function").    
+00012c10: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+00012c20: 6973 7428 290a 0a20 2020 2020 2020 2073  ist()..        s
+00012c30: 656c 662e 5f6c 6f67 6765 722e 6465 6275  elf._logger.debu
+00012c40: 6728 0a20 2020 2020 2020 2020 2020 2022  g(.            "
+00012c50: 7374 6172 7420 7265 636f 6469 6e67 2025  start recoding %
+00012c60: 6420 7265 6164 696e 6773 2077 6974 6820  d readings with 
+00012c70: 696e 7465 7276 616c 206f 6620 2564 20c2  interval of %d .
+00012c80: b573 222c 0a20 2020 2020 2020 2020 2020  .s",.           
+00012c90: 2064 7572 6174 696f 6e2c 0a20 2020 2020   duration,.     
+00012ca0: 2020 2020 2020 2069 6e74 6572 7661 6c2c         interval,
+00012cb0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00012cc0: 2020 2020 2320 7365 7420 696e 7465 7276      # set interv
+00012cd0: 616c 2061 6e64 2073 656c 6563 7420 7369  al and select si
+00012ce0: 676e 616c 730a 2020 2020 2020 2020 7061  gnals.        pa
+00012cf0: 796c 6f61 6420 3d20 6279 7465 6172 7261  yload = bytearra
+00012d00: 7928 290a 2020 2020 2020 2020 7061 796c  y().        payl
+00012d10: 6f61 642e 6578 7465 6e64 2873 7472 7563  oad.extend(struc
+00012d20: 742e 7061 636b 2822 214c 222c 2069 6e74  t.pack("!L", int
+00012d30: 6572 7661 6c29 290a 2020 2020 2020 2020  erval)).        
+00012d40: 666f 7220 7369 676e 616c 2069 6e20 7369  for signal in si
+00012d50: 676e 616c 5f6c 6973 743a 0a20 2020 2020  gnal_list:.     
+00012d60: 2020 2020 2020 2069 6620 696e 7465 7276         if interv
+00012d70: 616c 206e 6f74 2069 6e20 5b36 3030 2c20  al not in [600, 
+00012d80: 3330 3030 2c20 3231 3030 305d 3a0a 2020  3000, 21000]:.  
+00012d90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012da0: 6c66 2e5f 6c6f 6767 6572 2e77 6172 6e69  lf._logger.warni
+00012db0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00012dc0: 2020 2020 2020 2020 2274 6865 2073 656c          "the sel
+00012dd0: 6563 7465 6420 696e 7465 7276 616c 2064  ected interval d
+00012de0: 6f65 736e 2774 2066 6974 2066 6f72 2073  oesn't fit for s
+00012df0: 6967 6e61 6c73 2072 6561 6469 6e67 7321  ignals readings!
+00012e00: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012e10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00012e20: 2020 2020 7261 6973 6520 4c53 5632 5072      raise LSV2Pr
+00012e30: 6f74 6f63 6f6c 4578 6365 7074 696f 6e28  otocolException(
+00012e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012e50: 2020 2020 2022 7468 6520 7365 6c65 6374       "the select
+00012e60: 6564 2069 6e74 6572 7661 6c20 6d75 7374  ed interval must
+00012e70: 2062 653a 2036 3030 206f 7220 3330 3030   be: 600 or 3000
+00012e80: 206f 7220 3231 3030 3020 7573 220a 2020   or 21000 us".  
+00012e90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00012ea0: 2020 2020 2020 2020 2020 2020 7061 796c              payl
+00012eb0: 6f61 642e 6578 7465 6e64 2873 6967 6e61  oad.extend(signa
+00012ec0: 6c2e 746f 5f62 6128 2929 0a0a 2020 2020  l.to_ba())..    
+00012ed0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+00012ee0: 662e 5f73 656e 645f 7265 6369 7665 286c  f._send_recive(l
+00012ef0: 632e 434d 442e 525f 4f50 2c20 7061 796c  c.CMD.R_OP, payl
+00012f00: 6f61 642c 206c 632e 5253 502e 535f 4f50  oad, lc.RSP.S_OP
+00012f10: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
+00012f20: 6e73 7461 6e63 6528 7265 7375 6c74 2c20  nstance(result, 
+00012f30: 2862 7974 6561 7272 6179 2c29 2920 616e  (bytearray,)) an
+00012f40: 6420 6c65 6e28 7265 7375 6c74 2920 3e20  d len(result) > 
+00012f50: 303a 0a20 2020 2020 2020 2020 2020 2073  0:.            s
+00012f60: 6967 6e61 6c5f 6c69 7374 203d 206c 6d73  ignal_list = lms
+00012f70: 2e64 6563 6f64 655f 7369 676e 616c 5f64  .decode_signal_d
+00012f80: 6574 6169 6c73 2873 6967 6e61 6c5f 6c69  etails(signal_li
+00012f90: 7374 2c20 7265 7375 6c74 290a 2020 2020  st, result).    
+00012fa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012fb0: 2020 2020 2020 6966 2073 656c 662e 6c61        if self.la
+00012fc0: 7374 5f65 7272 6f72 2e65 5f63 6f64 6520  st_error.e_code 
+00012fd0: 3d3d 2038 353a 0a20 2020 2020 2020 2020  == 85:.         
+00012fe0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+00012ff0: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013010: 2022 746f 6f20 6d61 6e79 2073 6967 6e61   "too many signa
+00013020: 6c73 2073 656c 6563 7465 643a 2025 6422  ls selected: %d"
+00013030: 2c20 6c65 6e28 7369 676e 616c 5f6c 6973  , len(signal_lis
+00013040: 7429 290a 2020 2020 2020 2020 2020 2020  t)).            
+00013050: 2020 2020 7261 6973 6520 4c53 5632 5072      raise LSV2Pr
+00013060: 6f74 6f63 6f6c 4578 6365 7074 696f 6e28  otocolException(
+00013070: 2274 6f6f 206d 616e 7920 7369 676e 616c  "too many signal
+00013080: 7320 7365 6c65 6374 6564 3f3f 3f22 290a  s selected???").
+00013090: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000130a0: 656c 662e 6c61 7374 5f65 7272 6f72 2e65  elf.last_error.e
+000130b0: 5f63 6f64 6520 3d3d 206c 632e 4c53 5632  _code == lc.LSV2
+000130c0: 5374 6174 7573 436f 6465 2e54 5f45 525f  StatusCode.T_ER_
+000130d0: 4f53 5a49 5f43 4853 454c 3a0a 2020 2020  OSZI_CHSEL:.    
+000130e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000130f0: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
+00013100: 2822 4572 726f 7220 7365 7474 696e 6720  ("Error setting 
+00013110: 7570 2074 6865 2063 6861 6e6e 656c 7322  up the channels"
+00013120: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013130: 2020 7261 6973 6520 4c53 5632 5072 6f74    raise LSV2Prot
+00013140: 6f63 6f6c 4578 6365 7074 696f 6e28 2245  ocolException("E
+00013150: 7272 6f72 2073 6574 7469 6e67 2075 7020  rror setting up 
+00013160: 7468 6520 6368 616e 6e65 6c73 2229 0a20  the channels"). 
+00013170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013180: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
+00013190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000131a0: 2022 4572 726f 7220 7768 696c 6520 636f   "Error while co
+000131b0: 6e66 6967 7572 696e 6720 696e 7465 7276  nfiguring interv
+000131c0: 616c 2061 6e64 2073 6967 6e61 6c73 2229  al and signals")
+000131d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000131e0: 7365 204c 5356 3250 726f 746f 636f 6c45  se LSV2ProtocolE
+000131f0: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+00013200: 2020 2020 2020 2020 2020 2245 7272 6f72            "Error
+00013210: 2077 6869 6c65 2063 6f6e 6669 6775 7269   while configuri
+00013220: 6e67 2069 6e74 6572 7661 6c20 616e 6420  ng interval and 
+00013230: 7369 676e 616c 7322 290a 0a20 2020 2020  signals")..     
+00013240: 2020 2023 2073 6574 7570 2074 7269 6767     # setup trigg
+00013250: 6572 2061 6e64 2072 6561 6420 6461 7461  er and read data
+00013260: 2066 726f 6d20 636f 6e74 726f 6c0a 2020   from control.  
+00013270: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
+00013280: 6279 7465 6172 7261 7928 290a 2020 2020  bytearray().    
+00013290: 2020 2020 7061 796c 6f61 642e 6578 7465      payload.exte
+000132a0: 6e64 2873 7472 7563 742e 7061 636b 2822  nd(struct.pack("
+000132b0: 2148 222c 2036 2929 2020 2320 7472 6967  !H", 6))  # trig
+000132c0: 6765 7220 6368 616e 6e65 6c3f 0a20 2020  ger channel?.   
+000132d0: 2020 2020 2070 6179 6c6f 6164 2e65 7874       payload.ext
+000132e0: 656e 6428 7374 7275 6374 2e70 6163 6b28  end(struct.pack(
+000132f0: 2221 4822 2c20 3635 3533 3529 2920 2023  "!H", 65535))  #
+00013300: 2074 7269 6767 6572 206d 6f64 653f 0a20   trigger mode?. 
+00013310: 2020 2020 2020 2070 6179 6c6f 6164 2e65         payload.e
+00013320: 7874 656e 6428 7374 7275 6374 2e70 6163  xtend(struct.pac
+00013330: 6b28 2221 4c22 2c20 3029 2920 2023 2074  k("!L", 0))  # t
+00013340: 7269 6767 6572 206c 6576 656c 3f0a 2020  rigger level?.  
+00013350: 2020 2020 2020 7061 796c 6f61 642e 6578        payload.ex
+00013360: 7465 6e64 2873 7472 7563 742e 7061 636b  tend(struct.pack
+00013370: 2822 214c 222c 2030 2929 2020 2320 7072  ("!L", 0))  # pr
+00013380: 6520 7472 6967 6765 723f 0a20 2020 2020  e trigger?.     
+00013390: 2020 2070 6179 6c6f 6164 2e65 7874 656e     payload.exten
+000133a0: 6428 7374 7275 6374 2e70 6163 6b28 2221  d(struct.pack("!
+000133b0: 4c22 2c20 696e 7465 7276 616c 2929 0a0a  L", interval))..
+000133c0: 2020 2020 2020 2020 7374 6172 7420 3d20          start = 
+000133d0: 7469 6d65 2e74 696d 6528 2920 2023 2073  time.time()  # s
+000133e0: 7461 7274 2074 696d 6572 0a20 2020 2020  tart timer.     
+000133f0: 2020 2072 6563 6f72 6465 645f 6461 7461     recorded_data
+00013400: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+00013410: 2020 636f 6e74 656e 7420 3d20 7365 6c66    content = self
+00013420: 2e5f 7365 6e64 5f72 6563 6976 6528 6c63  ._send_recive(lc
+00013430: 2e43 4d44 2e52 5f4f 442c 2070 6179 6c6f  .CMD.R_OD, paylo
+00013440: 6164 2c20 6c63 2e52 5350 2e53 5f4f 4429  ad, lc.RSP.S_OD)
+00013450: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00013460: 2069 7369 6e73 7461 6e63 6528 636f 6e74   isinstance(cont
+00013470: 656e 742c 2028 6279 7465 6172 7261 792c  ent, (bytearray,
+00013480: 2929 206f 7220 6c65 6e28 636f 6e74 656e  )) or len(conten
+00013490: 7429 203c 3d20 303a 0a20 2020 2020 2020  t) <= 0:.       
+000134a0: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+000134b0: 722e 6572 726f 7228 0a20 2020 2020 2020  r.error(.       
+000134c0: 2020 2020 2020 2020 2022 736f 6d65 7468           "someth
+000134d0: 696e 6720 7765 6e74 2077 726f 6e67 2077  ing went wrong w
+000134e0: 6869 6c65 2072 6561 6469 6e67 2066 6972  hile reading fir
+000134f0: 7374 2064 6174 6120 7061 636b 6167 6520  st data package 
+00013500: 666f 7220 7369 676e 616c 7322 0a20 2020  for signals".   
+00013510: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00013520: 2020 2020 2020 2072 6169 7365 204c 5356         raise LSV
+00013530: 3250 726f 746f 636f 6c45 7863 6570 7469  2ProtocolExcepti
+00013540: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00013550: 2020 2020 2273 6f6d 6574 6869 6e67 2077      "something w
+00013560: 656e 7420 7772 6f6e 6720 7768 696c 6520  ent wrong while 
+00013570: 7265 6164 696e 6720 7363 6f70 6520 6461  reading scope da
+00013580: 7461 2229 0a0a 2020 2020 2020 2020 7265  ta")..        re
+00013590: 636f 7264 6564 5f64 6174 612e 6170 7065  corded_data.appe
+000135a0: 6e64 286c 6d73 2e64 6563 6f64 655f 7363  nd(lms.decode_sc
+000135b0: 6f70 655f 7265 6164 696e 6728 7369 676e  ope_reading(sign
+000135c0: 616c 5f6c 6973 742c 2063 6f6e 7465 6e74  al_list, content
+000135d0: 2929 0a20 2020 2020 2020 2065 6e64 203d  )).        end =
+000135e0: 2074 696d 652e 7469 6d65 2829 0a20 2020   time.time().   
+000135f0: 2020 2020 2074 696d 6572 203d 2065 6e64       timer = end
+00013600: 202d 2073 7461 7274 0a20 2020 2020 2020   - start.       
+00013610: 2077 6869 6c65 2074 696d 6572 203c 2064   while timer < d
+00013620: 7572 6174 696f 6e3a 0a20 2020 2020 2020  uration:.       
+00013630: 2020 2020 2063 6f6e 7465 6e74 203d 2073       content = s
+00013640: 656c 662e 5f6c 6c63 6f6d 2e74 656c 6567  elf._llcom.teleg
+00013650: 7261 6d28 6c63 2e52 5350 2e54 5f4f 4b29  ram(lc.RSP.T_OK)
+00013660: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013670: 7365 6c66 2e5f 6c6c 636f 6d2e 6c61 7374  self._llcom.last
+00013680: 5f72 6573 706f 6e73 6520 696e 206c 632e  _response in lc.
+00013690: 5253 502e 535f 4f44 3a0a 2020 2020 2020  RSP.S_OD:.      
+000136a0: 2020 2020 2020 2020 2020 7265 636f 7264            record
+000136b0: 6564 5f64 6174 612e 6170 7065 6e64 280a  ed_data.append(.
+000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136d0: 2020 2020 6c6d 732e 6465 636f 6465 5f73      lms.decode_s
+000136e0: 636f 7065 5f72 6561 6469 6e67 2873 6967  cope_reading(sig
+000136f0: 6e61 6c5f 6c69 7374 2c20 636f 6e74 656e  nal_list, conten
+00013700: 7429 290a 2020 2020 2020 2020 2020 2020  t)).            
+00013710: 2020 2020 7969 656c 6420 7265 636f 7264      yield record
+00013720: 6564 5f64 6174 615b 305d 0a20 2020 2020  ed_data[0].     
+00013730: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00013740: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013750: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
+00013760: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+00013770: 2020 2020 2020 2022 736f 6d65 7468 696e         "somethin
+00013780: 6720 7765 6e74 2077 726f 6e67 2064 7572  g went wrong dur
+00013790: 696e 6720 7065 7269 6f64 6963 616c 6c79  ing periodically
+000137a0: 2072 6561 6469 6e67 2073 636f 7065 2064   reading scope d
+000137b0: 6174 612c 2061 626f 7274 2072 6561 6469  ata, abort readi
+000137c0: 6e67 220a 2020 2020 2020 2020 2020 2020  ng".            
+000137d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000137e0: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+000137f0: 2020 2020 2020 2020 656e 6420 3d20 7469          end = ti
+00013800: 6d65 2e74 696d 6528 290a 2020 2020 2020  me.time().      
+00013810: 2020 2020 2020 7469 6d65 7220 3d20 656e        timer = en
+00013820: 6420 2d20 7374 6172 740a 2020 2020 2020  d - start.      
+00013830: 2020 2020 2020 7265 636f 7264 6564 5f64        recorded_d
+00013840: 6174 6120 3d20 6c69 7374 2829 0a0a 2020  ata = list()..  
+00013850: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
+00013860: 6572 2e64 6562 7567 2822 6669 6e69 7368  er.debug("finish
+00013870: 6564 2072 6561 6469 6e67 2073 636f 7065  ed reading scope
+00013880: 2064 6174 6122 290a                       data").
```

### Comparing `pyLSV2-1.1.2/pyLSV2/const.py` & `pyLSV2-1.2/pyLSV2/const.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/dat_cls.py` & `pyLSV2-1.2/pyLSV2/dat_cls.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/locales/de/LC_MESSAGES/error_text.mo` & `pyLSV2-1.2/pyLSV2/locales/de/LC_MESSAGES/error_text.mo`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/locales/de/LC_MESSAGES/message_text.mo` & `pyLSV2-1.2/pyLSV2/locales/de/LC_MESSAGES/message_text.mo`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/locales/en/LC_MESSAGES/error_text.mo` & `pyLSV2-1.2/pyLSV2/locales/en/LC_MESSAGES/error_text.mo`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/locales/en/LC_MESSAGES/message_text.mo` & `pyLSV2-1.2/pyLSV2/locales/en/LC_MESSAGES/message_text.mo`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/low_level_com.py` & `pyLSV2-1.2/pyLSV2/low_level_com.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/misc.py` & `pyLSV2-1.2/pyLSV2/misc.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/misc_scope.py` & `pyLSV2-1.2/pyLSV2/misc_scope.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2/table_reader.py` & `pyLSV2-1.2/pyLSV2/table_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,16 @@
             else:
                 units_string = " INCH"
         version_string = ""
         if self._version is not None:
             version_string = " Version:%s" % str(self._version)
 
         with open(file_path, "w", encoding="ascii") as tfp:
-            tfp.write("BEGIN %s%s%s\n" % (file_name, units_string, version_string))
+            tfp.write("BEGIN %s%s%s\n" %
+                      (file_name, units_string, version_string))
 
             for column_name in self._columns:
                 if column_name not in self._column_format:
                     raise Exception(
                         "configuration is incomplete, missing definition for column {column_name:s}"
                     )
                 fixed_width = self._column_format[column_name]["width"]
@@ -249,15 +250,16 @@
 
     def dump_csv(self, file_path: pathlib.Path, decimal_char: str = "."):
         """
         save content of table as csv file
 
         :param file_path: file location for csv file
         """
-        self._logger.debug("write table to csv, using decimal char '%s'", decimal_char)
+        self._logger.debug(
+            "write table to csv, using decimal char '%s'", decimal_char)
 
         def localize_floats(row):
             float_pattern = re.compile(r"^[+-]?\d+\.\d+$")
             for key in row.keys():
                 if float_pattern.match(row[key]):
                     row[key] = row[key].replace(".", decimal_char)
             return row
@@ -409,15 +411,15 @@
                 for line in tfp.readlines():
                     if line.startswith("[END]"):
                         break
 
                     table_entry = {}
                     for column in nctable.column_names:
                         table_entry[column] = line[
-                            nctable.get_column_start(column) : nctable.get_column_end(
+                            nctable.get_column_start(column): nctable.get_column_end(
                                 column
                             )
                         ].strip()
                     nctable.append_row(table_entry)
 
                 logger.debug("Found %d entries", len(nctable.rows))
 
@@ -502,15 +504,16 @@
             elif line.endswith(")") or line.endswith("]"):
                 object_list.pop()
             else:
                 last_object = object_list[-1]
                 if isinstance(last_object, (list,)):
                     if ":=" in line:
                         parts = line.split(":=")
-                        last_object.append({parts[0]: str_to_typed_value(parts[1])})
+                        last_object.append(
+                            {parts[0]: str_to_typed_value(parts[1])})
                     else:
                         last_object.append(line)
 
                 elif isinstance(last_object, (dict,)):
                     if ":=" in line:
                         parts = line.split(":=")
                         last_object[parts[0]] = str_to_typed_value(parts[1])
```

### Comparing `pyLSV2-1.1.2/pyLSV2/translate_messages.py` & `pyLSV2-1.2/pyLSV2/translate_messages.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/pyLSV2.egg-info/PKG-INFO` & `pyLSV2-1.2/pyLSV2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyLSV2
-Version: 1.1.2
+Version: 1.2
 Summary: A pure Python3 implementation of the LSV2 protocol
 Home-page: https://github.com/drunsinn/pyLSV2
 Author: drunsinn
 Author-email: dr.unsinn@googlemail.com
 License: MIT
 Keywords: LSV2 cnc communication transfer plc
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -133,40 +132,51 @@
  The following command reads 15 marker (bits) starting at address 32. This returns a list with 15 boolean values.
 
 ```
  con.read_plc_memory(32, pyLSV2.MemoryType.MARKER, 15)
 ```
  See [lsv2_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/lsv2_demo.py) for more examples.
 
- The available memory aread and their python data type
+ The available memory areas and their python data type
 | Memory Type              | Python Type |
 |--------------------------|-------------|
 | PLC_MEM_TYPE_MARKER      | bool        |
 | PLC_MEM_TYPE_INPUT       | bool        |
 | PLC_MEM_TYPE_OUTPUT      | bool        |
 | PLC_MEM_TYPE_COUNTER     | bool        |
 | PLC_MEM_TYPE_TIMER       | bool        |
 | PLC_MEM_TYPE_BYTE        | integer     |
 | PLC_MEM_TYPE_WORD        | integer     |
 | PLC_MEM_TYPE_DWORD       | integer     |
 | PLC_MEM_TYPE_STRING      | str         |
 | PLC_MEM_TYPE_INPUT_WORD  | integer     |
 | PLC_MEM_TYPE_OUTPUT_WORD | integer     |
 
+ Reading the values from the memory address takes the size of each memory type into account.
+
 #### Reading via Data Path
  The following command reads values from the control not via a memory address but via supplying a data access path. This will only work on iTNC controls!
  The advantage is that it also allows you to access tables like the tool table without reading the complete file.
 
 ```
  con.read_data_path('/PLC/memory/K/1')
  con.read_data_path('/TABLE/TOOL/T/1/DOC')
 ```
- 
+
  See [lsv2_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/lsv2_demo.py) for more examples.
 
+ Note that reading values from memory does not take into account the actual size in the control memory. This leads to an offset between the values read with `read_data_path` and `read_plc_memory`. As a workaround you have to multiply the address value with the number of bytes the data type requires. The following example tries to show how this can be accomplished:
+
+```
+ for mem_address in [0, 1, 2, 4, 8, 12, 68, 69, 151, 300, 368]:
+    v1 = lsv2.read_plc_memory(mem_address, pyLSV2.MemoryType.DWORD, 1)[0]
+    v2 = lsv2.read_data_path("/PLC/memory/D/%d" % (mem_address * 4))
+    assert v1 == v2
+```
+
 ### SSH Tunnel
  Newer controls allow the use of ssh to encrypt the communication via LSV2. 
  See [ssh_tunnel_demo.py](https://github.com/drunsinn/pyLSV2/blob/master/scripts/ssh_tunnel_demo.py) for an example on
  how to use the python library [sshtunnel](https://github.com/pahaz/sshtunnel) to achieve a secure connection.
 
 ## Compatibility
  Since there are a lot of different software versions and machine configurations out there
```

### Comparing `pyLSV2-1.1.2/pyLSV2.egg-info/SOURCES.txt` & `pyLSV2-1.2/pyLSV2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/lsv2_demo.py` & `pyLSV2-1.2/scripts/lsv2_demo.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/lsv2cmd.py` & `pyLSV2-1.2/scripts/lsv2cmd.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/real_time_readings.py` & `pyLSV2-1.2/scripts/real_time_readings.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/scope2csv.py` & `pyLSV2-1.2/scripts/scope2csv.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/scope_demo.py` & `pyLSV2-1.2/scripts/scope_demo.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/signals_assignment.py` & `pyLSV2-1.2/scripts/signals_assignment.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/ssh_tunnel_demo.py` & `pyLSV2-1.2/scripts/ssh_tunnel_demo.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/scripts/tab2csv.py` & `pyLSV2-1.2/scripts/tab2csv.py`

 * *Files identical despite different names*

### Comparing `pyLSV2-1.1.2/setup.py` & `pyLSV2-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     url="https://github.com/drunsinn/pyLSV2",
     license=__license__,
     install_requires=[],
     scripts=["scripts/lsv2cmd.py", "scripts/tab2csv.py", "scripts/scope2csv.py"],
     keywords="LSV2 cnc communication transfer plc",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
```

