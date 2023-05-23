# Comparing `tmp/pymycobot-3.0.9.tar.gz` & `tmp/pymycobot-3.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.0.9.tar", last modified: Thu Apr 27 09:44:30 2023, max compression
+gzip compressed data, was "pymycobot-3.1.0b1.tar", last modified: Tue May 23 05:46:01 2023, max compression
```

## Comparing `pymycobot-3.0.9.tar` & `pymycobot-3.1.0b1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 09:44:30.425070 pymycobot-3.0.9/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.0.9/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0    55518 2023-04-27 09:44:30.424054 pymycobot-3.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 09:44:30.366654 pymycobot-3.0.9/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.0.9/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1560 2023-04-27 09:42:11.000000 pymycobot-3.0.9/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2022-07-18 09:51:08.000000 pymycobot-3.0.9/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    12065 2023-03-06 07:56:35.000000 pymycobot-3.0.9/pymycobot/common.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.0.9/pymycobot/error.py
--rw-rw-rw-   0        0        0    32911 2023-03-13 09:04:37.000000 pymycobot-3.0.9/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.0.9/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.0.9/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.0.9/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8869 2023-01-10 08:08:44.000000 pymycobot-3.0.9/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13315 2023-04-14 05:34:53.000000 pymycobot-3.0.9/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.0.9/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.0.9/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.0.9/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7351 2022-11-29 03:08:51.000000 pymycobot-3.0.9/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7441 2022-06-28 10:56:36.000000 pymycobot-3.0.9/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8420 2022-11-14 07:30:15.000000 pymycobot-3.0.9/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7445 2022-10-20 05:52:29.000000 pymycobot-3.0.9/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19564 2023-04-27 09:34:23.000000 pymycobot-3.0.9/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.0.9/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 09:44:30.419985 pymycobot-3.0.9/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    55518 2023-04-27 09:44:29.000000 pymycobot-3.0.9/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-04-27 09:44:30.000000 pymycobot-3.0.9/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 09:44:29.000000 pymycobot-3.0.9/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 09:44:29.000000 pymycobot-3.0.9/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 09:44:29.000000 pymycobot-3.0.9/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 09:44:30.426080 pymycobot-3.0.9/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:46:01.789836 pymycobot-3.1.0b1/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    55520 2023-05-23 05:46:01.788772 pymycobot-3.1.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.0b1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 05:46:01.754319 pymycobot-3.1.0b1/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.0b1/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1562 2023-05-23 05:45:44.000000 pymycobot-3.1.0b1/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2022-07-18 09:51:08.000000 pymycobot-3.1.0b1/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    12065 2023-03-06 07:56:35.000000 pymycobot-3.1.0b1/pymycobot/common.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/error.py
+-rw-rw-rw-   0        0        0    32911 2023-03-13 09:04:37.000000 pymycobot-3.1.0b1/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.0b1/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8869 2023-01-10 08:08:44.000000 pymycobot-3.1.0b1/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13315 2023-04-14 05:34:53.000000 pymycobot-3.1.0b1/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.0b1/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.0b1/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.0b1/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7414 2023-05-23 05:42:22.000000 pymycobot-3.1.0b1/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7441 2022-06-28 10:56:36.000000 pymycobot-3.1.0b1/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8483 2023-05-23 05:43:01.000000 pymycobot-3.1.0b1/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7445 2022-10-20 05:52:29.000000 pymycobot-3.1.0b1/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19564 2023-04-27 09:34:23.000000 pymycobot-3.1.0b1/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:46:01.785533 pymycobot-3.1.0b1/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    55520 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 05:46:01.789836 pymycobot-3.1.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.0b1/setup.py
```

### Comparing `pymycobot-3.0.9/LICENSE` & `pymycobot-3.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/PKG-INFO` & `pymycobot-3.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.0.9
+Version: 3.1.0b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.0.9/README.md` & `pymycobot-3.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/Interface.py` & `pymycobot-3.1.0b1/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/__init__.py` & `pymycobot-3.1.0b1/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.0.9"
+__version__ = "3.1.0b1"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.0.9/pymycobot/bluet.py` & `pymycobot-3.1.0b1/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/common.py` & `pymycobot-3.1.0b1/pymycobot/common.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/error.py` & `pymycobot-3.1.0b1/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/generate.py` & `pymycobot-3.1.0b1/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/log.py` & `pymycobot-3.1.0b1/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/myarm.py` & `pymycobot-3.1.0b1/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/mybuddy.py` & `pymycobot-3.1.0b1/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.0b1/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.0b1/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/mybuddysocket.py` & `pymycobot-3.1.0b1/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/mycobot.py` & `pymycobot-3.1.0b1/pymycobot/mycobot.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,7 +205,10 @@
         self.gpio.setup(pin, self.gpio.OUT)
         self.gpio.output(pin, v)
 
     # Other
     def wait(self, t):
         time.sleep(t)
         return self
+    
+    def close(self):
+        self._serial_port.close()
```

### Comparing `pymycobot-3.0.9/pymycobot/mycobotsocket.py` & `pymycobot-3.1.0b1/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/mypalletizer.py` & `pymycobot-3.1.0b1/pymycobot/mypalletizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,7 +238,10 @@
             value: 
                 0 - Get data from a 3-axis gyroscope.\n
                 1 - Get data from a 2-axis gyroscope.
             
         """
         data_list = [[25, 21], [26, 32]]
         return self._mesg(ProtocolCode.GET_ACCEI_DATA, data_list[1] if value else data_list[0], has_reply=True)
+    
+    def close(self):
+        self._serial_port.close()
```

### Comparing `pymycobot-3.0.9/pymycobot/mypalletizersocket.py` & `pymycobot-3.1.0b1/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/ultraArm.py` & `pymycobot-3.1.0b1/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot/utils.py` & `pymycobot-3.1.0b1/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.0b1/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.0.9
+Version: 3.1.0b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.0.9/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.0b1/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.9/setup.py` & `pymycobot-3.1.0b1/setup.py`

 * *Files identical despite different names*

