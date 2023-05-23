# Comparing `tmp/vantage6-node-3.8.8rc3.tar.gz` & `tmp/vantage6-node-3.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-3.8.8rc3.tar", last modified: Mon May 22 13:38:29 2023, max compression
+gzip compressed data, was "vantage6-node-3.9.0rc2.tar", last modified: Tue May  9 13:37:05 2023, max compression
```

## Comparing `vantage6-node-3.8.8rc3.tar` & `vantage6-node-3.9.0rc2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.564135 vantage6-node-3.8.8rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-22 13:38:29.564135 vantage6-node-3.8.8rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 13:38:29.564135 vantage6-node-3.8.8rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.560135 vantage6-node-3.8.8rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.560135 vantage6-node-3.8.8rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.560135 vantage6-node-3.8.8rc3/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.560135 vantage6-node-3.8.8rc3/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.560135 vantage6-node-3.8.8rc3/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/server_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.564135 vantage6-node-3.8.8rc3/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-22 13:38:16.000000 vantage6-node-3.8.8rc3/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.564135 vantage6-node-3.8.8rc3/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-22 13:38:29.000000 vantage6-node-3.8.8rc3/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-22 13:38:29.000000 vantage6-node-3.8.8rc3/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:29.000000 vantage6-node-3.8.8rc3/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 13:38:29.000000 vantage6-node-3.8.8rc3/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 13:38:29.000000 vantage6-node-3.8.8rc3/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 13:38:29.000000 vantage6-node-3.8.8rc3/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    40378 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19478 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22416 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/server_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-3.8.8rc3/PKG-INFO` & `vantage6-node-3.9.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.8rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc2 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.8.8rc3/setup.py` & `vantage6-node-3.9.0rc2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'click==8.1.3',
-        'docker==6.1.2',
+        'docker==6.0.1',
         'gevent==22.10.2',
         'python-socketio==5.7.2',
         'requests==2.28.2',
         f'vantage6 == {version_ns["__version__"]}',
         f'vantage6-client == {version_ns["__version__"]}',
     ],
     extras_require={
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/__init__.py` & `vantage6-node-3.9.0rc2/vantage6/node/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,39 +31,41 @@
 import queue
 import json
 import shutil
 import requests.exceptions
 
 from pathlib import Path
 from threading import Thread
-from typing import Dict, List, Union, Type
 from socketio import Client as SocketIO
 from gevent.pywsgi import WSGIServer
 from enum import Enum
 
+from vantage6.common import logger_name
 from vantage6.common.docker.addons import (
     ContainerKillListener, check_docker_running, running_in_docker
 )
 from vantage6.common.globals import VPN_CONFIG_FILE, PING_INTERVAL_SECONDS
 from vantage6.common.exceptions import AuthenticationException
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.common.task_status import TaskStatus
+from vantage6.common.log import get_file_logger
 from vantage6.cli.context import NodeContext
 from vantage6.node.context import DockerNodeContext
 from vantage6.node.globals import (
     NODE_PROXY_SERVER_HOSTNAME, SLEEP_BTWN_NODE_LOGIN_TRIES,
     TIME_LIMIT_RETRY_CONNECT_NODE, TIME_LIMIT_INITIAL_CONNECTION_WEBSOCKET
 )
 from vantage6.node.server_io import NodeClient
 from vantage6.node import proxy_server
-from vantage6.node.util import logger_name, get_parent_id
+from vantage6.node.util import get_parent_id
 from vantage6.node.docker.docker_manager import DockerManager
 from vantage6.node.docker.vpn_manager import VPNManager
 from vantage6.node.socket import NodeTaskNamespace
 from vantage6.node.docker.ssh_tunnel import SSHTunnel
+from vantage6.node.docker.squid import Squid
 
 
 class VPNConnectMode(Enum):
     FIRST_TRY = 1
     REFRESH_KEYPAIR = 2
     REFRESH_COMPLETE = 3
 
@@ -74,19 +76,19 @@
     Authenticates to the central server, setup encryption, a
     websocket connection, retrieving task that were posted while
     offline, preparing dataset for usage and finally setup a
     local proxy server..
 
     Parameters
     ----------
-    ctx: Union[NodeContext, DockerNodeContext]
+    ctx: NodeContext | DockerNodeContext
         Application context object.
 
     """
-    def __init__(self, ctx: Union[NodeContext, DockerNodeContext]):
+    def __init__(self, ctx: NodeContext | DockerNodeContext):
 
         self.log = logging.getLogger(logger_name(__name__))
         self.ctx = ctx
 
         # Initialize the node. If it crashes, shut down the parts that started
         # already
         try:
@@ -123,14 +125,18 @@
 
         # Thread for proxy server for algorithm containers, so they can
         # communicate with the central server.
         self.log.info("Setting up proxy server")
         t = Thread(target=self.__proxy_server_worker, daemon=True)
         t.start()
 
+        # Create a long-lasting websocket connection.
+        self.log.debug("Creating websocket connection with the server")
+        self.connect_to_socket()
+
         # setup docker isolated network manager
         internal_ = running_in_docker()
         if not internal_:
             self.log.warn(
                 "Algorithms have internet connection! "
                 "This happens because you use 'vnode-local'!"
             )
@@ -143,28 +149,28 @@
         # Setup VPN connection
         self.vpn_manager = self.setup_vpn_connection(
             isolated_network_mgr, self.ctx)
 
         # Create SSH tunnel according to the node configuration
         self.ssh_tunnels = self.setup_ssh_tunnels(isolated_network_mgr)
 
+        # Create Squid proxy server
+        self.squid = self.setup_squid_proxy(isolated_network_mgr)
+
         # setup the docker manager
         self.log.debug("Setting up the docker manager")
         self.__docker = DockerManager(
             ctx=self.ctx,
             isolated_network_mgr=isolated_network_mgr,
             vpn_manager=self.vpn_manager,
             tasks_dir=self.__tasks_dir,
             client=self.server_io,
+            proxy=self.squid
         )
 
-        # Create a long-lasting websocket connection.
-        self.log.debug("Creating websocket connection with the server")
-        self.connect_to_socket()
-
         # Connect the node to the isolated algorithm network *only* if we're
         # running in a docker container.
         if self.ctx.running_in_docker:
             isolated_network_mgr.connect(
                 container_name=self.ctx.docker_container_name,
                 aliases=[NODE_PROXY_SERVER_HOSTNAME]
             )
@@ -211,19 +217,26 @@
         proxy_port = int(os.environ.get("PROXY_SERVER_PORT", 8080))
 
         # 'app' is defined in vantage6.node.proxy_server
         # app.debug = True
         proxy_server.app.config["SERVER_IO"] = self.server_io
         proxy_server.server_url = self.server_io.base_path
 
+        # set up proxy server logging
+        log_level = getattr(logging, self.config["logging"]["level"].upper())
+        self.proxy_log = get_file_logger(
+            'proxy_server', self.ctx.proxy_log_file, log_level_file=log_level
+        )
+
         # this is where we try to find a port for the proxyserver
         for try_number in range(5):
             self.log.info(
                 f"Starting proxyserver at '{proxy_host}:{proxy_port}'")
-            http_server = WSGIServer(('0.0.0.0', proxy_port), proxy_server.app)
+            http_server = WSGIServer(('0.0.0.0', proxy_port), proxy_server.app,
+                                     log=self.proxy_log)
 
             try:
                 http_server.serve_forever()
 
             except OSError as e:
                 self.log.debug(f'Error during attempt {try_number}')
                 self.log.debug(f'{type(e)}: {e}')
@@ -242,64 +255,20 @@
                 self.log.error(e)
 
     def sync_task_queue_with_server(self) -> None:
         """ Get all unprocessed tasks from the server for this node."""
         assert self.server_io.cryptor, "Encrpytion has not been setup"
 
         # request open tasks from the server
-        task_results = self.server_io.get_results(state="open",
-                                                  include_task=True)
-        self.log.debug(task_results)
-
-        # add the tasks to the queue
-        self.__add_tasks_to_queue(task_results)
-        self.log.info(f"Received {self.queue._qsize()} tasks")
+        tasks = self.server_io.get_results(state="open", include_task=True)
+        self.log.debug(tasks)
+        for task in tasks:
+            self.queue.put(task)
 
-    def get_task_and_add_to_queue(self, task_id: int) -> None:
-        """
-        Fetches (open) task with task_id from the server. The `task_id` is
-        delivered by the websocket-connection.
-
-        Parameters
-        ----------
-        task_id : int
-            Task identifier
-        """
-        # fetch (open) result for the node with the task_id
-        task_results = self.server_io.get_results(
-            include_task=True,
-            state='open',
-            task_id=task_id
-        )
-
-        # add the tasks to the queue
-        self.__add_tasks_to_queue(task_results)
-
-    def __add_tasks_to_queue(self, task_results: list[dict]) -> None:
-        """
-        Add a task to the queue.
-
-        Parameters
-        ----------
-        taskresult : list[dict]
-            A list of dictionaries with information required to run the
-            algorithm
-        """
-        for task_result in task_results:
-            try:
-                if not self.__docker.is_running(task_result['id']):
-                    self.queue.put(task_result)
-                else:
-                    self.log.info(
-                        f"Not starting task {task_result['task']['id']} - "
-                        f"{task_result['task']['name']} as it is already "
-                        "running"
-                    )
-            except Exception:
-                self.log.exception("Error while syncing task queue")
+        self.log.info(f"received {self.queue._qsize()} tasks")
 
     def __start_task(self, taskresult: dict) -> None:
         """
         Start the docker image and notify the server that the task has been
         started.
 
         Parameters
@@ -346,30 +315,16 @@
         update = {'status': task_status}
         if task_status == TaskStatus.NOT_ALLOWED:
             # set finished_at to now, so that the task is not picked up again
             # (as the task is not started at all, unlike other crashes, it will
             # never finish and hence not be set to finished)
             update['finished_at'] = datetime.datetime.now().isoformat()
         self.server_io.patch_results(
-            id=taskresult['id'], result=update
+            id_=taskresult['id'], result=update
         )
-
-        # ensure that the /tasks namespace is connected. This may take a while
-        # (usually < 5s) when the socket just (re)connected
-        MAX_ATTEMPTS = 30
-        retries = 0
-        while '/tasks' not in self.socketIO.namespaces and \
-                retries < MAX_ATTEMPTS:
-            retries += 1
-            self.log.debug('Waiting for /tasks namespace to connect...')
-            time.sleep(1)
-        self.log.debug('Connected to /tasks namespace')
-        # in case the namespace is still not connected, the socket notification
-        # will not be sent to other nodes, but the task will still be processed
-
         # send socket event to alert everyone of task status change
         self.socketIO.emit(
             'algorithm_status_change',
             data={
                 'node_id': self.server_io.whoami.id_,
                 'status': task_status,
                 'result_id': taskresult['id'],
@@ -477,15 +432,15 @@
                 if not init_org_id:
                     self.log.error(
                         f"Initiator organization from task (id={task_id})could"
                         " not be retrieved!"
                     )
 
                 self.server_io.patch_results(
-                    id=results.result_id,
+                    id_=results.result_id,
                     result={
                         'result': results.data,
                         'log': results.logs,
                         'status': results.status,
                         'finished_at': datetime.datetime.now().isoformat(),
                     },
                     init_org_id=init_org_id,
@@ -628,16 +583,70 @@
             os.makedirs(self.__tasks_dir, exist_ok=True)
             self.__vpn_dir = ctx.data_dir / 'vpn'
             os.makedirs(self.__vpn_dir, exist_ok=True)
         else:
             self.__tasks_dir = ctx.data_dir
             self.__vpn_dir = ctx.vpn_dir
 
-    def setup_ssh_tunnels(self, isolated_network_mgr: Type[NetworkManager]) \
-            -> List[SSHTunnel]:
+    def setup_squid_proxy(self, isolated_network_mgr: NetworkManager) \
+            -> Squid:
+        """
+        Initiates a Squid proxy if configured in the config.yml
+
+        Expects the configuration in the following format:
+
+        ```yaml
+        whitelist:
+            domains:
+                - domain1
+                - domain2
+            ips:
+                - ip1
+                - ip2
+            ports:
+                - port1
+                - port2
+        ```
+
+        Parameters
+        ----------
+        isolated_network_mgr: NetworkManager
+            Network manager for isolated network
+
+        Returns
+        -------
+        Squid
+            Squid proxy instance
+        """
+        if 'whitelist' not in self.config:
+            self.log.info("No squid proxy configured")
+            return
+
+        custom_squid_image = self.config.get('images', {}).get('squid') \
+            if 'images' in self.config else None
+
+        self.log.info("Setting up squid proxy")
+        config = self.config['whitelist']
+
+        volume = self.ctx.docker_squid_volume_name if \
+            self.ctx.running_in_docker else self.ctx.data_dir
+
+        try:
+            squid = Squid(isolated_network_mgr, config, self.ctx.name, volume,
+                          custom_squid_image)
+        except Exception as e:
+            self.log.critical("Squid proxy failed to initialize. "
+                              "Continuing without.")
+            self.log.debug(e, exc_info=True)
+            squid = None
+
+        return squid
+
+    def setup_ssh_tunnels(self, isolated_network_mgr: NetworkManager) \
+            -> list[SSHTunnel]:
         """
         Create a SSH tunnels when they are defined in the configuration file.
         For each tunnel a new container is created. The image used can be
         specified in the configuration file as `ssh-tunnel` in the `images`
         section, else the default image is used.
 
         Parameters
@@ -651,15 +660,15 @@
 
         custom_tunnel_image = self.config.get('images', {}).get('ssh-tunnel') \
             if 'images' in self.config else None
 
         configs = self.config['ssh-tunnels']
         self.log.info(f"Setting up {len(configs)} SSH tunnels")
 
-        tunnels: List[SSHTunnel] = []
+        tunnels: list[SSHTunnel] = []
         for config in configs:
             self.log.debug(f"SSH tunnel config: {config}")
 
             # copy (rename) the ssh key to the correct name, this is done so
             # that the file is in the volume (somehow we can not file mount
             # within a volume)
             if self.ctx.running_in_docker:
@@ -687,24 +696,24 @@
                 continue
 
             tunnels.append(new_tunnel)
 
         return tunnels
 
     def setup_vpn_connection(self, isolated_network_mgr: NetworkManager,
-                             ctx: Union[DockerNodeContext, NodeContext]
+                             ctx: DockerNodeContext | NodeContext
                              ) -> VPNManager:
         """
         Setup container which has a VPN connection
 
         Parameters
         ----------
         isolated_network_mgr: NetworkManager
             Manager for the isolated Docker network
-        ctx: NodeContext
+        ctx: DockerNodeContext | NodeContext
             Context object for the node
 
         Returns
         -------
         VPNManager
             Manages the VPN connection
         """
@@ -866,35 +875,54 @@
         connection to notify the server that this node is online
         """
         # Wait for the socket to be connected to the namespaces on startup
         time.sleep(5)
 
         while True:
             try:
-                if self.socketIO.connected:
-                    self.socketIO.emit('ping', namespace='/tasks')
-                else:
-                    self.log.debug('SocketIO is not connected, skipping ping')
+                self.socketIO.emit('ping', namespace='/tasks')
             except Exception:
                 self.log.exception('Ping thread had an exception')
             # Wait before sending next ping
             time.sleep(PING_INTERVAL_SECONDS)
 
+    def get_task_and_add_to_queue(self, task_id: int) -> None:
+        """
+        Fetches (open) task with task_id from the server. The `task_id` is
+        delivered by the websocket-connection.
+
+        Parameters
+        ----------
+        task_id : int
+            Task identifier
+        """
+        # fetch (open) result for the node with the task_id
+        tasks = self.server_io.get_results(
+            include_task=True,
+            state='open',
+            task_id=task_id
+        )
+
+        # in the current setup, only a single result for a single node
+        # in a task exists.
+        for task in tasks:
+            self.queue.put(task)
+
     def run_forever(self) -> None:
         """Keep checking queue for incoming tasks (and execute them)."""
         kill_listener = ContainerKillListener()
         try:
             while True:
                 # blocking untill a task comes available
                 # timeout specified, else Keyboard interupts are ignored
                 self.log.info("Waiting for new tasks....")
 
                 while not kill_listener.kill_now:
                     try:
-                        taskresult = self.queue.get(timeout=1)
+                        task = self.queue.get(timeout=1)
                         # if no item is returned, the Empty exception is
                         # triggered, thus break statement is not reached
                         break
 
                     except queue.Empty:
                         pass
 
@@ -902,36 +930,36 @@
                         self.log.debug(e)
 
                 if kill_listener.kill_now:
                     raise InterruptedError
 
                 # if task comes available, attempt to execute it
                 try:
-                    self.__start_task(taskresult)
+                    self.__start_task(task)
                 except Exception as e:
                     self.log.exception(e)
 
         except (KeyboardInterrupt, InterruptedError):
             self.log.info("Vnode is interrupted, shutting down...")
             self.cleanup()
             sys.exit()
 
-    def kill_containers(self, kill_info: Dict) -> List[Dict]:
+    def kill_containers(self, kill_info: dict) -> list[dict]:
         """
         Kill containers on instruction from socket event
 
         Parameters
         ----------
-        kill_info: Dict
+        kill_info: dict
             Dictionary received over websocket with instructions for which
             tasks to kill
 
         Returns
         -------
-        List[Dict]:
+        list[dict]:
             List of dictionaries with information on killed task (keys:
             result_id, task_id and parent_id)
         """
         if kill_info['collaboration_id'] != self.server_io.collaboration_id:
             self.log.debug(
                 "Not killing tasks as this node is in another collaboration."
             )
@@ -947,15 +975,15 @@
         kill_list = kill_info.get('kill_list')
         killed_algos = self.__docker.kill_tasks(
             org_id=self.server_io.whoami.organization_id, kill_list=kill_list
         )
         # update status of killed tasks
         for killed_algo in killed_algos:
             self.server_io.patch_results(
-                id=killed_algo.result_id, result={'status': TaskStatus.KILLED}
+                id_=killed_algo.result_id, result={'status': TaskStatus.KILLED}
             )
         return killed_algos
 
     def share_node_details(self) -> None:
         """
         Share part of the node's configuration with the server.
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/_version.py` & `vantage6-node-3.9.0rc2/vantage6/node/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 8, 'candidate', __build__, 0)))
+version_info = (3, 9, 0, 'candidate', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = f'' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/cli/node.py` & `vantage6-node-3.9.0rc2/vantage6/node/cli/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,24 @@
     configuration_wizard,
     select_configuration_questionaire
 )
 from vantage6.node._version import __version__
 
 
 @click.group(name="vnode-local")
-def cli_node():
+def cli_node() -> None:
     """Command `vnode-local`."""
     pass
 
 
 #
 #   list
 #
 @cli_node.command(name="list")
-def cli_node_list():
+def cli_node_list() -> None:
     """Lists all nodes in the default configuration directories."""
 
     # FIXME: use package 'table' for this.
     click.echo("\nName"+(21*" ")+"Environments"+(21*" ")+"System/User")
     click.echo("-" * 70)
 
     configs, f1 = NodeContext.available_configurations(system_folders=True)
@@ -69,15 +69,16 @@
               default=None,
               help='Configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True,
               help="Use configuration from system folders (default)")
 @click.option('--user', 'system_folders', flag_value=False,
               default=constants.DEFAULT_NODE_SYSTEM_FOLDERS,
               help="Use configuration from user folders")
-def cli_node_new_configuration(name, environment, system_folders):
+def cli_node_new_configuration(name: str, environment: str,
+                               system_folders: bool) -> None:
     """Create a new configation file.
 
     Checks if the configuration already exists. If this is not the case
     a questionaire is invoked to create a new configuration file.
     """
     # select configuration name if none supplied
     if not name:
@@ -117,15 +118,15 @@
               default=constants.DEFAULT_NODE_ENVIRONMENT,
               help='Configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True,
               help="Use configuration from system folders (default)")
 @click.option('--user', 'system_folders', flag_value=False,
               default=constants.DEFAULT_NODE_SYSTEM_FOLDERS,
               help="Use configuration from user folders")
-def cli_node_files(name, environment, system_folders):
+def cli_node_files(name: str, environment: str, system_folders: bool) -> None:
     """Print out the paths of important files.
 
     If the specified configuration cannot be found, it exits. Otherwise
     it returns the absolute path to the output.
     """
     # select configuration name if none supplied
     name, environment = (name, environment) if name else \
@@ -162,15 +163,16 @@
               help="Use configuration from system folders (default)")
 @click.option('--user', 'system_folders', flag_value=False,
               default=constants.DEFAULT_NODE_SYSTEM_FOLDERS,
               help="Use configuration from user folders")
 @click.option('--dockerized/-non-dockerized', default=False,
               help=("Whether to use DockerNodeContext or regular NodeContext "
                     "(default)"))
-def cli_node_start(name, config, environment, system_folders, dockerized):
+def cli_node_start(name: str, config: str, environment: str,
+                   system_folders: bool, dockerized: bool) -> None:
     """Start the node instance.
 
     If no name or config is specified the default.yaml configuation is used.
     In case the configuration file not excists, a questionaire is
     invoked to create one. Note that in this case it is not possible to
     specify specific environments for the configuration (e.g. test,
     prod, acc).
@@ -212,10 +214,10 @@
     node.run(ctx)
 
 
 #
 #   version
 #
 @cli_node.command(name='version')
-def cli_node_version():
+def cli_node_version() -> None:
     """Returns current version of vantage6 services installed."""
     click.echo(__version__)
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/context.py` & `vantage6-node-3.9.0rc2/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/docker/docker_base.py` & `vantage6-node-3.9.0rc2/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/docker/docker_manager.py` & `vantage6-node-3.9.0rc2/vantage6/node/docker/docker_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import os
 import time
 import logging
 import docker
 import re
 import shutil
 
-from typing import Dict, List, NamedTuple, Union
+from typing import NamedTuple
 from pathlib import Path
 
+from vantage6.common import logger_name
 from vantage6.common import get_database_config
 from vantage6.common.docker.addons import get_container, running_in_docker
 from vantage6.common.globals import APPNAME
 from vantage6.common.task_status import TaskStatus, has_task_failed
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.cli.context import NodeContext
 from vantage6.node.context import DockerNodeContext
 from vantage6.node.docker.docker_base import DockerBaseManager
 from vantage6.node.docker.vpn_manager import VPNManager
 from vantage6.node.docker.task_manager import DockerTaskManager
-from vantage6.node.util import logger_name
+from vantage6.node.docker.squid import Squid
 from vantage6.node.server_io import NodeClient
 from vantage6.node.docker.exceptions import (
     UnknownAlgorithmStartFail,
     PermanentAlgorithmStartFail,
     AlgorithmContainerNotFound
 )
 
@@ -54,15 +55,15 @@
         Status code of the algorithm run
     """
     result_id: int
     task_id: int
     logs: str
     data: str
     status: str
-    parent_id: Union[int, None]
+    parent_id: int | None
 
 
 class ToBeKilled(NamedTuple):
     """ Data class to store which tasks should be killed """
     task_id: int
     result_id: int
     organization_id: int
@@ -82,49 +83,53 @@
     This classes manages tasks related to Docker, such as logging in to
     docker registries, managing input/output files, logs etc. Results
     can be retrieved through `get_result()` which returns the first available
     algorithm result.
     """
     log = logging.getLogger(logger_name(__name__))
 
-    def __init__(self, ctx: Union[DockerNodeContext, NodeContext],
-                 isolated_network_mgr: NetworkManager, vpn_manager: VPNManager,
-                 tasks_dir: Path, client: NodeClient) -> None:
+    def __init__(self, ctx: DockerNodeContext | NodeContext,
+                 isolated_network_mgr: NetworkManager,
+                 vpn_manager: VPNManager, tasks_dir: Path, client: NodeClient,
+                 proxy: Squid | None = None) -> None:
         """ Initialization of DockerManager creates docker connection and
             sets some default values.
 
             Parameters
             ----------
-            ctx: DockerNodeContext or NodeContext
+            ctx: DockerNodeContext | NodeContext
                 Context object from which some settings are obtained
             isolated_network_mgr: NetworkManager
                 Manager for the isolated network
             vpn_manager: VPNManager
                 VPN Manager object
             tasks_dir: Path
                 Directory in which this task's data are stored
             client: NodeClient
                 Client object to communicate with the server
+            proxy: Squid | None
+                Squid proxy object
         """
         self.log.debug("Initializing DockerManager")
         super().__init__(isolated_network_mgr)
 
         self.data_volume_name = ctx.docker_volume_name
         config = ctx.config
         self.algorithm_env = config.get('algorithm_env', {})
         self.vpn_manager = vpn_manager
         self.client = client
         self.__tasks_dir = tasks_dir
         self.alpine_image = config.get('alpine')
+        self.proxy = proxy
 
         # keep track of the running containers
-        self.active_tasks: List[DockerTaskManager] = []
+        self.active_tasks: list[DockerTaskManager] = []
 
         # keep track of the containers that have failed to start
-        self.failed_tasks: List[DockerTaskManager] = []
+        self.failed_tasks: list[DockerTaskManager] = []
 
         # before a task is executed it gets exposed to these regex
         # TODO remove in v4+ as it is supersed by the 'policies' block
         self._allowed_images = config.get("allowed_images")
         self._policies = config.get("policies", {})
 
         # node name is used to identify algorithm containers belonging
@@ -142,24 +147,31 @@
         docker_registries = ctx.config.get("docker_registries", [])
         self.login_to_registries(docker_registries)
 
         # set database uri and whether or not it is a file
         self._set_database(ctx.databases)
 
         # keep track of linked docker services
-        self.linked_services: List[str] = []
+        self.linked_services: list[str] = []
 
-    def _set_database(self, databases: Union[Dict, List]) -> None:
-        """"
+        # set algorithm device requests
+        self.algorithm_device_requests = []
+        if 'algorithm_device_requests' in config:
+            self._set_algorithm_device_requests(
+                config['algorithm_device_requests']
+            )
+
+    def _set_database(self, databases: dict | list) -> None:
+        """
         Set database location and whether or not it is a file
 
         Parameters
         ----------
-        config: Dict
-            Configuration of the app
+        databases: dict | list
+            databases as specified in the config file
         """
 
         # Check wether the new or old database config is used.
         # TODO: we should remove the old way in v4+
         old_format = isinstance(databases, dict)
 
         # Check that the `default` database label is present. If this is
@@ -179,32 +191,51 @@
         # the environment variables for us. This has the added bonus that we
         # can override the URI from the command line as well.
         self.databases = {}
         for label in db_labels:
             label_upper = label.upper()
             db_config = get_database_config(databases, label)
             if running_in_docker():
-                uri = os.environ[f'{label_upper}_DATABASE_URI']
+                uri_env = os.environ[f'{label_upper}_DATABASE_URI']
+                uri = f'/mnt/{uri_env}'
             else:
                 uri = db_config['uri']
 
-            db_is_file = Path(uri).exists()
-            if running_in_docker() and db_is_file:
-                uri = f'/mnt/{uri}'
+            db_type = db_config['type']
 
+            db_is_file = Path(uri).exists()
             if db_is_file:
                 # We'll copy the file to the folder `data` in our task_dir.
                 self.log.info(f'Copying {uri} to {self.__tasks_dir}')
                 shutil.copy(uri, self.__tasks_dir)
                 uri = self.__tasks_dir / os.path.basename(uri)
 
             self.databases[label] = {'uri': uri, 'is_file': db_is_file,
-                                     'type': db_config['type']}
+                                     'type': db_type}
         self.log.debug(f"Databases: {self.databases}")
 
+    def _set_algorithm_device_requests(self, device_requests_config: dict) \
+            -> None:
+        """
+        Configure device access for the algorithm container.
+
+        Parameters
+        ----------
+        device_requests_config: dict
+           A dictionary containing configuration options for device access.
+           Supported keys:
+           - 'gpu': A boolean value indicating whether GPU access is required.
+        """
+        device_requests = []
+        if device_requests_config.get('gpu', False):
+            device = docker.types.DeviceRequest(count=-1,
+                                                capabilities=[['gpu']])
+            device_requests.append(device)
+        self.algorithm_device_requests = device_requests
+
     def create_volume(self, volume_name: str) -> None:
         """
         Create a temporary volume for a single run.
 
         A single run can consist of multiple algorithm containers. It is
         important to note that all algorithm containers having the same run_id
         have access to this container.
@@ -256,15 +287,15 @@
             found = False
             for regex_expr in allowed_algorithms:
                 expr_ = re.compile(regex_expr)
                 if expr_.match(docker_image_name):
                     found = True
             if not found:
                 self.log.warn("A task was sent with a docker image that this"
-                               " node does not allow to run.")
+                              " node does not allow to run.")
                 return False
 
         # check if user or their organization is allowed
         allowed_users = self._policies.get('allowed_users', [])
         allowed_orgs = self._policies.get('allowed_organizations', [])
         if allowed_users or allowed_orgs:
             # TODO in v4+, simpify this logic when part below is removed (
@@ -316,21 +347,21 @@
                 f"{APPNAME}-type=algorithm",
                 f"node={self.node_name}",
                 f"result_id={result_id}"
             ]
         })
         return bool(running_containers)
 
-    def cleanup_tasks(self) -> List[KilledResult]:
+    def cleanup_tasks(self) -> list[KilledResult]:
         """
         Stop all active tasks
 
         Returns
         -------
-        List[KilledResult]:
+        list[KilledResult]:
             List of information on tasks that have been killed
         """
         result_ids_killed = []
         if self.active_tasks:
             self.log.debug(f'Killing {len(self.active_tasks)} active task(s)')
         while self.active_tasks:
             task = self.active_tasks.pop()
@@ -359,41 +390,41 @@
         # remove the node container from the network, it runs this code.. so
         # it does not make sense to delete it just yet
         self.isolated_network_mgr.disconnect(self.node_container_name)
 
         # remove the connected containers and the network
         self.isolated_network_mgr.delete(kill_containers=True)
 
-    def run(self, result_id: int, task_info: Dict, image: str,
+    def run(self, result_id: int, task_info: dict, image: str,
             docker_input: bytes, tmp_vol_name: str, token: str, database: str
-            ) -> Union[List[Dict], None]:
+            ) -> list[dict] | None:
         """
         Checks if docker task is running. If not, creates DockerTaskManager to
         run the task
 
         Parameters
         ----------
         result_id: int
             Server result identifier
-        task_info: Dict
+        task_info: dict
             Dictionary with task information
         image: str
             Docker image name
         docker_input: bytes
             Input that can be read by docker container
         tmp_vol_name: str
             Name of temporary docker volume assigned to the algorithm
         token: str
             Bearer token that the container can use
         database: str
             Name of the Database to use
 
         Returns
         -------
-        List[Dict] or None
+        list[dict] | None
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is not set up.
         """
         # Verify that an allowed image is used
         if not self.is_docker_image_allowed(image, task_info):
             msg = f"Docker image {image} is not allowed on this Node!"
             self.log.critical(msg)
@@ -411,15 +442,17 @@
             task_info=task_info,
             vpn_manager=self.vpn_manager,
             node_name=self.node_name,
             tasks_dir=self.__tasks_dir,
             isolated_network_mgr=self.isolated_network_mgr,
             databases=self.databases,
             docker_volume_name=self.data_volume_name,
-            alpine_image=self.alpine_image
+            alpine_image=self.alpine_image,
+            proxy=self.proxy,
+            device_requests=self.algorithm_device_requests
         )
         database = database if (database and len(database)) else 'default'
 
         # attempt to kick of the task. If it fails do to unknown reasons we try
         # again. If it fails permanently we add it to the failed tasks to be
         # handled by the speaking worker of the node
         attempts = 1
@@ -564,30 +597,30 @@
         self.isolated_network_mgr.connect(
             container_name=container_name,
             aliases=[config_alias]
         )
         self.linked_services.append(container_name)
 
     def kill_selected_tasks(
-        self, org_id: int, kill_list: List[ToBeKilled] = None
-    ) -> List[KilledResult]:
+        self, org_id: int, kill_list: list[ToBeKilled] = None
+    ) -> list[KilledResult]:
         """
         Kill tasks specified by a kill list, if they are currently running on
         this node
 
         Parameters
         ----------
         org_id: int
             The organization id of this node
-        kill_list: List[ToBeKilled]
+        kill_list: list[ToBeKilled]
             A list of info about tasks that should be killed.
 
         Returns
         -------
-        List[KilledResult]
+        list[KilledResult]
             List with information on killed tasks
         """
         killed_list = []
         for container_to_kill in kill_list:
             if container_to_kill['organization_id'] != org_id:
                 continue  # this result is on another node
             # find the task
@@ -609,29 +642,29 @@
                 self.log.warn(
                     "Received instruction to kill result_id="
                     f"{container_to_kill['result_id']}, but it was not "
                     "found running on this node.")
         return killed_list
 
     def kill_tasks(self, org_id: int,
-                   kill_list: List[ToBeKilled] = None) -> List[KilledResult]:
+                   kill_list: list[ToBeKilled] = None) -> list[KilledResult]:
         """
         Kill tasks currently running on this node.
 
         Parameters
         ----------
         org_id: int
             The organization id of this node
-        kill_list: List[ToBeKilled] (optional)
+        kill_list: list[ToBeKilled] (optional)
             A list of info on tasks that should be killed. If the list
             is not specified, all running algorithm containers will be killed.
 
         Returns
         -------
-        List[KilledResult]
+        list[KilledResult]
             List of dictionaries with information on killed tasks
         """
         if kill_list:
             killed_results = self.kill_selected_tasks(org_id=org_id,
                                                       kill_list=kill_list)
         else:
             # received instruction to kill all tasks on this node
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/docker/exceptions.py` & `vantage6-node-3.9.0rc2/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-3.9.0rc2/vantage6/node/docker/ssh_tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 private network of the node and an external data source. This can then be used
 by the algorithm containers to access the data source. Multiple SSH tunnels
 can be created, each with a different configuration.
 """
 import logging
 import os
 
-from typing import Union, NamedTuple, Tuple
+from typing import NamedTuple
 from jinja2 import Environment, FileSystemLoader
 from pathlib import Path
 
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
 from vantage6.common.docker.addons import (
     remove_container,
@@ -76,15 +76,15 @@
     fingerprint: str
 
 
 class SSHTunnel(DockerBaseManager):
 
     def __init__(self, isolated_network_mgr: NetworkManager, config: dict,
                  node_name: str, config_volume: str,
-                 tunnel_image: Union[str, None] = None) -> None:
+                 tunnel_image: str | None = None) -> None:
         """
         Create a tunnel from the isolated network to a remote machine and
         bind the remote port to a local ssh-tunnel container to be used by
         an algorithm.
 
         Parameters
         ----------
@@ -92,15 +92,15 @@
             Isolated network manager
         config : dict
             ssh tunnel configuration
         node_name : str
             Node name to derive the ssh tunnel container name
         config_volume : str
             Name of the ssh config volume (or local path)
-        tunnel_image : Union[str, None], optional
+        tunnel_image : str | None, optional
             User defined image to use for the tunnel, by default None
 
         Raises
         ------
         KeyError
             Missing key in the configuration
         """
@@ -141,16 +141,15 @@
         self.create_ssh_config_file(self.ssh_tunnel_config)
         self.create_known_hosts_file(self.known_hosts_config)
 
         self.start()
         log.info(f"SSH tunnel {self.hostname} started")
 
     @staticmethod
-    def read_config(config: dict) \
-            -> Tuple[SSHTunnelConfig, KnownHostsConfig]:
+    def read_config(config: dict) -> tuple[SSHTunnelConfig, KnownHostsConfig]:
         """
         Read the SSH configuration from the config
 
         Parameters
         ----------
         config: dict
             Dictionary containing the SSH configuration
@@ -274,15 +273,16 @@
         )
         self.container = self.docker.containers.run(
             image=self.image,
             volumes=mounts,
             detach=True,
             name=self.container_name,
             command=self.ssh_tunnel_config.hostname,
-            auto_remove=False
+            auto_remove=False,
+            restart_policy={"Name": "always"}
         )
 
         # Connect to both the internal network and make an alias (=hostname).
         # This alias can be used by the algorithm containers.
         self.isolated_network_mgr.connect(self.container,
                                           aliases=[self.hostname])
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/docker/task_manager.py` & `vantage6-node-3.9.0rc2/vantage6/node/docker/task_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 to be cleaned at some point. """
 import logging
 import os
 import pickle
 import docker.errors
 import json
 
-from typing import Dict, List, Union
 from pathlib import Path
 
+from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
 from vantage6.common.docker.addons import (
     remove_container_if_exists, remove_container, pull_if_newer,
     running_in_docker
 )
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.common.task_status import TaskStatus
-from vantage6.node.util import logger_name, get_parent_id
+from vantage6.node.util import get_parent_id
 from vantage6.node.globals import ALPINE_IMAGE
 from vantage6.node.docker.vpn_manager import VPNManager
+from vantage6.node.docker.squid import Squid
 from vantage6.node.docker.docker_base import DockerBaseManager
 from vantage6.node.docker.exceptions import (
     UnknownAlgorithmStartFail,
     PermanentAlgorithmStartFail,
     AlgorithmContainerNotFound
 )
 
@@ -32,81 +33,90 @@
     Manager for running a vantage6 algorithm container within docker.
 
     Ensures that the environment is properly set up (docker volumes,
     directories, environment variables, etc). Then runs the algorithm as a
     docker container. Finally, it monitors the container state and can return
     it's results when the algorithm finished.
     """
+    log = logging.getLogger(logger_name(__name__))
 
     def __init__(self, image: str, vpn_manager: VPNManager, node_name: str,
-                 result_id: int, task_info: Dict, tasks_dir: Path,
+                 result_id: int, task_info: dict, tasks_dir: Path,
                  isolated_network_mgr: NetworkManager,
                  databases: dict, docker_volume_name: str,
-                 alpine_image: Union[str, None] = None):
+                 alpine_image: str | None = None, proxy: Squid | None = None,
+                 device_requests: list | None = None):
         """
         Initialization creates DockerTaskManager instance
 
         Parameters
         ----------
         image: str
             Name of docker image to be run
         vpn_manager: VPNManager
             VPN manager required to set up traffic forwarding via VPN
         node_name: str
             Name of the node, to track running algorithms
         result_id: int
             Server result identifier
-        task_info: Dict
+        task_info: dict
             Dictionary with info about the task
         tasks_dir: Path
             Directory in which this task's data are stored
         isolated_network_mgr: NetworkManager
             Manager of isolated network to which algorithm needs to connect
-        databases: Dict
+        databases: dict
             List of databases
         docker_volume_name: str
             Name of the docker volume
-        alpine_image: str or None
+        alpine_image: str | None
             Name of alternative Alpine image to be used
+        device_requests: list | None
+            List of DeviceRequest objects to be passed to the algorithm
+            container
         """
-        self.task_id = task_info['id']
-        self.log = logging.getLogger(f"task ({self.task_id})")
-
         super().__init__(isolated_network_mgr)
         self.image = image
         self.__vpn_manager = vpn_manager
         self.result_id = result_id
+        self.task_id = task_info['id']
         self.parent_id = get_parent_id(task_info)
         self.__tasks_dir = tasks_dir
         self.databases = databases
         self.data_volume_name = docker_volume_name
         self.node_name = node_name
         self.alpine_image = ALPINE_IMAGE if alpine_image is None \
             else alpine_image
+        self.proxy = proxy
 
         self.container = None
         self.status_code = None
         self.docker_input = None
 
         self.labels = {
             f"{APPNAME}-type": "algorithm",
             "node": node_name,
             "result_id": str(result_id)
         }
-        self.helper_labels = self.labels.copy()
+        self.helper_labels = self.labels
         self.helper_labels[f"{APPNAME}-type"] = "algorithm-helper"
 
         # FIXME: these values should be retrieved from DockerNodeContext
         #   in some way.
         self.tmp_folder = "/mnt/tmp"
         self.data_folder = "/mnt/data"
 
         # keep track of the task status
         self.status: TaskStatus = TaskStatus.INITIALIZING
 
+        # set device requests
+        self.device_requests = []
+        if device_requests:
+            self.device_requests = device_requests
+
     def is_finished(self) -> bool:
         """
         Checks if algorithm container is finished
 
         Returns
         -------
         bool:
@@ -173,35 +183,35 @@
         except Exception as e:
             self.log.debug('Failed to pull image')
             self.log.exception(e)
             self.status = TaskStatus.FAILED
             raise PermanentAlgorithmStartFail
 
     def run(self, docker_input: bytes, tmp_vol_name: str, token: str,
-            algorithm_env: Dict, database: str) -> List[Dict]:
+            algorithm_env: dict, database: str) -> list[dict]:
         """
         Runs the docker-image in detached mode.
 
         It will will attach all mounts (input, output and datafile) to the
         docker image. And will supply some environment variables.
 
         Parameters
         ----------
         docker_input: bytes
             Input that can be read by docker container
         tmp_vol_name: str
             Name of temporary docker volume assigned to the algorithm
         token: str
             Bearer token that the container can use
-        algorithm_env: Dict
+        algorithm_env: dict
             Dictionary with additional environment variables to set
 
         Returns
         -------
-        List[Dict] or None
+        list[dict] | None
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is not set up.
         """
         # generate task folders
         self._make_task_folders()
 
         # prepare volumes
@@ -219,69 +229,65 @@
         return vpn_ports
 
     def cleanup(self) -> None:
         """Cleanup the containers generated for this task"""
         remove_container(self.helper_container, kill=True)
         remove_container(self.container, kill=True)
 
-    def _run_algorithm(self) -> List[Dict]:
+    def _run_algorithm(self) -> list[dict]:
         """
         Run the algorithm container
 
         Start up a helper container to complete VPN setup, pull the latest
         image and then run the algorithm
 
         Returns
         -------
-        List[Dict] or None
+        list[dict] or None
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is inactive
         """
         vpn_ports = None
         container_name = f'{APPNAME}-{self.node_name}-result-{self.result_id}'
         helper_container_name = container_name + '-helper'
 
         # Try to pull the latest image
         self.pull()
 
         # remove algorithm containers if they were already running
-        self.log.debug("Check if algorithm container is already running")
         remove_container_if_exists(
             docker_client=self.docker, name=container_name
         )
         remove_container_if_exists(
             docker_client=self.docker, name=helper_container_name
         )
 
         if self.__vpn_manager:
             # if VPN is active, network exceptions must be configured
             # First, start a container that runs indefinitely. The algorithm
             # container will run in the same network and network exceptions
             # will therefore also affect the algorithm.
-            self.log.debug("Start helper container to setup VPN network")
             self.helper_container = self.docker.containers.run(
                 command='sleep infinity',
                 image=self.alpine_image,
                 labels=self.helper_labels,
                 network=self.isolated_network_mgr.network_name,
                 name=helper_container_name,
                 detach=True
             )
             # setup forwarding of traffic via VPN client to and from the
             # algorithm container:
-            self.log.debug("Setup port forwarder")
             vpn_ports = self.__vpn_manager.forward_vpn_traffic(
                 helper_container=self.helper_container,
                 algo_image_name=self.image
             )
 
         # try reading docker input
         deserialized_input = None
         if self.docker_input:
-            self.log.debug("Deserialize input")
             try:
                 deserialized_input = pickle.loads(self.docker_input)
             except Exception:
                 pass
 
         # attempt to run the image
         try:
@@ -293,39 +299,42 @@
             self.container = self.docker.containers.run(
                 self.image,
                 detach=True,
                 environment=self.environment_variables,
                 network='container:' + self.helper_container.id,
                 volumes=self.volumes,
                 name=container_name,
-                labels=self.labels
+                labels=self.labels,
+                device_requests=self.device_requests
             )
 
         except Exception as e:
             self.status = TaskStatus.START_FAILED
             raise UnknownAlgorithmStartFail(e)
 
         self.status = TaskStatus.ACTIVE
         return vpn_ports
 
     @staticmethod
-    def _printable_input(input_: str) -> str:
+    def _printable_input(input_: str | dict) -> str:
         """
         Return a version of the input with limited number of characters
 
         Parameters
         ----------
-        input: str
-            Input of a task
+        input: str | dict
+            Deserialized input of a task
 
         Returns
         -------
         str
             Input with limited number of characters, to be printed to logs
         """
+        if isinstance(input_, dict):
+            input_ = str(input_)
         if len(input_) > 550:
             return f'{input_[:500]}... ({len(input_)-500} characters omitted)'
         return input_
 
     def _make_task_folders(self) -> None:
         """ Generate task folders """
         # FIXME: We should have a separate mount/volume for this. At the
@@ -343,28 +352,28 @@
         # we can just copy the required files to it
         self.task_folder_name = f"task-{self.result_id:09d}"
         self.task_folder_path = \
             os.path.join(self.__tasks_dir, self.task_folder_name)
         os.makedirs(self.task_folder_path, exist_ok=True)
         self.output_file = os.path.join(self.task_folder_path, "output")
 
-    def _prepare_volumes(self, tmp_vol_name: str, token: str) -> Dict:
+    def _prepare_volumes(self, tmp_vol_name: str, token: str) -> dict:
         """
         Generate docker volumes required to run the algorithm
 
         Parameters
         ----------
         tmp_vol_name: str
             Name of temporary docker volume assigned to the algorithm
         token: str
             Bearer token that the container can use
 
         Returns
         -------
-        Dict:
+        dict:
             Volumes to support running the algorithm
         """
         if isinstance(self.docker_input, str):
             self.docker_input = self.docker_input.encode('utf8')
 
         # Create I/O files & token for the algorithm container
         self.log.debug("prepare IO files in docker volume")
@@ -388,39 +397,41 @@
             volumes[self.data_volume_name] = \
                 {"bind": self.data_folder, "mode": "rw"}
         else:
             volumes[self.__tasks_dir] = \
                 {"bind": self.data_folder, "mode": "rw"}
         return volumes
 
-    def _setup_environment_vars(self, algorithm_env: Dict = {},
-                                database: str = 'default') -> Dict:
+    def _setup_environment_vars(self, algorithm_env: dict,
+                                database: str = 'default') -> dict:
         """"
         Set environment variables required to run the algorithm
 
         Parameters
         ----------
-        algorithm_env: Dict
+        algorithm_env: dict
             Dictionary with additional environment variables to set
+        database: str
+            Label of the database to use
 
         Returns
         -------
-        Dict:
+        dict:
             Environment variables required to run algorithm
         """
         try:
             proxy_host = os.environ['PROXY_SERVER_HOST']
 
         except Exception:
             self.log.warn("PROXY_SERVER_HOST not set, using "
                           "host.docker.internal")
             self.log.debug(os.environ)
             proxy_host = 'host.docker.internal'
 
-        # define enviroment variables for the docker-container, the
+        # define environment variables for the docker-container, the
         # host, port and api_path are from the local proxy server to
         # facilitate indirect communication with the central server
         # FIXME: we should only prepend data_folder if database_uri is a
         #   filename
         environment_variables = {
             "INPUT_FILE": f"{self.data_folder}/{self.task_folder_name}/input",
             "OUTPUT_FILE":
@@ -428,23 +439,48 @@
             "TOKEN_FILE": f"{self.data_folder}/{self.task_folder_name}/token",
             "TEMPORARY_FOLDER": self.tmp_folder,
             "HOST": f"http://{proxy_host}",
             "PORT": os.environ.get("PROXY_SERVER_PORT", 8080),
             "API_PATH": "",
         }
 
+        # Add squid proxy environment variables
+        if self.proxy:
+            # applications/libraries in the algorithm container need to adhere
+            # to the proxy settings. Because we are not sure which application
+            # is used for the request we both set HTTP_PROXY and http_proxy and
+            # HTTPS_PROXY and https_proxy for the secure connection.
+            environment_variables["HTTP_PROXY"] = self.proxy.address
+            environment_variables["http_proxy"] = self.proxy.address
+            environment_variables["HTTPS_PROXY"] = self.proxy.address
+            environment_variables["https_proxy"] = self.proxy.address
+
+            no_proxy = []
+            if self.__vpn_manager:
+                # Computing all ips in the vpn network is not feasible as the
+                # no_proxy environment variable will be too long for the
+                # container to start. So we only add the net + mask. For some
+                # applications and libraries this is format is ignored.
+                no_proxy.append(self.__vpn_manager.subnet)
+            no_proxy.append("localhost")
+            no_proxy.append(proxy_host)
+
+            # Add the NO_PROXY and no_proxy environment variable.
+            environment_variables["NO_PROXY"] = ', '.join(no_proxy)
+            environment_variables["no_proxy"] = ', '.join(no_proxy)
+
         if database in self.databases:
             environment_variables["USER_REQUESTED_DATABASE_LABEL"] = database
         else:
             # In this case the algorithm might crash if it tries to access
             # the DATABASE_LABEL environment variable
             self.log.warning("A user specified a database that does not "
                              "exist. Available databases are: "
-                             f"{', '.join(list(self.databases.keys()))}. This "
-                             "is likely to result in an algorithm crash.")
+                             f"{self.databases.keys()}. This is likely to "
+                             "result in an algorithm crash.")
             self.log.debug(f"User specified database: {database}")
 
         # Only prepend the data_folder is it is a file-based database
         # This allows algorithms to access multiple data sources at the
         # same time
         db_labels = []
         for label in self.databases:
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/docker/vpn_manager.py` & `vantage6-node-3.9.0rc2/vantage6/node/docker/vpn_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import docker
 import logging
 import json
 import time
 import ipaddress
 
 from json.decoder import JSONDecodeError
-from typing import List, Union, Dict
 from docker.models.containers import Container
 
+from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME, VPN_CONFIG_FILE
 from vantage6.common.docker.addons import (
     remove_container_if_exists, remove_container, pull_if_newer
 )
-from vantage6.node.util import logger_name
 from vantage6.node.globals import (
     MAX_CHECK_VPN_ATTEMPTS, NETWORK_CONFIG_IMAGE, VPN_CLIENT_IMAGE,
     FREE_PORT_RANGE, DEFAULT_ALGO_VPN_PORT, ALPINE_IMAGE
 )
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.node.docker.docker_base import DockerBaseManager
 
@@ -26,32 +25,36 @@
     Setup a VPN client in a Docker container and configure the network so that
     the VPN container can forward traffic to and from algorithm containers.
     """
     log = logging.getLogger(logger_name(__name__))
 
     def __init__(self, isolated_network_mgr: NetworkManager,
                  node_name: str, vpn_volume_name: str, vpn_subnet: str,
-                 alpine_image: Union[str, None] = None,
-                 vpn_client_image: Union[str, None] = None,
-                 network_config_image: Union[str, None] = None) -> None:
+                 alpine_image: str | None = None,
+                 vpn_client_image: str | None = None,
+                 network_config_image: str | None = None) -> None:
         """
         Initializes a VPN manager instance
 
         Parameters
         ----------
         isolated_network_mgr: NetworkManager
             An object that manages the node's isolated network
         node_name: str
             The name of the node (from config)
         vpn_volume_name: str
             The name of the volume in which the VPN data resides
         vpn_subnet: str
             The IP mask of the VPN subnet
-        alpine_image: str or None
+        alpine_image: str | None
             Name of alternative Alpine image to be used
+        vpn_client_image: str | None
+            Name of alternative VPN client image to be used
+        network_config_image: str | None
+            Name of alternative network config image to be used
         """
         super().__init__(isolated_network_mgr)
 
         self.vpn_client_container_name = f'{APPNAME}-{node_name}-vpn-client'
         self.vpn_volume_name = vpn_volume_name
         self.subnet = vpn_subnet
         self.alpine_image = ALPINE_IMAGE if not alpine_image \
@@ -152,15 +155,22 @@
         if not self.isolated_bridge:
             self.log.error("Setting up VPN failed: could not find bridge "
                            "interface of isolated network")
             return
         self._configure_host_network()
 
     def has_connection(self) -> bool:
-        """ Return True if VPN connection is active """
+        """
+        Return True if VPN connection is active
+
+        Returns
+        -------
+        bool
+            True if VPN connection is active, False otherwise
+        """
         self.log.debug("Waiting for VPN connection. This may take a minute...")
         n_attempt = 0
         self.has_vpn = False
         while n_attempt < MAX_CHECK_VPN_ATTEMPTS:
             n_attempt += 1
             try:
                 _, vpn_interface = self.vpn_client_container.exec_run(
@@ -217,45 +227,41 @@
 
         Returns
         -------
         str
             IP address assigned to VPN client container by VPN server
         """
         try:
-            # use has_connection() to check if VPN is active. This function
-            # also waits for a connection to be established, which is helpful
-            # for unstable connections
-            if self.has_connection():
-                _, vpn_interface = self.vpn_client_container.exec_run(
-                    'ip --json addr show dev tun0'
-                )
-                vpn_interface = json.loads(vpn_interface)
+            _, vpn_interface = self.vpn_client_container.exec_run(
+                'ip --json addr show dev tun0'
+            )
+            vpn_interface = json.loads(vpn_interface)
         except (JSONDecodeError, docker.errors.APIError):
             # JSONDecodeError if VPN is not setup yet, APIError if VPN
             # container is restarting (e.g. due to connection errors)
             raise ConnectionError(
                 "Could not get VPN IP: VPN is not connected!")
         return vpn_interface[0]['addr_info'][0]['local']
 
     def forward_vpn_traffic(self, helper_container: Container,
-                            algo_image_name: str) -> List[Dict]:
+                            algo_image_name: str) -> list[dict] | None:
         """
         Setup rules so that traffic is properly forwarded between the VPN
         container and the algorithm container (and its helper container)
 
         Parameters
         ----------
         algo_helper_container: Container
             Helper algorithm container
         algo_image_name: str
             Name of algorithm image that is run
 
         Returns
         -------
-        List[Dict] or None
+        list[dict] | None
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is not set up.
         """
         ports = self._forward_traffic_to_algorithm(
             helper_container, algo_image_name)
         self._forward_traffic_from_algorithm(helper_container)
         return ports
@@ -288,30 +294,31 @@
             image=self.alpine_image,
             network=network,
             cap_add='NET_ADMIN',
             command=cmd,
             remove=True
         )
 
-    def _forward_traffic_to_algorithm(self, algo_helper_container: Container,
-                                      algo_image_name: str) -> List[Dict]:
+    def _forward_traffic_to_algorithm(
+        self, algo_helper_container: Container, algo_image_name: str
+    ) -> list[dict] | None:
         """
         Forward incoming traffic from the VPN client container to the
         algorithm container
 
         Parameters
         ----------
         algo_helper_container: Container
             Helper algorithm container
         algo_image_name: str
             Name of algorithm image that is run
 
         Returns
         -------
-        List[Dict] or None
+        list[dict] | None
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is not set up.
         """
         if not self.has_vpn:
             return None  # no port assigned if no VPN is available
 
         # Get IP Address of the algorithm container
@@ -375,28 +382,28 @@
             Whether the VPN IP address is part of the subnet or not
         """
         vpn_ip = self.get_vpn_ip()
         return (
             ipaddress.ip_address(vpn_ip) in ipaddress.ip_network(self.subnet)
         )
 
-    def _find_exposed_ports(self, image: str) -> List[Dict]:
+    def _find_exposed_ports(self, image: str) -> list[dict]:
         """
         Find which ports were exposed via the EXPOSE keyword in the dockerfile
         of the algorithm image. This port will be used for VPN traffic. If no
         port is specified, the default port is used
 
         Parameters
         ----------
         image: str
             Algorithm image name
 
         Returns
         -------
-        List[Dict]:
+        list[dict]:
             List of ports forward VPN traffic to. For each port, a dictionary
             containing port number and label is given
         """
         default_ports = [{'algo_port': DEFAULT_ALGO_VPN_PORT, 'label': None}]
         algo_image = self.docker.images.get(image)
 
         exposed_ports = []
@@ -440,15 +447,15 @@
     def _find_isolated_bridge(self) -> str:
         """
         Retrieve the linked network interface in the host namespace for
         network interface eth0 in the container namespace.
 
         Returns
         -------
-        string
+        str
             The name of the network interface in the host namespace
         """
         # Get the isolated network interface and extract its link index
         isolated_interface = self._get_isolated_interface()
         if isolated_interface:
             link_index = self._get_link_index(isolated_interface)
         else:
@@ -459,15 +466,16 @@
             image=self.network_config_image,
             network='host',
             command=['ip', '--json', 'addr'],
             remove=True
         )
         host_interfaces = json.loads(host_interfaces)
 
-        linked_interface = self._get_if(host_interfaces, link_index)
+        linked_interface = \
+            self._get_interface_from_idx(host_interfaces, link_index)
         bridge_interface = linked_interface['master']
         return bridge_interface
 
     def _get_isolated_interface(self):
         """
         Get the isolated network interface
 
@@ -481,31 +489,32 @@
         vpn_ip_isolated_netw = self.get_isolated_netw_ip(
             self.vpn_client_container)
         for ip_interface in interfaces:
             if self.is_isolated_interface(ip_interface, vpn_ip_isolated_netw):
                 isolated_interface = ip_interface
         return isolated_interface
 
-    def is_isolated_interface(self, ip_interface: Dict,
-                              vpn_ip_isolated_netw: str):
+    @staticmethod
+    def is_isolated_interface(ip_interface: dict,
+                              vpn_ip_isolated_netw: str) -> bool:
         """
         Return True if a network interface is the isolated network
         interface. Identify this based on the IP address of the VPN client in
         the isolated network
 
         Parameters
         ----------
         ip_interface: dict
             IP interface obtained by executing `ip --json addr` command
         vpn_ip_isolated_netw: str
             IP address of VPN container in isolated network
 
         Returns
         -------
-        boolean:
+        bool
             True if this is the interface describing the isolated network
         """
         # check if attributes exist in json: if not then it is not the right
         # interface
         if ('addr_info' in ip_interface and len(ip_interface['addr_info']) and
                 'local' in ip_interface['addr_info'][0]):
             # Right attributes are present: check if IP addresses match
@@ -536,30 +545,70 @@
             image=self.network_config_image,
             network='host',
             cap_add='NET_ADMIN',
             command=command,
             remove=True,
         )
 
-    def _get_if(self, interfaces, index) -> Union[Dict, None]:
-        """ Get interface configuration based on interface index """
+    @staticmethod
+    def _get_interface_from_idx(interfaces: list[dict],
+                                index: int) -> dict | None:
+        """
+        Get interface configuration based on interface index
+
+        Parameters
+        ----------
+        interfaces: list
+            List of interfaces as returned by `ip --json addr`
+        index: int
+            Interface index
+
+        Returns
+        -------
+        dict | None
+            Interface configuration or None if not found
+        """
         for interface in interfaces:
             if int(interface['ifindex']) == index:
                 return interface
 
         return None
 
-    def _get_link_index(self, if_json: Union[Dict, List]) -> int:
+    @staticmethod
+    def _get_link_index(if_json: dict | list) -> int:
+        """
+        Get the link index of an interface
+
+        Parameters
+        ----------
+        if_json: dict | list
+            Interface configuration as returned by `ip --json addr`
+
+        Returns
+        -------
+        int
+            Link index of the interface
+        """
         if isinstance(if_json, list):
             if_json = if_json[-1]
         return int(if_json['link_index'])
 
     def _is_ipv4_subnet(self, subnet: str) -> bool:
         """
         Validate if subnet has format '12.34.56.78/16'
+
+        Parameters
+        ----------
+        subnet: str
+            Subnet to validate
+
+        Returns
+        -------
+        bool
+            True if subnet is valid
         """
         parts = subnet.split('/')
         if len(parts) != 2:
             return False
         if not parts[1].isdigit() or int(parts[1]) > 32:
             return False
         octets = parts[0].split(".")
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/globals.py` & `vantage6-node-3.9.0rc2/vantage6/node/globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,9 +41,14 @@
 DEFAULT_ALGO_VPN_PORT = '8888'  # default VPN port for algorithm container
 
 #
 #   SSH TUNNEL RELATED CONSTANTS
 #
 SSH_TUNNEL_IMAGE = "harbor2.vantage6.ai/infrastructure/ssh-tunnel"
 
+#
+#   SQUID RELATED CONSTANTS
+#
+SQUID_IMAGE = "harbor2.vantage6.ai/infrastructure/squid"
+
 # start trying to refresh the JWT token 10 minutes before it expires.
 REFRESH_BEFORE_EXPIRES_SECONDS = 600
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/proxy_server.py` & `vantage6-node-3.9.0rc2/vantage6/node/proxy_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 """
 This module contains a proxy server implementation that the node uses to
 communicate with the server. It contains general methods for any routes, and
 methods to handle tasks and results, including their encryption and decryption.
+
+(!) Not to be confused with the squid proxy that allows algorithm containers
+to access other places in the network.
 """
 import requests
 import logging
 
 from http import HTTPStatus
 from requests import Response
-from typing import Callable, Union
 
 from flask import Flask, request, jsonify
 
+from vantage6.common import bytes_to_base64s, base64s_to_bytes, logger_name
 from vantage6.node.server_io import NodeClient
-from vantage6.node.util import (
-    logger_name,
-    base64s_to_bytes,
-    bytes_to_base64s
-)
 
 # Initialize FLASK
 app = Flask(__name__)
 log = logging.getLogger(logger_name(__name__))
 
 # Need to be set when the proxy server is initialized
 app.config["SERVER_IO"] = None
 server_url = None
 
 # Number of times the request is retried before the proxy server gives up
 RETRY = 3
 
 
-def get_method(method: str) -> Callable:
+def get_method(method: str) -> callable:
     """
     Obtain http method based on string identifier
 
     Parameters
     ----------
     method : str
         Http method requested
@@ -166,26 +164,26 @@
         log.exception("Unable to decrypt and/or decode results, sending them "
                       "to the algorithm...")
 
     return result
 
 
 def get_response_json_and_handle_exceptions(
-        response: Response) -> Union[dict, None]:
+        response: Response) -> dict | None:
     """
     Obtain json content from request response
 
     Parameters
     ----------
     response : requests.Response
         Requests response object
 
     Returns
     -------
-    dict or None
+    dict | None
         Dict containing the json body
     """
     try:
         return response.json()
     except (requests.exceptions.JSONDecodeError, Exception):
         log.exception('Failed to extract JSON')
     return None
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/server_io.py` & `vantage6-node-3.9.0rc2/vantage6/node/server_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module provides a client interface for the node to communicate with the
 central server.
 """
 import jwt
 import datetime
 import time
 
-from typing import Dict, Tuple
 from threading import Thread
 
 from vantage6.common import WhoAmI
 from vantage6.client import ClientBase
 from vantage6.node.globals import REFRESH_BEFORE_EXPIRES_SECONDS
 
 
@@ -20,23 +19,26 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # self.name = None
         self.collaboration_id = None
         self.whoami = None
 
-    def authenticate(self, api_key: str):
-        """ Nodes authentication at the central server.
+    def authenticate(self, api_key: str) -> None:
+        """
+        Nodes authentication at the central server.
 
-            It also identifies itself by retrieving the collaboration
-            and organization to which this node belongs. The server
-            returns a JWT-token that is used in all succeeding requests.
+        It also identifies itself by retrieving the collaboration
+        and organization to which this node belongs. The server
+        returns a JWT-token that is used in all succeeding requests.
 
-            :param api_key: api-key used to authenticate to the central
-                server
+        Parameters
+        ----------
+        api_key : str
+            The api key of the node.
         """
         super().authenticate({"api_key": api_key}, path="token/node")
 
         # obtain the server authenticatable id
         jwt_payload = jwt.decode(self.token,
                                  options={"verify_signature": False})
 
@@ -84,88 +86,122 @@
                 time.sleep(
                     int(time_until_expiry - REFRESH_BEFORE_EXPIRES_SECONDS + 1)
                 )
 
     def request_token_for_container(self, task_id: int, image: str):
         """ Request a container-token at the central server.
 
-            This token is used by algorithm containers that run on this
-            node. These algorithms can then post tasks and retrieve
-            child-results (usually refered to as a master container).
-            The server performs a few checks (e.g. if the task you
-            request the key for is still open) before handing out this
-            token.
-
-            :param task_id: id from the task, which is going to use this
-                container-token (a task results in a algorithm-
-                container at the node)
-            :param image: image-name of the task
+        This token is used by algorithm containers that run on this
+        node. These algorithms can then post tasks and retrieve
+        child-results (usually refered to as a master container).
+        The server performs a few checks (e.g. if the task you
+        request the key for is still open) before handing out this
+        token.
+
+        Parameters
+        ----------
+        task_id : int
+            id from the task, which is going to use this container token
+        image : str
+            Docker image name of the task
+
+        Returns
+        -------
+        dict
+            The container token.
         """
         self.log.debug(
             f"requesting container token for task_id={task_id} "
             f"and image={image}"
         )
         return self.request('/token/container', method="post", json={
             "task_id": task_id,
             "image": image
         })
 
-    def get_results(self, id=None, state=None, include_task=False,
-                    task_id=None):
-        """ Obtain the results for a specific task.
+    def get_results(
+        self, id_: int = None, state: str = None, include_task: bool = False,
+        task_id: int = None
+    ) -> dict:
+        """
+        Obtain the results for a specific task.
+
+        Overload the definition of the parent by entering the
+        task_id automatically.
 
-            Overload the definition of the parent by entering the
-            task_id automatically.
+        Parameters
+        ----------
+        id_ : int, optional
+            ID of the result, by default None
+        state : str, optional
+            State of the result, by default None
+        include_task : bool, optional
+            Include the task in the result, by default False
+        task_id : int, optional
+            ID of the task, by default None
+
+        Returns
+        -------
+        dict
+            The results.
         """
         return super().get_results(
-            id_=id,
+            id=id_,
             state=state,
             include_task=include_task,
             task_id=task_id,
             node_id=self.whoami.id_
         )
 
-    def is_encrypted_collaboration(self):
-        """ Boolean whenever the encryption is enabled.
+    def is_encrypted_collaboration(self) -> bool:
+        """
+        Check whether the encryption is enabled.
+
+        End-to-end encryption is per collaboration managed at the
+        central server. It is important to note that the local
+        configuration-file should allow explicitly for unencrpyted
+        messages. This function returns the setting from the server.
 
-            End-to-end encryption is per collaboration managed at the
-            central server. It is important to note that the local
-            configuration-file should allow explicitly for unencrpyted
-            messages. This function returns the setting from the server.
+        Returns
+        -------
+        bool
+            True if the collaboration is encrypted, False otherwise.
         """
         response = self.request(f"collaboration/{self.collaboration_id}")
         return response.get("encrypted") == 1
 
-    def set_task_start_time(self, id: int):
-        """ Sets the start time of the task at the central server.
-
-            This is important as this will note that the task has been
-            started, and is waiting for restuls.
+    def set_task_start_time(self, id_: int) -> None:
+        """
+        Sets the start time of the task at the central server.
 
-            :param id: id of the task to set the start-time of
+        This is important as this will note that the task has been
+        started, and is waiting for restuls.
 
-            TODO the initiator_id does not make sens here...
+        Parameters
+        ----------
+        id_ : int
+            ID of the task.
         """
-        self.patch_results(id, result={
+        self.patch_results(id_, result={
             "started_at": datetime.datetime.now().isoformat()
         })
 
-    def patch_results(self, id: int, result: Dict,
+    def patch_results(self, id_: int, result: dict,
                       init_org_id: int = None) -> None:
         """
         Update the results at the central server.
 
         Typically used when to algorithm container is finished or
         when a status-update is posted (started, finished)
 
         Parameters
         ----------
         id: int
             ID of the result to patch
-        result: Dict
+        result: dict
             Dictionary of fields that are to be patched
         init_org_id: int, optional
             Organization id of the origin of the task. This is required
             when the result dict includes results, because then results have
             to be encrypted specifically for them
         """
         # TODO: the key `result` is not always present, e.g. when
@@ -193,17 +229,17 @@
                 public_key
             )
 
             self.log.debug("Sending results to server")
         else:
             self.log.debug("Just patchin'")
 
-        return self.request(f"result/{id}", json=result, method='patch')
+        return self.request(f"result/{id_}", json=result, method='patch')
 
-    def get_vpn_config(self) -> Tuple[bool, str]:
+    def get_vpn_config(self) -> tuple[bool, str]:
         """
         Obtain VPN configuration from the server
 
         Returns
         -------
         bool
             Whether or not obtaining VPN config was successful
@@ -226,14 +262,19 @@
         """
         Refresh the client's keypair in an ovpn configuration file
 
         Parameters
         ----------
         ovpn_file: str
             The path to the current ovpn configuration on disk
+
+        Returns
+        -------
+        bool
+            Whether or not the refresh was successful
         """
         # Extract the contents of the VPN file
         with open(ovpn_file, 'r') as file:
             ovpn_config = file.read()
 
         response = self.request(
             "vpn/update",
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/socket.py` & `vantage6-node-3.9.0rc2/vantage6/node/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import logging
 
 from socketio import ClientNamespace
-from typing import Dict
 
+from vantage6.common import logger_name
 from vantage6.common.task_status import TaskStatus, has_task_failed
-from vantage6.node.util import logger_name
-
 
 
 class NodeTaskNamespace(ClientNamespace):
     """Class that handles incoming websocket events."""
 
     # reference to the node objects, so a callback can edit the
     # node instance.
@@ -98,20 +96,20 @@
         self.node_worker_ref.server_io.refresh_token()
         self.log.debug("Token refreshed")
         self.node_worker_ref.connect_to_socket()
         self.log.debug("Connected to socket")
         self.node_worker_ref.sync_task_queue_with_server()
         self.log.debug("Tasks synced again with the server...")
 
-    def on_kill_containers(self, kill_info: Dict):
+    def on_kill_containers(self, kill_info: dict):
         """
         Action to be taken when nodes are instructed by server to kill one or
         more tasks
 
-        kill_info: Dict
+        kill_info: dict
             A dictionary that contains information on which tasks should be
             killed. This information may instruct a node to kill all its tasks
             or include a list of which tasks should be killed.
         """
         self.log.info(f"Received instruction to kill task: {kill_info}")
         killed_ids = self.node_worker_ref.kill_containers(kill_info)
         for killed in killed_ids:
```

### Comparing `vantage6-node-3.8.8rc3/vantage6/node/util/colorer.py` & `vantage6-node-3.9.0rc2/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.8rc3/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-3.9.0rc2/vantage6_node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.8rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc2 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.8.8rc3/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-3.9.0rc2/vantage6_node.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 vantage6/node/server_io.py
 vantage6/node/socket.py
 vantage6/node/cli/__init__.py
 vantage6/node/cli/node.py
 vantage6/node/docker/docker_base.py
 vantage6/node/docker/docker_manager.py
 vantage6/node/docker/exceptions.py
+vantage6/node/docker/squid.py
 vantage6/node/docker/ssh_tunnel.py
 vantage6/node/docker/task_manager.py
 vantage6/node/docker/vpn_manager.py
 vantage6/node/util/__init__.py
 vantage6/node/util/colorer.py
 vantage6_node.egg-info/PKG-INFO
 vantage6_node.egg-info/SOURCES.txt
```

