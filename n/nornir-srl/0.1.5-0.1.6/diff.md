# Comparing `tmp/nornir_srl-0.1.5.tar.gz` & `tmp/nornir_srl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_srl-0.1.5.tar", max compression
+gzip compressed data, was "nornir_srl-0.1.6.tar", max compression
```

## Comparing `nornir_srl-0.1.5.tar` & `nornir_srl-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7447 2023-05-17 13:47:26.925426 nornir_srl-0.1.5/README.md
--rw-r--r--   0        0        0       22 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/connections/__init__.py
--rw-r--r--   0        0        0     3904 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/connections/helpers.py
--rw-r--r--   0        0        0    25396 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/connections/srlinux.py
--rw-r--r--   0        0        0    14699 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/fsc.py
--rw-r--r--   0        0        0        0 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/tasks/__init__.py
--rw-r--r--   0        0        0      374 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/tasks/helpers.py
--rw-r--r--   0        0        0     9178 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/nornir_srl/tasks/srl_config.py
--rw-r--r--   0        0        0      860 2023-05-17 13:47:26.929426 nornir_srl-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     8508 1970-01-01 00:00:00.000000 nornir_srl-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7948 2023-05-23 13:26:00.224039 nornir_srl-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/connections/__init__.py
+-rw-r--r--   0        0        0     3904 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/connections/helpers.py
+-rw-r--r--   0        0        0    25396 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/connections/srlinux.py
+-rw-r--r--   0        0        0    15049 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/fsc.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/tasks/__init__.py
+-rw-r--r--   0        0        0      374 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/tasks/helpers.py
+-rw-r--r--   0        0        0     9178 2023-05-23 13:26:00.252039 nornir_srl-0.1.6/nornir_srl/tasks/srl_config.py
+-rw-r--r--   0        0        0      889 2023-05-23 13:26:00.256039 nornir_srl-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9009 1970-01-01 00:00:00.000000 nornir_srl-0.1.6/PKG-INFO
```

### Comparing `nornir_srl-0.1.5/README.md` & `nornir_srl-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,91 @@
+
+![Demo](https://github.com/wdesmedt/nornir_srl/blob/main/imgs/fcli_demo.gif)
 # nornir-srl
+
 This module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations and the [PyGNMI](https://github.com/akarneliuk/pygnmi) Python module to interact with gNMI. 
 
 Rather than limiting the connection plugin to primitives like `open_connection`, `close_connection`, `get`, `set`, etc, this module provides also methods to get information from the device for common resources. Since the device model tends to change between releases, it was considered a better approach to provide this functionality as part of the connection plugin and hide complexity of model changes to the user or Nornir tasks. 
 
 In addition to the connection plugin, there is a set of Nornir tasks that use the connection plugin to perform common operations on the device, like get BGP peers, get MAC table, get subinterfaces, etc. These Nornir tasks are called by a command-line interface `fcli` that provides a network-wide CLI to perform show commands across an entire set or subset for SRLinux nodes.
 
 The current functionality is focused on a read-only _network-wide CLI_ to perform show commands across an entire set or subset for SRLinux nodes, as defined in the Nornir inventory and through command-line filter options. It shows output in a tabular format for easy reading.
 Following versions may focus on configuration management and command execution on the nodes.
 
-# Prerequisites
+# Installation
 
-This module requires [Nornir Core](https://github.com/nornir-automation/nornir) that includes the Nornir core components for which this module is an add-on.
-Nornir needs a [configuration file](https://nornir.readthedocs.io/en/latest/configuration/index.html) to tell it at a minimum where to find the inventory and what inventory plugin is used. Also runner configuration parameters, like #threads/workers for parallel execution are defined here but sane defaults are used.
+## Docker-based installation
 
-Since this module is using gNMI as the management inteface, at a minimum, a CA certificate is required that was used to create per-device certs and keys. If you use [Containerlab](https://containerlab.dev/) this root cert is auto-generated for SRLinux nodes and available in the lab subfolder created by the containerlab cli. This file needs to be referenced via the inventory (per-device or per-group). See below for details.
+This is the easiest way to get started. It requires [Docker](https://docs.docker.com/get-docker/) and optionally  [Containerlab](https://containerlab.dev/) to be installed on your system.
 
-# Installation
+> NOTE: if you have issues connecting to the docker network of containerlab, make sure proper `iptables` rules are in place to permit incomming traffic on the docker network interface. For example, on Ubuntu 20.04, you can use the following command:
+
+```
+iptables -I DOCKER-USER -o docker0 -j ACCEPT -m comment --comment "allow inter-network comms"
+```
+
+To run fcli, create an alias in your shell profile, for example, assuming that you have a `clab_topo.yml` file in your current directory and lab is up and running:
+
+```
+CLAB_TOPO=clab_topo.yml alias fcli="docker run -t --rm -v /etc/hosts:/etc/hosts:ro -v ${PWD}/${CLAB_TOPO}:/topo.yml wdesmedt/srl-fcli -t /topo.yml"
+```
+To run a report, specify the report name as the first argument to the alias, for example:
+```
+fcli sys-info # for system information like NOS version, uptime, etc
+
+fcli bgp-peers # for BGP peers
+```
+
+## Python-based installation with `pip`
 
 Create a Python virtual-env using your favorite workflow, For example:
 ```
 mkdir nornir-srl && cd nornir-srl
 python3 -m venv .venv
 source .venv/bin/activate
 ```
 Following command will install the the `nornir_srl` module and all its dependencies, including Nornir core.
 
 ```
 pip install wheel
 pip install -U nornir-srl
 ```
+
+
+# Use
+
+Currently, only the network-wide report functionality is supported via the `fcli` command
+```
+$ fcli --help
+Usage: fcli [OPTIONS] REPORT
+
+Options:
+  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]
+  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf
+  -f, --field-filter TEXT    filter fields with <field-name>=<glob-pattern>,
+                             e.g. -f state=up -f admin_state="ena*"
+  -b, --box-type TEXT        box type of printed table, e.g. -b
+                             minimal_double_head. 'python -m rich.box' for
+                             options
+  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn
+                             -o route_type=2 for 'bgp-rib report
+  -t, --topo-file TEXT       CLAB topology file, e.g. -t topo.yaml
+  --cert-file TEXT           CLAB certificate file, e.g. -c ca-root.pem
+  --help                     Show this message and exit.
+  ```
+  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:
+```
+$ fcli test
+Report test not found. Available reports: ['bgp-peers', 'subinterface', 'ipv4-rib', 'mac-table', 'sys-info', 'nwi-itfs', 'lldp-nbrs']
+```
+
+## Nornir-based inventory mode
+
+In this mode, a Nornir configuration file must be provided with the `-c` option. The Nornir inventory is polulated by the `InventoryPlugin` and associated options as specified in the config file. See below for an example with the included `YAMLInventory` plugin and the associated inventory files.
+
 Create the Nornir confguration file, for example:
 
 ```yaml
 # nornir_config.yaml
 inventory:
     #    plugin: SimpleInventory
     plugin: YAMLInventory
@@ -41,15 +94,17 @@
         group_file: "./inventory/groups.yaml"
         defaults_file: "./inventory/defaults.yaml"
 runner:
     plugin: threaded
     options:
         num_workers: 20
 ```
+
 Create the inventory files as referenced in the above configuration file, for example:
+
 ```yaml
 ## hosts.yaml
 clab-4l2s-l1:
     hostname: clab-4l2s-l1
     groups: [srl, fabric, leafs]
 clab-4l2s-l2:
     hostname: clab-4l2s-l2
@@ -81,47 +136,25 @@
     groups: [ global ]
     data:
         role: leaf
         type: ixr-d2
 ```
 The root certificate is specified once for all devices in group `srl` via the `connection_options.srlinux.extras.path_cert` parameter.
 
-# Use
-
-Currently, only the network-wide cli functionality is supported via the `fcli` command
-```
-$ fcli --help
-Usage: fcli [OPTIONS] REPORT
+This mode is used for real hardware-based fabric.
 
-Options:
-  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]
-  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf
-  -f, --field-filter TEXT    filter fields, e.g. -f state=up -f
-                             admin_state=enable
-  -b, --box-type TEXT        box type of printed table, e.g. -b
-                             minimal_double_head. 'python -m rich.box' for
-                             options
-  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn
-                             -o route_type=2 for 'bgp-rib report
-  --help                     Show this message and exit.
-  ```
-  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:
-```
-$ fcli test
-Report test not found. Available reports: ['bgp-peers', 'subinterface', 'ipv4-rib', 'mac-table', 'sys-info', 'nwi-itfs', 'lldp-nbrs']
-```
+## CLAB-based inventory mode
 
-## Nornir-based inventory mode
+In this mode, the Nornir inventory is populated by a containerlab topology file and no further configuration files are needed. The containerlab topo file is specified with the `-t` option. 
 
-In this mode, a Nornir configuration file must be provided with the `-c` option. The Nornir inventory is polulated by the `InventoryPlugin` and associated options as specified in the config file. See above for an example with the included `YAMLInventory` plugin and the associated inventory files.
+`fcli` converts the topology file to a _hosts_ and _groups_ file and only nodes of kind=srl are populated in the host inventory. Furthermore, the `prefix` parameter in the topo file is considered to generate the hostnames. The presence of _labels_ in the topo file is mapped into node-specific attribs that can be used in inventory filters (`-i` option).
 
-This mode is used for real hardware-based fabric.
-## CLAB-based inventory mode
+## Filtering
 
-In this mode, the Nornir inventory is populated by a containerlab topology file and no further configuration files are needed. The containerlab topo file is specified with the `-t` option. `fcli` converts the topology file to a _hosts_ and _groups_ file. Only nodes of kind=srl are populated in the host inventory. Furthermore, the `prefix` parameter in the topo file is considered to generate the hostnames. Also, the presence of _labels_ in the topo file is mapped into node-specific attribs that can be used in inventory filters (`-i` option).
+## Filtering
 
 Optionally, you can specify filters to control the output. There are 2 types of filters:
 
 - inventory filters, specified with the `-i` option, filter on the inventory, e.g. `-i hostname=clab-4l2s-l1`  or `-i role=leaf` based on inventory data
 - field filters, specified with the `-f` option. This filters based on the fields shown in the report and a glob pattern, e.g. `-f state="esta*"`. Multiple field filters can be specified by repeated `-f` options
 - report-specific options are options specific to a report, if applicable. Currently, the only report that needs extra arguments is 'bgp-rib', i.e. `route_fam=evpn|ipv4|ipv6` and `route_type=1|2|3|4|5`. The latter relates to EVPN route-trypes and is optional. Defaults to '2' (mac-ip-routes).
```

### Comparing `nornir_srl-0.1.5/nornir_srl/connections/helpers.py` & `nornir_srl-0.1.6/nornir_srl/connections/helpers.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.1.5/nornir_srl/connections/srlinux.py` & `nornir_srl-0.1.6/nornir_srl/connections/srlinux.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.1.5/nornir_srl/fsc.py` & `nornir_srl-0.1.6/nornir_srl/fsc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List, Optional, Callable
 import importlib
 import fnmatch
 import sys
 import tempfile
+import pkg_resources
 
 from ruamel.yaml import YAML
 
 from nornir import InitNornir
 
 from nornir.core.task import Result, Task, AggregatedResult
 from nornir.core.inventory import Host
@@ -22,14 +23,16 @@
 from nornir_utils.plugins.functions import print_result
 from nornir_srl.tasks.srl_config import configure_device, restore_config
 
 from nornir_srl.connections.srlinux import CONNECTION_NAME
 
 import click
 
+PYTHON_PKG_NAME = "nornir_srl"
+
 SRL_DEFAULT_USERNAME = "admin"
 SRL_DEFAULT_PASSWORD = "NokiaSrl1!"
 SRL_DEFAULT_GNMI_PORT = 57400
 
 NORNIR_DEFAULT_CONFIG: Dict[str, Any] = {
     "inventory": {
         "plugin": "YAMLInventory",
@@ -47,14 +50,23 @@
     },
     "user_defined": {
         "intent_dir": "intent",
     },
 }
 
 
+def get_project_version():
+    try:
+        version = pkg_resources.get_distribution(PYTHON_PKG_NAME).version
+    except pkg_resources.DistributionNotFound:
+        version = "Version not found"
+
+    return version
+
+
 def sys_info(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     return Result(host=task.host, result=device.get_info())
 
 
 def get_itfs(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
@@ -126,14 +138,15 @@
         "routed": "[cyan]",
         "bridged": "[blue]",
         "established": "[ok]",
         "active": "[cyan]",
     }
 
     console = Console(theme=table_theme)
+    console._emoji = False
     if kwargs.get("box_type") and kwargs["box_type"] != None:
         box_type = str(kwargs["box_type"]).upper()
         try:
             box_t = getattr(importlib.import_module("rich.box"), box_type)
         except AttributeError:
             print(
                 f"Unknown box type {box_type}. Check 'python -m rich.box' for valid box types."
@@ -301,14 +314,15 @@
     help="CLAB topology file, e.g. -t topo.yaml",
 )
 @click.option(
     "--cert-file",
     multiple=False,
     help="CLAB certificate file, e.g. -c ca-root.pem",
 )
+@click.version_option(version=get_project_version())
 def cli(
     report: str,
     cfg: str,
     inv_filter: Optional[List] = None,
     field_filter: Optional[List] = None,
     report_options: Optional[List] = None,
     box_type: Optional[str] = None,
```

### Comparing `nornir_srl-0.1.5/nornir_srl/tasks/srl_config.py` & `nornir_srl-0.1.6/nornir_srl/tasks/srl_config.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.1.5/pyproject.toml` & `nornir_srl-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "nornir_srl"
-version = "0.1.5"
+version = "0.1.6"
 description = "Nornir connection plugin for SRLinux"
 authors = ["Walter De Smedt <walter.de.smedt@gmail.com>"]
 readme = "README.md"
-repository = "https://github.com/wdesmedt/nornir_srl"
+repository = "https://github.com/srl-labs/nornir-srl"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nornir = "^3.3.0"
 nornir-utils = "^0.2.0"
 pygnmi = "^0.8.9"
 nornir-jinja2 = "^0.2.0"
@@ -24,14 +24,15 @@
 "srlinux" = "nornir_srl.connections.srlinux:SrLinux"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 blessings = "^1.7"
 black = "^23.3.0"
 mypy = "^0.991"
+types-setuptools = "^67.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fcli = 'nornir_srl.fsc:cli'
```

### Comparing `nornir_srl-0.1.5/PKG-INFO` & `nornir_srl-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nornir-srl
-Version: 0.1.5
+Version: 0.1.6
 Summary: Nornir connection plugin for SRLinux
-Home-page: https://github.com/wdesmedt/nornir_srl
+Home-page: https://github.com/srl-labs/nornir-srl
 Author: Walter De Smedt
 Author-email: walter.de.smedt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,48 +18,101 @@
 Requires-Dist: natsort (>=8.2.0,<9.0.0)
 Requires-Dist: nornir (>=3.3.0,<4.0.0)
 Requires-Dist: nornir-jinja2 (>=0.2.0,<0.3.0)
 Requires-Dist: nornir-scrapli (>=2022.1.30,<2023.0.0)
 Requires-Dist: nornir-utils (>=0.2.0,<0.3.0)
 Requires-Dist: pygnmi (>=0.8.9,<0.9.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
-Project-URL: Repository, https://github.com/wdesmedt/nornir_srl
+Project-URL: Repository, https://github.com/srl-labs/nornir-srl
 Description-Content-Type: text/markdown
 
+
+![Demo](https://github.com/wdesmedt/nornir_srl/blob/main/imgs/fcli_demo.gif)
 # nornir-srl
+
 This module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations and the [PyGNMI](https://github.com/akarneliuk/pygnmi) Python module to interact with gNMI. 
 
 Rather than limiting the connection plugin to primitives like `open_connection`, `close_connection`, `get`, `set`, etc, this module provides also methods to get information from the device for common resources. Since the device model tends to change between releases, it was considered a better approach to provide this functionality as part of the connection plugin and hide complexity of model changes to the user or Nornir tasks. 
 
 In addition to the connection plugin, there is a set of Nornir tasks that use the connection plugin to perform common operations on the device, like get BGP peers, get MAC table, get subinterfaces, etc. These Nornir tasks are called by a command-line interface `fcli` that provides a network-wide CLI to perform show commands across an entire set or subset for SRLinux nodes.
 
 The current functionality is focused on a read-only _network-wide CLI_ to perform show commands across an entire set or subset for SRLinux nodes, as defined in the Nornir inventory and through command-line filter options. It shows output in a tabular format for easy reading.
 Following versions may focus on configuration management and command execution on the nodes.
 
-# Prerequisites
+# Installation
 
-This module requires [Nornir Core](https://github.com/nornir-automation/nornir) that includes the Nornir core components for which this module is an add-on.
-Nornir needs a [configuration file](https://nornir.readthedocs.io/en/latest/configuration/index.html) to tell it at a minimum where to find the inventory and what inventory plugin is used. Also runner configuration parameters, like #threads/workers for parallel execution are defined here but sane defaults are used.
+## Docker-based installation
 
-Since this module is using gNMI as the management inteface, at a minimum, a CA certificate is required that was used to create per-device certs and keys. If you use [Containerlab](https://containerlab.dev/) this root cert is auto-generated for SRLinux nodes and available in the lab subfolder created by the containerlab cli. This file needs to be referenced via the inventory (per-device or per-group). See below for details.
+This is the easiest way to get started. It requires [Docker](https://docs.docker.com/get-docker/) and optionally  [Containerlab](https://containerlab.dev/) to be installed on your system.
 
-# Installation
+> NOTE: if you have issues connecting to the docker network of containerlab, make sure proper `iptables` rules are in place to permit incomming traffic on the docker network interface. For example, on Ubuntu 20.04, you can use the following command:
+
+```
+iptables -I DOCKER-USER -o docker0 -j ACCEPT -m comment --comment "allow inter-network comms"
+```
+
+To run fcli, create an alias in your shell profile, for example, assuming that you have a `clab_topo.yml` file in your current directory and lab is up and running:
+
+```
+CLAB_TOPO=clab_topo.yml alias fcli="docker run -t --rm -v /etc/hosts:/etc/hosts:ro -v ${PWD}/${CLAB_TOPO}:/topo.yml wdesmedt/srl-fcli -t /topo.yml"
+```
+To run a report, specify the report name as the first argument to the alias, for example:
+```
+fcli sys-info # for system information like NOS version, uptime, etc
+
+fcli bgp-peers # for BGP peers
+```
+
+## Python-based installation with `pip`
 
 Create a Python virtual-env using your favorite workflow, For example:
 ```
 mkdir nornir-srl && cd nornir-srl
 python3 -m venv .venv
 source .venv/bin/activate
 ```
 Following command will install the the `nornir_srl` module and all its dependencies, including Nornir core.
 
 ```
 pip install wheel
 pip install -U nornir-srl
 ```
+
+
+# Use
+
+Currently, only the network-wide report functionality is supported via the `fcli` command
+```
+$ fcli --help
+Usage: fcli [OPTIONS] REPORT
+
+Options:
+  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]
+  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf
+  -f, --field-filter TEXT    filter fields with <field-name>=<glob-pattern>,
+                             e.g. -f state=up -f admin_state="ena*"
+  -b, --box-type TEXT        box type of printed table, e.g. -b
+                             minimal_double_head. 'python -m rich.box' for
+                             options
+  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn
+                             -o route_type=2 for 'bgp-rib report
+  -t, --topo-file TEXT       CLAB topology file, e.g. -t topo.yaml
+  --cert-file TEXT           CLAB certificate file, e.g. -c ca-root.pem
+  --help                     Show this message and exit.
+  ```
+  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:
+```
+$ fcli test
+Report test not found. Available reports: ['bgp-peers', 'subinterface', 'ipv4-rib', 'mac-table', 'sys-info', 'nwi-itfs', 'lldp-nbrs']
+```
+
+## Nornir-based inventory mode
+
+In this mode, a Nornir configuration file must be provided with the `-c` option. The Nornir inventory is polulated by the `InventoryPlugin` and associated options as specified in the config file. See below for an example with the included `YAMLInventory` plugin and the associated inventory files.
+
 Create the Nornir confguration file, for example:
 
 ```yaml
 # nornir_config.yaml
 inventory:
     #    plugin: SimpleInventory
     plugin: YAMLInventory
@@ -68,15 +121,17 @@
         group_file: "./inventory/groups.yaml"
         defaults_file: "./inventory/defaults.yaml"
 runner:
     plugin: threaded
     options:
         num_workers: 20
 ```
+
 Create the inventory files as referenced in the above configuration file, for example:
+
 ```yaml
 ## hosts.yaml
 clab-4l2s-l1:
     hostname: clab-4l2s-l1
     groups: [srl, fabric, leafs]
 clab-4l2s-l2:
     hostname: clab-4l2s-l2
@@ -108,47 +163,25 @@
     groups: [ global ]
     data:
         role: leaf
         type: ixr-d2
 ```
 The root certificate is specified once for all devices in group `srl` via the `connection_options.srlinux.extras.path_cert` parameter.
 
-# Use
-
-Currently, only the network-wide cli functionality is supported via the `fcli` command
-```
-$ fcli --help
-Usage: fcli [OPTIONS] REPORT
+This mode is used for real hardware-based fabric.
 
-Options:
-  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]
-  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf
-  -f, --field-filter TEXT    filter fields, e.g. -f state=up -f
-                             admin_state=enable
-  -b, --box-type TEXT        box type of printed table, e.g. -b
-                             minimal_double_head. 'python -m rich.box' for
-                             options
-  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn
-                             -o route_type=2 for 'bgp-rib report
-  --help                     Show this message and exit.
-  ```
-  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:
-```
-$ fcli test
-Report test not found. Available reports: ['bgp-peers', 'subinterface', 'ipv4-rib', 'mac-table', 'sys-info', 'nwi-itfs', 'lldp-nbrs']
-```
+## CLAB-based inventory mode
 
-## Nornir-based inventory mode
+In this mode, the Nornir inventory is populated by a containerlab topology file and no further configuration files are needed. The containerlab topo file is specified with the `-t` option. 
 
-In this mode, a Nornir configuration file must be provided with the `-c` option. The Nornir inventory is polulated by the `InventoryPlugin` and associated options as specified in the config file. See above for an example with the included `YAMLInventory` plugin and the associated inventory files.
+`fcli` converts the topology file to a _hosts_ and _groups_ file and only nodes of kind=srl are populated in the host inventory. Furthermore, the `prefix` parameter in the topo file is considered to generate the hostnames. The presence of _labels_ in the topo file is mapped into node-specific attribs that can be used in inventory filters (`-i` option).
 
-This mode is used for real hardware-based fabric.
-## CLAB-based inventory mode
+## Filtering
 
-In this mode, the Nornir inventory is populated by a containerlab topology file and no further configuration files are needed. The containerlab topo file is specified with the `-t` option. `fcli` converts the topology file to a _hosts_ and _groups_ file. Only nodes of kind=srl are populated in the host inventory. Furthermore, the `prefix` parameter in the topo file is considered to generate the hostnames. Also, the presence of _labels_ in the topo file is mapped into node-specific attribs that can be used in inventory filters (`-i` option).
+## Filtering
 
 Optionally, you can specify filters to control the output. There are 2 types of filters:
 
 - inventory filters, specified with the `-i` option, filter on the inventory, e.g. `-i hostname=clab-4l2s-l1`  or `-i role=leaf` based on inventory data
 - field filters, specified with the `-f` option. This filters based on the fields shown in the report and a glob pattern, e.g. `-f state="esta*"`. Multiple field filters can be specified by repeated `-f` options
 - report-specific options are options specific to a report, if applicable. Currently, the only report that needs extra arguments is 'bgp-rib', i.e. `route_fam=evpn|ipv4|ipv6` and `route_type=1|2|3|4|5`. The latter relates to EVPN route-trypes and is optional. Defaults to '2' (mac-ip-routes).
```

