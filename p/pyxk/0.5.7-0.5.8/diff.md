# Comparing `tmp/pyxk-0.5.7.tar.gz` & `tmp/pyxk-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.7.tar", last modified: Sun May 14 14:03:29 2023, max compression
+gzip compressed data, was "pyxk-0.5.8.tar", last modified: Tue May 23 04:41:28 2023, max compression
```

## Comparing `pyxk-0.5.7.tar` & `pyxk-0.5.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.231998 pyxk-0.5.7/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.7/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-14 14:03:29.231998 pyxk-0.5.7/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.7/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-14 14:00:13.000000 pyxk-0.5.7/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-13 08:37:44.000000 pyxk-0.5.7/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    18023 2023-05-14 13:50:42.000000 pyxk-0.5.7/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-13 05:40:17.000000 pyxk-0.5.7/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-04-10 03:10:37.000000 pyxk-0.5.7/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-08 07:57:14.000000 pyxk-0.5.7/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-08 07:56:51.000000 pyxk-0.5.7/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.231998 pyxk-0.5.7/pyxk/m3u8downloader/
--rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-08 07:55:15.000000 pyxk-0.5.7/pyxk/m3u8downloader/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3448 2023-05-13 14:37:26.000000 pyxk-0.5.7/pyxk/m3u8downloader/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4907 2023-05-14 14:00:57.000000 pyxk-0.5.7/pyxk/m3u8downloader/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-08 04:33:43.000000 pyxk-0.5.7/pyxk/m3u8downloader/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    11732 2023-05-13 09:23:24.000000 pyxk-0.5.7/pyxk/m3u8downloader/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.231998 pyxk-0.5.7/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-08 07:57:36.000000 pyxk-0.5.7/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-08 07:58:19.000000 pyxk-0.5.7/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3309 2023-05-09 03:19:15.000000 pyxk-0.5.7/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    14682 2023-05-09 03:23:24.000000 pyxk-0.5.7/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-14 13:59:58.000000 pyxk-0.5.7/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-14 14:03:29.231998 pyxk-0.5.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-14 14:03:10.000000 pyxk-0.5.7/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.8/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-23 04:41:28.367688 pyxk-0.5.8/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.8/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.357688 pyxk-0.5.8/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    18325 2023-05-22 03:35:48.000000 pyxk-0.5.8/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/m3u8downloader/
+-rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/m3u8downloader/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3391 2023-05-23 04:31:51.000000 pyxk-0.5.8/pyxk/m3u8downloader/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4907 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/m3u8downloader/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/m3u8downloader/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    11879 2023-05-23 04:35:40.000000 pyxk-0.5.8/pyxk/m3u8downloader/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3502 2023-05-23 04:20:34.000000 pyxk-0.5.8/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    15210 2023-05-23 04:29:24.000000 pyxk-0.5.8/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.357688 pyxk-0.5.8/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-23 04:41:28.367688 pyxk-0.5.8/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-23 04:41:14.000000 pyxk-0.5.8/setup.py
```

### Comparing `pyxk-0.5.7/LICENSE` & `pyxk-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk/aclient/client.py` & `pyxk-0.5.8/pyxk/aclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,24 @@
     :params: aiohttp_kwargs: aiohttp.ClientSession 实例化参数
     :params: retry_status_code: 请求状态码，包含在列表中的进行重新发送
     :params: error_status_code: 请求状态码，包含在列表中直接抛出错误
     :params: until_request_succeed: 请求状态码，知道请求成功为止
 
     __init__ parameters - 实例化参数
 
-    :params: base_url : base_url
+    :params: base_url: base_url
+    :params: **kwargs: 关键字 实例化参数
     """
 
     limit: Optional[int] = None
     timeout: Timeout = None
     async_sleep: Optional[int] = None
     maximum_retry: Optional[int] = None
     headers: Optional[Union[dict, CIMDict]] = None
-    semaphore: Optional[int] = None
+    semaphore: Union[Optional[int], asyncio.Semaphore] = None
     verify: Optional[bool] = None
     start_urls: Union[List[str], List[Tuple[str, dict]]] = []
     user_agent: Optional[str] = None
     aiohttp_kwargs: Optional[dict] = None
     retry_status_code: Optional[list] = None
     error_status_code: Optional[list] = None
     until_request_succeed: Optional[Union[bool, List[int]]] = None
@@ -84,15 +85,22 @@
         ("async_sleep", 1),
         ("maximum_retry", 20),
         ("user_agent", get_user_agent()),
         ("aiohttp_kwargs", {}),
         ("until_request_succeed", False),
     )
 
-    def __init__(self, *, base_url: StrOrURL=None):
+    def __init__(self, *, base_url: StrOrURL=None, **kwargs):
+        """Client init
+
+        :params: base_url: base_url
+        :params: **kwargs: 关键字 实例化参数
+        """
+        for key, val in kwargs.items():
+            setattr(self, key, val)
         # event loop
         self._loop: EventLoop = None
         # aiohttp session
         self._session: Session = None
         # base_url
         self._base_url: StrOrURL = self.set_base_url(base_url)
 
@@ -336,17 +344,17 @@
             )
             tasks.append(task)
         result = await asyncio.gather(*tasks, return_exceptions=return_exceptions)
         return result
 
     async def sleep(self, delay: Optional[Union[int, float]]=None, result: Any=None):
         """异步休眠"""
-        if not isinstance(delay, int) or delay <= 0:
+        if not isinstance(delay, (int, float)) or delay < 0:
             delay = self.async_sleep \
-                if isinstance(self.async_sleep, int) and self.async_sleep > 0 else dict(self.attr)["async_sleep"]
+                if isinstance(self.async_sleep, (int, float)) and self.async_sleep > 0 else dict(self.attr)["async_sleep"]
         return await asyncio.sleep(delay, result=result)
 
     def build_url(self, _url) -> StrOrURL:
         """构造完整url地址"""
         if not isinstance(_url, (str, _yarl.URL)):
             return _url
         _url = _yarl.URL(_url)
```

### Comparing `pyxk-0.5.7/pyxk/aclient/typedef.py` & `pyxk-0.5.8/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk/aes/_fmtdata.py` & `pyxk-0.5.8/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk/aes/cryptor.py` & `pyxk-0.5.8/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk/m3u8downloader/enter_point.py` & `pyxk-0.5.8/pyxk/m3u8downloader/enter_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=16, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
 @click.pass_context
 def main(ctx, output, reload, reserve, headers, verify, limit, user_agent):
     """m3u8下载器"""
-    if not ctx.obj or not isinstance(ctx.obj, dict):
-        ctx.obj = {}
+    ctx.obj = {}
     # 将参数传递给子命令
     if ctx.invoked_subcommand:
         ctx.obj.update(ctx.params)
 
 @main.command
 @click.pass_obj
 @click.argument("content", type=click.Path(exists=True), metavar="<File>")
```

### Comparing `pyxk-0.5.7/pyxk/m3u8downloader/m3u8download.py` & `pyxk-0.5.8/pyxk/m3u8downloader/m3u8download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk/m3u8downloader/m3u8parse.py` & `pyxk-0.5.8/pyxk/m3u8downloader/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk/m3u8downloader/main.py` & `pyxk-0.5.8/pyxk/m3u8downloader/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,28 +153,30 @@
         """开始解析m3u8内容
 
         :params: content: m3u8 内容
         :params: url: m3u8 链接
         """
         m3u8parse = M3U8Parae.run(content=content, url=url, instance=self)
         # 可视化内容
-        table = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD)
+        table = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD, padding=0)
         table.add_column(justify="left", overflow="fold")
-        table.add_row(f"[yellow b]url[/]: [blue u]{url}[/]")
-        table.add_section()
+        table1 = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD, padding=0)
+        table1.add_column(justify="left", overflow="ellipsis")
+        table1.add_row(f"[yellow b]url[/]: [blue u]{url}[/]")
+        table.add_row(table1)
         table.add_row(f"[yellow b]maximum[/]: {m3u8parse['maximum']}")
         table.add_row(f"[yellow b]duration[/]: {human_playtime(m3u8parse['duration'])}")
         table.add_row(f"[yellow b]encryption[/]: {bool(m3u8parse['m3u8keys'])}")
         table.add_row(f"[yellow b]output[/]: [blue]{self.output}[/]")
-        table.add_section()
         # 添加进度条
         progress, download = None, None
         if m3u8parse["segments"] and self.output and self._tempfiles:
             progress = progress_column(add_task=False)
             download = download_column(add_task=False, show_transfer_speed=False)
+            table.add_section()
             table.add_row(progress)
             table.add_row(download)
         panel = _rich_panel.Panel(
             table,
             subtitle=f"[dim i]limit: {self._limit}[/]",
             subtitle_align="right",
             border_style="bright_blue",
@@ -194,18 +196,15 @@
         # 删除m3u8文件
         if not self._reserve:
             import shlex, subprocess
             args = shlex.split(f"rm -rf {self._tempfiles}")
             subprocess.run(args, check=True)
 
     def get_m3u8_content(
-        self,
-        url: Optional[str],
-        *,
-        is_m3u8key: bool = False
+        self, url: Optional[str], *, is_m3u8key: bool=False
     ) -> Optional[str]:
         """获取m3u8内容
 
         :params: url: url
         :params: is_m3u8key: m3u8 key(type: bool)
         """
         if not(url and isinstance(url, str)):
```

### Comparing `pyxk-0.5.7/pyxk/requests/api.py` & `pyxk-0.5.8/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk/requests/entry_point.py` & `pyxk-0.5.8/pyxk/requests/entry_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import click
-from pyxk.utils import LazyLoader
+from pyxk.utils import LazyLoader, get_user_agent
 from pyxk.requests import downloader
 
 _json = LazyLoader("_json", globals(), "json")
 
 
 def validate_json(ctx, param, value):
     if value is None:
@@ -136,16 +136,24 @@
 @click.option(
     "--thread",
     "thread",
     type=int,
     default=1,
     help="Multithreaded download"
 )
+@click.option(
+    "-ua",
+    "--user-agent",
+    "user_agent",
+    type=str,
+    default=None,
+    help="User-Agent"
+)
 def main(
-    method, url, params, headers, data, json, files, cookies, auth, proxies, timeout, allow_redirects, verify, output, restore, thread,
+    method, url, params, headers, data, json, files, cookies, auth, proxies, timeout, allow_redirects, verify, output, restore, thread, user_agent
 ):
     if not method:
         method = "POST" if data or files or json else "GET"
     downloader(
         method=method,
         url=url,
         params=dict(params) or None,
@@ -157,8 +165,9 @@
         timeout=timeout,
         allow_redirects=allow_redirects,
         verify=verify,
         auth=auth,
         output=output,
         restore=restore,
         thread_num=thread,
+        user_agent=get_user_agent(user_agent)
     )
```

### Comparing `pyxk-0.5.7/pyxk/requests/sessions.py` & `pyxk-0.5.8/pyxk/requests/sessions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import time
 import warnings
+from typing import Union, Optional
 from urllib.parse import urlsplit, urljoin
 from concurrent.futures import ThreadPoolExecutor
 
 from requests.models import Response
 from requests import Session as _Session
 from requests import exceptions as requests_exceptions
 from requests.structures import CaseInsensitiveDict as CIDict
@@ -24,18 +25,25 @@
 _rich_table = LazyLoader("_rich_table", globals(), "rich.table")
 _rich_console = LazyLoader("_rich_console", globals(), "rich.console")
 
 
 
 class Session(_Session):
 
-    def __init__(self, *, headers=None, base_url=None, user_agent=None):
+    def __init__(
+        self,
+        *,
+        headers: Optional[Union[CIDict, dict]] = None,
+        base_url: Optional[str] = None,
+        user_agent: Optional[str] = None
+    ):
         super().__init__()
         headers = CIDict(headers)
-        headers.setdefault("User-Agent", user_agent or get_user_agent())
+        if user_agent and isinstance(user_agent, str):
+            headers.__setitem__("User-Agent", user_agent or get_user_agent())
         self.headers.update(headers)
         self._base_url = self.set_base_url(base_url)
         self._console = _rich_console.Console()
 
     def request(
         self, method, url, *, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
     ) -> Response:
@@ -156,16 +164,18 @@
         # content type
         content_type = response.headers.get("Content-Type")
         # output
         output = os.path.abspath(output) if output and isinstance(output, str) else None
         if not output:
             table = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD)
             table.add_column(justify="left", overflow="fold")
-            table.add_row(f"<[cyan]Response[/] [{response.status_code}]> [blue u]{url}[/]")
-            table.add_section()
+            table1 = _rich_table.Table(show_header=False, padding=0, box=_rich_box.SIMPLE_HEAD)
+            table1.add_column(justify="left", overflow="ellipsis")
+            table1.add_row(f"<[cyan]Response[/] [{response.status_code}]> [blue u]{url}[/]")
+            table.add_row(table1)
             if not length:
                 table.add_row("[red]content-length is not available![/]")
                 table.add_section()
             table.add_row(f"[green]filetype[/]: [yellow]{content_type}[/]")
             table.add_row(f"[green]filesize[/]: [yellow]{units_conversion_from_byte(length)}[/] ({length})")
             panel = _rich_panel.Panel(
                 table, title="[red b]Downloader[red]", title_align="center", border_style="bright_blue"
@@ -181,22 +191,24 @@
             thread_num = 1
         # 线程池
         progress = download_column(add_task=False)
         thread_pool = ThreadPoolExecutor(max_workers=8)
 
         table = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD)
         table.add_column(justify="left", overflow="fold")
-        table.add_row(f"<[cyan]Response[/] [{response.status_code}]> [blue u]{url}[/]")
-        table.add_section()
+        table1 = _rich_table.Table(show_header=False, padding=0, box=_rich_box.SIMPLE_HEAD)
+        table1.add_column(justify="left", overflow="ellipsis")
+        table1.add_row(f"<[cyan]Response[/] [{response.status_code}]> [blue u]{url}[/]")
+        table.add_row(table1)
         if not length:
             table.add_row("[red]content-length is not available![/]")
             table.add_section()
         table.add_row(f"[green]filetype[/]: [yellow]{content_type}[/]")
         table.add_row(f"[green]filesize[/]: [yellow]{units_conversion_from_byte(length)}[/] ({length})")
-        table.add_row(f"[green]filename[/]: [yellow u]{output}[/]")
+        table.add_row(f"[green]filename[/]: [blue]{output}[/]")
         table.add_section()
         table.add_row(progress)
         panel = _rich_panel.Panel(
             table,
             title="[red b]Downloader[red]",
             title_align="center",
             border_style="bright_blue",
```

### Comparing `pyxk-0.5.7/pyxk/utils.py` & `pyxk-0.5.8/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/pyxk.egg-info/SOURCES.txt` & `pyxk-0.5.8/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.7/setup.py` & `pyxk-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.5.7",
+    version="0.5.8",
     author="pengke",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
```

