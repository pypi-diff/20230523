# Comparing `tmp/pye2-0.4.1.tar.gz` & `tmp/pye2-0.4.2.tar.gz`

## Comparing `pye2-0.4.1.tar` & `pye2-0.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.1/TODOs.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.1/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.1/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.1/winrun.bat
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/version.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/__init__.py
--rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/logger.py
--rw-r--r--   0        0        0    22815 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/pipeline.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/base.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/comms.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/misc.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/default/__init__.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/consts.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/mixins/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/mixins/plugins_manager_mixin.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/utils/code.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/.example_env
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/attach_example.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/ex1.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/hello.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/remote_exec.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/decentralized/dedist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/decentralized/dedist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/decentralized/dedist_example_worker.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.4.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.1/LICENSE
--rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 pye2-0.4.1/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 pye2-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.2/TODOs.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.2/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.2/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.2/winrun.bat
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/version.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/logger.py
+-rw-r--r--   0        0        0    22815 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/base.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/comms.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/misc.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/consts.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/mixins/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/mixins/plugins_manager_mixin.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/.example_env
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/attach_example.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/ex1.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/hello.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/remote_exec.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/decentralized/dedist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/decentralized/dedist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/decentralized/dedist_example_worker.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.4.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.2/LICENSE
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 pye2-0.4.2/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 pye2-0.4.2/PKG-INFO
```

### Comparing `pye2-0.4.1/.github/workflows/python-publish.yml` & `pye2-0.4.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/base/__init__.py` & `pye2-0.4.2/PyE2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/base/generic_session.py` & `pye2-0.4.2/PyE2/base/generic_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
       },
       "PAYLOADS_CHANNEL": {
           "TOPIC": "lummetry/payloads"
       },
       "QOS": 0
   }
 
-  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
+  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_payload=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
     """
     A Session is a connection to a communication server which provides the channel to interact with nodes from the AiXpand network.
     A Session manages `Pipelines` and handles all messages received from the communication server.
     The Session handles all callbacks that are user-defined and passed as arguments in the API calls.  
 
     Parameters
     ----------
@@ -110,14 +110,15 @@
     self._online_boxes = {}
     self._last_seen_boxes = {}
     self.online_timeout = 60
     self.filter_workers = filter_workers
 
     self._fill_config(host, port, user, pwd, name)
 
+    self.custom_on_payload = on_payload
     self.custom_on_heartbeat = on_heartbeat
     self.custom_on_notification = on_notification
 
     self.on_payload = self._on_payload_default
     self.on_heartbeat = self._on_heartbeat_default
     self.on_notification = self._on_notification_default
 
@@ -245,14 +246,18 @@
     for pipeline, callback in self.payload_pipeline_callbacks:
       if msg_eeid == pipeline.e2id and msg_stream == pipeline.name:
         callback(pipeline, msg_signature, msg_instance, Payload(msg_data))
 
     for pipeline, signature, instance, callback in self.payload_instance_callbacks:
       if msg_eeid == pipeline.e2id and msg_stream == pipeline.name and msg_signature == signature and msg_instance == instance:
         callback(pipeline, Payload(msg_data))
+
+    if self.custom_on_payload is not None:
+      self.custom_on_payload(self, msg_eeid, msg_signature, msg_instance, Payload(msg_data))
+
     return
 
   def _send_command_to_box(self, command, worker, payload):
     msg_to_send = {
         'EE_ID': worker,
         'SB_ID': worker,
         'ACTION': command,
```

### Comparing `pye2-0.4.1/PyE2/base/logger.py` & `pye2-0.4.2/PyE2/base/logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/base/pipeline.py` & `pye2-0.4.2/PyE2/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/base/payload/payload.py` & `pye2-0.4.2/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/comm/__init__.py` & `pye2-0.4.2/PyE2/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/comm/amqp_wrapper.py` & `pye2-0.4.2/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/comm/mqtt_wrapper.py` & `pye2-0.4.2/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/const/__init__.py` & `pye2-0.4.2/PyE2/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/const/base.py` & `pye2-0.4.2/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/const/comms.py` & `pye2-0.4.2/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/const/heartbeat.py` & `pye2-0.4.2/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/const/misc.py` & `pye2-0.4.2/PyE2/const/misc.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/const/payload.py` & `pye2-0.4.2/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/default/mqtt_session.py` & `pye2-0.4.2/PyE2/default/mqtt_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/__init__.py` & `pye2-0.4.2/PyE2/io_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/consts.py` & `pye2-0.4.2/PyE2/io_formatter/consts.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.4.2/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/base/__init__.py` & `pye2-0.4.2/PyE2/io_formatter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.4.2/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/default/__init__.py` & `pye2-0.4.2/PyE2/io_formatter/default/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.4.2/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/default/cavi2.py` & `pye2-0.4.2/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/io_formatter/mixins/plugins_manager_mixin.py` & `pye2-0.4.2/PyE2/io_formatter/mixins/plugins_manager_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,21 @@
     super(_PluginsManagerMixin, self).__init__()
     return
 
   def _get_plugin_by_name(self, lst_plugins_locations, name):
     name = self.log.camel_to_snake(name)
     for loc in lst_plugins_locations:
       candidate = loc + '.' + name
-      self.P("    Trying '{}'".format(candidate))
+      self.D("    Trying '{}'".format(candidate))
       try:
         found = importlib.util.find_spec(candidate)
         if found is not None:
           return candidate
       except:
-        self.P("      Invalid package: '{}'".format(candidate))
+        self.D("      Invalid package: '{}'".format(candidate))
     return
 
   def _get_module_name_and_class(self,
                                  locations,
                                  name,
                                  suffix=None,
                                  verbose=1,
@@ -92,15 +92,15 @@
       _module_name = _safe_module_name
 
     if _module_name is None:
       if verbose >= 1:
         self.P("Error with finding plugin '{}' in locations '{}'".format(simple_name, locations), color='r')
       return _module_name, _class_name, _cls_def, _config_dict
 
-    self.P("  Found {} plugin '{}'".format(
+    self.D("  Found {} plugin '{}'".format(
         'safe' if is_safe_plugin else 'user', name),
         color='g' if is_safe_plugin else 'm'
     )
 
     safety_check = False if is_safe_plugin else safety_check
     class_safety_check = False if is_safe_plugin else class_safety_check
 
@@ -123,15 +123,15 @@
       # change below to False to replicate issue !
       if isinstance(_config_dict_from_file, dict) and True:
         _config_dict = deepcopy(_config_dict_from_file)
       else:
         _config_dict = _config_dict_from_file
 
       _found_location = ".".join(_module_name.split('.')[:-1])
-      self.P("  Plugin '{}' loaded and code checked from {}".format(name, _found_location), color='g')
+      self.D("  Plugin '{}' loaded and code checked from {}".format(name, _found_location), color='g')
     except:
       str_err = traceback.format_exc()
       msg = "Error preparing {} with module {}:\n{}".format(
           name, _module_name, str_err)
       self.P(msg, color='error')
 
     return module, _class_name, _cls_def, _config_dict
```

### Comparing `pye2-0.4.1/PyE2/utils/code.py` & `pye2-0.4.2/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/PyE2/utils/code_exec.py` & `pye2-0.4.2/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/xperimental/attach_example.py` & `pye2-0.4.2/xperimental/attach_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/xperimental/ex1.py` & `pye2-0.4.2/xperimental/ex1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/xperimental/hello.py` & `pye2-0.4.2/xperimental/hello.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/xperimental/remote_exec.py` & `pye2-0.4.2/xperimental/remote_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/xperimental/save_images.py` & `pye2-0.4.2/xperimental/save_images.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from PyE2 import Session, Payload
 import os
 from time import sleep
 
 from dotenv import load_dotenv
 
 from PyE2 import Payload, Pipeline, Session
```

### Comparing `pye2-0.4.1/xperimental/decentralized/dedist_example.py` & `pye2-0.4.2/xperimental/decentralized/dedist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/xperimental/decentralized/dedist_example_initiator.py` & `pye2-0.4.2/xperimental/decentralized/dedist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/.gitignore` & `pye2-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/LICENSE` & `pye2-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/README.md` & `pye2-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pye2-0.4.1/pyproject.toml` & `pye2-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pika", "paho-mqtt", "Pillow", "numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@global-technical.com" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@global-technical.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
 ]
 description = "PyE2 is an SDK used to communicate with the AiXpand network"
 readme = "README.md"
```

### Comparing `pye2-0.4.1/PKG-INFO` & `pye2-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyE2
-Version: 0.4.1
+Version: 0.4.2
 Summary: PyE2 is an SDK used to communicate with the AiXpand network
 Project-URL: Homepage, https://github.com/AiXpand/PyE2
 Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
 Author-email: Stefan Saraev <stefan.saraev@global-technical.com>, Cristan Bleotiu <cristan.bleotiu@global-technical.com>, Andrei Ionut Damian <andrei.damian@lummetry.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

