# Comparing `tmp/pye2-0.4.2.tar.gz` & `tmp/pye2-0.4.3.tar.gz`

## Comparing `pye2-0.4.2.tar` & `pye2-0.4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.2/TODOs.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.2/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.2/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.2/winrun.bat
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/version.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/__init__.py
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/logger.py
--rw-r--r--   0        0        0    22815 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/pipeline.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/base.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/comms.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/misc.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/default/__init__.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/consts.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/mixins/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/io_formatter/mixins/plugins_manager_mixin.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/utils/code.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.2/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/.example_env
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/attach_example.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/ex1.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/hello.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/remote_exec.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/decentralized/dedist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/decentralized/dedist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.2/xperimental/decentralized/dedist_example_worker.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.4.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.2/LICENSE
--rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 pye2-0.4.2/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 pye2-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.3/TODOs.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.3/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.3/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.3/winrun.bat
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/version.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    22829 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/base/logger.py
+-rw-r--r--   0        0        0    22815 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/const/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/const/base.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/const/comms.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/const/misc.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/consts.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/mixins/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/io_formatter/mixins/plugins_manager_mixin.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.3/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/.example_env
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/attach_example.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/ex1.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/hello.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/remote_exec.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/decentralized/dedist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/decentralized/dedist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.3/xperimental/decentralized/dedist_example_worker.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.4.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.3/LICENSE
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 pye2-0.4.3/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 pye2-0.4.3/PKG-INFO
```

### Comparing `pye2-0.4.2/.github/workflows/python-publish.yml` & `pye2-0.4.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/base/__init__.py` & `pye2-0.4.3/PyE2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/base/generic_session.py` & `pye2-0.4.3/PyE2/base/generic_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,19 @@
     filter_workers: list, optional
         If set, process the messages that come only from the nodes from this list. 
         Defaults to None
     log : Logger, optional
         A logger object which implements basic logging functionality and some other utils stuff. Can be ignored for now.
         In the future, the documentation for the Logger base class will be available and developers will be able to use
         custom-made Loggers. 
+    on_payload : Callable[[Session, str, str, str, dict], None], optional
+        Callback that handles all payloads received from this network.
+        As arguments, it has a reference to this Session object, the node name, the pipeline, signature and instance, and the payload. 
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
     on_notification : Callable[[Session, str, dict], None], optional
         Callback that handles notifications received from this network. 
         As arguments, it has a reference to this Session object, the node name and the notification payload. 
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
         This callback will be called when there are notifications related to the node itself, e.g. when the node runs
         low on memory.
```

### Comparing `pye2-0.4.2/PyE2/base/logger.py` & `pye2-0.4.3/PyE2/base/logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/base/pipeline.py` & `pye2-0.4.3/PyE2/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/base/payload/payload.py` & `pye2-0.4.3/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/comm/__init__.py` & `pye2-0.4.3/PyE2/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/comm/amqp_wrapper.py` & `pye2-0.4.3/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/comm/mqtt_wrapper.py` & `pye2-0.4.3/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/const/__init__.py` & `pye2-0.4.3/PyE2/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/const/base.py` & `pye2-0.4.3/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/const/comms.py` & `pye2-0.4.3/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/const/heartbeat.py` & `pye2-0.4.3/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/const/misc.py` & `pye2-0.4.3/PyE2/const/misc.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/const/payload.py` & `pye2-0.4.3/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/default/mqtt_session.py` & `pye2-0.4.3/PyE2/default/mqtt_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 from ..comm import MQTTWrapper
 from ..base import GenericSession
 
 
 # TODO: implement send_command, send_payload,
 #       to be used by the Pipeline class
 class MqttSession(GenericSession):
-  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
+  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_payload=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
     super(MqttSession, self).__init__(host=host, port=port, user=user, pwd=pwd, name=name, config=config, filter_workers=filter_workers,
-                                      log=log, on_notification=on_notification, on_heartbeat=on_heartbeat, silent=silent, **kwargs)
+                                      log=log, on_payload=on_payload, on_notification=on_notification, on_heartbeat=on_heartbeat, silent=silent, **kwargs)
 
     self._payload_messages = deque()
     self._default_communicator = MQTTWrapper(
         log=self.log,
         config=self._config,
         send_channel_name=comm_ct.COMMUNICATION_CONFIG_CHANNEL,
         recv_channel_name=comm_ct.COMMUNICATION_PAYLOADS_CHANNEL,
```

### Comparing `pye2-0.4.2/PyE2/io_formatter/__init__.py` & `pye2-0.4.3/PyE2/io_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/consts.py` & `pye2-0.4.3/PyE2/io_formatter/consts.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.4.3/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/base/__init__.py` & `pye2-0.4.3/PyE2/io_formatter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.4.3/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/default/__init__.py` & `pye2-0.4.3/PyE2/io_formatter/default/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.4.3/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/default/cavi2.py` & `pye2-0.4.3/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/io_formatter/mixins/plugins_manager_mixin.py` & `pye2-0.4.3/PyE2/io_formatter/mixins/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/utils/code.py` & `pye2-0.4.3/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/PyE2/utils/code_exec.py` & `pye2-0.4.3/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/xperimental/attach_example.py` & `pye2-0.4.3/xperimental/attach_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/xperimental/ex1.py` & `pye2-0.4.3/xperimental/ex1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/xperimental/hello.py` & `pye2-0.4.3/xperimental/hello.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/xperimental/remote_exec.py` & `pye2-0.4.3/xperimental/remote_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/xperimental/save_images.py` & `pye2-0.4.3/xperimental/save_images.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/xperimental/decentralized/dedist_example.py` & `pye2-0.4.3/xperimental/decentralized/dedist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/xperimental/decentralized/dedist_example_initiator.py` & `pye2-0.4.3/xperimental/decentralized/dedist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/.gitignore` & `pye2-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/LICENSE` & `pye2-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/README.md` & `pye2-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pye2-0.4.2/pyproject.toml` & `pye2-0.4.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pika", "paho-mqtt", "Pillow", "numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@global-technical.com" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@global-technical.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
 ]
 description = "PyE2 is an SDK used to communicate with the AiXpand network"
 readme = "README.md"
```

### Comparing `pye2-0.4.2/PKG-INFO` & `pye2-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyE2
-Version: 0.4.2
+Version: 0.4.3
 Summary: PyE2 is an SDK used to communicate with the AiXpand network
 Project-URL: Homepage, https://github.com/AiXpand/PyE2
 Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
 Author-email: Stefan Saraev <stefan.saraev@global-technical.com>, Cristan Bleotiu <cristan.bleotiu@global-technical.com>, Andrei Ionut Damian <andrei.damian@lummetry.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

