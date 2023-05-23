# Comparing `tmp/win_defender-0.1.1.tar.gz` & `tmp/win_defender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win_defender-0.1.1.tar", max compression
+gzip compressed data, was "win_defender-0.2.0.tar", max compression
```

## Comparing `win_defender-0.1.1.tar` & `win_defender-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-05-22 08:25:36.210303 win_defender-0.1.1/LICENSE
--rw-r--r--   0        0        0      507 2023-05-22 10:39:58.877514 win_defender-0.1.1/README.md
--rw-r--r--   0        0        0      425 2023-05-22 11:02:43.147420 win_defender-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 10:03:18.011429 win_defender-0.1.1/win_defender/__init__.py
--rw-r--r--   0        0        0     1724 2023-05-22 11:02:41.126435 win_defender-0.1.1/win_defender/tools.py
--rw-r--r--   0        0        0      987 2023-05-22 10:03:18.012403 win_defender-0.1.1/win_defender/utils.py
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 win_defender-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-23 10:47:18.918465 win_defender-0.2.0/LICENSE
+-rw-r--r--   0        0        0      507 2023-05-23 10:47:18.918465 win_defender-0.2.0/README.md
+-rw-r--r--   0        0        0      425 2023-05-23 10:47:18.918465 win_defender-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 10:47:18.918465 win_defender-0.2.0/win_defender/__init__.py
+-rw-r--r--   0        0        0     2302 2023-05-23 10:47:18.918465 win_defender-0.2.0/win_defender/tools.py
+-rw-r--r--   0        0        0     1017 2023-05-23 10:47:18.918465 win_defender-0.2.0/win_defender/utils.py
+-rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 win_defender-0.2.0/PKG-INFO
```

### Comparing `win_defender-0.1.1/LICENSE` & `win_defender-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `win_defender-0.1.1/win_defender/utils.py` & `win_defender-0.2.0/win_defender/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO,
                     format='[%(asctime)s] [%(levelname)s] - %(message)s')
 
-def run_cmd(cmd:str, succ_msg:str, err_msg:str, succ_rcode:int=0) -> tuple:
+def run_cmd(cmd:str, succ_msg:str='', err_msg:str='', succ_rcode:int=None) -> tuple:
     '''Run shell commands
     
     Args:
         cmd (str): command to be executed
         succ_msg (str): message to be logged if cmd is executed successfully
         err_msg (str): message to be logged if cmd is interrupted
         succ_rcode (int): return status code after successfully executing code
@@ -21,11 +21,11 @@
     '''
     result = run(split(cmd), stderr=PIPE, stdout=PIPE)
     res = result.stdout.decode('utf-8') or result.stderr.decode('utf-8')
     rcode = result.returncode
 
     if rcode == succ_rcode:
         logger.info(succ_msg)
-    else:
+    elif rcode and succ_rcode:
         logger.error(err_msg)
 
     return (res, rcode)
```

### Comparing `win_defender-0.1.1/PKG-INFO` & `win_defender-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-defender
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tools to defend windows and get compliant with common regulations
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

