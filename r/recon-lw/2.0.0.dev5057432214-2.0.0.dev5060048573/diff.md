# Comparing `tmp/recon_lw-2.0.0.dev5057432214.tar.gz` & `tmp/recon_lw-2.0.0.dev5060048573.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5057432214.tar", last modified: Tue May 23 12:46:43 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5060048573.tar", last modified: Tue May 23 17:01:34 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5057432214.tar` & `recon_lw-2.0.0.dev5060048573.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-23 12:46:23.000000 recon_lw-2.0.0.dev5057432214/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    28164 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:46:43.000000 recon_lw-2.0.0.dev5057432214/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-23 12:46:16.000000 recon_lw-2.0.0.dev5057432214/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-23 17:01:13.000000 recon_lw-2.0.0.dev5060048573/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28164 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 17:01:34.000000 recon_lw-2.0.0.dev5060048573/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-23 17:01:04.000000 recon_lw-2.0.0.dev5060048573/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5057432214/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5060048573/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5057432214/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5060048573/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5057432214/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5060048573/recon_lw/TimeCacheMatcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,51 +9,60 @@
         self._time_index = SortedKeyList(key=lambda t: recon_lw.time_stamp_key(t[0]))
         self._get_timestamp_key1_key2 = get_timestamp_key1_key2
         self._interpret_func = interpret_func
         self._create_event = create_event
         self._send_events = send_events
         self._horizon_delay_seconds = horizon_delay_seconds
         self._custom_settings = custom_settings
+        self._debug = True
+
+    def debug(self, body):
+        ev = self._create_event("TCMDebug", "TCMDebug", True, message_dict)
+        self._send_events([ev])
 
     def process_objects_batch(self, batch: list) -> None:
         stream_time = None
         for o in batch:
             ts, key1, key2 = self._get_timestamp_key1_key2(o, self._custom_settings)
-            log_event = self._create_event("MatcherLog" + str(self._custom_settings),
-                                           "MatcherLog",
-                                           False,
-                                           {"ts": ts,
-                                            "key1": key1,
-                                            "key2": key2,
-                                            "sourceEvent": o})
-            self._send_events([log_event])
             if ts is None:
                 continue
             stream_time = ts
             if key1 is not None:
                 if key1 not in self._match_index:
                     self._match_index[key1] = [o, None]
                     self._time_index.add([ts, key1])
+                    if self._debug:
+                        self.debug({"event": "key1 added", "key": key1, "ts": ts})
                 else:
                     self._match_index[key1][0] = o
+                    if self._debug:
+                        self.debug({"event": "key1 updated", "key": key1, "ts": ts})
             elif key2 is not None:
                 if key2 not in self._match_index:
                     self._match_index[key2] = [None, o]
                     self._time_index.add([ts, key2])
+                    if self._debug:
+                        self.debug({"event": "key2 added", "key": key2, "ts": ts})
                 else:
                     self._match_index[key2][1] = o
+                    if self._debug:
+                        self.debug({"event": "key2 updated", "key": key2, "ts": ts})
 
         if stream_time is not None:
             edge_timestamp = {"epochSecond": stream_time["epochSecond"] - self._horizon_delay_seconds,
                               "nano": 0}
             horizon_edge = self._time_index.bisect_key_left(recon_lw.time_stamp_key(edge_timestamp))
             if horizon_edge > 0:
                 for n in range(horizon_edge):
                     nxt = self._time_index.pop(0)
                     match = self._match_index.pop(nxt[1])
                     self._interpret_func(match, self._custom_settings, self._create_event, self._send_events)
+                    if self._debug:
+                        self.debug({"event": "key processed", "key": nxt, "ts": stream_time})
 
     def flush_all(self) -> None:
         self._time_index.clear()
-        for match in self._match_index.values():
+        for key, match in self._match_index.items():
             self._interpret_func(match, self._custom_settings, self._create_event, self._send_events)
+            if self._debug:
+                self.debug({"event": "key processed at the end", "key": key, "ts": None})
         self._match_index.clear()
```

### Comparing `recon_lw-2.0.0.dev5057432214/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5060048573/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5060048573/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5057432214/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5060048573/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5057432214/setup.py` & `recon_lw-2.0.0.dev5060048573/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5057432214/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5060048573/test/test_recon_ob.py`

 * *Files identical despite different names*

