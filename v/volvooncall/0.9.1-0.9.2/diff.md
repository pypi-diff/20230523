# Comparing `tmp/volvooncall-0.9.1.tar.gz` & `tmp/volvooncall-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volvooncall-0.9.1.tar", last modified: Mon Nov  1 22:46:55 2021, max compression
+gzip compressed data, was "volvooncall-0.9.2.tar", last modified: Tue Jan 25 18:13:41 2022, max compression
```

## Comparing `volvooncall-0.9.1.tar` & `volvooncall-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jkeslin    (502) staff       (20)        0 2021-11-01 22:46:54.988367 volvooncall-0.9.1/
--rw-r--r--   0 jkeslin    (502) staff       (20)     1210 2021-10-27 20:39:17.000000 volvooncall-0.9.1/LICENSE
--rw-r--r--   0 jkeslin    (502) staff       (20)       41 2021-10-27 20:39:17.000000 volvooncall-0.9.1/MANIFEST.in
--rw-r--r--   0 jkeslin    (502) staff       (20)      284 2021-11-01 22:46:54.988608 volvooncall-0.9.1/PKG-INFO
--rw-r--r--   0 jkeslin    (502) staff       (20)     2409 2021-10-29 16:47:29.000000 volvooncall-0.9.1/README.md
--rw-r--r--   0 jkeslin    (502) staff       (20)       78 2021-10-28 22:24:08.000000 volvooncall-0.9.1/requirements.txt
--rw-r--r--   0 jkeslin    (502) staff       (20)      347 2021-11-01 22:46:55.009815 volvooncall-0.9.1/setup.cfg
--rw-r--r--   0 jkeslin    (502) staff       (20)      461 2021-11-01 22:46:25.000000 volvooncall-0.9.1/setup.py
--rwxr-xr-x   0 jkeslin    (502) staff       (20)     9140 2021-10-28 22:24:08.000000 volvooncall-0.9.1/voc
-drwxr-xr-x   0 jkeslin    (502) staff       (20)        0 2021-11-01 22:46:54.979297 volvooncall-0.9.1/volvooncall/
--rw-r--r--   0 jkeslin    (502) staff       (20)      275 2021-10-28 22:24:08.000000 volvooncall-0.9.1/volvooncall/__init__.py
--rw-r--r--   0 jkeslin    (502) staff       (20)    14628 2021-11-01 22:46:03.000000 volvooncall-0.9.1/volvooncall/dashboard.py
--rwxr-xr-x   0 jkeslin    (502) staff       (20)    13478 2021-10-20 20:58:17.000000 volvooncall-0.9.1/volvooncall/mqtt.py
--rw-r--r--   0 jkeslin    (502) staff       (20)     3692 2021-10-28 22:24:08.000000 volvooncall-0.9.1/volvooncall/util.py
--rwxr-xr-x   0 jkeslin    (502) staff       (20)    13321 2021-11-01 22:46:25.000000 volvooncall-0.9.1/volvooncall/volvooncall.py
-drwxr-xr-x   0 jkeslin    (502) staff       (20)        0 2021-11-01 22:46:54.987450 volvooncall-0.9.1/volvooncall.egg-info/
--rw-r--r--   0 jkeslin    (502) staff       (20)      284 2021-11-01 22:46:53.000000 volvooncall-0.9.1/volvooncall.egg-info/PKG-INFO
--rw-r--r--   0 jkeslin    (502) staff       (20)      359 2021-11-01 22:46:53.000000 volvooncall-0.9.1/volvooncall.egg-info/SOURCES.txt
--rw-r--r--   0 jkeslin    (502) staff       (20)        1 2021-11-01 22:46:53.000000 volvooncall-0.9.1/volvooncall.egg-info/dependency_links.txt
--rw-r--r--   0 jkeslin    (502) staff       (20)       96 2021-11-01 22:46:53.000000 volvooncall-0.9.1/volvooncall.egg-info/requires.txt
--rw-r--r--   0 jkeslin    (502) staff       (20)       12 2021-11-01 22:46:53.000000 volvooncall-0.9.1/volvooncall.egg-info/top_level.txt
+drwxr-xr-x   0 jkeslin    (502) staff       (20)        0 2022-01-25 18:13:41.214732 volvooncall-0.9.2/
+-rw-r--r--   0 jkeslin    (502) staff       (20)     1210 2021-10-27 20:39:17.000000 volvooncall-0.9.2/LICENSE
+-rw-r--r--   0 jkeslin    (502) staff       (20)       41 2021-10-27 20:39:17.000000 volvooncall-0.9.2/MANIFEST.in
+-rw-r--r--   0 jkeslin    (502) staff       (20)      307 2022-01-25 18:13:41.214867 volvooncall-0.9.2/PKG-INFO
+-rw-r--r--   0 jkeslin    (502) staff       (20)     2409 2021-10-29 16:47:29.000000 volvooncall-0.9.2/README.md
+-rw-r--r--   0 jkeslin    (502) staff       (20)       93 2022-01-25 18:12:31.000000 volvooncall-0.9.2/requirements.txt
+-rw-r--r--   0 jkeslin    (502) staff       (20)      347 2022-01-25 18:13:41.218467 volvooncall-0.9.2/setup.cfg
+-rw-r--r--   0 jkeslin    (502) staff       (20)      489 2022-01-25 18:13:29.000000 volvooncall-0.9.2/setup.py
+-rwxr-xr-x   0 jkeslin    (502) staff       (20)     9140 2021-10-28 22:24:08.000000 volvooncall-0.9.2/voc
+drwxr-xr-x   0 jkeslin    (502) staff       (20)        0 2022-01-25 18:13:41.208852 volvooncall-0.9.2/volvooncall/
+-rw-r--r--   0 jkeslin    (502) staff       (20)      275 2021-10-28 22:24:08.000000 volvooncall-0.9.2/volvooncall/__init__.py
+-rw-r--r--   0 jkeslin    (502) staff       (20)    14628 2021-11-01 22:46:03.000000 volvooncall-0.9.2/volvooncall/dashboard.py
+-rwxr-xr-x   0 jkeslin    (502) staff       (20)    13475 2022-01-25 18:12:31.000000 volvooncall-0.9.2/volvooncall/mqtt.py
+-rw-r--r--   0 jkeslin    (502) staff       (20)     3692 2021-10-28 22:24:08.000000 volvooncall-0.9.2/volvooncall/util.py
+-rwxr-xr-x   0 jkeslin    (502) staff       (20)    13321 2022-01-25 18:13:29.000000 volvooncall-0.9.2/volvooncall/volvooncall.py
+drwxr-xr-x   0 jkeslin    (502) staff       (20)        0 2022-01-25 18:13:41.214273 volvooncall-0.9.2/volvooncall.egg-info/
+-rw-r--r--   0 jkeslin    (502) staff       (20)      307 2022-01-25 18:13:41.000000 volvooncall-0.9.2/volvooncall.egg-info/PKG-INFO
+-rw-r--r--   0 jkeslin    (502) staff       (20)      359 2022-01-25 18:13:41.000000 volvooncall-0.9.2/volvooncall.egg-info/SOURCES.txt
+-rw-r--r--   0 jkeslin    (502) staff       (20)        1 2022-01-25 18:13:41.000000 volvooncall-0.9.2/volvooncall.egg-info/dependency_links.txt
+-rw-r--r--   0 jkeslin    (502) staff       (20)      111 2022-01-25 18:13:41.000000 volvooncall-0.9.2/volvooncall.egg-info/requires.txt
+-rw-r--r--   0 jkeslin    (502) staff       (20)       12 2022-01-25 18:13:41.000000 volvooncall-0.9.2/volvooncall.egg-info/top_level.txt
```

### Comparing `volvooncall-0.9.1/LICENSE` & `volvooncall-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `volvooncall-0.9.1/README.md` & `volvooncall-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `volvooncall-0.9.1/voc` & `volvooncall-0.9.2/voc`

 * *Files identical despite different names*

### Comparing `volvooncall-0.9.1/volvooncall/dashboard.py` & `volvooncall-0.9.2/volvooncall/dashboard.py`

 * *Files identical despite different names*

### Comparing `volvooncall-0.9.1/volvooncall/mqtt.py` & `volvooncall-0.9.2/volvooncall/mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from os.path import expanduser, join
 from time import time
 import string
 from platform import node as hostname
 import asyncio
 
 import certifi
-from hbmqtt.client import ClientException, ConnectException, MQTTClient
+from amqtt.client import ClientException, ConnectException, MQTTClient
 
 from .dashboard import Lock, Position, Sensor, BinarySensor, Switch
 from .util import camel2slug, whitelisted, owntracks_encrypt
 
 _LOGGER = logging.getLogger(__name__)
 
 STATE_ON = "on"
@@ -284,15 +284,15 @@
         await self.client.publish(
             topic, payload.encode("utf-8"), retain=retain
         )
         _LOGGER.debug("Published on %s: %s", topic, payload)
 
     async def subscribe_to(self, topic):
         _LOGGER.debug("Subscribing to %s", topic)
-        from hbmqtt.mqtt.constants import QOS_1
+        from amqtt.mqtt.constants import QOS_1
 
         await self.client.subscribe([(topic, QOS_1)])
         _LOGGER.debug("Subscribed to %s", topic)
         Entity.subscriptions[topic] = self
 
     def receive_command(self, command):
 
@@ -375,15 +375,15 @@
             await self.publish(self.state_topic, self.state)
         else:
             _LOGGER.warning("No state available for %s", self)
 
 
 async def run(voc, config):
 
-    logging.getLogger("hbmqtt.client.plugins.packet_logger_plugin").setLevel(
+    logging.getLogger("amqtt.client.plugins.packet_logger_plugin").setLevel(
         logging.WARNING
     )
 
     client_id = "voc_{hostname}_{time}".format(
         hostname=hostname(), time=time()
     )
```

### Comparing `volvooncall-0.9.1/volvooncall/util.py` & `volvooncall-0.9.2/volvooncall/util.py`

 * *Files identical despite different names*

### Comparing `volvooncall-0.9.1/volvooncall/volvooncall.py` & `volvooncall-0.9.2/volvooncall/volvooncall.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     json_serialize,
     is_valid_path,
     find_path,
     json_loads,
     read_config,
 )
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 _LOGGER = logging.getLogger(__name__)
 
 SERVICE_URL = "https://vocapi{region}.wirelesscar.net/customerapi/rest/v3.0/"
 DEFAULT_SERVICE_URL = SERVICE_URL.format(region="")
 
 HEADERS = {
```

