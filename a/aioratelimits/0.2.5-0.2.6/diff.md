# Comparing `tmp/aioratelimits-0.2.5.tar.gz` & `tmp/aioratelimits-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioratelimits-0.2.5.tar", max compression
+gzip compressed data, was "aioratelimits-0.2.6.tar", max compression
```

## Comparing `aioratelimits-0.2.5.tar` & `aioratelimits-0.2.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      868 2022-08-21 06:32:22.351981 aioratelimits-0.2.5/README.md
--rw-r--r--   0        0        0     1257 2023-05-22 06:57:52.472737 aioratelimits-0.2.5/aioratelimits.py
--rw-r--r--   0        0        0      475 2023-05-22 06:58:27.072846 aioratelimits-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1384 2023-05-22 06:58:59.785410 aioratelimits-0.2.5/setup.py
--rw-r--r--   0        0        0     1472 2023-05-22 06:58:59.785678 aioratelimits-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      868 2022-08-21 06:32:22.351981 aioratelimits-0.2.6/README.md
+-rw-r--r--   0        0        0     1322 2023-05-23 05:47:24.535061 aioratelimits-0.2.6/aioratelimits.py
+-rw-r--r--   0        0        0      475 2023-05-23 05:47:40.150776 aioratelimits-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1384 2023-05-23 05:48:02.128266 aioratelimits-0.2.6/setup.py
+-rw-r--r--   0        0        0     1472 2023-05-23 05:48:02.128620 aioratelimits-0.2.6/PKG-INFO
```

### Comparing `aioratelimits-0.2.5/README.md` & `aioratelimits-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `aioratelimits-0.2.5/aioratelimits.py` & `aioratelimits-0.2.6/aioratelimits.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     async def worker(self):
         while True:
             coro, future = await self.call_queue.get()
 
             try:
                 result = await coro
                 future.set_result(result)
+            except asyncio.CancelledError:
+                raise
             except Exception as exc:
                 future.set_exception(exc)
 
             await asyncio.sleep(self.delay)
 
     def run(self, coro: Coroutine) -> asyncio.Future:
         future = asyncio.get_running_loop().create_future()
```

### Comparing `aioratelimits-0.2.5/setup.py` & `aioratelimits-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['aioratelimits']
 setup_kwargs = {
     'name': 'aioratelimits',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': '',
     'long_description': "# aioratelimits\n\nClient rate limiter. It enqueues function calls and run them as leaky bucket to\nensure specified rates.\n\n## Implementation\n\nLeaky bucket. We have one queue for requests and `count` number of workers.\nEach worker can handle one request per `delay` seconds\n\n## Install\n\n```\npip install aioratelimits\n```\n\n## Use\n\nThe following code prints not more than 2 lines per second.\n\n```python\nimport asyncio\nfrom aioratelimits import RateLimiter\n\n\nasync def critical_resource(i: int):\n    print('request:', i)\n\n\nasync def main():\n    async with RateLimiter(count=2, delay=1) as limiter:\n        await asyncio.gather(*(\n            limiter.run(critical_resource(i))\n            for i in range(10)\n        ))\n\n\nasyncio.run(main())\n```\n\nArguments to `RateLimiter`:\n- `count` - how many calls can we do in the specified interval\n- `delay` - the interval in seconds \n",
     'author': 'Dmitry Kostromin',
     'author_email': 'kupec-k@ya.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kupec/aioratelimits',
```

### Comparing `aioratelimits-0.2.5/PKG-INFO` & `aioratelimits-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioratelimits
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Home-page: https://github.com/kupec/aioratelimits
 Keywords: rates,ratelimit,ratelimiter,leaky,bucket
 Author: Dmitry Kostromin
 Author-email: kupec-k@ya.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

