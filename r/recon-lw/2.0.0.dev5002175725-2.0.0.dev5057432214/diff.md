# Comparing `tmp/recon_lw-2.0.0.dev5002175725.tar.gz` & `tmp/recon_lw-2.0.0.dev5057432214.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5002175725.tar", last modified: Wed May 17 10:32:21 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5057432214.tar", last modified: Tue May 23 12:46:43 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5002175725.tar` & `recon_lw-2.0.0.dev5057432214.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-17 10:32:03.000000 recon_lw-2.0.0.dev5002175725/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    28052 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 10:32:21.000000 recon_lw-2.0.0.dev5002175725/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-17 10:31:41.000000 recon_lw-2.0.0.dev5002175725/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-23 12:46:23.000000 recon_lw-2.0.0.dev5057432214/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28164 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5002175725/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5057432214/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5002175725/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5057432214/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5002175725/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5057432214/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5002175725/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5057432214/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5002175725/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,16 @@
 
 def combine_operations(operations_list):
     combined_operations = [[]]
     for operation_entry in operations_list:
         if len(combined_operations[-1]) == 0:
             combined_operations[-1].append(operation_entry)
         else:
-            if operation_entry[2]["messageId"] == combined_operations[-1][-1][2]["messageId"]:
+            #if operation_entry[2]["messageId"] == combined_operations[-1][-1][2]["messageId"]:
+            if operation_entry[1]["str_time_of_event"] == combined_operations[-1][-1][1]["str_time_of_event"]:
                 combined_operations[-1].append(operation_entry)
             else:
                 combined_operations.append([operation_entry])
     return combined_operations
 
 
 def process_operations_batch(operations_batch, events, book_id ,book, check_book_rule,
```

### Comparing `recon_lw-2.0.0.dev5002175725/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5002175725/setup.py` & `recon_lw-2.0.0.dev5057432214/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5002175725/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5057432214/test/test_recon_ob.py`

 * *Files identical despite different names*

