# Comparing `tmp/eventloop-0.0.8.tar.gz` & `tmp/eventloop-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventloop-0.0.8.tar", last modified: Wed Jun 30 18:31:52 2021, max compression
+gzip compressed data, was "eventloop-0.0.9.tar", last modified: Tue Jul  6 14:36:38 2021, max compression
```

## Comparing `eventloop-0.0.8.tar` & `eventloop-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-06-30 18:31:52.768154 eventloop-0.0.8/
--rw-rw-rw-   0        0        0     4182 2021-06-30 18:31:52.767164 eventloop-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2021-06-07 15:05:30.000000 eventloop-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2021-06-30 18:31:52.761158 eventloop-0.0.8/eventloop/
--rw-rw-rw-   0        0        0     3273 2021-06-30 18:19:29.000000 eventloop-0.0.8/eventloop/__init__.py
--rw-rw-rw-   0        0        0     2214 2021-05-19 17:03:03.000000 eventloop-0.0.8/eventloop/__main__.py
--rw-rw-rw-   0        0        0     1114 2021-06-07 13:03:18.000000 eventloop-0.0.8/eventloop/base.py
--rw-rw-rw-   0        0        0     1898 2021-05-19 16:17:17.000000 eventloop-0.0.8/eventloop/common.py
--rw-rw-rw-   0        0        0     2285 2021-05-19 16:24:54.000000 eventloop-0.0.8/eventloop/qt.py
--rw-rw-rw-   0        0        0     2597 2021-05-19 16:32:51.000000 eventloop-0.0.8/eventloop/uv.py
-drwxrwxrwx   0        0        0        0 2021-06-30 18:31:52.766155 eventloop-0.0.8/eventloop.egg-info/
--rw-rw-rw-   0        0        0     4182 2021-06-30 18:31:52.000000 eventloop-0.0.8/eventloop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2021-06-30 18:31:52.000000 eventloop-0.0.8/eventloop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-30 18:31:52.000000 eventloop-0.0.8/eventloop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-06-30 18:31:52.000000 eventloop-0.0.8/eventloop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-06-30 18:31:52.768154 eventloop-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      452 2021-06-30 18:30:30.000000 eventloop-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-06 14:36:38.367194 eventloop-0.0.9/
+-rw-rw-rw-   0        0        0     4182 2021-07-06 14:36:38.367194 eventloop-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2021-06-07 15:05:30.000000 eventloop-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2021-07-06 14:36:38.363196 eventloop-0.0.9/eventloop/
+-rw-rw-rw-   0        0        0     3273 2021-07-06 14:12:48.000000 eventloop-0.0.9/eventloop/__init__.py
+-rw-rw-rw-   0        0        0     2214 2021-05-19 17:03:03.000000 eventloop-0.0.9/eventloop/__main__.py
+-rw-rw-rw-   0        0        0     1114 2021-07-06 14:12:39.000000 eventloop-0.0.9/eventloop/base.py
+-rw-rw-rw-   0        0        0     1898 2021-05-19 16:17:17.000000 eventloop-0.0.9/eventloop/common.py
+-rw-rw-rw-   0        0        0     2285 2021-07-06 14:12:32.000000 eventloop-0.0.9/eventloop/qt.py
+-rw-rw-rw-   0        0        0     2615 2021-07-06 14:14:28.000000 eventloop-0.0.9/eventloop/uv.py
+drwxrwxrwx   0        0        0        0 2021-07-06 14:36:38.366195 eventloop-0.0.9/eventloop.egg-info/
+-rw-rw-rw-   0        0        0     4182 2021-07-06 14:36:38.000000 eventloop-0.0.9/eventloop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2021-07-06 14:36:38.000000 eventloop-0.0.9/eventloop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-06 14:36:38.000000 eventloop-0.0.9/eventloop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2021-07-06 14:36:38.000000 eventloop-0.0.9/eventloop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-06 14:36:38.367194 eventloop-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      452 2021-07-06 14:35:55.000000 eventloop-0.0.9/setup.py
```

### Comparing `eventloop-0.0.8/PKG-INFO` & `eventloop-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: eventloop
-Version: 0.0.8
+Version: 0.0.9
 Summary: Abstraction layer for filesystem events
 Home-page: https://github.com/mugiseyebrows/event-loop
 Author: Stanislav Doronin
 Author-email: mugisbrows@gmail.com
 License: UNKNOWN
 Description: ==================================================
         eventloop: Abstraction layer for filesystem events
```

### Comparing `eventloop-0.0.8/README.rst` & `eventloop-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `eventloop-0.0.8/eventloop/__init__.py` & `eventloop-0.0.9/eventloop/__init__.py`

 * *Files identical despite different names*

### Comparing `eventloop-0.0.8/eventloop/__main__.py` & `eventloop-0.0.9/eventloop/__main__.py`

 * *Files identical despite different names*

### Comparing `eventloop-0.0.8/eventloop/base.py` & `eventloop-0.0.9/eventloop/base.py`

 * *Files identical despite different names*

### Comparing `eventloop-0.0.8/eventloop/common.py` & `eventloop-0.0.9/eventloop/common.py`

 * *Files identical despite different names*

### Comparing `eventloop-0.0.8/eventloop/qt.py` & `eventloop-0.0.9/eventloop/qt.py`

 * *Files identical despite different names*

### Comparing `eventloop-0.0.8/eventloop/uv.py` & `eventloop-0.0.9/eventloop/uv.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,31 +57,31 @@
         super().start(path, callback, include, exclude, recursive)
         if sys.platform not in ['win32','darwin'] and recursive:
             print("Warning: recursive not implemented for this platform")
             # TODO: workaround for recursive
         loop = pyuv.Loop.default_loop()
         handle = pyuv.fs.FSEvent(loop)
         UV_FS_EVENT_RECURSIVE = 4
-        handle.start(path, UV_FS_EVENT_RECURSIVE if recursive else 0, self.onPyuvChanged)
+        handle.start(path, UV_FS_EVENT_RECURSIVE if recursive else 0, self.onChanged)
         handle.ref = False
         self._watch = handle
+        self._isdir = os.path.isdir(path)
 
     def stop(self):
         pass
 
-    def onPyuvChanged(self, handle, filename, events, error):
+    def onChanged(self, handle, filename, events, error):
         events_ = []
 
-        if os.path.isfile(self._path):
-            path = self._path
-        else:
+        if self._isdir:
             path = os.path.join(self._path, filename)
-        
-        if not path_matches(path, self._include, self._exclude):
-            return
+            if not path_matches(path, self._include, self._exclude):
+                return
+        else:
+            path = self._path
 
         if events & pyuv.fs.UV_RENAME:
             events_.append(EVENT_RENAME)
             
         if events & pyuv.fs.UV_CHANGE:
             events_.append(EVENT_CHANGE)
```

### Comparing `eventloop-0.0.8/eventloop.egg-info/PKG-INFO` & `eventloop-0.0.9/eventloop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: eventloop
-Version: 0.0.8
+Version: 0.0.9
 Summary: Abstraction layer for filesystem events
 Home-page: https://github.com/mugiseyebrows/event-loop
 Author: Stanislav Doronin
 Author-email: mugisbrows@gmail.com
 License: UNKNOWN
 Description: ==================================================
         eventloop: Abstraction layer for filesystem events
```

