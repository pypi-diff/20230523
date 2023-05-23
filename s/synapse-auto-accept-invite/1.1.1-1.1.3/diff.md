# Comparing `tmp/synapse_auto_accept_invite-1.1.1.tar.gz` & `tmp/synapse_auto_accept_invite-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapse_auto_accept_invite-1.1.1.tar", last modified: Thu May 26 13:59:56 2022, max compression
+gzip compressed data, was "synapse_auto_accept_invite-1.1.3.tar", last modified: Tue May 23 19:40:36 2023, max compression
```

## Comparing `synapse_auto_accept_invite-1.1.1.tar` & `synapse_auto_accept_invite-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 rei       (1000) rei       (1000)        0 2022-05-26 13:59:56.233506 synapse_auto_accept_invite-1.1.1/
--rw-rw-r--   0 rei       (1000) rei       (1000)    10174 2021-12-16 16:26:58.000000 synapse_auto_accept_invite-1.1.1/LICENSE
--rw-rw-r--   0 rei       (1000) rei       (1000)     2754 2022-05-26 13:59:56.233506 synapse_auto_accept_invite-1.1.1/PKG-INFO
--rw-rw-r--   0 rei       (1000) rei       (1000)     2345 2022-05-26 13:56:50.000000 synapse_auto_accept_invite-1.1.1/README.md
--rw-rw-r--   0 rei       (1000) rei       (1000)      192 2021-12-16 16:26:58.000000 synapse_auto_accept_invite-1.1.1/pyproject.toml
--rw-rw-r--   0 rei       (1000) rei       (1000)      664 2022-05-26 13:59:56.233506 synapse_auto_accept_invite-1.1.1/setup.cfg
-drwxrwxr-x   0 rei       (1000) rei       (1000)        0 2022-05-26 13:59:56.233506 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite/
--rw-rw-r--   0 rei       (1000) rei       (1000)     5603 2022-05-26 13:56:53.000000 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite/__init__.py
-drwxrwxr-x   0 rei       (1000) rei       (1000)        0 2022-05-26 13:59:56.233506 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite.egg-info/
--rw-rw-r--   0 rei       (1000) rei       (1000)     2754 2022-05-26 13:59:55.000000 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite.egg-info/PKG-INFO
--rw-rw-r--   0 rei       (1000) rei       (1000)      330 2022-05-26 13:59:56.000000 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite.egg-info/SOURCES.txt
--rw-rw-r--   0 rei       (1000) rei       (1000)        1 2022-05-26 13:59:55.000000 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite.egg-info/dependency_links.txt
--rw-rw-r--   0 rei       (1000) rei       (1000)      141 2022-05-26 13:59:56.000000 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite.egg-info/requires.txt
--rw-rw-r--   0 rei       (1000) rei       (1000)       27 2022-05-26 13:59:56.000000 synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite.egg-info/top_level.txt
+drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/
+-rw-rw-r--   0 shay      (1000) shay      (1000)    10174 2023-05-04 18:07:33.000000 synapse_auto_accept_invite-1.1.3/LICENSE
+-rw-rw-r--   0 shay      (1000) shay      (1000)     3158 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/PKG-INFO
+-rw-rw-r--   0 shay      (1000) shay      (1000)     2749 2023-05-23 19:03:03.000000 synapse_auto_accept_invite-1.1.3/README.md
+-rw-rw-r--   0 shay      (1000) shay      (1000)      192 2023-05-04 18:07:33.000000 synapse_auto_accept_invite-1.1.3/pyproject.toml
+-rw-rw-r--   0 shay      (1000) shay      (1000)      664 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/setup.cfg
+-rw-rw-r--   0 shay      (1000) shay      (1000)       36 2023-05-12 19:46:18.000000 synapse_auto_accept_invite-1.1.3/setup.py
+drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite/
+-rw-rw-r--   0 shay      (1000) shay      (1000)     7216 2023-05-16 20:22:10.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite/__init__.py
+drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/
+-rw-rw-r--   0 shay      (1000) shay      (1000)     3158 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/PKG-INFO
+-rw-rw-r--   0 shay      (1000) shay      (1000)      367 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/SOURCES.txt
+-rw-rw-r--   0 shay      (1000) shay      (1000)        1 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/dependency_links.txt
+-rw-rw-r--   0 shay      (1000) shay      (1000)      141 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/requires.txt
+-rw-rw-r--   0 shay      (1000) shay      (1000)       27 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/top_level.txt
+drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/tests/
+-rw-rw-r--   0 shay      (1000) shay      (1000)    14715 2023-05-16 20:22:10.000000 synapse_auto_accept_invite-1.1.3/tests/test_accept_invite.py
```

### Comparing `synapse_auto_accept_invite-1.1.1/LICENSE` & `synapse_auto_accept_invite-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_auto_accept_invite-1.1.1/PKG-INFO` & `synapse_auto_accept_invite-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: synapse_auto_accept_invite
-Version: 1.1.1
+Version: 1.1.3
 Summary: "Synapse module to automatically accept invites"
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Auto-accept invites
 
 Synapse module to automatically accept invites.
 
-Compatible with Synapse v1.57.0 and later.
+Compatible with Synapse v1.84.0 and later.
 
 ## Installation
 
 From the virtual environment that you use for Synapse, install this module with:
 ```shell
 pip install synapse-auto-accept-invite
 ```
@@ -32,18 +32,25 @@
     config:
       # Optional: if set to true, then only invites for direct messages (1:1 rooms)
       # will be auto accepted. Otherwise, all room invites are accepted.
       # Defaults to false.
       accept_invites_only_for_direct_messages: false
 
       # (For workerised Synapse deployments)
-      # If you want to accept invites on a specific worker, specify its instance
-      # name here. Otherwise, invites will be processed on the main process.
       #
-      # Any worker can be used.
+      # This module should only be active on a single worker process at once,
+      # otherwise invites may be accepted by multiple workers simultaneously.
+      #
+      # By default, this module is only enabled on the main process, and is disabled
+      # on workers. To choose a worker to run this module on (to reduce load on the
+      # main process), specify that worker's configured 'worker_name' below.
+      #
+      # Any worker may be specified. If this worker does not have the ability to
+      # write to Synapse's events stream, it will end up calling out to one that
+      # does.
       #
       #worker_to_run_on: workername1
 ```
 
 
 ### A note about logging
```

### Comparing `synapse_auto_accept_invite-1.1.1/README.md` & `synapse_auto_accept_invite-1.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Auto-accept invites
 
 Synapse module to automatically accept invites.
 
-Compatible with Synapse v1.57.0 and later.
+Compatible with Synapse v1.84.0 and later.
 
 ## Installation
 
 From the virtual environment that you use for Synapse, install this module with:
 ```shell
 pip install synapse-auto-accept-invite
 ```
@@ -20,18 +20,25 @@
     config:
       # Optional: if set to true, then only invites for direct messages (1:1 rooms)
       # will be auto accepted. Otherwise, all room invites are accepted.
       # Defaults to false.
       accept_invites_only_for_direct_messages: false
 
       # (For workerised Synapse deployments)
-      # If you want to accept invites on a specific worker, specify its instance
-      # name here. Otherwise, invites will be processed on the main process.
       #
-      # Any worker can be used.
+      # This module should only be active on a single worker process at once,
+      # otherwise invites may be accepted by multiple workers simultaneously.
+      #
+      # By default, this module is only enabled on the main process, and is disabled
+      # on workers. To choose a worker to run this module on (to reduce load on the
+      # main process), specify that worker's configured 'worker_name' below.
+      #
+      # Any worker may be specified. If this worker does not have the ability to
+      # write to Synapse's events stream, it will end up calling out to one that
+      # does.
       #
       #worker_to_run_on: workername1
 ```
 
 
 ### A note about logging
```

### Comparing `synapse_auto_accept_invite-1.1.1/setup.cfg` & `synapse_auto_accept_invite-1.1.3/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = synapse_auto_accept_invite
 description = "Synapse module to automatically accept invites"
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 1.1.1
+version = 1.1.3
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 python_requires = >= 3.7
 
 [options.extras_require]
 dev = 
-	matrix-synapse >= 1.57.0
+	matrix-synapse >= 1.84.0
 	tox
 	twisted
 	aiounittest
 	attrs
 	frozendict
 	mypy == 0.931
 	types-frozendict
```

### Comparing `synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite/__init__.py` & `synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import logging
 from typing import Any, Dict, Optional, Tuple
 
 import attr
-from synapse.module_api import EventBase, ModuleApi
+from synapse.module_api import EventBase, ModuleApi, run_as_background_process
 
 logger = logging.getLogger(__name__)
 ACCOUNT_DATA_DIRECT_MESSAGE_LIST = "m.direct"
 
 
 @attr.s(auto_attribs=True, frozen=True)
 class InviteAutoAccepterConfig:
@@ -91,20 +91,24 @@
             is_direct_message = event.content.get("is_direct", False)
 
             # Only accept invites for direct messages if the configuration mandates it, otherwise accept all invites.
             if (
                 not self._config.accept_invites_only_for_direct_messages
                 or is_direct_message is True
             ):
-                # Make the user join the room.
-                await self._api.update_room_membership(
-                    sender=event.state_key,
-                    target=event.state_key,
-                    room_id=event.room_id,
-                    new_membership="join",
+                # Make the user join the room. We run this as a background process to circumvent a race condition
+                # that occurs when responding to invites over federation (see https://github.com/matrix-org/synapse-auto-accept-invite/issues/12)
+                run_as_background_process(
+                    "retry_make_join",
+                    self._retry_make_join,
+                    event.state_key,
+                    event.state_key,
+                    event.room_id,
+                    "join",
+                    bg_start_span=False,
                 )
 
                 if is_direct_message:
                     # Mark this room as a direct message!
                     await self._mark_room_as_direct_message(
                         event.state_key, event.sender, event.room_id
                     )
@@ -145,7 +149,44 @@
                 return
 
             dm_map[dm_user_id] = tuple(dm_rooms_for_user) + (room_id,)
 
         await self._api.account_data_manager.put_global(
             user_id, ACCOUNT_DATA_DIRECT_MESSAGE_LIST, dm_map
         )
+
+    async def _retry_make_join(
+        self, sender: str, target: str, room_id: str, new_membership: str
+    ) -> None:
+        """
+        A function to retry sending the `make_join` request with an increasing backoff. This is
+        implemented to work around a race condition when receiving invites over federation.
+
+        Args:
+            sender: the user performing the membership change
+            target: the for whom the membership is changing
+            room_id: room id of the room to join to
+            new_membership: the type of membership event (in this case will be "join")
+        """
+
+        sleep = 0
+        retries = 0
+        join_event = None
+
+        while retries < 5:
+            try:
+                await self._api.sleep(sleep)
+                join_event = await self._api.update_room_membership(
+                    sender=sender,
+                    target=target,
+                    room_id=room_id,
+                    new_membership=new_membership,
+                )
+            except Exception as e:
+                logger.info(
+                    f"Update_room_membership raised the following exception: {e}"
+                )
+                sleep = 2**retries
+                retries += 1
+
+            if join_event is not None:
+                break
```

### Comparing `synapse_auto_accept_invite-1.1.1/synapse_auto_accept_invite.egg-info/PKG-INFO` & `synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: synapse-auto-accept-invite
-Version: 1.1.1
+Version: 1.1.3
 Summary: "Synapse module to automatically accept invites"
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Auto-accept invites
 
 Synapse module to automatically accept invites.
 
-Compatible with Synapse v1.57.0 and later.
+Compatible with Synapse v1.84.0 and later.
 
 ## Installation
 
 From the virtual environment that you use for Synapse, install this module with:
 ```shell
 pip install synapse-auto-accept-invite
 ```
@@ -32,18 +32,25 @@
     config:
       # Optional: if set to true, then only invites for direct messages (1:1 rooms)
       # will be auto accepted. Otherwise, all room invites are accepted.
       # Defaults to false.
       accept_invites_only_for_direct_messages: false
 
       # (For workerised Synapse deployments)
-      # If you want to accept invites on a specific worker, specify its instance
-      # name here. Otherwise, invites will be processed on the main process.
       #
-      # Any worker can be used.
+      # This module should only be active on a single worker process at once,
+      # otherwise invites may be accepted by multiple workers simultaneously.
+      #
+      # By default, this module is only enabled on the main process, and is disabled
+      # on workers. To choose a worker to run this module on (to reduce load on the
+      # main process), specify that worker's configured 'worker_name' below.
+      #
+      # Any worker may be specified. If this worker does not have the ability to
+      # write to Synapse's events stream, it will end up calling out to one that
+      # does.
       #
       #worker_to_run_on: workername1
 ```
 
 
 ### A note about logging
```

