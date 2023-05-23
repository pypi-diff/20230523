# Comparing `tmp/PrSpiders-0.4.8.tar.gz` & `tmp/PrSpiders-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.4.8.tar", last modified: Fri May 19 08:09:35 2023, max compression
+gzip compressed data, was "PrSpiders-0.4.9.tar", last modified: Tue May 23 06:30:14 2023, max compression
```

## Comparing `PrSpiders-0.4.8.tar` & `PrSpiders-0.4.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:35.111789 PrSpiders-0.4.8/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.8/LICENSE.txt
--rw-rw-rw-   0        0        0     5678 2023-05-19 08:09:35.107789 PrSpiders-0.4.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:34.836786 PrSpiders-0.4.8/PrSpider/
--rw-rw-rw-   0        0        0    12713 2023-05-18 01:02:32.000000 PrSpiders-0.4.8/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       79 2023-05-17 09:01:20.000000 PrSpiders-0.4.8/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11011 2023-05-19 08:04:11.000000 PrSpiders-0.4.8/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4468 2023-05-18 02:26:44.000000 PrSpiders-0.4.8/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.8/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:34.917788 PrSpiders-0.4.8/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5678 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:34.935788 PrSpiders-0.4.8/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.4.8/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:35.013786 PrSpiders-0.4.8/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.8/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.8/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.8/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.4.8/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:35.080802 PrSpiders-0.4.8/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.8/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.8/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.8/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.8/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-19 08:09:35.112786 PrSpiders-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-19 08:09:27.000000 PrSpiders-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.477264 PrSpiders-0.4.9/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     5678 2023-05-23 06:30:14.451264 PrSpiders-0.4.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.232270 PrSpiders-0.4.9/PrSpider/
+-rw-rw-rw-   0        0        0    12780 2023-05-23 06:27:19.000000 PrSpiders-0.4.9/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.4.9/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11047 2023-05-23 06:28:34.000000 PrSpiders-0.4.9/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     2675 2023-05-23 06:26:59.000000 PrSpiders-0.4.9/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.4.9/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.9/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.334265 PrSpiders-0.4.9/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5678 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.348269 PrSpiders-0.4.9/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.4.9/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.393265 PrSpiders-0.4.9/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.9/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.9/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.9/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.4.9/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.438271 PrSpiders-0.4.9/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.9/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.9/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.9/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.9/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 06:30:14.483267 PrSpiders-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-23 06:28:54.000000 PrSpiders-0.4.9/setup.py
```

### Comparing `PrSpiders-0.4.8/LICENSE.txt` & `PrSpiders-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/PKG-INFO` & `PrSpiders-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.8
+Version: 0.4.9
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.8/PrSpider/PrSpiders.py` & `PrSpiders-0.4.9/PrSpider/PrSpiders.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import re
 import sys
 import time
 from typing import Optional
 from loguru import logger as loguer
 from .requestXpath import prequest
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from .pyconn import PrMysql
+
+
 
 
 class settions(object):
     workers: Optional[int] = 10000
     request_num: Optional[int] = 0
     retry_num: Optional[int] = 0
     success_num: Optional[int] = 0
@@ -25,43 +28,43 @@
     logger: Optional[bool or str] = False
     log_level: Optional[str] = "info"
     log_stdout: Optional[bool] = False
     futures: Optional[list] = set()
 
 
 class PrSpiders(settions):
-    def __init__(self) -> None:
+    def __init__(self, **kwargs) -> None:
         settions.request_num = self.request_num
         settions.success_num = self.success_num
         settions.false_num = self.false_num
         settions.retry = self.retry
         settions.futures = self.futures
         settions.workers = self.workers
         settions.download_delay = self.download_delay
         settions.executor = ThreadPoolExecutor(settions.workers)
         settions.download_num = self.download_num
         settions.logger = self.logger
         settions.log_stdout = self.log_stdout
         settions.log_level = self.log_level
-        self.loggering(self.logger, self.log_level)
+        self.loguer = self.loggering(self.logger, self.log_level)
         loguer.warning(
             "\033[31m~~~ @PrSpider Start  @Workers %s  @Retry %s  @Pid %s @Download_Delay %s @Download_Num %s @LOG_LEVEL %s ~~~\033[0m"
             % (
                 self.workers,
                 self.retry,
                 self.pid,
                 self.download_delay,
                 self.download_num,
                 self.log_level.upper(),
             )
         )
         if not self.start_urls and not hasattr(self, "start_requests"):
             raise AttributeError("Crawling could not start: 'start_urls' not found ")
         else:
-            self.start_requests()
+            self.start_requests(**kwargs)
 
     def start_requests(self, **kwargs):
         if isinstance(self.start_urls, str):
             self.start_urls = [self.start_urls]
         url_dim_list = [
             self.start_urls[i: i + self.download_num]
             for i in range(0, len(self.start_urls), self.download_num)
@@ -284,14 +287,18 @@
                 else file_log + ".log"
             )
             filename = f"./{file_log}"
             loguer.add(filename, level=levels)
 
         return loguer
 
+    @classmethod
+    def PrMysql(self, **kwargs):
+        return PrMysql(loguer=loguer, **kwargs)
+
     def __del__(self):
         end_time = time.time()
         spend_time = end_time - self.start_time
         try:
             average_time = spend_time / self.request_num
         except ZeroDivisionError:
             average_time = 0
@@ -328,14 +335,7 @@
 class InterceptHandler():
     def write(self, message):
         if message.strip():
             loguer.log("Print", message.strip())
 
     def flush(self):
         pass
-
-
-class SpiderItem(object):
-    def __init__(self, **kwargs):
-        print(kwargs)
-
-    pass
```

### Comparing `PrSpiders-0.4.8/PrSpider/pxpath.py` & `PrSpiders-0.4.9/PrSpider/pxpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from urllib.parse import urljoin
 import re, time, copy
 from lxml import etree
 from datetime import timedelta, datetime
 import unicodedata
-
+from PrSpider.PrSpiders import loguer
 
 class Xpath(object):
     def __init__(self, response, encoding="utf-8"):
         if isinstance(response, str):
             self.res = etree.HTML(response)
         else:
             response.encoding = encoding
@@ -188,15 +188,15 @@
         if data is None or len(data) == 0:
             return None
         data = self.parse_txt(data)
         try:
             result = self.parse_time(data)
             return result
         except Exception as e:
-            logging.error(e)
+            loguer.error(e)
             return None
 
     @classmethod
     def repl_date(self, l: list):
         if len(l) > 1:
             raise ValueError("匹配时间数量超过一个 <str>%s</str>" % l)
         res = "".join(l).strip()
```

### Comparing `PrSpiders-0.4.8/PrSpider/requestXpath.py` & `PrSpiders-0.4.9/PrSpider/requestXpath.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,26 +37,26 @@
     def header(self):
         """
         :return: basic header
         """
         return {"user-agent": self.user_agent}
 
     def get(
-        self,
-        url,
-        headers=None,
-        retry_time=3,
-        method="GET",
-        meta=None,
-        encoding="utf-8",
-        retry_interval=1,
-        timeout=3,
-        settion=None,
-        *args,
-        **kwargs,
+            self,
+            url,
+            headers=None,
+            retry_time=3,
+            method="GET",
+            meta=None,
+            encoding="utf-8",
+            retry_interval=1,
+            timeout=3,
+            settion=None,
+            *args,
+            **kwargs,
     ):
         """
         get method
         :param url: target url
         :param header: headers default:
         :param retry_time: retry time default: 3
         :param retry_interval: retry interval default: 1
@@ -84,32 +84,32 @@
                     *args,
                     **kwargs,
                 )
                 self.response.encoding = encoding
                 if self.response.ok:
                     return self
                 else:
-                    raise Exception(f"Response.ok is False")
+                    raise Exception(f"Requests False %s" % self.code)
 
             except Exception as e:
                 retry_time -= 1
                 self.retry_num += 1
                 if retry_time < 0 or settion.retry is False:
-                    self.log.error("[Retry Fasle] %s [Error] %s" % (url, e))
+                    self.log.error("\033[31m[Retry Fasle] %s %s %s\033[0m" % (self.method, url, e))
                     self.response.status_code = (
                         410
                         if not self.response.status_code
                         else self.response.status_code
                     )
                     self.meta_["retry_num"] = self.retry_num
                     return self
                 else:
                     self.log.info(
-                        "[Retry] %s [Error] %s [Interval] %ss"
-                        % (url, e, retry_interval)
+                        "\033[31m[Retry] %s %s %s %ss\033[0m"
+                        % (url, self.method, e, retry_interval)
                     )
 
                 time.sleep(retry_interval)
 
     @property
     def text(self):
         return self.response.text
```

### Comparing `PrSpiders-0.4.8/PrSpider/useragent.py` & `PrSpiders-0.4.9/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.4.9/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.8
+Version: 0.4.9
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.8/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.4.9/PrSpiders.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 README.md
 setup.py
 PrSpider/PrSpiders.py
 PrSpider/__init__.py
 PrSpider/pxpath.py
+PrSpider/pyconn.py
 PrSpider/requestXpath.py
 PrSpider/useragent.py
 PrSpiders.egg-info/PKG-INFO
 PrSpiders.egg-info/SOURCES.txt
 PrSpiders.egg-info/dependency_links.txt
 PrSpiders.egg-info/entry_points.txt
 PrSpiders.egg-info/requires.txt
```

### Comparing `PrSpiders-0.4.8/README.md` & `PrSpiders-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.4.9/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/pkg/prspider/start.py` & `PrSpiders-0.4.9/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/requestXpath/__init__.py` & `PrSpiders-0.4.9/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/requestXpath/pxpath.py` & `PrSpiders-0.4.9/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/requestXpath/requestXpath.py` & `PrSpiders-0.4.9/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/requestXpath/useragent.py` & `PrSpiders-0.4.9/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.8/setup.py` & `PrSpiders-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

