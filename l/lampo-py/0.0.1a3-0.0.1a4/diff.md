# Comparing `tmp/lampo_py-0.0.1a3.tar.gz` & `tmp/lampo_py-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampo_py-0.0.1a3.tar", max compression
+gzip compressed data, was "lampo_py-0.0.1a4.tar", max compression
```

## Comparing `lampo_py-0.0.1a3.tar` & `lampo_py-0.0.1a4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      143 2023-05-02 04:25:55.140684 lampo_py-0.0.1a3/README.md
--rw-r--r--   0        0        0       31 2023-05-02 04:25:55.140684 lampo_py-0.0.1a3/lampo_py/__init__.py
--rw-r--r--   0        0        0     1955 2023-05-02 05:31:45.809387 lampo_py-0.0.1a3/lampo_py/lampo.py
--rw-r--r--   0        0        0      432 2023-05-02 05:33:21.333143 lampo_py-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 lampo_py-0.0.1a3/setup.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-19 20:34:41.067709 lampo_py-0.0.1a4/README.md
+-rw-r--r--   0        0        0       31 2023-05-19 20:34:41.067709 lampo_py-0.0.1a4/lampo_py/__init__.py
+-rw-r--r--   0        0        0     2953 2023-05-23 20:36:58.462585 lampo_py-0.0.1a4/lampo_py/lampo.py
+-rw-r--r--   0        0        0      432 2023-05-23 21:34:12.275383 lampo_py-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a4/PKG-INFO
```

### Comparing `lampo_py-0.0.1a3/lampo_py/lampo.py` & `lampo_py-0.0.1a4/lampo_py/lampo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,58 @@
 from cffi import FFI
 
 ffi = FFI()
 
 ffi.cdef(
     """
+    /**
+    * LampoDaemon is the main data structure that uses the facade
+    * pattern to hide the complexity of the LDK library. You can interact
+    * with the LampoDaemon's components through access
+    * methods (similar to get methods in modern procedural languages).
+    *
+    * Another way to view the LampoDaemon is as
+    * a microkernel pattern, especially for developers
+    * who are interested in building their own node on
+    * top of the LampoDaemon.
+    */
     typedef struct LampoDeamon LampoDeamon;
 
     /**
     * Add a JSON RPC 2.0 Sever that listen on a unixsocket, and return a error code
     * < 0 is an error happens, or 0 is all goes well.
     */
     int64_t add_jsonrpc_on_unixsocket(struct LampoDeamon *lampod);
 
     /**
     * Allow to create a lampo deamon from a configuration patch!
     */
     void free_lampod(struct LampoDeamon *lampod);
 
+    /**
+    * Add a JSON RPC 2.0 Sever that listen on a unixsocket, and return a error code
+    * < 0 is an error happens, or 0 is all goes well.
+    */
+    const char *lampo_last_errror(void);
+
+    /**
+    * Allow to create a lampo deamon from a configuration patch!
+    */
+    void lampo_listen(struct LampoDeamon *lampod);
+
     const char *lampod_call(struct LampoDeamon *lampod, const char *method, const char *buffer);
 
     /**
     * Allow to create a lampo deamon from a configuration patch!
     */
     struct LampoDeamon *new_lampod(const char *conf_path);
-
-    void lampo_listen(struct LampoDeamon *lampod);
 """
 )
 
-lampod = ffi.dlopen("/usr/local/lib/liblampo_lib.so")
+lampod = ffi.dlopen("/usr/local/lib/liblampo.so")
 
 import json
 import logging
 from typing import Dict, Any
 
 
 class LampoDeamon:
@@ -40,21 +60,26 @@
     Python Wrapper around the Lampo Lightning Network Node
 
     Based on https://bheisler.github.io/post/calling-rust-in-python
     """
 
     def __init__(self, home_path: str) -> None:
         # FIXME: add the way to create the dir inside the lampod
+        home_path = ffi.new("char[]", home_path.encode('ascii'))
+        logging.info(f'home path {ffi.string(home_path)}')
         self.__inner = lampod.new_lampod(home_path)
+        if self.__inner == ffi.NULL:
+            err = ffi.string(lampod.lampo_last_errror())
+            raise Exception(err)
 
     def listen(self):
         """ ""
         Run The lightning node!
         """
-        lampod.add_jsonrpc_on_unixsocket(self.__inner)
+        #lampod.add_jsonrpc_on_unixsocket(self.__inner)
         lampod.lampo_listen(self.__inner)
 
     def call(self, method: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         """ " Perform a call to the lightning node"""
         result = lampod.lampod_call(self.__inner, bytes(method, "utf-8"), b"{}")
         logging.debug(f"raw data {result}")
         result = ffi.string(result).decode("utf-8")
```

### Comparing `lampo_py-0.0.1a3/PKG-INFO` & `lampo_py-0.0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lampo-py
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: 
 Author: Vincenzo Palazzo
 Author-email: vincenzopalazzodev@gmail.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

