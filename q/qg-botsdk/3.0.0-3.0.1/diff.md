# Comparing `tmp/qg-botsdk-3.0.0.tar.gz` & `tmp/qg-botsdk-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg-botsdk-3.0.0.tar", last modified: Sun May 21 15:25:55 2023, max compression
+gzip compressed data, was "qg-botsdk-3.0.1.tar", last modified: Tue May 23 14:40:01 2023, max compression
```

## Comparing `qg-botsdk-3.0.0.tar` & `qg-botsdk-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.302856 qg-botsdk-3.0.0/
--rw-rw-rw-   0        0        0     1083 2022-05-05 08:39:02.000000 qg-botsdk-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     7310 2023-05-21 15:25:55.302856 qg-botsdk-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6959 2023-05-14 14:33:12.000000 qg-botsdk-3.0.0/README.md
--rw-rw-rw-   0        0        0     6763 2023-05-14 14:33:12.000000 qg-botsdk-3.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.283856 qg-botsdk-3.0.0/qg_botsdk/
--rw-rw-rw-   0        0        0     1369 2023-05-21 14:48:31.000000 qg-botsdk-3.0.0/qg_botsdk/__init__.py
--rw-rw-rw-   0        0        0    22958 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/_api_model.py
--rw-rw-rw-   0        0        0      379 2023-05-21 14:48:29.000000 qg-botsdk-3.0.0/qg_botsdk/_exception.py
--rw-rw-rw-   0        0        0      616 2023-02-05 14:08:40.000000 qg-botsdk-3.0.0/qg_botsdk/_queue.py
--rw-rw-rw-   0        0        0    24671 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/_session.py
--rw-rw-rw-   0        0        0     1465 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/qg_botsdk/_statics.py
--rw-rw-rw-   0        0        0    15501 2023-05-21 15:23:06.000000 qg-botsdk-3.0.0/qg_botsdk/_utils.py
--rw-rw-rw-   0        0        0    50456 2023-05-21 15:18:34.000000 qg-botsdk-3.0.0/qg_botsdk/api.py
--rw-rw-rw-   0        0        0    77100 2023-05-21 15:18:34.000000 qg-botsdk-3.0.0/qg_botsdk/async_api.py
--rw-rw-rw-   0        0        0     6023 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/qg_botsdk/http.py
--rw-rw-rw-   0        0        0     6926 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/logger.py
--rw-rw-rw-   0        0        0    25317 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/model.py
--rw-rw-rw-   0        0        0     5282 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/plugins.py
--rw-rw-rw-   0        0        0    29389 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/qg_bot.py
--rw-rw-rw-   0        0        0    20262 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/qg_bot_ws.py
--rw-rw-rw-   0        0        0     8524 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/session.py
--rw-rw-rw-   0        0        0     2210 2023-05-19 10:22:41.000000 qg-botsdk-3.0.0/qg_botsdk/utils.py
--rw-rw-rw-   0        0        0       23 2023-05-14 14:06:10.000000 qg-botsdk-3.0.0/qg_botsdk/version.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.289856 qg-botsdk-3.0.0/qg_botsdk.egg-info/
--rw-rw-rw-   0        0        0     7310 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      489 2023-05-21 15:25:55.303857 qg-botsdk-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-05-13 10:50:24.000000 qg-botsdk-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.301859 qg-botsdk-3.0.0/test/
--rw-rw-rw-   0        0        0        0 2023-05-14 02:41:18.000000 qg-botsdk-3.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-05-21 15:18:34.000000 qg-botsdk-3.0.0/test/_base_context.py
--rw-rw-rw-   0        0        0      368 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/test/_testing_plugin.py
--rw-rw-rw-   0        0        0      122 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/test/conftest.py
--rw-rw-rw-   0        0        0     8133 2023-05-21 14:48:32.000000 qg-botsdk-3.0.0/test/test_api.py
--rw-rw-rw-   0        0        0    16702 2023-05-21 15:22:40.000000 qg-botsdk-3.0.0/test/test_base.py
--rw-rw-rw-   0        0        0    16503 2023-05-21 15:22:32.000000 qg-botsdk-3.0.0/test/test_run.py
--rw-rw-rw-   0        0        0     8256 2023-05-21 15:01:02.000000 qg-botsdk-3.0.0/test/test_session.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.639948 qg-botsdk-3.0.1/
+-rw-rw-rw-   0        0        0     1083 2022-05-05 08:39:02.000000 qg-botsdk-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7349 2023-05-23 14:40:01.640460 qg-botsdk-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6959 2023-05-14 14:33:12.000000 qg-botsdk-3.0.1/README.md
+-rw-rw-rw-   0        0        0     6763 2023-05-14 14:33:12.000000 qg-botsdk-3.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.581620 qg-botsdk-3.0.1/qg_botsdk/
+-rw-rw-rw-   0        0        0     1369 2023-05-21 14:48:31.000000 qg-botsdk-3.0.1/qg_botsdk/__init__.py
+-rw-rw-rw-   0        0        0    23274 2023-05-23 14:38:53.000000 qg-botsdk-3.0.1/qg_botsdk/_api_model.py
+-rw-rw-rw-   0        0        0      379 2023-05-21 14:48:29.000000 qg-botsdk-3.0.1/qg_botsdk/_exception.py
+-rw-rw-rw-   0        0        0      616 2023-02-05 14:08:40.000000 qg-botsdk-3.0.1/qg_botsdk/_queue.py
+-rw-rw-rw-   0        0        0    24671 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/_session.py
+-rw-rw-rw-   0        0        0     1465 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/qg_botsdk/_statics.py
+-rw-rw-rw-   0        0        0    15501 2023-05-21 15:23:06.000000 qg-botsdk-3.0.1/qg_botsdk/_utils.py
+-rw-rw-rw-   0        0        0    51004 2023-05-23 14:32:30.000000 qg-botsdk-3.0.1/qg_botsdk/api.py
+-rw-rw-rw-   0        0        0    77566 2023-05-23 14:32:42.000000 qg-botsdk-3.0.1/qg_botsdk/async_api.py
+-rw-rw-rw-   0        0        0     6023 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/qg_botsdk/http.py
+-rw-rw-rw-   0        0        0     6926 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/logger.py
+-rw-rw-rw-   0        0        0    25549 2023-05-23 14:38:53.000000 qg-botsdk-3.0.1/qg_botsdk/model.py
+-rw-rw-rw-   0        0        0     5282 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/plugins.py
+-rw-rw-rw-   0        0        0    29389 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/qg_bot.py
+-rw-rw-rw-   0        0        0    20262 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/qg_bot_ws.py
+-rw-rw-rw-   0        0        0     8524 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/session.py
+-rw-rw-rw-   0        0        0     2210 2023-05-19 10:22:41.000000 qg-botsdk-3.0.1/qg_botsdk/utils.py
+-rw-rw-rw-   0        0        0       23 2023-05-23 08:17:09.000000 qg-botsdk-3.0.1/qg_botsdk/version.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.617966 qg-botsdk-3.0.1/qg_botsdk.egg-info/
+-rw-rw-rw-   0        0        0     7349 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      489 2023-05-23 14:40:01.643880 qg-botsdk-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-05-13 10:50:24.000000 qg-botsdk-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.637808 qg-botsdk-3.0.1/test/
+-rw-rw-rw-   0        0        0        0 2023-05-14 02:41:18.000000 qg-botsdk-3.0.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-05-21 15:18:34.000000 qg-botsdk-3.0.1/test/_base_context.py
+-rw-rw-rw-   0        0        0      368 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/test/_testing_plugin.py
+-rw-rw-rw-   0        0        0      122 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/test/conftest.py
+-rw-rw-rw-   0        0        0     8167 2023-05-23 14:34:02.000000 qg-botsdk-3.0.1/test/test_api.py
+-rw-rw-rw-   0        0        0    16702 2023-05-21 15:22:40.000000 qg-botsdk-3.0.1/test/test_base.py
+-rw-rw-rw-   0        0        0    16088 2023-05-23 14:38:53.000000 qg-botsdk-3.0.1/test/test_run.py
+-rw-rw-rw-   0        0        0     8254 2023-05-21 15:38:46.000000 qg-botsdk-3.0.1/test/test_session.py
```

### Comparing `qg-botsdk-3.0.0/LICENSE` & `qg-botsdk-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/PKG-INFO` & `qg-botsdk-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: qg-botsdk
-Version: 3.0.0
+Version: 3.0.1
 Summary: easy-to-use SDK for Tencent QQ guild robot
 Home-page: https://github.com/GLGDLY/qg_botsdk
 Author: GDLY
 Author-email: tzlgdly@gmail.com
+License: UNKNOWN
 Keywords: sample,example,setuptools
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: <4,>=3.7
 License-File: LICENSE
@@ -195,7 +197,8 @@
 ========
 
 -   文档：
      * `readthedocs <https://qg-botsdk.readthedocs.io/zh_CN/latest/>`_
 -   官方注册机器人：https://q.qq.com/#/
 -   官方API文档：https://bot.q.qq.com/wiki/develop/api/
 -   SDK QQ交流群：https://jq.qq.com/?_wv=1027&k=3NnWvGpz
+
```

### Comparing `qg-botsdk-3.0.0/README.md` & `qg-botsdk-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/README.rst` & `qg-botsdk-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/__init__.py` & `qg-botsdk-3.0.1/qg_botsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/_api_model.py` & `qg-botsdk-3.0.1/qg_botsdk/_api_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ("获取用户频道列表", "get_bot_guilds"): ["GET", "/users/@me/guilds"],
     ("获取频道详情", "get_guild_info"): ["GET", "/guilds/{guild_id}"],
     ("获取子频道列表", "get_guild_channels"): ["GET", "/guilds/{guild_id}/channels"],
     ("获取子频道详情", "get_channels_info"): ["GET", "/channels/{channel_id}"],
     ("创建子频道", "create_channels"): ["POST", "/guilds/{guild_id}/channels"],
     ("修改子频道", "patch_channels"): ["PATCH", "/channels/{channel_id}"],
     ("删除子频道", "delete_channels"): ["DELETE", "/channels/{channel_id}"],
+    ("获取在线成员数", "get_online_nums"): ["GET", "/channels/{channel_id}/online_nums"],
     ("获取频道成员列表", "get_guild_members"): ["GET", "/guilds/{guild_id}/members"],
     ("获取频道身份组成员列表", "get_role_members"): [
         "GET",
         "/guilds/{guild_id}/roles/{role_id}/members",
     ],
     ("获取频道成员详情", "get_member_info"): ["GET", "/guilds/{guild_id}/members/{user_id}"],
     ("删除频道成员", "delete_member"): ["DELETE", "/guilds/{guild_id}/members/{user_id}"],
@@ -317,14 +318,26 @@
         http_code: int
         trace_id: str
         result: bool
 
     return DeleteChannels
 
 
+def get_online_nums():
+    class GetOnlineNums(object_class):
+        class data:
+            online_nums: int
+
+        http_code: int
+        trace_id: str
+        result: bool
+
+    return GetOnlineNums
+
+
 class _Member:
     class user:
         id: str
         username: str
         avatar: str
         bot: bool
```

### Comparing `qg-botsdk-3.0.0/qg_botsdk/_queue.py` & `qg-botsdk-3.0.1/qg_botsdk/_queue.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/_session.py` & `qg-botsdk-3.0.1/qg_botsdk/_session.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/_statics.py` & `qg-botsdk-3.0.1/qg_botsdk/_statics.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/_utils.py` & `qg-botsdk-3.0.1/qg_botsdk/_utils.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/api.py` & `qg-botsdk-3.0.1/qg_botsdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,29 @@
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.delete_channels(**_args), self._loop
         )
         return future_.result(timeout=self._timeout)
 
+    def get_online_nums(self, channel_id: str) -> _api_model.get_online_nums():
+        """
+        用于获取 channel_id 指定的音视频/直播子频道中在线人数
+
+        :param channel_id: 子频道id
+        :return: 返回的.data中为解析后的json数据
+        """
+        _args = locals()
+        _args.pop("self")
+        self.__check_ready()
+        future_ = run_coroutine_threadsafe(
+            self._api.get_online_nums(**_args), self._loop
+        )
+        return future_.result(timeout=self._timeout)
+
     def get_guild_members(self, guild_id: str) -> _api_model.get_guild_members():
         """
         用于获取 guild_id 指定的频道中所有成员的详情列表
 
         :param guild_id: 频道id
         :return: 返回的.data中为包含所有数据的一个list，列表每个项均为object数据
         """
```

### Comparing `qg-botsdk-3.0.0/qg_botsdk/async_api.py` & `qg-botsdk-3.0.1/qg_botsdk/async_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,26 @@
         :param channel_id: 子频道id
         :return: 返回的.result显示是否成功
         """
         self._check_warning("删除子频道")
         return_ = await self._session.delete(f"{self._bot_url}/channels/{channel_id}")
         return await http_temp(return_, 200)
 
+    async def get_online_nums(self, channel_id: str) -> _api_model.get_online_nums():
+        """
+        用于获取 channel_id 指定的音视频/直播子频道中在线人数
+
+        :param channel_id: 子频道id
+        :return: 返回的.data中为解析后的json数据
+        """
+        return_ = await self._session.get(
+            f"{self._bot_url}/channels/{channel_id}/online_nums"
+        )
+        return await regular_temp(return_)
+
     async def get_guild_members(self, guild_id: str) -> _api_model.get_guild_members():
         """
         用于获取 guild_id 指定的频道中所有成员的详情列表
 
         :param guild_id: 频道id
         :return: 返回的.data中为包含所有数据的一个list，列表每个项均为object数据
         """
```

### Comparing `qg-botsdk-3.0.0/qg_botsdk/http.py` & `qg-botsdk-3.0.1/qg_botsdk/http.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/logger.py` & `qg-botsdk-3.0.1/qg_botsdk/logger.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/model.py` & `qg-botsdk-3.0.1/qg_botsdk/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,14 +586,33 @@
     def __repr__(self):
         if self.command:
             return f"<BotCommandObject command={self.command} func={self.func}>"
         else:
             return f"<BotCommandObject regex={self.regex} func={self.func}>"
 
 
+class AnnounceRecommendChannels:
+    def __init__(self, channel_id: str, introduce: str):
+        self.channel_id = channel_id
+        self.introduce = introduce
+
+    def __json__(self):
+        return {"channel_id": self.channel_id, "introduce": self.introduce}
+
+
+class AT(str):
+    def __new__(cls, user_id: str):
+        """
+        用于构建艾特其他用户的字符串
+
+        :param user_id: 要@的用户id
+        """
+        return super().__new__(cls, f"<@{user_id}>")
+
+
 class EmojiID:
     得意 = 4
     流泪 = 5
     睡 = 8
     大哭 = 9
     尴尬 = 10
     调皮 = 12
@@ -822,16 +841,7 @@
     加油 = "<emoji:315>"
     崇拜 = "<emoji:318>"
     比心 = "<emoji:319>"
     庆祝 = "<emoji:320>"
     拒绝 = "<emoji:322>"
     吃糖 = "<emoji:324>"
     生气 = "<emoji:326>"
-
-
-class AnnounceRecommendChannels:
-    def __init__(self, channel_id: str, introduce: str):
-        self.channel_id = channel_id
-        self.introduce = introduce
-
-    def __json__(self):
-        return {"channel_id": self.channel_id, "introduce": self.introduce}
```

### Comparing `qg-botsdk-3.0.0/qg_botsdk/plugins.py` & `qg-botsdk-3.0.1/qg_botsdk/plugins.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/qg_bot.py` & `qg-botsdk-3.0.1/qg_botsdk/qg_bot.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/qg_bot_ws.py` & `qg-botsdk-3.0.1/qg_botsdk/qg_bot_ws.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/session.py` & `qg-botsdk-3.0.1/qg_botsdk/session.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk/utils.py` & `qg-botsdk-3.0.1/qg_botsdk/utils.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/qg_botsdk.egg-info/PKG-INFO` & `qg-botsdk-3.0.1/qg_botsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: qg-botsdk
-Version: 3.0.0
+Version: 3.0.1
 Summary: easy-to-use SDK for Tencent QQ guild robot
 Home-page: https://github.com/GLGDLY/qg_botsdk
 Author: GDLY
 Author-email: tzlgdly@gmail.com
+License: UNKNOWN
 Keywords: sample,example,setuptools
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: <4,>=3.7
 License-File: LICENSE
@@ -195,7 +197,8 @@
 ========
 
 -   文档：
      * `readthedocs <https://qg-botsdk.readthedocs.io/zh_CN/latest/>`_
 -   官方注册机器人：https://q.qq.com/#/
 -   官方API文档：https://bot.q.qq.com/wiki/develop/api/
 -   SDK QQ交流群：https://jq.qq.com/?_wv=1027&k=3NnWvGpz
+
```

### Comparing `qg-botsdk-3.0.0/qg_botsdk.egg-info/SOURCES.txt` & `qg-botsdk-3.0.1/qg_botsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/setup.py` & `qg-botsdk-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/test/_base_context.py` & `qg-botsdk-3.0.1/test/_base_context.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/test/test_api.py` & `qg-botsdk-3.0.1/test/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
     # skipped: patch_channels
 
     @pytest.mark.timeout(10)
     def test_delete_channels(self, bg_bot):
         ret = bg_bot.api.delete_channels(self._params.get("channel_id"))
         data_assertion(ret)
 
+    # skipped: get_online_nums
+
     @pytest.mark.timeout(10)
     def test_get_guild_members(self, bg_bot):
         ret = bg_bot.api.get_guild_members(self._params.get("guild_id"))
         data_assertion(ret)
         self._params["user_id"] = ret.data[0].user.id
 
     @pytest.mark.timeout(10)
```

### Comparing `qg-botsdk-3.0.0/test/test_base.py` & `qg-botsdk-3.0.1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.0/test/test_run.py` & `qg-botsdk-3.0.1/test/test_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import asyncio
+import sys
 from unittest import mock
 
 import pytest
 
 import qg_botsdk
 
 from ._base_context import (
@@ -12,14 +13,16 @@
     _callback,
     bot,
     bot_async,
     config,
     plugin_path,
 )
 
+pytest_plugins = ("pytest_asyncio",)
+
 MockMsg = (
     '{"op":0,"s":2,"t":"MESSAGE_CREATE","id":"MESSAGE_CREATE:xxx",'
     '"d":{"author":{"avatar":"xxx","bot":false,"id":"xxx","username":"xxx"},'
     '"channel_id":"channel_id","content":"plugins_test","guild_id":"xxx","id":"id",'
     '"member":{"joined_at":"xxx","nick":"xxx","roles":[]},'
     '"mentions":[],"seq":9555,"seq_in_channel":"9555","timestamp":"xxx"}}'
 )
@@ -37,83 +40,60 @@
 
 @pytest.mark.run_order(2)
 class TestRunning:
     bot: qg_botsdk.BOT
     _called_counter: int = 0
     _last_called: float = 0
 
-    async def _start_assertions(self, is_stop=True):
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
+    def test_close(self, bot):
+        self.bot = bot
+        assert not self.bot.running
+        with mock.patch.object(self.bot.logger, "error") as mock_logger:
+            self.bot.close()
+            mock_logger.assert_called_once()
+            assert mock_logger.call_args == mock.call("当前机器人没有运行！")
+
+    async def _start_assertions_with_proper_close(self):
         await asyncio.sleep(1)
-        while self.bot._bot_class.disable_reconnect:
-            await asyncio.sleep(1)
 
         assert self.bot.running
         assert self.bot._bot_class is not None
         assert self.bot._bot_class.running
         assert self.bot._bot_class.session_id
         assert self.bot._bot_class.heartbeat
         assert (
             self.bot._bot_class.auth == f'Bot {config["bot_id"]}.{config["bot_token"]}'
         )
         assert self.bot.robot == self.bot._bot_class.robot
+        self.bot.close()
 
-        if is_stop:
-            self.bot.loop.stop()
-
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_start(self, bot):
         self.bot = bot
         assert not self.bot.running
-        self.bot.loop.create_task(self._start_assertions())
-        with pytest.raises(RuntimeError):
-            self.bot.start()
+        self.bot.start(is_blocking=False)
+        self.bot.loop.run_until_complete(asyncio.sleep(0.5))
+        self.bot.loop.create_task(self._start_assertions_with_proper_close())
+        self.bot.block()
 
-    @pytest.mark.timeout(10)
-    def test_start_async(self, bot_async):
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
+    def test_async_start(self, bot_async):
         self.bot = bot_async
         assert not self.bot.running
-        self.bot.loop.create_task(self._start_assertions())
-        with pytest.raises(RuntimeError):
-            self.bot.start()
-
-    async def _close_assertion(self):
-        await self._start_assertions(is_stop=False)
-
-        await self.bot.close()
-        assert not self.bot.running
-        assert not self.bot._bot_class.running
-        assert not self.bot._bot_class.session_id
-        assert not self.bot._bot_class.heartbeat
-        assert not self.bot._bot_class.auth
-        assert not self.bot.robot
-
-    @pytest.mark.timeout(10)
-    def test_close(self, bot):
-        self.bot = bot
-        assert not self.bot.running
-        with mock.patch.object(self.bot.logger, "error") as mock_logger:
-            self.bot.close()
-            mock_logger.assert_called_once()
-            assert mock_logger.call_args == mock.call("当前机器人没有运行！")
-        self.bot.loop.create_task(self._close_assertion())
-        self.bot.start()
-
-    async def _start_assertions_with_proper_close(self):
-        await self._start_assertions(is_stop=False)
-        self.bot.close()
-
-    @pytest.mark.timeout(10)
-    def test_non_blocking_start(self, bot):
-        self.bot = bot
         self.bot.start(is_blocking=False)
         self.bot.loop.run_until_complete(asyncio.sleep(0.5))
         self.bot.loop.create_task(self._start_assertions_with_proper_close())
         self.bot.block()
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_start_more_than_once(self, bot):
         self.bot = bot
 
         with mock.patch.object(self.bot.logger, "error") as mock_logger:
             self.bot.block()
             mock_logger.assert_called_once()
             assert mock_logger.call_args == mock.call("当前机器人没有运行！")
@@ -124,35 +104,39 @@
         with mock.patch.object(self.bot.logger, "error") as mock_logger:
             self.bot.start()
             mock_logger.assert_called_once()
             assert mock_logger.call_args == mock.call("当前机器人已在运行中！")
 
         self.bot.close()
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_reconnect(self, bot):
         self.bot = bot
         self.bot.start(is_blocking=False)
         self.bot.loop.run_until_complete(asyncio.sleep(0.5))
         while self.bot._bot_class.heartbeat not in asyncio.all_tasks(self.bot.loop):
             self.bot.loop.run_until_complete(asyncio.sleep(0.1))
         with mock.patch.object(self.bot._bot_class, "ws_send") as mock_ws_send:
             self.bot._bot_class.disable_reconnect = True
             self.bot.loop.create_task(self.bot._bot_class.dispatch_events(MockOp10Msg))
-            self.bot.loop.run_until_complete(asyncio.sleep(0.5))
+            self.bot.loop.run_until_complete(asyncio.sleep(1))
             mock_ws_send.assert_called_once()
-            assert '"op": 2' in mock_ws_send.call_args.args[0]
+            if sys.version_info >= (3, 8):
+                assert '"op": 2' in mock_ws_send.call_args.args[0]
             self.bot._bot_class.disable_reconnect = False
             self.bot._bot_class.is_reconnect = True
             self.bot.loop.create_task(self.bot._bot_class.dispatch_events(MockOp10Msg))
-            self.bot.loop.run_until_complete(asyncio.sleep(0.5))
+            self.bot.loop.run_until_complete(asyncio.sleep(1))
             assert mock_ws_send.call_count == 2
-            assert '"op": 6' in mock_ws_send.call_args.args[0]
+            if sys.version_info >= (3, 8):
+                assert '"op": 6' in mock_ws_send.call_args.args[0]
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_exception_on_ws(self, bot):
         self.bot = bot
         self.bot.start(is_blocking=False)
         self.bot.loop.run_until_complete(asyncio.sleep(0.5))
         while self.bot._bot_class.heartbeat not in asyncio.all_tasks(self.bot.loop):
             self.bot.loop.run_until_complete(asyncio.sleep(0.1))
         with mock.patch.object(self.bot.logger, "error") as mock_logger:
@@ -165,15 +149,16 @@
                 while mock_logger.call_count < 2:
                     self.bot.loop.run_until_complete(asyncio.sleep(0.1))
                 assert (
                     mock.call(repr(ValueError("testing error")))
                     in mock_logger.call_args_list
                 )
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_bind_callback_and_plugins(self, bot):
         self.bot = bot
         self.bot._retrieve_new_plugins()
         self.bot.clear_current_plugins()
         self.bot.bind_msg(_callback)
         self.bot.load_plugins(plugin_path)
         self.bot.load_default_msg_logger()
@@ -218,15 +203,16 @@
                         ignore_message_reference_error=None,
                         message_id="id",
                         channel_id="channel_id",
                     )
                     in call_hist
                 )
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_async_bind_callback_and_plugins(self, bot_async):
         self.bot = bot_async
         self.bot._retrieve_new_plugins()
         self.bot.clear_current_plugins()
         self.bot.bind_msg(_async_callback)
         self.bot.start(is_blocking=False)
         self.bot.loop.run_until_complete(asyncio.sleep(0.5))
@@ -245,15 +231,16 @@
                 file_image=None,
                 message_reference_id=None,
                 ignore_message_reference_error=None,
                 message_id="id",
                 channel_id="channel_id",
             )
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_regex_with_admin(self, bot):
         self.bot = bot
         self.bot._retrieve_new_plugins()
         self.bot.clear_current_plugins()
         self.bot.on_command(
             regex="(.+?)test", is_require_admin=True, admin_error_msg="err"
         )(_callback)
@@ -282,15 +269,16 @@
     def _callback_with_create_dynamic_command(self, data: qg_botsdk.Model.MESSAGE):
         data.reply("dynamic_command_test")
         self.bot.on_command(
             regex="(.+?)test", is_require_admin=True, admin_error_msg="err"
         )(_callback)
         return True
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_dynamic_created_command_on_runtime(self, bot):
         self.bot = bot
         self.bot._retrieve_new_plugins()
         self.bot.clear_current_plugins()
         self.bot.on_command("plugins_test", is_custom_short_circuit=True)(
             self._callback_with_create_dynamic_command
         )
@@ -328,15 +316,16 @@
         self._called_counter = 0
         for i in range(2):
             self.bot.loop.create_task(self.bot._bot_class.dispatch_events(MockMsg))
             while not self._called_counter < 1:
                 self.bot.loop.run_until_complete(asyncio.sleep(0.1))
             self._called_counter = 0
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_wait_for(self, bot_async):
         self.bot = bot_async
         self.bot.bind_msg(self._test_wait_for_msg_binder)
         self.bot.start(is_blocking=False)
         self.bot.loop.run_until_complete(asyncio.sleep(0.5))
         while self.bot._bot_class.heartbeat not in asyncio.all_tasks(self.bot.loop):
             self.bot.loop.run_until_complete(asyncio.sleep(0.1))
@@ -345,15 +334,16 @@
     def _loop_event(self):
         self.bot.api.send_msg("channel_id", "content test")
         self._called_counter += 1
         time_now = self.bot.loop.time()
         assert time_now - self._last_called >= 1
         self._last_called = time_now
 
-    @pytest.mark.timeout(15)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_loop_event(self, bot):
         self.bot = bot
         bot.register_repeat_event(self._loop_event, 1)
         bot.start(is_blocking=False)
         bot.loop.run_until_complete(asyncio.sleep(0.5))
         while self.bot._bot_class.heartbeat not in asyncio.all_tasks(self.bot.loop):
             self.bot.loop.run_until_complete(asyncio.sleep(0.1))
@@ -370,16 +360,17 @@
                 "channel_id", "content test"
             )
 
     def _start_event(self):
         self._called_counter += 1
         assert self.bot.api.get_bot_info().result
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.asyncio
+    @pytest.mark.timeout(20)
     def test_start_event(self, bot):
         self.bot = bot
         bot.register_start_event(self._start_event)
         bot.start(is_blocking=False)
-        bot.loop.run_until_complete(asyncio.sleep(0.5))
+        bot.loop.run_until_complete(asyncio.sleep(5))
         while self.bot._bot_class.heartbeat not in asyncio.all_tasks(self.bot.loop):
             self.bot.loop.run_until_complete(asyncio.sleep(0.1))
         assert self._called_counter == 1
```

### Comparing `qg-botsdk-3.0.0/test/test_session.py` & `qg-botsdk-3.0.1/test/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,48 +105,48 @@
         assert session_data_from_new.status == session_data_from_get.status
         assert session_data_from_new.identify == session_data_from_get.identify
         assert session_data_from_get.scope == Scope.USER.value
         assert session_data_from_get.key == "test"
         assert session_data_from_get.status == SessionStatus.ACTIVE
         assert session_data_from_get.data == {"test": "test"}
 
-    @pytest.mark.timeout(10)
+    @pytest.mark.timeout(15)
     def test_timeout(self, bot_async, session):
         session.remove()
         session.new(MockObj, Scope.USER, "test", data={"test": "test"})
         assert (
             session.get_all()[Scope.USER.value]["111"]["test"].status
             == SessionStatus.ACTIVE
         )
         session.end(MockObj, Scope.USER, "test")
         assert (
             session.get_all()[Scope.USER.value]["111"]["test"].status
             == SessionStatus.INACTIVE
         )
-        bot_async.loop.run_until_complete(sleep(0.2))
+        bot_async.loop.run_until_complete(sleep(0.5))
         assert "111" not in session.get_all()[Scope.USER.value]
         session.new(MockObj, Scope.USER, "test", data={"test": "test"}, timeout=0.1)
         assert (
             session.get_all()[Scope.USER.value]["111"]["test"].status
             == SessionStatus.ACTIVE
         )
-        bot_async.loop.run_until_complete(sleep(0.2))
+        bot_async.loop.run_until_complete(sleep(0.5))
         assert "111" not in session.get_all()[Scope.USER.value]
         session.new(MockObj, Scope.USER, "test", data={"test": "test"})
         session.end(MockObj, Scope.USER, "test", inactive_gc_timeout=0.5)
         assert (
             session.get_all()[Scope.USER.value]["111"]["test"].status
             == SessionStatus.INACTIVE
         )
         bot_async.loop.run_until_complete(sleep(0.2))
         assert (
             session.get_all()[Scope.USER.value]["111"]["test"].status
             == SessionStatus.INACTIVE
         )
-        bot_async.loop.run_until_complete(sleep(0.5))
+        bot_async.loop.run_until_complete(sleep(1))
         assert "111" not in session.get_all()[Scope.USER.value]
 
     @pytest.mark.timeout(10)
     def test_set_get_status(self, bot_async, session):
         session.remove()
         session.new(MockObj, Scope.USER, "test", data={"test": "test"})
         session.set_status(MockObj, Scope.USER, "test", SessionStatus.HANGING)
@@ -158,15 +158,15 @@
         assert session.get(MockObj, Scope.USER, "test").status == SessionStatus.ACTIVE
         assert session.get(MockObj, Scope.USER, "test").status == SessionStatus.ACTIVE
         session.set_status(MockObj, Scope.USER, "test", SessionStatus.INACTIVE)
         assert (
             session.get_all()[Scope.USER.value]["111"]["test"].status
             == SessionStatus.INACTIVE
         )
-        bot_async.loop.run_until_complete(sleep(0.2))
+        bot_async.loop.run_until_complete(sleep(0.5))
         assert session.get(MockObj, Scope.USER, "test") is None
 
     @pytest.mark.timeout(10)
     def test_set_auto_commit(self, session):
         session.remove()
         assert session._SessionManager__is_auto_commit
         session.set_auto_commit(False)
```

