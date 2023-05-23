# Comparing `tmp/nonebot_plugin_smallapi-1.0.3.tar.gz` & `tmp/nonebot_plugin_smallapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smallapi-1.0.3.tar", last modified: Mon May 15 02:53:53 2023, max compression
+gzip compressed data, was "nonebot_plugin_smallapi-1.0.4.tar", last modified: Tue May 23 15:23:11 2023, max compression
```

## Comparing `nonebot_plugin_smallapi-1.0.3.tar` & `nonebot_plugin_smallapi-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:53.442324 nonebot_plugin_smallapi-1.0.3/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-15 02:53:53.441324 nonebot_plugin_smallapi-1.0.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     4851 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:53.439324 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_menu.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_pic.py
--rw-r--r--   0 root         (0) root         (0)     4418 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_site.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_text.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/hander.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/hander_site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:53:53.441324 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-15 02:53:53.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-05-15 02:53:53.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:53:53.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-15 02:53:53.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-15 02:53:53.000000 nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      918 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 02:53:53.442324 nonebot_plugin_smallapi-1.0.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-15 02:53:46.000000 nonebot_plugin_smallapi-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:23:11.667311 nonebot_plugin_smallapi-1.0.4/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 15:23:11.667311 nonebot_plugin_smallapi-1.0.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     4993 2023-05-23 15:19:42.000000 nonebot_plugin_smallapi-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:23:11.664311 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_menu.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_pic.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2023-05-23 15:11:46.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_site.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_text.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander_site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:23:11.666311 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      918 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:23:11.667311 nonebot_plugin_smallapi-1.0.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-23 15:14:44.000000 nonebot_plugin_smallapi-1.0.4/setup.py
```

### Comparing `nonebot_plugin_smallapi-1.0.3/LICENSE` & `nonebot_plugin_smallapi-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.3/README.md` & `nonebot_plugin_smallapi-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 
 ## 🎉 功能
   
   1. 齐全的API随机图片系统  
   2. 齐全的API随机文本系统  
-  3. 不太好使的网站工具系统
+  3. 好使的网站工具系统
 
 ## 👉 命令
   
   PS: 请查看你env中起始符的配置(默认```/```)  
   1. API图片系统(图片系统)  
   2. API文字系统(文字系统)
   3. API站点系统(站点系统)
@@ -126,16 +126,31 @@
  还没有呢～
 
 ## 📝 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
-### 0.0.1
+### 1.0.0
 
-- 插件初次发布  
+-
 
+### 1.0.1
+
+- 修复依赖问题  
+
+### 1.0.2
+  
+- 梅开二度  
+  
+### 1.0.3  
+  
+- 梅开三度，终于修好了依赖
+
+### 1.0.4
+
+- 更换稳定API, 修复部分Bug
 </details>
 
 ## 致谢
 - [借鉴的代码](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py)
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
```

#### html2text {}

```diff
@@ -29,19 +29,20 @@
 ### æ´æ°çæ¬ ``` nb plugin update nonebot_plugin_smallapi ``` ## ð§
 éç½® ### envéç½® ``` #
 å¨ä½ çenvæä»¶ä¸­æ·»å å¦ä¸éç½®ï¼æçæ¯.envï¼ 114514 =
 'ç¬æ­»ï¼è¿ç©ææ²¡éç½®ï¼ä¸è¦æ114514åè¿å»ï¼ï¼ï¼' ``` |
 éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:----------------:|:----:|:----:|:--
 --------------------------:| | `` | å¦ | `""` | ç©ºç©ºå¦ä¹ | ## ð åè½
 1. é½å¨çAPIéæºå¾çç³»ç» 2. é½å¨çAPIéæºææ¬ç³»ç» 3.
-ä¸å¤ªå¥½ä½¿çç½ç«å·¥å·ç³»ç» ## ð å½ä»¤ PS:
+å¥½ä½¿çç½ç«å·¥å·ç³»ç» ## ð å½ä»¤ PS:
 è¯·æ¥çä½ envä¸­èµ·å§ç¬¦çéç½®(é»è®¤```/```) 1. APIå¾çç³»ç»
 (å¾çç³»ç») 2. APIæå­ç³»ç»(æå­ç³»ç») 3. APIç«ç¹ç³»ç»
 (ç«ç¹ç³»ç») ### APIå¾çç³»ç» å½ä»¤ç»æï¼```(/)APIå¾çç³»ç»```
 ä¾å¦ï¼```APIå¾çç³»ç»``` ### APIæå­ç³»ç» å½ä»¤ç»æï¼```(/
 )APIæå­ç³»ç»``` ä¾å¦ï¼```APIæå­ç³»ç»``` ### APIç«ç¹ç³»ç»
 å½ä»¤ç»æï¼```(/)APIç«ç¹ç³»ç»``` ä¾å¦ï¼```APIç«ç¹ç³»ç»``` ## â
-æå± è¿æ²¡æå¢ï½ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
-æä»¶åæ¬¡åå¸  ## è´è°¢ - [åé´çä»£ç ](https://github.com/lgc-
-NB2Dev/ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/
-__main__.py) - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-
-plugin-template)
+æå± è¿æ²¡æå¢ï½ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 1.0.0 - ###
+1.0.1 - ä¿®å¤ä¾èµé®é¢ ### 1.0.2 - æ¢å¼äºåº¦ ### 1.0.3 -
+æ¢å¼ä¸åº¦ï¼ç»äºä¿®å¥½äºä¾èµ ### 1.0.4 - æ´æ¢ç¨³å®API,
+ä¿®å¤é¨åBug  ## è´è°¢ - [åé´çä»£ç ](https://github.com/lgc-NB2Dev/
+ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py) -
+[nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
```

### Comparing `nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_menu.py` & `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,10 +45,10 @@
         )
     await matcher.finish(msg_api_text,at_sender=True)
 
 @api_site.handle()
 @error_handle()
 async def handle_onebot(matcher: Matcher,bot: OneBot):
     msg_api_site = MessageSegment.text(
-            "API站点系统\n|ip查询|网站测速|\n|ping|icp查询|\n|whois查询|"
+            "API站点系统\n|ip查询|拦截检测|\n|ping|icp查询|\n|whois查询|收录查询|"
         )
     await matcher.finish(msg_api_site,at_sender=True)
```

### Comparing `nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_pic.py` & `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,57 @@
 from .hander import *
-pic_ecy = on_command("次元图", priority=6)
+text_tgrj = on_command("舔狗日记", priority=3)
 
-pic_dm = on_command("动漫图", priority=6)
+text_wenan = on_command("文案", priority=3)
 
-pic_bing = on_command("Bing图", aliases={"bing图"} , priority=6)
+text_xh = on_command("笑话" ,priority=3)
 
-pic_fj = on_command("风景图", priority=6)
-
-@pic_ecy.handle()
+@text_tgrj.handle()
 @error_handle()
 async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
     await matcher.finish(
         format_return(
             {
                 "code": "200",
                 "msg": "请求成功",
-                "data": MessageSegment.image(
-                    await get_api_resp("randomAcgPic?type=pc" , "data" , original=True)
+                "data": MessageSegment.text(
+                    await get_api_resp("Dog" , "data.text" , original=True)
                 ),
             },
             lambda ret: ret,
         ),
         at_sender=True,
     )
 
-@pic_dm.handle()
+@text_wenan.handle()
 @error_handle()
-async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
+async def handle_onebot(matcher: Matcher, args: Message = CommandArg()):
     await matcher.finish(
         format_return(
             {
                 "code": "200",
                 "msg": "请求成功",
-                "data": MessageSegment.image(
-                    await get_api_resp("random4kPic?type=acg" , "data" , original=True)
+                "data": MessageSegment.text(
+                    await get_api_resp("WaSentence" , "data.text" , original=True)
                 ),
             },
             lambda ret: ret,
         ),
         at_sender=True,
     )
 
-@pic_bing.handle()
+@text_xh.handle()
 @error_handle()
-async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
-    await matcher.finish(
-        format_return(
-            {
-                "code": "200",
-                "msg": "请求成功",
-                "data": MessageSegment.image(
-                    await get_api_resp("bing" , "data" , original=True)
-                ),
-            },
-            lambda ret: ret,
-        ),
-        at_sender=True,
-    )
-
-@pic_fj.handle()
-@error_handle()
-async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
+async def handle_onebot(matcher: Matcher, args: Message = CommandArg()):
     await matcher.finish(
         format_return(
             {
                 "code": "200",
                 "msg": "请求成功",
-                "data": MessageSegment.image(
-                    await get_api_resp("random4kPic?type=wallpaper" , "data" , original=True)
+                "data": MessageSegment.text(
+                    await get_api_resp("Xiaohua" , "data.text" , original=True)
                 ),
             },
             lambda ret: ret,
         ),
         at_sender=True,
     )
```

### Comparing `nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_site.py` & `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_site.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,114 +2,139 @@
 @on_command("ip查询", aliases={"IP查询", "IPSOSO"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入IP/域名")
 
     await matcher.finish(
-        format_return_site(
-            await get_api_resp_site("ip", {"ip": arg}),
-            lambda ret_site: (
-                #f'查询目标：{ret_site["url"]}\n'
-                f'IP地址：{ret_site["address"]}\n'
-                f'IP类型：{ret_site["type"]}\n'
-                f'IP段起始: {ret_site["begin"]}\n'
-                f'IP段结束: {ret_site["end"]}'
-                #f'更多信息：{ret_site["domain_ip"]}'
+        format_return(
+            await get_api_resp("IP", {"ip": arg}),
+            lambda ret_web: (
+                f'查询目标：{ret_web["ip"]}\n'
+                f'IP地址：{(ret_web["location"].get("ip"))}\n'
+                f'IP类型：{ret_web["isp"]}\n'
+                f'IP地区：{ret_web["country"]}\n'
+                f'IP段起始: {ret_web["range.start"]}\n'
+                f'IP段结束: {ret_web["range.end"]}'
+                f'更多信息：{ret_web["area"]}'
             ),
         ),
         at_sender=True,
     )
 
-@on_command("网站测速", aliases={"web测速", "WEB测速"}).handle()
+@on_command("ping", aliases={"Ping", "PING"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
-        await matcher.finish("请输入域名")
+        await matcher.finish("请输入IP/域名")
 
     await matcher.finish(
-        format_return_site(
-            await get_api_resp_site("speed", {"url": "http://" + arg}),
-            lambda ret_site: (
-                f'访问速度：{ret_site}'
-                ),
+        format_return(
+            await get_api_resp("Ping", {"ip": arg}),
+            lambda ret_web: (
+                f'查询目标：{ret_web["host"]}\n'
+                f'IP地址：{ret_web["ip"]}\n'
+                f'延迟：{ret_web["ping_avg"]}\n'
+                f'主机位置：{ret_web["location"]}\n'
+                f'请求节点: {ret_web["node"]}\n'
+                #f'主机类型: {ret_web["type"]}\n'
+                #f'IP段起始/结束: {ret_web["begin"]}\n{ret_web["end"]}'
+                f'更多信息：{ret_web["domain_ip"]}'
+            ),
         ),
         at_sender=True,
     )
 
-
-
-
-
-@on_command("ping", aliases={"Ping", "PING"}).handle()
+@on_command("ICP查询", aliases={"icp查询", "Icp查询", "备案查询"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
-        await matcher.finish("请输入IP/域名")
+        await matcher.finish("请输入域名")
 
     await matcher.finish(
-        format_return_site(
-            await get_api_resp_site("ping", {"url": arg}),
-            lambda ret_site: (
-                f'查询目标：{ret_site["url"]}\n'
-                f'IP地址：{ret_site["ip"]}\n'
-                f'延迟：{ret_site["time"]}\n'
-                f'主机位置：{ret_site["address"]}\n'
-                f'请求节点: {ret_site["server"]}\n'
-                f'主机类型: {ret_site["type"]}\n'
-                f'IP段起始/结束: {ret_site["begin"]}\n{ret_site["end"]}'
-                #f'更多信息：{ret_site["domain_ip"]}'
+        format_return(
+            await get_api_resp("ICP", {"domain": arg}),
+            lambda ret_web: (
+                f'查询域名：{ret_web["domain"]}\n'
+                f'网站名称：{ret_web["serviceName"]}\n'
+                f'主页地址：{ret_web["homeUrl"]}\n'
+                f'主办单位名称：{ret_web["unitName"]}\n'
+                f'主办单位性质：{ret_web["class"]}\n'
+                f'备案号：{ret_web["icp"]}\n'
+                f'备案号名称: {ret_web["mainLicence"]}\n'
+                f'更新时间：{ret_web["time"]}'
             ),
         ),
         at_sender=True,
     )
 
+@on_command("拦截检测").handle()
+@error_handle()
+async def _(matcher: Matcher, args: Message = CommandArg()):
+    if not (arg := args.extract_plain_text()):
+        await matcher.finish("请输入网址")
 
-@on_command("ICP查询", aliases={"icp查询", "Icp查询", "备案查询"}).handle()
+    params = {"url": arg}
+    qq = await get_api_resp("TencentUrl", params)
+    if qq["code"] != 200:
+        await matcher.finish(format_return(qq))
+
+    wx = await get_api_resp("WxUrl", params)
+    if wx["code"] != 200:
+        await matcher.finish(format_return(wx))
+
+    qq["data"]["type"] = wx["data"]["type"]
+    await matcher.finish(
+        format_return(
+            wx,
+            lambda ret_web: f'查询网址：{ret_web["url"]}\nQQ/微信拦截状态：{ret_web["type"]}/{ret_web["type"]}',
+        ),
+        at_sender=True,
+    )
+
+@on_command("收录查询").handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入域名")
 
-    #if (await get_api_resp_site("icp", {"domain": arg})) is None:
-    #            await matcher.finish(f'icp查询返回为空: 找不到备案信息～')
-
-    else: 
-        await matcher.finish(
-        format_return_site(
-            await get_api_resp_site("icp", {"domain": arg}),
-            lambda ret_site: (
-                f'查询域名：{ret_site["domain"]}\n'
-                #f'网站名称：{ret_site["serviceName"]}\n'
-                f'主页地址：{ret_site["domain"]}\n'
-                f'主办单位名称：{ret_site["unitName"]}\n'
-                f'主办单位性质：{ret_site["natureName"]}\n'
-                f'备案号：{ret_site["mainLicence"]}\n{ret_site["serviceLicence"]}\n'
-                f'更新时间：{ret_site["updateRecordTime"]}'
+    await matcher.finish(
+        format_return(
+            await get_api_resp("CheckSEO", {"domain": arg}),
+            lambda ret_web: (
+                f'查询域名：{ret_web["domain"]}\n'
+                f'网站标题：{title if (title := ret_web["title"]) else "未知"}\n'
+                f'百度收录量：{ret_web["baidu"]}\n'
+                f'好搜收录量：{ret_web["haoso"]}\n'
+                f'神马收录量：{ret_web["sm"]}\n'
+                f'搜狗收录量：{ret_web["sogou"]}\n'
+                f'Bing/必应中国：{ret_web["bing"]}/{ret_web["bingZh"]}\n'
+                f'Google：{ret_web["google"]}'
             ),
         ),
         at_sender=True,
     )
 
 @on_command("whois查询", aliases={"Whois查询", "WhoIs查询", "WHOIS查询"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入域名")
 
     await matcher.finish(
-        format_return_site(
-            await get_api_resp_site("whois", {"domain": arg}),
-            lambda ret_site: (
-                f'查询域名：{ret_site["Domain Name"]}\n'
-                f'注册商：{ret_site["Sponsoring Registrar"]}\n'
-                f'注册人：{ret_site["Registrant"]}\n'
-                f'注册邮箱：{ret_site["Registrant Contact Email"]}\n'
-                f'注册时间：{format_json_time(ret_site["Registration Time"])}\n'
-                f'到期时间：{format_json_time(ret_site["Expiration Time"])}\n'
-                f'DNS服务器：{ret_site["DNS Serve"]}\n'
-                #f'域名状态：{", ".join([x["domainState"] for x in ret_site["domainState"]])}\n'
-                #f'数据更新时间：{ret_site["updateTime"]}'
+        format_return(
+            await get_api_resp("Whois", {"domain": arg}),
+            lambda ret_web: (
+                f'查询域名：{ret_web["domain"]}\n'
+                f'注册商：{ret_web["registrar"]}\n'
+                f'注册人：{ret_web["registrant"]}\n'
+                f'注册邮箱：{ret_web["email"]}\n'
+                f'注册时间：{format_json_time(ret_web["registrationTime"])}\n'
+                f'到期时间：{format_json_time(ret_web["expirationTime"])}\n'
+                f'DNS服务器：{ret_web["nameServer"]}\n'
+                #f'域名状态：{", ".join([x["domainState"] for x in ret_web["domainState"]])}\n'
+                f'域名状态：{ret_web["domainState"]}\n'
+                f'数据更新时间：{ret_web["updateTime"]}'
             ),
         ),
         at_sender=True,
     )
```

### Comparing `nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/api_text.py` & `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_pic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,76 @@
 from .hander import *
-text_tgrj = on_command("舔狗日记", priority=3)
+pic_ecy = on_command("次元图", priority=6)
 
-text_wenan = on_command("文案", priority=3)
+pic_dm = on_command("动漫图", priority=6)
 
-text_xh = on_command("笑话" ,priority=3)
+pic_bing = on_command("Bing图", aliases={"bing图"} , priority=6)
 
-@text_tgrj.handle()
+pic_fj = on_command("风景图", priority=6)
+
+@pic_ecy.handle()
 @error_handle()
 async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
     await matcher.finish(
         format_return(
             {
                 "code": "200",
                 "msg": "请求成功",
-                "data": MessageSegment.text(
-                    await get_api_resp("dog" , "data" , original=True)
+                "data": MessageSegment.image(
+                    await get_api_resp("DmImg" , "data.url" , original=True)
                 ),
             },
             lambda ret: ret,
         ),
         at_sender=True,
     )
 
-@text_wenan.handle()
+@pic_dm.handle()
 @error_handle()
-async def handle_onebot(matcher: Matcher, args: Message = CommandArg()):
+async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
     await matcher.finish(
         format_return(
             {
                 "code": "200",
                 "msg": "请求成功",
-                "data": MessageSegment.text(
-                    await get_api_resp("renjian" , "data" , original=True)
+                "data": MessageSegment.image(
+                    await get_api_resp("DmImgS" , "data.url" , original=True)
                 ),
             },
             lambda ret: ret,
         ),
         at_sender=True,
     )
 
-@text_xh.handle()
+@pic_bing.handle()
 @error_handle()
-async def handle_onebot(matcher: Matcher, args: Message = CommandArg()):
+async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
+    await matcher.finish(
+        format_return(
+            {
+                "code": "200",
+                "msg": "请求成功",
+                "data": MessageSegment.image(
+                    await get_api_resp("BingImg" , "data.url" , original=True)
+                ),
+            },
+            lambda ret: ret,
+        ),
+        at_sender=True,
+    )
+
+@pic_fj.handle()
+@error_handle()
+async def handle_onebot(bot: OneBot, matcher: Matcher, args: Message = CommandArg()):
     await matcher.finish(
         format_return(
             {
                 "code": "200",
                 "msg": "请求成功",
-                "data": MessageSegment.text(
-                    await get_api_resp("aiqinggongyu" , "data" , original=True)
+                "data": MessageSegment.image(
+                    await get_api_resp("FjImg" , "data.url" , original=True)
                 ),
             },
             lambda ret: ret,
         ),
         at_sender=True,
     )
```

### Comparing `nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/hander.py` & `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,18 +44,18 @@
         msg += "\n--------\n" + func(ret["data"])  # MessageSegment拼接
     return msg + "\n--------\nAPI from Me！"
 
 async def get_api_resp(name , params , original=True) -> dict | list | str:
     async with aiohttp.ClientSession() as client:
         ret = f'{None}'
         if original:
-            async with client.get(f'https://v2.api-m.com/api/{name}') as resp:
+            async with client.get(f'https://api.gumengya.com/Api/{name}') as resp:
                 ret_old_1 = str(await resp.json())
                 ret_old_1 = ast.literal_eval(ret_old_1)
                 ret = jsonpath.jsonpath(ret_old_1, f"$.{params}")[0]
                 logger.info(f"有人调用了API: {name} {ret_old_1}")
                 return ret
         else:
-            async with client.get(f'https://v2.api-m.com/api/{name}') as resp:
+            async with client.get(f'https://api.gumengya.com/Api/{name}') as resp:
                 ret = await resp.text()
                 logger.info(f"有人调用了API: {name} {ret}")
                 return ret
```

### Comparing `nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi/hander_site.py` & `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander_site.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     msg = f'\n[{(code := ret_site["code"])}]{ret_site["msg"]}'
     if str(code) == "200":
         msg += "\n--------\n" + func(ret_site["data"])
     return msg + "\n--------\nAPI from Me！"
 
 async def get_api_resp_site(name, params, original=False) -> dict | list | bytes:
     async with aiohttp.ClientSession() as s:
-        async with s.get(f"https://v2.api-m.com/api/{name}", params=params) as resp:
+        async with s.get(f"https://api.gumengya.com/Api/{name}", params=params) as resp:
             ret_site = f'{None}'
             if original:
                 ret_site = await resp.read()
             else:
                 ret_site = await resp.json()
             logger.info(f"有人调用了API For Web: {ret_site}")
             #logger.info(f"$.data.{params}")
```

### Comparing `nonebot_plugin_smallapi-1.0.3/nonebot_plugin_smallapi.egg-info/SOURCES.txt` & `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.3/pyproject.toml` & `nonebot_plugin_smallapi-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.3/setup.py` & `nonebot_plugin_smallapi-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools #导入setuptools打包工具
 
 setuptools.setup(
     install_requires=['jsonpath','nonebot2[aiohttp]','nonebot-adapter-onebot','nonebot2[httpx]'],
     name="nonebot_plugin_smallapi", # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.3",    #包版本号，便于维护版本
+    version="1.0.4",    #包版本号，便于维护版本
     author="Chaichaisi",    #作者，可以写自己的姓名
     author_email="chaichaisi@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small nonebot_plugin_smallapi plugin",#包的简述
     long_description="come in to read more",    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/chaichaisi/nonebot_plugin_smallapi",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

