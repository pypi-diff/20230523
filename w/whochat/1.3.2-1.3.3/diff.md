# Comparing `tmp/whochat-1.3.2.tar.gz` & `tmp/whochat-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whochat-1.3.2.tar", last modified: Tue May  9 06:17:33 2023, max compression
+gzip compressed data, was "whochat-1.3.3.tar", last modified: Tue May 23 03:09:23 2023, max compression
```

## Comparing `whochat-1.3.2.tar` & `whochat-1.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.797035 whochat-1.3.2/
--rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.2/LICENSE
--rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.2/MANIFEST.in
--rw-r--r--   0 luming     (501) staff       (20)     7346 2023-05-09 06:17:33.797110 whochat-1.3.2/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)     6693 2023-05-09 01:37:34.000000 whochat-1.3.2/README.md
--rw-r--r--   0 luming     (501) staff       (20)     1292 2023-05-09 06:17:33.797452 whochat-1.3.2/setup.cfg
--rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.2/setup.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.793158 whochat-1.3.2/whochat/
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.794836 whochat-1.3.2/whochat/ComWeChatRobot/
--rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.2/whochat/ComWeChatRobot/CWeChatRobot.exe
--rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.2/whochat/ComWeChatRobot/DWeChatRobot.dll
--rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.2/whochat/ComWeChatRobot/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)       65 2023-05-09 06:17:19.000000 whochat-1.3.2/whochat/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.2/whochat/__main__.py
--rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.2/whochat/_comtypes.py
--rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.2/whochat/abc.py
--rw-r--r--   0 luming     (501) staff       (20)    17254 2023-04-28 02:15:11.000000 whochat-1.3.2/whochat/bot.py
--rw-r--r--   0 luming     (501) staff       (20)     4952 2023-05-09 03:02:54.000000 whochat-1.3.2/whochat/cli.py
--rw-r--r--   0 luming     (501) staff       (20)      762 2023-05-09 03:05:41.000000 whochat-1.3.2/whochat/logger.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.795488 whochat-1.3.2/whochat/messages/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.2/whochat/messages/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      447 2023-03-09 10:27:55.000000 whochat-1.3.2/whochat/messages/constants.py
--rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.2/whochat/messages/tcp.py
--rw-r--r--   0 luming     (501) staff       (20)     6857 2023-04-25 09:55:38.000000 whochat-1.3.2/whochat/messages/websocket.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.795993 whochat-1.3.2/whochat/rpc/
--rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.2/whochat/rpc/__init__.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.796215 whochat-1.3.2/whochat/rpc/clients/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-03-09 10:27:55.000000 whochat-1.3.2/whochat/rpc/clients/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)     4314 2023-04-25 10:04:51.000000 whochat-1.3.2/whochat/rpc/clients/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)     1823 2023-03-09 10:27:55.000000 whochat-1.3.2/whochat/rpc/docs.py
--rw-r--r--   0 luming     (501) staff       (20)     9767 2023-03-09 10:27:55.000000 whochat-1.3.2/whochat/rpc/handlers.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.796806 whochat-1.3.2/whochat/rpc/servers/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.2/whochat/rpc/servers/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.2/whochat/rpc/servers/http.py
--rw-r--r--   0 luming     (501) staff       (20)     1138 2023-04-25 09:55:38.000000 whochat-1.3.2/whochat/rpc/servers/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)      315 2023-05-09 02:41:10.000000 whochat-1.3.2/whochat/settings.py
--rw-r--r--   0 luming     (501) staff       (20)     1108 2023-01-29 06:35:29.000000 whochat-1.3.2/whochat/signals.py
--rw-r--r--   0 luming     (501) staff       (20)     3091 2023-03-09 10:27:55.000000 whochat-1.3.2/whochat/utils.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 06:17:33.793910 whochat-1.3.2/whochat.egg-info/
--rw-r--r--   0 luming     (501) staff       (20)     7346 2023-05-09 06:17:33.000000 whochat-1.3.2/whochat.egg-info/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      870 2023-05-09 06:17:33.000000 whochat-1.3.2/whochat.egg-info/SOURCES.txt
--rw-r--r--   0 luming     (501) staff       (20)        1 2023-05-09 06:17:33.000000 whochat-1.3.2/whochat.egg-info/dependency_links.txt
--rw-r--r--   0 luming     (501) staff       (20)       50 2023-05-09 06:17:33.000000 whochat-1.3.2/whochat.egg-info/entry_points.txt
--rw-r--r--   0 luming     (501) staff       (20)      115 2023-05-09 06:17:33.000000 whochat-1.3.2/whochat.egg-info/requires.txt
--rw-r--r--   0 luming     (501) staff       (20)        8 2023-05-09 06:17:33.000000 whochat-1.3.2/whochat.egg-info/top_level.txt
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.927396 whochat-1.3.3/
+-rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.3/LICENSE
+-rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.3/MANIFEST.in
+-rw-r--r--   0 luming     (501) staff       (20)     7460 2023-05-23 03:09:23.927528 whochat-1.3.3/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)     6807 2023-05-23 03:09:03.000000 whochat-1.3.3/README.md
+-rw-r--r--   0 luming     (501) staff       (20)     1292 2023-05-23 03:09:23.928126 whochat-1.3.3/setup.cfg
+-rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.3/setup.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.921625 whochat-1.3.3/whochat/
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.924437 whochat-1.3.3/whochat/ComWeChatRobot/
+-rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/ComWeChatRobot/CWeChatRobot.exe
+-rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/ComWeChatRobot/DWeChatRobot.dll
+-rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/ComWeChatRobot/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)       65 2023-05-23 03:06:59.000000 whochat-1.3.3/whochat/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/__main__.py
+-rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/_comtypes.py
+-rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/abc.py
+-rw-r--r--   0 luming     (501) staff       (20)    18091 2023-05-23 03:05:16.000000 whochat-1.3.3/whochat/bot.py
+-rw-r--r--   0 luming     (501) staff       (20)     4952 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/cli.py
+-rw-r--r--   0 luming     (501) staff       (20)      762 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/logger.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.925272 whochat-1.3.3/whochat/messages/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/messages/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      447 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/messages/constants.py
+-rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/messages/tcp.py
+-rw-r--r--   0 luming     (501) staff       (20)     7055 2023-05-23 03:05:36.000000 whochat-1.3.3/whochat/messages/websocket.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.926343 whochat-1.3.3/whochat/rpc/
+-rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/rpc/__init__.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.926706 whochat-1.3.3/whochat/rpc/clients/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/rpc/clients/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)     4314 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/rpc/clients/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)     1823 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/rpc/docs.py
+-rw-r--r--   0 luming     (501) staff       (20)     9767 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/rpc/handlers.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.927239 whochat-1.3.3/whochat/rpc/servers/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/rpc/servers/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/rpc/servers/http.py
+-rw-r--r--   0 luming     (501) staff       (20)     1138 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/rpc/servers/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)      315 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/settings.py
+-rw-r--r--   0 luming     (501) staff       (20)     1108 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/signals.py
+-rw-r--r--   0 luming     (501) staff       (20)     3091 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/utils.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.922787 whochat-1.3.3/whochat.egg-info/
+-rw-r--r--   0 luming     (501) staff       (20)     7460 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      870 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/SOURCES.txt
+-rw-r--r--   0 luming     (501) staff       (20)        1 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/dependency_links.txt
+-rw-r--r--   0 luming     (501) staff       (20)       50 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/entry_points.txt
+-rw-r--r--   0 luming     (501) staff       (20)      115 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/requires.txt
+-rw-r--r--   0 luming     (501) staff       (20)        8 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/top_level.txt
```

### Comparing `whochat-1.3.2/LICENSE` & `whochat-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/PKG-INFO` & `whochat-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.2
+Version: 1.3.3
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
@@ -189,15 +189,19 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
-## v1.3.1
+## v1.3.3
+* 增加获取微信最新版本号的方法
+* 修复Mac用户发送@消息无法正确解析的问题
+
+## v1.3.2
 * 修改日志级别，增加日志文件记录
 
 ## v1.3.0
 * 增加RPC Websocket客户端
 * 消息转发命令行增加`--welcome`参数决定是否在客户端连接是发送"hello"
 * `hook_`方法返回路径
 * 增加`prevent_revoke`阻止文件消息被撤回时被删除
```

### Comparing `whochat-1.3.2/README.md` & `whochat-1.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -170,15 +170,19 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
-## v1.3.1
+## v1.3.3
+* 增加获取微信最新版本号的方法
+* 修复Mac用户发送@消息无法正确解析的问题
+
+## v1.3.2
 * 修改日志级别，增加日志文件记录
 
 ## v1.3.0
 * 增加RPC Websocket客户端
 * 消息转发命令行增加`--welcome`参数决定是否在客户端连接是发送"hello"
 * `hook_`方法返回路径
 * 增加`prevent_revoke`阻止文件消息被撤回时被删除
```

### Comparing `whochat-1.3.2/setup.cfg` & `whochat-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/ComWeChatRobot/CWeChatRobot.exe` & `whochat-1.3.3/whochat/ComWeChatRobot/CWeChatRobot.exe`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/ComWeChatRobot/DWeChatRobot.dll` & `whochat-1.3.3/whochat/ComWeChatRobot/DWeChatRobot.dll`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/_comtypes.py` & `whochat-1.3.3/whochat/_comtypes.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/abc.py` & `whochat-1.3.3/whochat/abc.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/bot.py` & `whochat-1.3.3/whochat/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import functools
 import json
 import os
 import pathlib
+import re
 import shutil
 import tempfile
 import threading
 import time
 from datetime import datetime
 from typing import Dict, List, Union
+from urllib import request
 
 import psutil
 
 from ._comtypes import client as com_client
 from .abc import CWechatRobotABC, RobotEventABC, RobotEventSinkABC
 from .logger import logger
 from .utils import guess_wechat_base_directory, guess_wechat_user_by_paths
@@ -568,7 +570,28 @@
         connection = com_client.GetEvents(cls.robot_event, event_sink)
         for wx_pid in wx_pids:
             cls.robot_event.CRegisterWxPidWithCookie(wx_pid, connection.cookie)
 
     @classmethod
     def get_current_dir(cls):
         return os.getcwd()
+
+    @classmethod
+    def get_latest_wechat_version(cls):
+        logger.info("获取微信最新版本号...")
+        with request.urlopen(
+            request.Request(
+                "https://pc.weixin.qq.com/?lang=zh_CN",
+                headers={
+                    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
+                },
+                method="GET",
+            )
+        ) as fp:
+            html = fp.read().decode()
+        m = re.search(r"download-version\">(.*?)</span>", html)
+        if not m:
+            logger.warning("获取微信最新版本号异常")
+            return
+        version = m.group(1)
+        logger.info(f"微信最新版本号：{version}")
+        return version
```

### Comparing `whochat-1.3.2/whochat/cli.py` & `whochat-1.3.3/whochat/cli.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/logger.py` & `whochat-1.3.3/whochat/logger.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/messages/tcp.py` & `whochat-1.3.3/whochat/messages/tcp.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/messages/websocket.py` & `whochat-1.3.3/whochat/messages/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,19 @@
 class MessageEventStoreSink(RobotEventSinkABC):
     def __init__(self, deque_: deque):
         self.deque_ = deque_
 
     @staticmethod
     def _parse_extrainfo(extrainfo):
         extra = {"is_at_msg": False}
-        m = re.search(r"<atuserlist><!\[CDATA\[(.*?)\]\]></atuserlist>", extrainfo)
+        android_windows_at_pattern = r"<atuserlist><!\[CDATA\[(.*?)\]\]></atuserlist>"
+        m = re.search(android_windows_at_pattern, extrainfo)
+        if not m:
+            mac_at_pattern = r"<atuserlist>(.*?)</atuserlist>"
+            m = re.search(mac_at_pattern, extrainfo)
         if m:
             extra["is_at_msg"] = True
             extra["at_user_list"] = m.group(1).split(",")
         m = re.search(r"<membercount>(\d+)</membercount>", extrainfo)
         if m:
             extra["member_count"] = int(m.group(1))
         return extra
```

### Comparing `whochat-1.3.2/whochat/rpc/clients/websocket.py` & `whochat-1.3.3/whochat/rpc/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/rpc/docs.py` & `whochat-1.3.3/whochat/rpc/docs.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/rpc/handlers.py` & `whochat-1.3.3/whochat/rpc/handlers.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/rpc/servers/http.py` & `whochat-1.3.3/whochat/rpc/servers/http.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/rpc/servers/websocket.py` & `whochat-1.3.3/whochat/rpc/servers/websocket.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/signals.py` & `whochat-1.3.3/whochat/signals.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat/utils.py` & `whochat-1.3.3/whochat/utils.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.2/whochat.egg-info/PKG-INFO` & `whochat-1.3.3/whochat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.2
+Version: 1.3.3
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
@@ -189,15 +189,19 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
-## v1.3.1
+## v1.3.3
+* 增加获取微信最新版本号的方法
+* 修复Mac用户发送@消息无法正确解析的问题
+
+## v1.3.2
 * 修改日志级别，增加日志文件记录
 
 ## v1.3.0
 * 增加RPC Websocket客户端
 * 消息转发命令行增加`--welcome`参数决定是否在客户端连接是发送"hello"
 * `hook_`方法返回路径
 * 增加`prevent_revoke`阻止文件消息被撤回时被删除
```

### Comparing `whochat-1.3.2/whochat.egg-info/SOURCES.txt` & `whochat-1.3.3/whochat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

