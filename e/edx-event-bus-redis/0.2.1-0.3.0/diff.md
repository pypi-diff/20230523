# Comparing `tmp/edx_event_bus_redis-0.2.1.tar.gz` & `tmp/edx_event_bus_redis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_redis-0.2.1.tar", last modified: Mon May 15 13:30:40 2023, max compression
+gzip compressed data, was "edx_event_bus_redis-0.3.0.tar", last modified: Tue May 23 18:16:21 2023, max compression
```

## Comparing `edx_event_bus_redis-0.2.1.tar` & `edx_event_bus_redis-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8372 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.396540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    20866 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/message.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.396540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8372 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-15 13:30:40.404540 edx_event_bus_redis-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8537 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20754 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.737677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8537 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/tests/test_models.py
```

### Comparing `edx_event_bus_redis-0.2.1/CHANGELOG.rst` & `edx_event_bus_redis-0.3.0/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.3.0] - 2023-05-23
+************************************************
+
+Changed
+=======
+* **BREAKING CHANGE**: Removed deprecated ``signal`` argument from consumer.
+
 [0.2.1] - 2023-05-12
 ************************************************
 
 Changed
 =======
 * Deprecated ``signal`` argument in consumer (made optional in preparation for removal)
```

### Comparing `edx_event_bus_redis-0.2.1/LICENSE.txt` & `edx_event_bus_redis-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/PKG-INFO` & `edx_event_bus_redis-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_redis
-Version: 0.2.1
+Version: 0.3.0
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -236,14 +236,21 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.3.0] - 2023-05-23
+************************************************
+
+Changed
+=======
+* **BREAKING CHANGE**: Removed deprecated ``signal`` argument from consumer.
+
 [0.2.1] - 2023-05-12
 ************************************************
 
 Changed
 =======
 * Deprecated ``signal`` argument in consumer (made optional in preparation for removal)
```

### Comparing `edx_event_bus_redis-0.2.1/README.rst` & `edx_event_bus_redis-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/config.py` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/consumer.py` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,28 +85,27 @@
     Note that the topic should be specified here *without* the optional environment prefix.
 
     Can also consume messages indefinitely off the queue.
 
     Attributes:
         topic: Topic/stream name.
         group_id: consumer group name.
-        signal: DEPRECATED, will be removed in a future release
         consumer_name: unique name for consumer within a group.
         last_read_msg_id: Start reading msgs from a specific redis msg id.
         check_backlog: flag to process all messages that were not read by this consumer group.
         claim_msgs_older_than: claim pending msgs from other consumers in the group with idle time older
             than a specific time (in milliseconds).
         has_pending_msgs: flag to process pending msgs first.
         db: Walrus object for redis connection.
         full_topic: topic prefixed with environment name.
         consumer: consumer instance.
     """
 
-    def __init__(self, topic, group_id, consumer_name, signal=None,  # pylint: disable=unused-argument
-                 last_read_msg_id=None, check_backlog=False, claim_msgs_older_than=None):
+    def __init__(self, topic, group_id, consumer_name, last_read_msg_id=None,
+                 check_backlog=False, claim_msgs_older_than=None):
         self.topic = topic
         self.group_id = group_id
         self.consumer_name = consumer_name
         self.last_read_msg_id = last_read_msg_id
         self.check_backlog = check_backlog
         # always process read but pending msgs first for the consumer in the group.
         self.has_pending_msgs = True
```

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/message.py` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/message.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/producer.py` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/utils.py` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/produce_event.py` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/PKG-INFO` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-bus-redis
-Version: 0.2.1
+Version: 0.3.0
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -236,14 +236,21 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.3.0] - 2023-05-23
+************************************************
+
+Changed
+=======
+* **BREAKING CHANGE**: Removed deprecated ``signal`` argument from consumer.
+
 [0.2.1] - 2023-05-12
 ************************************************
 
 Changed
 =======
 * Deprecated ``signal`` argument in consumer (made optional in preparation for removal)
```

### Comparing `edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/SOURCES.txt` & `edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/requirements/constraints.txt` & `edx_event_bus_redis-0.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.2.1/setup.py` & `edx_event_bus_redis-0.3.0/setup.py`

 * *Files identical despite different names*

