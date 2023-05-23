# Comparing `tmp/th2_check2_recon-4.0.0.dev3884233338.tar.gz` & `tmp/th2_check2_recon-4.0.0.dev4312132973.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th2_check2_recon-4.0.0.dev3884233338.tar", max compression
+gzip compressed data, was "dist/th2_check2_recon-4.0.0.dev4312132973.tar", last modified: Thu Mar  2 08:45:51 2023, max compression
```

## Comparing `th2_check2_recon-4.0.0.dev3884233338.tar` & `th2_check2_recon-4.0.0.dev4312132973.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-01-10 14:24:42.822410 th2_check2_recon-4.0.0.dev3884233338/LICENSE
--rw-r--r--   0        0        0      227 2023-01-10 14:24:42.822410 th2_check2_recon-4.0.0.dev3884233338/README.md
--rw-r--r--   0        0        0      734 2023-01-10 14:25:02.294502 th2_check2_recon-4.0.0.dev3884233338/pyproject.toml
--rw-r--r--   0        0        0      813 2023-01-10 14:24:42.822410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/__init__.py
--rw-r--r--   0        0        0     6649 2023-01-10 14:24:42.822410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/builders.py
--rw-r--r--   0        0        0     1269 2023-01-10 14:24:42.822410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/new.py
--rw-r--r--   0        0        0     4427 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/recon.py
--rw-r--r--   0        0        0    11786 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/recon_message.py
--rw-r--r--   0        0        0     2806 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/rule.py
--rw-r--r--   0        0        0        0 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/cache/__init__.py
--rw-r--r--   0        0        0     2153 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/cache/cache.py
--rw-r--r--   0        0        0     4000 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/cache/message_groups.py
--rw-r--r--   0        0        0     2060 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/cache/storages.py
--rw-r--r--   0        0        0     3262 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/configuration.py
--rw-r--r--   0        0        0        0 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/events/__init__.py
--rw-r--r--   0        0        0     2423 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/events/event_manager.py
--rw-r--r--   0        0        0     8570 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/events/event_producers.py
--rw-r--r--   0        0        0     5194 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/handler.py
--rw-r--r--   0        0        0     2538 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/message_processor.py
--rw-r--r--   0        0        0     4516 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/process_units.py
--rw-r--r--   0        0        0     3376 2023-01-10 14:24:42.826410 th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/utils.py
--rw-r--r--   0        0        0     1183 1970-01-01 00:00:00.000000 th2_check2_recon-4.0.0.dev3884233338/setup.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 th2_check2_recon-4.0.0.dev3884233338/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5951 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2763 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5659 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4819 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/recon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/reconcommon.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11316 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/rule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24660 2023-03-02 08:45:35.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/services.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-02 08:45:51.000000 th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/__init__.py` & `th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/recon.py` & `th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/recon.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,91 +8,95 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import importlib
 import logging
-from typing import Dict, Optional
+from typing import Optional
 
-from th2_check2_recon.util.events.event_manager import EventManager
-from th2_check2_recon.util.events.event_producers import ReconEventProducer, EventType
+from grpc import Server
+from th2_common.schema.event.event_batch_router import EventBatchRouter
 from th2_common.schema.message.message_router import MessageRouter
-from th2_common_utils import event_utils
-from th2_grpc_common.common_pb2 import EventID, Event
 from th2_grpc_crawler_data_processor import crawler_data_processor_pb2_grpc
 
-from th2_check2_recon.recon_message import MessageGroupDescription, ReconMessage
-from th2_check2_recon.util.cache.cache import MessageGroup
-from th2_check2_recon.util.configuration import ReconConfiguration
-from th2_check2_recon.util.handler import GRPCHandler, MessageHandler
-from th2_check2_recon.util.message_processor import MessageProcessor
+from th2_check2_recon.configuration import ReconConfiguration
+from th2_check2_recon.handler import GRPCHandler
+from th2_check2_recon.reconcommon import MessageGroupType, ReconMessage
+from th2_check2_recon.services import EventStore, MessageComparator
 
 logger = logging.getLogger(__name__)
 
 
-class Recon(ReconEventProducer):
-
-    def __init__(self, name: str) -> None:
-        super().__init__(name)
+class Recon:
+    def __init__(self, event_router: EventBatchRouter, message_router: MessageRouter, custom_config: dict,
+                 message_comparator: Optional[MessageComparator] = None,
+                 grpc_server: Optional[Server] = None) -> None:
         logger.info('Recon initializing...')
-        self.message_processors: list = []
-        self.name = name
-
-        # self.configuration = ReconConfiguration(**custom_config)
-        self.message_router: Optional[MessageRouter] = None
-        self.event_router: Optional[MessageRouter] = None
-        # self.event_manager = EventManager(event_router, self.configuration.event_batch_send_interval)
-        # self.message_comparator: Optional[MessageComparator] = message_comparator
-        # self.grpc_server: Optional[Server] = grpc_server
-        self.shared_message_groups: Dict[str, MessageGroup] = {}
-
-        self.event_batch = None
-        self.event_producers = None
-
-    def add_message_processor(self, message_processor: MessageProcessor) -> None:
-        self.message_processors.append(message_processor)
+        self.rules = []
+        self._config = ReconConfiguration(**custom_config)
+        self.__message_router = message_router
+        self.event_store = EventStore(event_router=event_router,
+                                      recon_name=self._config.recon_name,
+                                      event_batch_max_size=self._config.event_batch_max_size,
+                                      event_batch_send_interval=self._config.event_batch_send_interval)
+        self.message_comparator: Optional[MessageComparator] = message_comparator
+        self.grpc_server: Optional[Server] = grpc_server
+        self.shared_message_groups = dict()
 
-    def start(self, message_router: MessageRouter, recon_configuration: ReconConfiguration, grpc_server) -> None:
+    def start(self):
         try:
-            self.message_router = message_router
-            self.message_router.subscribe_all(MessageHandler(self.message_processors), *recon_configuration.attributes)
+            logger.info('Recon running...')
+            self.rules = self.__load_rules()
+            for rule in self.rules:
+                for attrs in rule.get_attributes():
+                    self.__message_router.subscribe_all(rule.get_listener(), *attrs)
 
-            if grpc_server is not None:
-                grpc_handler = GRPCHandler(self.message_processors,
-                                           recon_configuration.crawler_connection_configuration,
-                                           self.event_id)
-                crawler_data_processor_pb2_grpc.add_DataProcessorServicer_to_server(grpc_handler, grpc_server)
-                grpc_server.start()
+            if self.grpc_server is not None:
+                grpc_handler = GRPCHandler(self.rules, self._config.crawler_connection_configuration,
+                                           self.event_store.recon_event_id)
+                crawler_data_processor_pb2_grpc.add_DataProcessorServicer_to_server(grpc_handler, self.grpc_server)
+                self.grpc_server.start()
 
+            logger.info('Recon started!')
         except Exception:
             logger.exception('Recon work interrupted')
             raise
 
-    def stop(self) -> None:
-        logger.info('Recon is trying to stop')
+    def stop(self):
+        logger.info('Recon try to stop')
         try:
-            self.message_router.unsubscribe_all()
+            self.__message_router.unsubscribe_all()
             for rule in self.rules:
                 rule.stop()
             if self.message_comparator is not None:
                 self.message_comparator.stop()
-            # self.event_manager.stop()
-        except Exception as e:
-            logger.exception(f'Error while stopping Recon: {e}')
+            self.event_store.stop()
+        except Exception:
+            logger.exception('Error while stop Recon')
         finally:
-            logger.info('Recon was stopped!')
+            logger.info('Recon stopped!')
+
+    def __load_rules(self):
+        logger.info('Try load rules')
+        rules_package = importlib.import_module(self._config.rules_package_path)
+        loaded_rules = []
+        for number, rule_config in enumerate(self._config.rules):
+            if rule_config.enabled:
+                module = importlib.import_module(rules_package.__name__ + '.' + rule_config.name)
+                match_timeout = rule_config.match_timeout * 1_000_000_000 + rule_config.match_timeout_offset_ns
+                loaded_rules.append(module.Rule(recon=self,
+                                                cache_size=self._config.cache_size,
+                                                match_timeout=match_timeout,
+                                                autoremove_timeout=rule_config.autoremove_timeout,
+                                                configuration=rule_config.configuration,
+                                                metric_number=number + 1))
+        logger.info('Rules loaded')
+        return loaded_rules
 
-    def put_shared_message(self, recon_message: ReconMessage) -> None:
+    def put_shared_message(self, shared_group_id: str, new_message: ReconMessage, attributes: tuple):
         for rule in self.rules:
-            if recon_message.group_name is None:
-                raise AttributeError('Group name should be set in ReconMessage before putting it in shared group')
-            message_group = recon_message.group_name
-            rule_groups: Dict[str, MessageGroupDescription] = rule.description_of_groups()
-            if message_group in rule_groups:
-                if rule_groups[message_group].shared:
-                    recon_message._shared = True
-                else:
-                    raise AttributeError(
-                        f'Trying to put shared message in group that '
-                        f'is not shared: {message_group}')
+            groups = rule.description_of_groups_bridge()
+            if shared_group_id in groups.keys() and MessageGroupType.shared in groups[shared_group_id]:
+                rule.process(new_message, attributes)
```

### Comparing `th2_check2_recon-4.0.0.dev3884233338/th2_check2_recon/util/configuration.py` & `th2_check2_recon-4.0.0.dev4312132973/th2_check2_recon/configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,67 +9,50 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
-from typing import Dict, Optional, Union, List, Any
+from typing import Optional, Dict
 
 
 class RuleConfiguration:
 
-    def __init__(self,
-                 name: str,
-                 enabled: str,
-                 cache_size: int,
-                 match_timeout: str,
-                 match_timeout_offset_ns: str,
-                 match_all: Optional[str] = None,
-                 autoremove_timeout: Optional[str] = None,
-                 custom_configuration: Optional[Any] = None) -> None:
+    def __init__(self, name, enabled, match_timeout, match_timeout_offset_ns, autoremove_timeout=None, configuration=None) -> None:
         self.name = str(name)
-        self.enabled = enabled.lower() == 'true'
-        self.cache_size = int(cache_size)
-        self.match_timeout = float(match_timeout)
+        self.enabled = True if enabled.lower() == 'true' else False
+        self.match_timeout = int(match_timeout)
         self.match_timeout_offset_ns = int(match_timeout_offset_ns)
-        self.match_all = match_all is not None and match_all.lower() == 'true'
-        self.autoremove_timeout: Optional[Union[int, datetime.datetime]]
         if autoremove_timeout is not None:
             try:
-                timeout_int = int(autoremove_timeout)
-                self.autoremove_timeout = timeout_int
+                self.autoremove_timeout = int(autoremove_timeout)
             except ValueError:
-                timeout = datetime.datetime.strptime(autoremove_timeout, '%H:%M')
-                self.autoremove_timeout = timeout.combine(datetime.datetime.now().date(), timeout.time())
+                self.autoremove_timeout = datetime.datetime.strptime(autoremove_timeout, '%H:%M')
+                self.autoremove_timeout = self.autoremove_timeout.combine(datetime.datetime.now().date(),
+                                                                          self.autoremove_timeout.time())
         else:
             self.autoremove_timeout = None
-        self.custom_configuration = custom_configuration
+        self.configuration = configuration
 
 
 class CrawlerConnectionConfiguration:
 
     def __init__(self, name: str = 'Recon Data Processor', version: str = '1.0.0') -> None:
         self.name = name
         self.version = version
 
 
 class ReconConfiguration:
-    def __init__(self,
-                 *,
-                 recon_name: str,
-                 attributes: List[str],
-                 event_batch_max_size: int,
-                 event_batch_send_interval: int,
-                 rules_package_path: str,
-                 rules: list,
+    def __init__(self, recon_name: str, cache_size: int, event_batch_max_size: int,
+                 event_batch_send_interval: int, rules_package_path: str, rules: list,
                  crawler_connection_configuration: Optional[Dict[str, str]] = None,
-                 configuration: Optional[str] = None) -> None:
+                 configuration=None) -> None:
         self.recon_name = recon_name
-        self.attributes = attributes
+        self.cache_size = int(cache_size)
         self.event_batch_max_size = int(event_batch_max_size)
         self.event_batch_send_interval = int(event_batch_send_interval)
         self.rules_package_path = rules_package_path
         self.rules = [RuleConfiguration(**rule) for rule in rules]
 
         if crawler_connection_configuration is None:
             self.crawler_connection_configuration = CrawlerConnectionConfiguration()
```

