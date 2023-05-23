# Comparing `tmp/reaktion-0.1.8.tar.gz` & `tmp/reaktion-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaktion-0.1.8.tar", max compression
+gzip compressed data, was "reaktion-0.1.9.tar", max compression
```

## Comparing `reaktion-0.1.8.tar` & `reaktion-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,32 @@
--rw-r--r--   0        0        0      506 2022-06-21 09:29:56.234418 reaktion-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-17 08:42:08.083694 reaktion-0.1.8/reaktion/__init__.py
--rw-r--r--   0        0        0     4187 2022-05-19 11:38:29.786027 reaktion-0.1.8/reaktion/actor.py
--rw-r--r--   0        0        0      312 2022-05-19 11:41:01.646136 reaktion-0.1.8/reaktion/agent.py
--rw-r--r--   0        0        0       47 2021-09-20 09:42:53.060166 reaktion-0.1.8/reaktion/atoms/__init__.py
--rw-r--r--   0        0        0      602 2022-04-04 16:29:22.860863 reaktion-0.1.8/reaktion/atoms/arkitekt.py
--rw-r--r--   0        0        0      965 2022-04-04 16:24:35.941336 reaktion-0.1.8/reaktion/atoms/base.py
--rw-r--r--   0        0        0        0 2022-04-04 16:23:46.665416 reaktion-0.1.8/reaktion/atoms/combination/__init__.py
--rw-r--r--   0        0        0       77 2022-04-04 16:29:38.416837 reaktion-0.1.8/reaktion/atoms/combination/base.py
--rw-r--r--   0        0        0     2534 2022-04-04 16:30:06.264791 reaktion-0.1.8/reaktion/atoms/combination/zip.py
--rw-r--r--   0        0        0       88 2022-04-04 16:21:02.517678 reaktion-0.1.8/reaktion/atoms/errors.py
--rw-r--r--   0        0        0     3807 2022-04-04 16:22:59.253492 reaktion-0.1.8/reaktion/atoms/generic.py
--rw-r--r--   0        0        0        0 2022-04-04 16:21:41.017617 reaktion-0.1.8/reaktion/atoms/reactive.py
--rw-r--r--   0        0        0     1348 2022-04-04 16:30:26.880756 reaktion-0.1.8/reaktion/atoms/utils.py
--rw-r--r--   0        0        0     1287 2022-04-04 16:20:03.497770 reaktion-0.1.8/reaktion/events.py
--rw-r--r--   0        0        0       84 2021-09-20 09:29:46.924529 reaktion-0.1.8/reaktion/exceptions.py
--rw-r--r--   0        0        0     3556 2022-05-19 11:41:01.646136 reaktion-0.1.8/reaktion/run.py
--rw-r--r--   0        0        0      469 2022-04-04 16:28:18.180971 reaktion-0.1.8/reaktion/utils.py
--rw-r--r--   0        0        0      654 2022-06-21 09:29:56.556907 reaktion-0.1.8/setup.py
--rw-r--r--   0        0        0      419 2022-06-21 09:29:56.557085 reaktion-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1012 2023-02-15 09:35:11.915431 reaktion-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-09-17 08:42:08.083694 reaktion-0.1.9/reaktion/__init__.py
+-rw-r--r--   0        0        0    11428 2023-02-08 10:53:03.584408 reaktion-0.1.9/reaktion/actor.py
+-rw-r--r--   0        0        0     1444 2023-02-06 15:04:34.112053 reaktion-0.1.9/reaktion/agent.py
+-rw-r--r--   0        0        0       47 2021-09-20 09:42:53.060165 reaktion-0.1.9/reaktion/atoms/__init__.py
+-rw-r--r--   0        0        0     1413 2023-01-27 17:18:03.117101 reaktion-0.1.9/reaktion/atoms/arkitekt.py
+-rw-r--r--   0        0        0     2272 2022-12-06 17:51:58.972143 reaktion-0.1.9/reaktion/atoms/base.py
+-rw-r--r--   0        0        0        0 2022-04-04 16:23:46.665416 reaktion-0.1.9/reaktion/atoms/combination/__init__.py
+-rw-r--r--   0        0        0       97 2022-12-06 14:55:06.089120 reaktion-0.1.9/reaktion/atoms/combination/base.py
+-rw-r--r--   0        0        0     2822 2022-12-06 14:29:45.350744 reaktion-0.1.9/reaktion/atoms/combination/combinelatest.py
+-rw-r--r--   0        0        0     2609 2023-02-07 14:23:56.076396 reaktion-0.1.9/reaktion/atoms/combination/withlatest.py
+-rw-r--r--   0        0        0     2770 2022-12-06 14:58:51.801537 reaktion-0.1.9/reaktion/atoms/combination/zip.py
+-rw-r--r--   0        0        0       88 2022-04-04 16:21:02.517678 reaktion-0.1.9/reaktion/atoms/errors.py
+-rw-r--r--   0        0        0     5541 2023-01-27 17:18:10.809060 reaktion-0.1.9/reaktion/atoms/generic.py
+-rw-r--r--   0        0        0       79 2022-08-29 14:09:01.909567 reaktion-0.1.9/reaktion/atoms/helpers.py
+-rw-r--r--   0        0        0      156 2022-12-06 14:54:55.253098 reaktion-0.1.9/reaktion/atoms/reactive.py
+-rw-r--r--   0        0        0     1024 2022-12-02 13:37:22.335094 reaktion-0.1.9/reaktion/atoms/template.py
+-rw-r--r--   0        0        0        0 2022-08-20 12:55:04.395533 reaktion-0.1.9/reaktion/atoms/transformation/__init__.py
+-rw-r--r--   0        0        0       80 2022-08-20 12:55:14.207540 reaktion-0.1.9/reaktion/atoms/transformation/base.py
+-rw-r--r--   0        0        0     3000 2023-02-10 17:05:31.078666 reaktion-0.1.9/reaktion/atoms/transformation/chunk.py
+-rw-r--r--   0        0        0      534 2022-12-06 14:56:56.029334 reaktion-0.1.9/reaktion/atoms/transport.py
+-rw-r--r--   0        0        0     2778 2022-12-13 10:39:52.202589 reaktion-0.1.9/reaktion/atoms/utils.py
+-rw-r--r--   0        0        0     1767 2023-02-06 15:38:20.438665 reaktion-0.1.9/reaktion/contractors.py
+-rw-r--r--   0        0        0      184 2022-06-22 15:55:48.466311 reaktion-0.1.9/reaktion/engine.py
+-rw-r--r--   0        0        0       89 2022-12-06 18:01:58.113316 reaktion-0.1.9/reaktion/errors.py
+-rw-r--r--   0        0        0     2358 2022-12-06 16:11:22.542952 reaktion-0.1.9/reaktion/events.py
+-rw-r--r--   0        0        0       84 2021-09-20 09:29:46.924529 reaktion-0.1.9/reaktion/exceptions.py
+-rw-r--r--   0        0        0      345 2022-06-27 14:32:55.166555 reaktion-0.1.9/reaktion/plant.py
+-rw-r--r--   0        0        0     4867 2023-02-02 15:45:24.549058 reaktion-0.1.9/reaktion/run.py
+-rw-r--r--   0        0        0     1553 2022-12-06 18:05:03.801643 reaktion-0.1.9/reaktion/utils.py
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 reaktion-0.1.9/setup.py
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 reaktion-0.1.9/PKG-INFO
```

### Comparing `reaktion-0.1.8/reaktion/atoms/combination/zip.py` & `reaktion-0.1.9/reaktion/atoms/combination/zip.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import asyncio
-from typing import Tuple
+from typing import List, Tuple
+import uuid
+from rekuest.api.schema import AssignationLogLevel
 from reaktion.atoms.combination.base import CombinationAtom
 from reaktion.events import EventType, OutEvent, Returns
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class ZipAtom(CombinationAtom):
-    state: Tuple[Returns, Returns] = (None, None)
+    state: List[Returns] = [None, None]
     complete: Tuple[bool, bool] = (False, False)
 
     async def run(self):
         try:
             while True:
-                event = await self.private_queue.get()
+                event = await self.get()
 
                 if event.type == EventType.ERROR:
-                    await self.event_queue.put(
+                    await self.transport.put(
                         OutEvent(
                             handle="return_0",
                             type=EventType.ERROR,
                             value=event.value,
                             source=self.node.id,
                         )
                     )
@@ -36,26 +38,31 @@
                 if event.handle == "arg_1":
                     if event.type == EventType.COMPLETE:
                         self.complete = (self.complete[0], True)
                     else:
                         self.state = (self.state[0], event)
 
                 if self.complete == (True, True):
-                    await self.event_queue.put(
+                    if self.alog:
+                        await self.alog(
+                            self.node.id,
+                            AssignationLogLevel.INFO,
+                            "ZipAtom: Complete",
+                        )
+                    await self.transport.put(
                         OutEvent(
                             handle="return_0",
                             type=EventType.COMPLETE,
                             source=self.node.id,
                         )
                     )
                     break  # Everything left of us is done, so we can shut down as well
 
                 if self.state[0] is not None and self.state[1] is not None:
-                    print("Zipping", self.state)
-                    await self.event_queue.put(
+                    await self.transport.put(
                         OutEvent(
                             handle="return_0",
                             type=EventType.NEXT,
                             value=self.state[0].value + self.state[1].value,
                             source=self.node.id,
                         )
                     )
```

### Comparing `reaktion-0.1.8/setup.py` & `reaktion-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['reaktion', 'reaktion.atoms', 'reaktion.atoms.combination']
+['reaktion',
+ 'reaktion.atoms',
+ 'reaktion.atoms.combination',
+ 'reaktion.atoms.transformation']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['arkitekt>=0.1.114,<0.2.0', 'fluss>=0.1.21,<0.2.0']
+['fluss>=0.1.24', 'rekuest>=0.1.10']
 
 setup_kwargs = {
     'name': 'reaktion',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

