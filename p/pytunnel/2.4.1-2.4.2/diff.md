# Comparing `tmp/pytunnel-2.4.1.tar.gz` & `tmp/pytunnel-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytunnel-2.4.1.tar", last modified: Tue May 23 02:44:15 2023, max compression
+gzip compressed data, was "dist/pytunnel-2.4.2.tar", last modified: Tue May 23 02:57:58 2023, max compression
```

## Comparing `pytunnel-2.4.1.tar` & `pytunnel-2.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:44:15.000000 pytunnel-2.4.1/
--rw-r--r--   0 Robin      (501) staff       (20)     1695 2023-05-23 02:44:15.000000 pytunnel-2.4.1/PKG-INFO
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel/
--rw-r--r--   0 Robin      (501) staff       (20)    27344 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel/tunnel.pyc
--rw-r--r--   0 Robin      (501) staff       (20)       56 2019-10-01 15:35:14.000000 pytunnel-2.4.1/pytunnel/__init__.py
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel/__pycache__/
--rw-r--r--   0 Robin      (501) staff       (20)      236 2023-05-23 02:05:20.000000 pytunnel-2.4.1/pytunnel/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 Robin      (501) staff       (20)    45061 2023-05-23 02:40:46.000000 pytunnel-2.4.1/pytunnel/__pycache__/tunnel.cpython-311.pyc
--rw-r--r--   0 Robin      (501) staff       (20)    21214 2023-05-23 02:40:22.000000 pytunnel-2.4.1/pytunnel/__pycache__/tunnel.cpython-37.pyc
--rw-r--r--   0 Robin      (501) staff       (20)      212 2020-09-24 07:58:32.000000 pytunnel-2.4.1/pytunnel/__pycache__/__main__.cpython-37.pyc
--rw-r--r--   0 Robin      (501) staff       (20)      216 2023-05-23 02:05:20.000000 pytunnel-2.4.1/pytunnel/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 Robin      (501) staff       (20)    21479 2023-05-23 02:38:37.000000 pytunnel-2.4.1/pytunnel/__pycache__/tunnel.cpython-39.pyc
--rw-r--r--   0 Robin      (501) staff       (20)      232 2020-09-24 07:58:32.000000 pytunnel-2.4.1/pytunnel/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 Robin      (501) staff       (20)      286 2023-05-23 02:07:08.000000 pytunnel-2.4.1/pytunnel/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 Robin      (501) staff       (20)      298 2023-05-23 02:07:08.000000 pytunnel-2.4.1/pytunnel/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0 Robin      (501) staff       (20)    25242 2023-05-23 02:43:22.000000 pytunnel-2.4.1/pytunnel/tunnel.py
--rw-r--r--   0 Robin      (501) staff       (20)      263 2019-10-02 16:26:54.000000 pytunnel-2.4.1/pytunnel/__init__.pyc
--rw-r--r--   0 Robin      (501) staff       (20)       64 2019-09-03 13:21:42.000000 pytunnel-2.4.1/pytunnel/__main__.py
--rw-r--r--   0 Robin      (501) staff       (20)       41 2019-09-03 11:24:00.000000 pytunnel-2.4.1/MANIFEST.in
--rw-r--r--   0 Robin      (501) staff       (20)      751 2021-05-31 15:50:19.000000 pytunnel-2.4.1/README.md
--rwxr-xr-x   0 Robin      (501) staff       (20)      745 2019-10-01 15:35:14.000000 pytunnel-2.4.1/setup.py
--rw-r--r--   0 Robin      (501) staff       (20)      192 2022-07-09 16:49:10.000000 pytunnel-2.4.1/CHANGES.md
--rw-r--r--   0 Robin      (501) staff       (20)       38 2023-05-23 02:44:15.000000 pytunnel-2.4.1/setup.cfg
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel.egg-info/
--rw-r--r--   0 Robin      (501) staff       (20)     1695 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel.egg-info/PKG-INFO
--rw-r--r--   0 Robin      (501) staff       (20)        1 2019-09-03 11:25:35.000000 pytunnel-2.4.1/pytunnel.egg-info/not-zip-safe
--rw-r--r--   0 Robin      (501) staff       (20)      705 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel.egg-info/SOURCES.txt
--rw-r--r--   0 Robin      (501) staff       (20)        9 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel.egg-info/top_level.txt
--rw-r--r--   0 Robin      (501) staff       (20)        1 2023-05-23 02:44:15.000000 pytunnel-2.4.1/pytunnel.egg-info/dependency_links.txt
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:57:58.000000 pytunnel-2.4.2/
+-rw-r--r--   0 Robin      (501) staff       (20)     2503 2023-05-23 02:57:58.000000 pytunnel-2.4.2/PKG-INFO
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel/
+-rw-r--r--   0 Robin      (501) staff       (20)    27344 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel/tunnel.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)       56 2019-10-01 15:35:14.000000 pytunnel-2.4.2/pytunnel/__init__.py
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel/__pycache__/
+-rw-r--r--   0 Robin      (501) staff       (20)      236 2023-05-23 02:05:20.000000 pytunnel-2.4.2/pytunnel/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)    45061 2023-05-23 02:40:46.000000 pytunnel-2.4.2/pytunnel/__pycache__/tunnel.cpython-311.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)    21214 2023-05-23 02:40:22.000000 pytunnel-2.4.2/pytunnel/__pycache__/tunnel.cpython-37.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)      212 2020-09-24 07:58:32.000000 pytunnel-2.4.2/pytunnel/__pycache__/__main__.cpython-37.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)      216 2023-05-23 02:05:20.000000 pytunnel-2.4.2/pytunnel/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)    21479 2023-05-23 02:38:37.000000 pytunnel-2.4.2/pytunnel/__pycache__/tunnel.cpython-39.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)      232 2020-09-24 07:58:32.000000 pytunnel-2.4.2/pytunnel/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)      286 2023-05-23 02:07:08.000000 pytunnel-2.4.2/pytunnel/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)      298 2023-05-23 02:07:08.000000 pytunnel-2.4.2/pytunnel/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)    25242 2023-05-23 02:57:05.000000 pytunnel-2.4.2/pytunnel/tunnel.py
+-rw-r--r--   0 Robin      (501) staff       (20)      263 2019-10-02 16:26:54.000000 pytunnel-2.4.2/pytunnel/__init__.pyc
+-rw-r--r--   0 Robin      (501) staff       (20)       64 2019-09-03 13:21:42.000000 pytunnel-2.4.2/pytunnel/__main__.py
+-rw-r--r--   0 Robin      (501) staff       (20)       41 2019-09-03 11:24:00.000000 pytunnel-2.4.2/MANIFEST.in
+-rw-r--r--   0 Robin      (501) staff       (20)     1367 2023-05-23 02:56:38.000000 pytunnel-2.4.2/README.md
+-rwxr-xr-x   0 Robin      (501) staff       (20)      745 2019-10-01 15:35:14.000000 pytunnel-2.4.2/setup.py
+-rw-r--r--   0 Robin      (501) staff       (20)      192 2022-07-09 16:49:10.000000 pytunnel-2.4.2/CHANGES.md
+-rw-r--r--   0 Robin      (501) staff       (20)       38 2023-05-23 02:57:58.000000 pytunnel-2.4.2/setup.cfg
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel.egg-info/
+-rw-r--r--   0 Robin      (501) staff       (20)     2503 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel.egg-info/PKG-INFO
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2019-09-03 11:25:35.000000 pytunnel-2.4.2/pytunnel.egg-info/not-zip-safe
+-rw-r--r--   0 Robin      (501) staff       (20)      705 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        9 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel.egg-info/top_level.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2023-05-23 02:57:58.000000 pytunnel-2.4.2/pytunnel.egg-info/dependency_links.txt
```

### Comparing `pytunnel-2.4.1/PKG-INFO` & `pytunnel-2.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytunnel
-Version: 2.4.1
+Version: 2.4.2
 Summary: A TCP tunnel server/client by Python.
 Home-page: https://github.com/sintrb/pytunnel/
 Author: trb
 Author-email: sintrb@gmail.com
 License: UNKNOWN
 Description: pytunnel
         ===============
@@ -33,14 +33,38 @@
         python -m pytunnel --port 1090 --target 127.0.0.1:8080 --server 192.168.1.102:1990
         ```
         
         It will make a tunnel with 192.168.1.102:1090 and 127.0.0.1:8080.
         
         Now, you can open 192.168.1.102:1090 to access the local computer port 8080.
         
+        Other
+        ===============
+        
+        You can use ```-e``` to set the password:
+        
+        ```bash
+        # server
+        python -m pytunnel --bind 0.0.0.0:1990 -e "abcdef"
+        # client
+        python -m pytunnel --port 1090 --target 127.0.0.1:8080 --server 192.168.1.102:1990 -e "abcdef"
+        ```
+        
+        Client can use ```-c``` to excute a command at the server computer:
+        
+        ```bash
+        # show server status
+        python -m pytunnel --server 192.168.1.102:1990 -c "status"
+        
+        # let server exit
+        python -m pytunnel --server 192.168.1.102:1990 -c "exit"
+        
+        # kill some client, the client-key can found with "status" command
+        python -m pytunnel --server 192.168.1.102:1990 -c "kill client-key"
+        ```
         
         [Click to view more information!](https://github.com/sintrb/pytunnel)
         
         
         CHANGES
         ===============
         1.0.0
```

### Comparing `pytunnel-2.4.1/pytunnel/tunnel.pyc` & `pytunnel-2.4.2/pytunnel/tunnel.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 4a28 6c64 6300 0000 0000 0000  ....J(ldc.......
+00000000: 03f3 0d0a 812b 6c64 6300 0000 0000 0000  .....+ldc.......
 00000010: 0003 0000 0040 0001 0073 1302 0000 6400  .....@...s....d.
 00000020: 0064 0100 6c00 006d 0100 5a01 0001 6400  .d..l..m..Z...d.
 00000030: 0064 0200 6c02 005a 0200 6400 0064 0200  .d..l..Z..d..d..
 00000040: 6c03 005a 0300 6400 0064 0200 6c04 005a  l..Z..d..d..l..Z
 00000050: 0400 6400 0064 0200 6c05 005a 0500 6403  ..d..d..l..Z..d.
 00000060: 005a 0600 6404 005a 0700 6405 005a 0800  .Z..d..Z..d..Z..
 00000070: 6406 005a 0900 642f 005a 0a00 6502 006a  d..Z..d/.Z..e..j
@@ -31,15 +31,15 @@
 000001e0: 0100 6429 0084 0000 8300 0059 5a29 0064  ..d).......YZ).d
 000001f0: 2a00 6526 0066 0100 642b 0084 0000 8300  *.e&.f..d+......
 00000200: 0059 5a2a 0064 2c00 8400 005a 2b00 642d  .YZ*.d,....Z+.d-
 00000210: 0084 0000 5a2c 0065 2d00 642e 006b 0200  ....Z,.e-.d..k..
 00000220: 720f 0265 2c00 8300 0001 6e00 0064 0200  r..e,.....n..d..
 00000230: 5328 3100 0000 69ff ffff ff28 0100 0000  S(1...i....(....
 00000240: 740e 0000 0070 7269 6e74 5f66 756e 6374  t....print_funct
-00000250: 696f 6e4e 7305 0000 0032 2e34 2e31 6914  ionNs....2.4.1i.
+00000250: 696f 6e4e 7305 0000 0032 2e34 2e32 6914  ionNs....2.4.2i.
 00000260: 0500 0069 0300 0000 693c 0000 0069 0200  ...i....i<...i..
 00000270: 0000 6900 0000 0063 0000 0000 0200 0000  ..i....c........
 00000280: 0300 0000 4700 0100 7326 0000 0064 0100  ....G...s&...d..
 00000290: 6400 006c 0000 7d01 0074 0100 7c01 006a  d..l..}..t..|..j
 000002a0: 0000 6a02 0083 0000 7c00 008c 0100 0164  ..j.....|......d
 000002b0: 0000 5328 0200 0000 4e69 ffff ffff 2803  ..S(....Ni....(.
 000002c0: 0000 0074 0800 0000 6461 7465 7469 6d65  ...t....datetime
```

### Comparing `pytunnel-2.4.1/pytunnel/__pycache__/tunnel.cpython-311.pyc` & `pytunnel-2.4.2/pytunnel/__pycache__/tunnel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pytunnel-2.4.1/pytunnel/__pycache__/tunnel.cpython-37.pyc` & `pytunnel-2.4.2/pytunnel/__pycache__/tunnel.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pytunnel-2.4.1/pytunnel/__pycache__/tunnel.cpython-39.pyc` & `pytunnel-2.4.2/pytunnel/__pycache__/tunnel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytunnel-2.4.1/pytunnel/tunnel.py` & `pytunnel-2.4.2/pytunnel/tunnel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import print_function
 
 import sys, time, json
 import socket
 
-__version__ = '2.4.1'
+__version__ = '2.4.2'
 
 READ_BUF_LEN = 1300
 TIME_WAIT_SEND_S = 3
 TIME_FOR_PING_S = 60
 TIME_FOR_DOG_TIMEOUT = 60 * 2
 IS_PY3 = sys.version_info >= (3, 0)
```

### Comparing `pytunnel-2.4.1/README.md` & `pytunnel-2.4.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -25,9 +25,33 @@
 python -m pytunnel --port 1090 --target 127.0.0.1:8080 --server 192.168.1.102:1990
 ```
 
 It will make a tunnel with 192.168.1.102:1090 and 127.0.0.1:8080.
 
 Now, you can open 192.168.1.102:1090 to access the local computer port 8080.
 
+Other
+===============
+
+You can use ```-e``` to set the password:
+
+```bash
+# server
+python -m pytunnel --bind 0.0.0.0:1990 -e "abcdef"
+# client
+python -m pytunnel --port 1090 --target 127.0.0.1:8080 --server 192.168.1.102:1990 -e "abcdef"
+```
+
+Client can use ```-c``` to excute a command at the server computer:
+
+```bash
+# show server status
+python -m pytunnel --server 192.168.1.102:1990 -c "status"
+
+# let server exit
+python -m pytunnel --server 192.168.1.102:1990 -c "exit"
+
+# kill some client, the client-key can found with "status" command
+python -m pytunnel --server 192.168.1.102:1990 -c "kill client-key"
+```
 
 [Click to view more information!](https://github.com/sintrb/pytunnel)
```

### Comparing `pytunnel-2.4.1/setup.py` & `pytunnel-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytunnel-2.4.1/pytunnel.egg-info/PKG-INFO` & `pytunnel-2.4.2/pytunnel.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytunnel
-Version: 2.4.1
+Version: 2.4.2
 Summary: A TCP tunnel server/client by Python.
 Home-page: https://github.com/sintrb/pytunnel/
 Author: trb
 Author-email: sintrb@gmail.com
 License: UNKNOWN
 Description: pytunnel
         ===============
@@ -33,14 +33,38 @@
         python -m pytunnel --port 1090 --target 127.0.0.1:8080 --server 192.168.1.102:1990
         ```
         
         It will make a tunnel with 192.168.1.102:1090 and 127.0.0.1:8080.
         
         Now, you can open 192.168.1.102:1090 to access the local computer port 8080.
         
+        Other
+        ===============
+        
+        You can use ```-e``` to set the password:
+        
+        ```bash
+        # server
+        python -m pytunnel --bind 0.0.0.0:1990 -e "abcdef"
+        # client
+        python -m pytunnel --port 1090 --target 127.0.0.1:8080 --server 192.168.1.102:1990 -e "abcdef"
+        ```
+        
+        Client can use ```-c``` to excute a command at the server computer:
+        
+        ```bash
+        # show server status
+        python -m pytunnel --server 192.168.1.102:1990 -c "status"
+        
+        # let server exit
+        python -m pytunnel --server 192.168.1.102:1990 -c "exit"
+        
+        # kill some client, the client-key can found with "status" command
+        python -m pytunnel --server 192.168.1.102:1990 -c "kill client-key"
+        ```
         
         [Click to view more information!](https://github.com/sintrb/pytunnel)
         
         
         CHANGES
         ===============
         1.0.0
```

### Comparing `pytunnel-2.4.1/pytunnel.egg-info/SOURCES.txt` & `pytunnel-2.4.2/pytunnel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

