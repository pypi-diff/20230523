# Comparing `tmp/ovos-config-0.0.9a3.tar.gz` & `tmp/ovos-config-0.0.9a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-config-0.0.9a3.tar", last modified: Fri May 19 18:30:32 2023, max compression
+gzip compressed data, was "ovos-config-0.0.9a4.tar", last modified: Tue May 23 18:37:50 2023, max compression
```

## Comparing `ovos-config-0.0.9a3.tar` & `ovos-config-0.0.9a4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:30:32.980147 ovos-config-0.0.9a3/
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-19 18:30:32.980147 ovos-config-0.0.9a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:30:32.976146 ovos-config-0.0.9a3/ovos_config/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/mycroft.conf
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:30:32.980147 ovos-config-0.0.9a3/ovos_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/ovos_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:30:32.980147 ovos-config-0.0.9a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-19 18:30:32.000000 ovos-config-0.0.9a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:37:50.927511 ovos-config-0.0.9a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-23 18:37:50.927511 ovos-config-0.0.9a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:37:50.923511 ovos-config-0.0.9a4/ovos_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15910 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/mycroft.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/ovos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:37:50.927511 ovos-config-0.0.9a4/ovos_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/ovos_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:37:50.927511 ovos-config-0.0.9a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-23 18:37:50.000000 ovos-config-0.0.9a4/setup.py
```

### Comparing `ovos-config-0.0.9a3/PKG-INFO` & `ovos-config-0.0.9a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-config
-Version: 0.0.9a3
+Version: 0.0.9a4
 Summary: ovos-core configuration module
 Home-page: https://github.com/OpenVoiceOS/ovos-config
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `ovos-config-0.0.9a3/README.md` & `ovos-config-0.0.9a4/README.md`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a3/ovos_config/__main__.py` & `ovos-config-0.0.9a4/ovos_config/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a3/ovos_config/config.py` & `ovos-config-0.0.9a4/ovos_config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import json
 from os.path import isfile
+from typing import Optional
 from time import sleep
 
-
-
-from ovos_config.models import LocalConf, MycroftDefaultConfig, MycroftSystemConfig, MycroftUserConfig, RemoteConf
-from ovos_config.locations import OLD_USER_CONFIG, get_xdg_config_save_path, get_xdg_config_locations
+from ovos_config.models import LocalConf, MycroftDefaultConfig, \
+    MycroftSystemConfig, MycroftUserConfig, RemoteConf
+from ovos_config.locations import OLD_USER_CONFIG, get_xdg_config_save_path, \
+    get_xdg_config_locations
 from ovos_config.utils import FileWatcher
 
 from ovos_utils.json_helper import flattened_delete, merge_dict
 from ovos_utils.log import LOG
 
 
 def _log_old_location_deprecation(old_user_config=OLD_USER_CONFIG):
@@ -136,44 +137,55 @@
         system_constraints = Configuration.get_system_constraints()
         if not remote:
             system_constraints["disable_remote_config"] = True
         return Configuration.load_all_configs(system_constraints)
 
     @staticmethod
     def reset():
+        """
+        Remove any configuration patches and reload configuration
+        """
         Configuration.__patch = {}
         Configuration.reload()
 
     @staticmethod
     def reload():
+        """
+        Reload all configuration files
+        """
         Configuration.default.reload()
         Configuration.system.reload()
         Configuration.remote.reload()
         for cfg in Configuration.xdg_configs:
             cfg.reload()
 
     @staticmethod
-    def get_system_constraints():
-        # constraints must come from SYSTEM config
-        # if not defined then load the DEFAULT constraints
-        # these settings can not be set anywhere else!
+    def get_system_constraints() -> dict:
+        """
+        Get Configuration constraints. Constraints must come from SYSTEM config.
+        If not defined, then load the DEFAULT constraints.
+        These settings can not be set anywhere else!
+        @return: dict of system configuration constraints
+        """
+
         return Configuration.system.get("system") or \
-               Configuration.default.get("system") or \
-               {}
+            Configuration.default.get("system") or \
+            {}
 
     @staticmethod
-    def load_all_configs(system_constraints=None):
-        """Load the stack of config files into a single dict
-
-        Returns:
-            (dict) merged dict of all configuration files
+    def load_all_configs(system_constraints: Optional[dict] = None) -> dict:
+        """
+        Load the stack of config files into a single dict
+        @param system_constraints: constraints to limit user/remote config usage
+        @return: merged dict of all configuration files
         """
         # system administrators can define different constraints in how
         # configurations are loaded
-        system_constraints = system_constraints or Configuration.get_system_constraints()
+        system_constraints = system_constraints or \
+            Configuration.get_system_constraints()
         skip_user = system_constraints.get("disable_user_config", False)
         skip_remote = system_constraints.get("disable_remote_config", False)
 
         configs = [Configuration.default, Configuration.system]
         if not skip_remote:
             configs.insert(1, Configuration.remote)
         if not skip_user:
@@ -185,15 +197,20 @@
         # runtime patches by skills / bus events
         configs.append(Configuration.__patch)
 
         # Merge all configs into one
         return Configuration.filter_and_merge(configs)
 
     @staticmethod
-    def filter_and_merge(configs):
+    def filter_and_merge(configs) -> dict:
+        """
+        Build and return a configuration dict based on configuration files
+        @param configs: List of Configuration objects to load
+        @return: dict Configuration, built from `configs`
+        """
         # ensure type
         for index, item in enumerate(configs):
             if isinstance(item, str):
                 configs[index] = LocalConf(item)
             elif not isinstance(item, LocalConf):
                 configs[index] = LocalConf(None)
                 configs[index].merge(item)
@@ -224,18 +241,17 @@
                 for protection in protected_user:
                     flattened_delete(cfg, protection)
             merge_dict(base, cfg)
         return base
 
     @staticmethod
     def set_config_update_handlers(bus):
-        """Setup websocket handlers to update config.
-
-        Args:
-            bus: Message bus client instance
+        """
+        Setup websocket handlers to update config on emitted changes.
+        @param bus: Message bus client instance
         """
         from ovos_utils.network_utils import is_connected
 
         # remove any old event listeners
         Configuration.deregister_bus()
 
         # attach new bus and listeners
@@ -251,69 +267,89 @@
         Configuration.set_config_watcher()
 
         # do the initial remote fetch
         if is_connected():
             Configuration.remote.reload()
 
     @staticmethod
-    def set_config_watcher(callback=None):
-        """Setup filewatcher to monitor for config file changes"""
+    def set_config_watcher(callback: Optional[callable] = None):
+        """
+        Setup filewatcher to monitor for config file changes
+        @param callback: optional method to call when configuration is changed
+        """
         paths = [Configuration.system.path] + \
                 [c.path for c in Configuration.xdg_configs]
         if callback:
             Configuration._callbacks.append(callback)
         if not Configuration._watchdog:
             Configuration._watchdog = FileWatcher(
                 [p for p in paths if isfile(p)],
                 Configuration._on_file_change
             )
 
     @staticmethod
-    def _on_file_change(path):
+    def _on_file_change(path: str):
+        """
+        Callback method for FileWatcher
+        @param path: Configuration file path reporting a change
+        """
         LOG.info(f'{path} changed on disk, reloading!')
         # reload updated config
         for cfg in Configuration.xdg_configs + [Configuration.system]:
             if cfg.path == path:
                 try:
                     cfg.reload()
+                    break
                 except:
                     # got the file changed signal before write finished
                     sleep(0.5)
-                    try:
-                        cfg.reload()
-                    except:
-                        LOG.exception("Failed to load configuration, syntax seems invalid!")
+                try:
+                    cfg.reload()
+                except:
+                    LOG.exception("Failed to load configuration, "
+                                  "syntax seems invalid!")
                 break
         else:
+            LOG.info(f"Reloading all configuration files, got: {path}")
             # reload all configs
             try:
                 Configuration.reload()
             except:
                 # got the file changed signal before write finished
                 sleep(0.5)
                 try:
                     Configuration.reload()
                 except:
-                    LOG.exception("Failed to load configuration, syntax seems invalid!")
+                    LOG.exception("Failed to load configuration, "
+                                  "syntax seems invalid!")
 
         for handler in Configuration._callbacks:
             try:
                 handler()
             except:
                 LOG.exception("Error in config update callback handler")
 
     @staticmethod
     def deregister_bus():
+        """
+        Remove messagebus handlers for configuration updates
+        """
         if Configuration.bus:
-            Configuration.bus.remove("configuration.updated", Configuration.updated)
-            Configuration.bus.remove("configuration.patch", Configuration.patch)
-            Configuration.bus.remove("configuration.patch.clear", Configuration.patch_clear)
-            Configuration.bus.remove("configuration.cache.clear", Configuration.clear_cache)
-            Configuration.bus.remove("mycroft.paired", Configuration.handle_remote_update)
-            Configuration.bus.remove("mycroft.internet.connected", Configuration.handle_remote_update)
+            Configuration.bus.remove("configuration.updated",
+                                     Configuration.updated)
+            Configuration.bus.remove("configuration.patch",
+                                     Configuration.patch)
+            Configuration.bus.remove("configuration.patch.clear",
+                                     Configuration.patch_clear)
+            Configuration.bus.remove("configuration.cache.clear",
+                                     Configuration.clear_cache)
+            Configuration.bus.remove("mycroft.paired",
+                                     Configuration.handle_remote_update)
+            Configuration.bus.remove("mycroft.internet.connected",
+                                     Configuration.handle_remote_update)
 
     @staticmethod
     def handle_remote_update(message):
         """Handler for paired/internet connect
 
         Triggers an update of remote config.
         """
```

### Comparing `ovos-config-0.0.9a3/ovos_config/locale.py` & `ovos-config-0.0.9a4/ovos_config/locale.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a3/ovos_config/locations.py` & `ovos-config-0.0.9a4/ovos_config/locations.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a3/ovos_config/meta.py` & `ovos-config-0.0.9a4/ovos_config/meta.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a3/ovos_config/models.py` & `ovos-config-0.0.9a4/ovos_config/models.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a3/ovos_config/mycroft.conf` & `ovos-config-0.0.9a4/ovos_config/mycroft.conf`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a3/ovos_config.egg-info/PKG-INFO` & `ovos-config-0.0.9a4/ovos_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-config
-Version: 0.0.9a3
+Version: 0.0.9a4
 Summary: ovos-core configuration module
 Home-page: https://github.com/OpenVoiceOS/ovos-config
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `ovos-config-0.0.9a3/setup.py` & `ovos-config-0.0.9a4/setup.py`

 * *Files identical despite different names*

