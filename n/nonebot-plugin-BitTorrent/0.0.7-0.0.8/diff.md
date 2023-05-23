# Comparing `tmp/nonebot_plugin_BitTorrent-0.0.7.tar.gz` & `tmp/nonebot_plugin_BitTorrent-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_BitTorrent-0.0.7.tar", last modified: Fri Apr 14 13:42:13 2023, max compression
+gzip compressed data, was "nonebot_plugin_BitTorrent-0.0.8.tar", last modified: Tue May 23 19:24:39 2023, max compression
```

## Comparing `nonebot_plugin_BitTorrent-0.0.7.tar` & `nonebot_plugin_BitTorrent-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:13.252030 nonebot_plugin_BitTorrent-0.0.7/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_BitTorrent-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      305 2023-04-14 13:42:13.251028 nonebot_plugin_BitTorrent-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2022-06-23 16:37:02.000000 nonebot_plugin_BitTorrent-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:13.244030 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/
--rw-rw-rw-   0        0        0      217 2023-04-14 12:38:11.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/__init__.py
--rw-rw-rw-   0        0        0     6121 2023-04-14 13:36:51.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:13.250030 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/
--rw-rw-rw-   0        0        0      305 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 13:42:13.252030 nonebot_plugin_BitTorrent-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      534 2023-04-14 13:42:01.000000 nonebot_plugin_BitTorrent-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:24:39.585351 nonebot_plugin_BitTorrent-0.0.8/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_BitTorrent-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      305 2023-05-23 19:24:39.584352 nonebot_plugin_BitTorrent-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2022-06-23 16:37:02.000000 nonebot_plugin_BitTorrent-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 19:24:39.572568 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/
+-rw-rw-rw-   0        0        0      502 2023-05-23 19:24:17.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/__init__.py
+-rw-rw-rw-   0        0        0     6162 2023-05-23 19:17:30.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:24:39.582831 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-23 19:24:39.000000 nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 19:24:39.585351 nonebot_plugin_BitTorrent-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      534 2023-05-23 19:23:27.000000 nonebot_plugin_BitTorrent-0.0.8/setup.py
```

### Comparing `nonebot_plugin_BitTorrent-0.0.7/LICENSE` & `nonebot_plugin_BitTorrent-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_BitTorrent-0.0.7/README.md` & `nonebot_plugin_BitTorrent-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/utils.py` & `nonebot_plugin_BitTorrent-0.0.8/nonebot_plugin_BitTorrent/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import nonebot
 from bs4 import BeautifulSoup
 from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import Message
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
-
+from urllib.parse import unquote
 
 class BitTorrent:
     def __init__(self) -> None:
         """初始化一些变量, 用env拿到magnet_max_num参数"""
         try:
             self.max_num = nonebot.get_driver().config.magnet_max_num
         except Exception:
@@ -127,13 +127,13 @@
 
 
     async def release_b64(self, target: str) -> str:
         """解除网页的base64加密, 传入get得到的text"""
         soup = BeautifulSoup(target, "lxml")
         script = soup.find_all("script")[-1]
         script = str(script).split('"')[1]
-        return base64.b64decode(script).decode()
+        return unquote(base64.b64decode(script).decode())
 
     
 
 # 实例化
 bittorrent = BitTorrent()
```

### Comparing `nonebot_plugin_BitTorrent-0.0.7/setup.py` & `nonebot_plugin_BitTorrent-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_BitTorrent'
 
 setup(
     name=name,  
-    version='0.0.7',
+    version='0.0.8',
     author="Special-Week",
     author_email='2749903559@qq.com',
     description="encapsulate logger",
-    python_requires=">=3.8.*",
+    python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="nonebot2磁力搜索插件",
     url="https://github.com/Special-Week/nonebot_plugin_BitTorrent",
 
     # 设置依赖包
     install_requires=["lxml","httpx","bs4","nonebot2","nonebot-adapter-onebot"],
 )
```

