# Comparing `tmp/dingtalk2-0.1.1.tar.gz` & `tmp/dingtalk2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk2-0.1.1.tar", max compression
+gzip compressed data, was "dingtalk2-0.1.2.tar", max compression
```

## Comparing `dingtalk2-0.1.1.tar` & `dingtalk2-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-25 16:05:24.322545 dingtalk2-0.1.1/LICENSE
--rw-r--r--   0        0        0      904 2023-04-25 16:05:24.322749 dingtalk2-0.1.1/README.md
--rw-r--r--   0        0        0      114 2023-05-22 15:29:39.421324 dingtalk2-0.1.1/dingtalk2/__init__.py
--rw-r--r--   0        0        0    10480 2023-05-22 15:26:01.155034 dingtalk2-0.1.1/dingtalk2/dingtalk.py
--rw-r--r--   0        0        0       98 2021-11-22 11:13:38.082454 dingtalk2-0.1.1/dingtalk2/exceptions.py
--rw-r--r--   0        0        0     5373 2023-05-22 15:14:59.343673 dingtalk2-0.1.1/dingtalk2/items.py
--rw-r--r--   0        0        0      298 2023-05-22 15:14:12.650930 dingtalk2-0.1.1/dingtalk2/logger.py
--rw-r--r--   0        0        0     1661 2023-05-22 15:27:29.054233 dingtalk2-0.1.1/dingtalk2/request.py
--rw-r--r--   0        0        0      419 2021-11-22 11:13:38.082852 dingtalk2-0.1.1/dingtalk2/utils.py
--rw-r--r--   0        0        0      872 2023-05-22 15:29:39.443474 dingtalk2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 dingtalk2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-23 03:52:24.950537 dingtalk2-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1274 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/README.md
+-rw-r--r--   0        0        0      114 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/constants.py
+-rw-r--r--   0        0        0    10612 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/dingtalk.py
+-rw-r--r--   0        0        0       98 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/exceptions.py
+-rw-r--r--   0        0        0     4415 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/items.py
+-rw-r--r--   0        0        0      328 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/logger.py
+-rw-r--r--   0        0        0     1613 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/request.py
+-rw-r--r--   0        0        0      419 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/dingtalk2/utils.py
+-rw-r--r--   0        0        0     1103 2023-05-23 03:52:24.954537 dingtalk2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 dingtalk2-0.1.2/setup.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 dingtalk2-0.1.2/PKG-INFO
```

### Comparing `dingtalk2-0.1.1/LICENSE` & `dingtalk2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk2-0.1.1/dingtalk2/dingtalk.py` & `dingtalk2-0.1.2/dingtalk2/dingtalk.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,147 +2,148 @@
 import hashlib
 import hmac
 import queue
 import re
 import time
 from urllib.parse import quote_plus
 
+from .constants import HEADERS, GATEWAY
 from .items import ActionCard
 from .items import CardItem
 from .items import FeedLink
 from .logger import logger
 from .request import Request
 from .utils import is_not_null_and_blank_str
 
 
 class DingTalk:
     """
     钉钉群自定义机器人（每个机器人每分钟最多发送20条），支持文本（text）、连接（link）、markdown三种消息类型！
     """
 
-    gateway = 'https://oapi.dingtalk.com/robot/send'
-    headers = {'Content-Type': 'application/json; charset=utf-8'}
-    options = {}
-    webhook = ''
+    # gateway = 'https://oapi.dingtalk.com/robot/send'
+    # headers = {'Content-Type': 'application/json; charset=utf-8'}
+    # options = {}
+    # webhook = ''
     session: Request
 
-    def __init__(self, access: str = '', secret=None, pc_slide=False, fail_notice=False):
+    def __init__(self, access: str = None, secret: str = None, pc_slide=False, fail_notice=False):
         """
         机器人初始化
         :param access: 钉钉群自定义机器人webhook地址
         :param secret: 机器人安全设置页面勾选“加签”时需要传入的密钥
         :param pc_slide: 消息链接打开方式，默认False为浏览器打开，设置为True时为PC端侧边栏打开
         :param fail_notice: 消息发送失败提醒，默认为False不提醒，开发者可以根据返回的消息发送结果自行判断和处理
         """
 
         self.queue = queue.Queue(20)  # 钉钉官方限流每分钟发送20条信息
         self.secret = secret
 
         # self.webhook = f"https://oapi.dingtalk.com/robot/send?access_token={access}"
-        self.options = {'access_token': access, }
+        self.options = {'access_token': access}
 
         self.fail_notice = fail_notice
         self.start_time = time.time()
         self.pc_slide = pc_slide
 
         # 初始化参数
-        self._initialize()
+        self._signature()
 
-    def _initialize(self):
+    def _signature(self):
         """ 钉钉群自定义机器人安全设置加签时，签名中的时间戳与请求时不能超过一个小时，所以每个1小时需要更新签名 """
         if self.secret and self.secret.startswith('SEC'):
             timestamp = round(self.start_time * 1000)
             string_to_sign = f'{timestamp}\n{self.secret}'
 
             code = hmac.new(self.secret.encode(), string_to_sign.encode(), digestmod=hashlib.sha256).digest()
             sign = quote_plus(base64.b64encode(code))
 
             self.options.update({'timestamp': timestamp, 'sign': sign})
 
-        self.session = Request(webhook=self.gateway, headers=self.headers, options=self.options)
+        self.session = Request(webhook=GATEWAY, headers=HEADERS, options=self.options)
 
     def _open_type(self, url):
         """ 消息链接的打开方式
         1、默认或不设置时，为浏览器打开：pc_slide=False
         2、在PC端侧边栏打开：pc_slide=True
         """
-        slide = 'true' if self.pc_slide else 'false'
+        slide = ('false', 'true')[bool(self.pc_slide)]
 
         return f'dingtalk://dingtalkclient/page/link?url={quote_plus(url)}&pc_slide={slide}'
 
     def text(self, msg, at_all=False, at: list = None, at_ids: list = None, auto_at=True):
         """ text类型
         :type at_ids: object
         :param msg: 消息内容
         :param at_all: @所有人时：true，否则为false（可选）
         :param at: 被@人的手机号（注意：可以在msg内容里自定义@手机号的位置，也支持同时@多个手机号，可选）
         :param at_ids: 被@人的dingtalkId（可选）
         :param auto_at: 是否自动在msg内容末尾添加@手机号，默认自动添加，可设置为False取消（可选）
         :return: 返回消息发送结果
         """
-        data = {'msgtype': 'text', 'at': {}}
+        payload = {'msgtype': 'text', 'at': {}}
 
         if not is_not_null_and_blank_str(msg):
             raise ValueError('text类型，消息内容不能为空！')
 
-        data['text'] = {'content': msg}
+        payload['text'] = {'content': msg}
 
         if at_all:
-            data['at']['isAtAll'] = at_all
+            payload['at']['isAtAll'] = at_all
 
         if at:
             at = list(map(str, at))
-            data['at']['atMobiles'] = at
+            payload['at']['atMobiles'] = at
 
             if auto_at:
                 mobiles_text = '\n@' + '@'.join(at)
-                data['text']['content'] = msg + mobiles_text
+                payload['text']['content'] = msg + mobiles_text
 
         if at_ids:
             at_ids = list(map(str, at_ids))
-            data['at']['atDingtalkIds'] = at_ids
+            payload['at']['atDingtalkIds'] = at_ids
 
-        logger.debug(f'text类型：{data}')
+        logger.debug(f'text类型：{payload}')
 
-        return self._request(data)
+        return self._request(payload)
 
     def image(self, pic_url):
         """ image类型（表情）
         :param pic_url: 图片链接
         :return: 返回消息发送结果
         """
         if is_not_null_and_blank_str(pic_url):
             data = {'msgtype': 'image', 'image': {'picURL': pic_url}}
-            logger.debug('image类型：%s' % data)
+            logger.debug(f'image类型：{data}')
             return self._request(data)
 
         raise ValueError('image类型中图片链接不能为空！')
 
     def link(self, title, text, message_url, pic_url=''):
         """ link类型
         :param title: 消息标题
         :param text: 消息内容（如果太长自动省略显示）
         :param message_url: 点击消息触发的URL
         :param pic_url: 图片URL（可选）
         :return: 返回消息发送结果
 
         """
         if all(map(is_not_null_and_blank_str, [title, text, message_url])):
-            data = {
+            payload = {
                 'msgtype': 'link',
                 'link': {
                     'text': text,
                     'title': title,
                     'picUrl': pic_url,
                     'messageUrl': self._open_type(message_url)
                 }
             }
 
-            logger.debug('link类型：%s' % data)
-            return self._request(data)
+            logger.debug(f'link类型：{payload}')
+            return self._request(payload)
 
         raise ValueError('link类型中消息标题或内容或链接不能为空！')
 
     def markdown(self, title, text, is_at_all=False, at_mobiles=None, at_dingtalk_ids=None, is_auto_at=True):
         """ markdown类型
         :param title: 首屏会话透出的展示内容
         :param text: markdown格式的消息内容
@@ -156,53 +157,56 @@
             at_mobiles = []
 
         if at_dingtalk_ids is None:
             at_dingtalk_ids = []
 
         if all(map(is_not_null_and_blank_str, [title, text])):
             # 给 Markdown 文本消息中的跳转链接添加上跳转方式
-            text = re.sub(r'(?<!!)\[.*?\]\((.*?)\)', lambda m: m.group(0).replace(m.group(1), self._open_type(m.group(1))), text)  # noqa
-            data = {'msgtype': 'markdown', 'markdown': {'title': title, 'text': text}, 'at': {}}
+            func = lambda m: m.group(0).replace(m.group(1), self._open_type(m.group(1)))  # noqa
+            text = re.sub(r'(?<!!)\[.*?\]\((.*?)\)', func, text)  # noqa
+
+            payload = {'msgtype': 'markdown', 'markdown': {'title': title, 'text': text}, 'at': {}}
 
             if is_at_all:
-                data['at']['isAtAll'] = is_at_all
+                payload['at']['isAtAll'] = is_at_all
 
             if at_mobiles:
                 at_mobiles = list(map(str, at_mobiles))
-                data['at']['atMobiles'] = at_mobiles
+                payload['at']['atMobiles'] = at_mobiles
 
                 if is_auto_at:
                     mobiles_text = '\n@' + '@'.join(at_mobiles)
-                    data['markdown']['text'] = text + mobiles_text
+                    payload['markdown']['text'] = text + mobiles_text
 
             if at_dingtalk_ids:
                 at_dingtalk_ids = list(map(str, at_dingtalk_ids))
-                data['at']['atDingtalkIds'] = at_dingtalk_ids
+                payload['at']['atDingtalkIds'] = at_dingtalk_ids
 
-            logger.debug('markdown类型：%s' % data)
-            return self._request(data)
+            logger.debug(f'markdown类型：{payload}')
+            return self._request(payload)
 
         raise ValueError('markdown类型中消息标题或内容不能为空！')
 
     def action(self, action_card):
         """ ActionCard类型
         :param action_card: 整体跳转ActionCard类型实例或独立跳转ActionCard类型实例
         :return: 返回消息发送结果
         """
         if isinstance(action_card, ActionCard):
-            data = action_card.get_data()
+            payload = action_card.get_data()
+
+            if 'singleURL' in payload['actionCard']:
+                payload['actionCard']['singleURL'] = self._open_type(payload['actionCard']['singleURL'])
 
-            if 'singleURL' in data['actionCard']:
-                data['actionCard']['singleURL'] = self._open_type(data['actionCard']['singleURL'])
-            elif 'btns' in data['actionCard']:
-                for btn in data['actionCard']['btns']:
+            if 'btns' in payload['actionCard']:
+                for btn in payload['actionCard']['btns']:
                     btn['actionURL'] = self._open_type(btn['actionURL'])
 
-            logger.debug('ActionCard类型：%s' % data)
-            return self._request(data)
+            logger.debug('ActionCard类型：%s' % payload)
+            return self._request(payload)
 
         raise TypeError(f'ActionCard类型：传入的实例类型不正确，内容为：{str(action_card)}')
 
     def feed(self, links):
         """ FeedCard类型
         :param links: FeedLink实例列表 or CardItem实例列表
         :return: 返回消息发送结果
@@ -210,50 +214,50 @@
         if not isinstance(links, list):
             logger.error(f'FeedLink类型：传入的数据格式不正确，内容为：{str(links)}')
             raise ValueError(f'FeedLink类型：传入的数据格式不正确，内容为：{str(links)}')
 
         link_list = []
 
         for link in links:
-            # 兼容：1、传入FeedLink实例列表；2、CardItem实例列表；
-            if isinstance(link, FeedLink) or isinstance(link, CardItem):
-                link = link.get_data()
-                link['messageURL'] = self._open_type(link['messageURL'])
-                link_list.append(link)
-            else:
+            if not isinstance(link, FeedLink) and not isinstance(link, CardItem):
                 raise ValueError(f'FeedLink类型，传入的数据格式不正确，内容为：{str(link)}')
 
-        data = {'msgtype': 'feedCard', 'feedCard': {'links': link_list}}
-        logger.debug('FeedCard类型：%s' % data)
+            # 兼容：1、传入FeedLink实例列表；2、CardItem实例列表；
+            link = link.get_data()
+            link['messageURL'] = self._open_type(link['messageURL'])
+            link_list.append(link)
+
+        payload = {'msgtype': 'feedCard', 'feedCard': {'links': link_list}}
+        logger.debug(f'FeedCard类型：{payload}')
 
-        return self._request(data)
+        return self._request(payload)
 
-    def _request(self, data: dict) -> dict:
+    def _request(self, payload: dict) -> dict:
         """ 发送消息（内容UTF-8编码）
-        :param data: 消息数据（字典）
+        :param payload: 消息数据（字典）
         :return: 返回消息发送结果
         """
         now = time.time()
 
         # 钉钉自定义机器人安全设置加签时，签名中的时间戳与请求时不能超过一个小时，所以每个1小时需要更新签名
-        if now - self.start_time >= 3600 and self.secret is not None and self.secret.startswith('SEC'):
+        if now - self.start_time >= 3600 and self.secret and self.secret.startswith('SEC'):
             self.start_time = now
-            self._initialize()
+            self._signature()
 
         # 钉钉自定义机器人现在每分钟最多发送20条消息
         self.queue.put(now)
 
         if self.queue.full():
             elapse_time = now - self.queue.get()
             if elapse_time < 60:
                 sleep_time = int(60 - elapse_time) + 1
                 logger.debug(f'钉钉官方限制机器人每分钟最多发送20条，当前发送频率已达限制条件，休眠 {str(sleep_time)}s')
                 time.sleep(sleep_time)
 
-        return self.session.post(data)
+        return self.session.post(payload)
 
     def send(self, action='text', **kwargs):
         """
         发送消息
 
         :param action:
         :param kwargs:
```

### Comparing `dingtalk2-0.1.1/dingtalk2/items.py` & `dingtalk2-0.1.2/dingtalk2/items.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,124 @@
-from .logger import logger
 from .utils import is_not_null_and_blank_str
 
 
 class ActionCard:
     """
     ActionCard类型消息格式（整体跳转、独立跳转）
     """
 
-    def __init__(self, title, text, btns, btn_orientation=0, hide_avatar=0):
+    def __init__(self, title=None, text=None, btns=None, btn_orientation=0, hide_avatar=0):
         """
         ActionCard初始化
         :param title: 首屏会话透出的展示内容
         :param text: markdown格式的消息
         :param btns: 按钮列表：（1）按钮数量为1时，整体跳转ActionCard类型；（2）按钮数量大于1时，独立跳转ActionCard类型；
         :param btn_orientation: 0：按钮竖直排列，1：按钮横向排列（可选）
         :param hide_avatar: 0：正常发消息者头像，1：隐藏发消息者头像（可选）
         """
         self.title = title
         self.text = text
+
         self.btn_orientation = btn_orientation
         self.hide_avatar = hide_avatar
 
         btn_list = [btn.get_data() for btn in btns if isinstance(btn, CardItem)]
 
         # 兼容：1、传入CardItem示例列表；2、传入数据字典列表
         self.btns = btn_list if btn_list else btns
 
     def get_data(self):
         """
-        获取ActionCard类型消息数据（字典）
-        :return: 返回ActionCard数据
+        获取 ActionCard 类型消息数据（字典）
+        :return: 返回 ActionCard 数据
         """
+        payloads = {
+            'msgtype': 'actionCard',
+            'actionCard': {
+                'title': self.title,
+                'text': self.text,
+                'hideAvatar': self.hide_avatar,
+                'btnOrientation': self.btn_orientation,
+            }
+        }
+
         if all(map(is_not_null_and_blank_str, [self.title, self.text])) and len(self.btns):
             if len(self.btns) == 1:
-                # 整体跳转ActionCard类型
-                data = {
-                    'msgtype': 'actionCard',
-                    'actionCard': {
-                        'title': self.title,
-                        'text': self.text,
-                        'hideAvatar': self.hide_avatar,
-                        'btnOrientation': self.btn_orientation,
-                        'singleTitle': self.btns[0]['title'],
-                        'singleURL': self.btns[0]['actionURL']
-                    }
-                }
-                return data
+                # 整体跳转 ActionCard 类型
+                payloads['actionCard']['singleTitle'] = self.btns[0]['title']
+                payloads['actionCard']['singleURL'] = self.btns[0]['actionURL']
             else:
-                # 独立跳转ActionCard类型
-                data = {
-                    'msgtype': 'actionCard',
-                    'actionCard': {
-                        'title': self.title,
-                        'text': self.text,
-                        'hideAvatar': self.hide_avatar,
-                        'btnOrientation': self.btn_orientation,
-                        'btns': self.btns
-                    }
-                }
-                return data
+                # 独立跳转 ActionCard 类型
+                payloads['actionCard']['btns'] = self.btns
+
+            return payloads
 
-        logger.error('ActionCard类型，消息标题或内容或按钮数量不能为空！')
         raise ValueError('ActionCard类型，消息标题或内容或按钮数量不能为空！')
 
 
 class FeedLink:
     """
     FeedCard类型单条消息格式
     """
 
-    def __init__(self, title, message_url, pic_url):
+    def __init__(self, title=None, message_url=None, pic_url=None):
         """
         初始化单条消息文本
         :param title: 单条消息文本
         :param message_url: 点击单条信息后触发的URL
         :param pic_url: 点击单条消息后面图片触发的URL
         """
         super().__init__()
-        self.title = title
         self.message_url = message_url
+
         self.pic_url = pic_url
+        self.title = title
 
     def get_data(self):
         """
-        获取FeedLink消息数据（字典）
-        :return: 本FeedLink消息的数据
+        获取 FeedLink 消息数据（字典）
+        :return: 本 FeedLink 消息的数据
         """
         if all(map(is_not_null_and_blank_str, [self.title, self.message_url, self.pic_url])):
-            data = {
-                'title': self.title,
-                'messageURL': self.message_url,
-                'picURL': self.pic_url
-            }
-            return data
+            return {'title': self.title, 'messageURL': self.message_url, 'picURL': self.pic_url}
 
-        logger.error('FeedCard类型单条消息文本、消息链接、图片链接不能为空！')
         raise ValueError('FeedCard类型单条消息文本、消息链接、图片链接不能为空！')
 
 
 class CardItem:
     """
     ActionCard和FeedCard消息类型中的子控件
 
     注意：
     1、发送FeedCard消息时，参数pic_url必须传入参数值；
     2、发送ActionCard消息时，参数pic_url不需要传入参数值；
     """
 
     def __init__(self, title, url, pic_url=None):
         """
-        CardItem初始化
+        CardItem 初始化
         @param title: 子控件名称
         @param url: 点击子控件时触发的URL
-        @param pic_url: FeedCard的图片地址，ActionCard时不需要，故默认为None
+        @param pic_url: FeedCard 的图片地址，ActionCard 时不需要，故默认为 None
         """
         self.url = url
         self.title = title
         self.pic_url = pic_url
 
     def get_data(self):
         """
-        获取CardItem子控件数据（字典）
+        获取 CardItem 子控件数据（字典）
         @return: 子控件的数据
         """
+        # FeedCard 类型
         if all(map(is_not_null_and_blank_str, [self.title, self.url, self.pic_url])):
-            # FeedCard类型
-            data = {
-                'title': self.title,
-                'picURL': self.pic_url,
-                'messageURL': self.url,
-            }
-
-            return data
-        elif all(map(is_not_null_and_blank_str, [self.title, self.url])):
-            # ActionCard类型
-            data = {
-                'title': self.title,
-                'actionURL': self.url,
-            }
+            return {'title': self.title, 'picURL': self.pic_url, 'messageURL': self.url}
 
-            return data
+        # ActionCard 类型
+        if all(map(is_not_null_and_blank_str, [self.title, self.url])):
+            return {'title': self.title, 'actionURL': self.url}
 
-        logger.error('CardItem是ActionCard的子控件时，title、url不能为空；是FeedCard的子控件时，title、url、pic_url不能为空！')
-        raise ValueError('CardItem是ActionCard的子控件时，title、url不能为空；是FeedCard的子控件时，title、url、pic_url不能为空！')
+        errmsg = 'CardItem是ActionCard的子控件时,title、url不能为空；是FeedCard的子控件时，title、url、pic_url不能为空！'
+        raise ValueError(errmsg)
 
 
 __all__ = ('ActionCard', 'FeedLink', 'CardItem')
```

### Comparing `dingtalk2-0.1.1/dingtalk2/request.py` & `dingtalk2-0.1.2/dingtalk2/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-import requests
+import httpx
 
 from .logger import logger
 
 
 class Request:
     def __init__(self, webhook, headers, options):
         self.webhook = webhook
         self.headers = headers
         self.options = options
-        self.session = requests.Session()
+        self.session = httpx.Client(verify=False)
 
     def get(self, payloads=None):
         return self.request(method='GET', data=payloads)
 
     def post(self, payloads):
         return self.request(method='POST', data=payloads)
 
     def request(self, method='GET', data: dict = None):
-        logger.debug(self.webhook)
-
         try:
-            response = self.session.request(method=method, url=self.webhook, headers=self.headers, json=data, params=self.options)
+            payloads = dict(method=method, url=self.webhook, headers=self.headers, json=data, params=self.options)
+            response = self.session.request(**payloads)
             response.raise_for_status()
             return response.json()
-        except requests.exceptions.HTTPError as exc:
+        except httpx.HTTPStatusError as exc:
             logger.warning(f'Error response {exc.response.status_code} while requesting {exc.request.url!r}.')
             logger.error(f'消息发送失败， HTTP error: {exc.response.status_code:d}, reason: {exc}')
             logger.exception(exc)
             return exc.response.json()
-        except requests.exceptions.ConnectTimeout:
+        except httpx.ConnectTimeout:
             logger.error('消息发送失败，Timeout error!')
             return None
-        except requests.exceptions.ConnectionError as exc:
+        except httpx.ConnectError as exc:
             logger.exception(exc)
             logger.error('消息发送失败，HTTP connection error!')
             return None
-        except requests.exceptions.RequestException as exc:
+        except httpx.RequestError as exc:
             logger.warning(f'An error occurred while requesting {exc.request.url!r}.')
             return None
 
     @staticmethod
     def _success(response):
         return response.json()
```

