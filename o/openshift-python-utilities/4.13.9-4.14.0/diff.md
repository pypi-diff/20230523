# Comparing `tmp/openshift-python-utilities-4.13.9.tar.gz` & `tmp/openshift-python-utilities-4.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-python-utilities-4.13.9.tar", last modified: Thu May  4 10:33:39 2023, max compression
+gzip compressed data, was "openshift-python-utilities-4.14.0.tar", last modified: Tue May 23 07:14:02 2023, max compression
```

## Comparing `openshift-python-utilities-4.13.9.tar` & `openshift-python-utilities-4.14.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1455 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 10:33:37.000000 openshift-python-utilities-4.13.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/ocp_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/debugger.py
--rw-r--r--   0 root         (0) root         (0)      452 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/infra.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/must_gather.py
--rw-r--r--   0 root         (0) root         (0)     6768 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/operators.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1455 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1494 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:14:02.929366 openshift-python-utilities-4.14.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-05-23 07:14:02.929366 openshift-python-utilities-4.14.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-23 07:14:01.000000 openshift-python-utilities-4.14.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:14:02.929366 openshift-python-utilities-4.14.0/ocp_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/debugger.py
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13883 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/infra.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/must_gather.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/operators.py
+-rw-r--r--   0 root         (0) root         (0)     3104 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/ocp_utilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:14:02.929366 openshift-python-utilities-4.14.0/openshift_python_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-05-23 07:14:02.000000 openshift-python-utilities-4.14.0/openshift_python_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-23 07:14:02.000000 openshift-python-utilities-4.14.0/openshift_python_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 07:14:02.000000 openshift-python-utilities-4.14.0/openshift_python_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-23 07:14:02.000000 openshift-python-utilities-4.14.0/openshift_python_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-23 07:14:02.000000 openshift-python-utilities-4.14.0/openshift_python_utilities.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-05-23 07:13:59.000000 openshift-python-utilities-4.14.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 07:14:02.929366 openshift-python-utilities-4.14.0/setup.cfg
```

### Comparing `openshift-python-utilities-4.13.9/LICENSE` & `openshift-python-utilities-4.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.13.9/PKG-INFO` & `openshift-python-utilities-4.14.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.13.9
+Version: 4.14.0
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.13.9/README.md` & `openshift-python-utilities-4.14.0/README.md`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.13.9/ocp_utilities/debugger.py` & `openshift-python-utilities-4.14.0/ocp_utilities/debugger.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.13.9/ocp_utilities/infra.py` & `openshift-python-utilities-4.14.0/ocp_utilities/infra.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+import base64
 import importlib
 import json
+import os
+import shlex
 
 import kubernetes
+from ocp_resources.image_content_source_policy import ImageContentSourcePolicy
 from ocp_resources.node import Node
+from ocp_resources.resource import ResourceEditor
+from ocp_resources.secret import Secret
 from ocp_wrapper_data_collector.data_collector import (
     get_data_collector_base_dir,
     get_data_collector_dict,
 )
 from simple_logger.logger import get_logger
 from urllib3.exceptions import MaxRetryError
 
 from ocp_utilities.exceptions import (
     NodeNotReadyError,
     NodesNotHealthyConditionError,
     NodeUnschedulableError,
     PodsFailedOrPendingError,
 )
+from ocp_utilities.utils import run_command
 
 
 LOGGER = get_logger(name=__name__)
 
 
 def get_client(config_file=None, config_dict=None, context=None, **kwargs):
     """
@@ -284,7 +291,128 @@
             client=unprivileged_client,
             body=fedora_vm_body(name=name),
         ) as vm:
             running_vm(vm=vm)
     """
     creator = DynamicClassCreator()
     return creator(base_class=base_class)
+
+
+def create_icsp_command(
+    image, source_url, folder_name, pull_secret=None, filter_options=""
+):
+    """
+        Create ImageContentSourcePolicy command.
+
+    Args:
+        image (str): name of image to be mirrored.
+        source_url (str): source url of image registry to which contents mirror.
+        folder_name (str): local path to store manifests.
+        pull_secret (str): Path to your registry credentials, default set to None(until passed)
+        filter_options (str): when filter passed it will choose image from multiple variants.
+
+    Returns:
+        str: base command to create icsp in the cluster.
+    """
+    base_command = (
+        f"oc adm catalog mirror {image} {source_url} --manifests-only "
+        f"--to-manifests {folder_name} {filter_options}"
+    )
+    if pull_secret:
+        base_command = f"{base_command} --registry-config={pull_secret}"
+    return base_command
+
+
+def generate_icsp_file(
+    folder_name, image, source_url, pull_secret=None, filter_options=""
+):
+    base_command = create_icsp_command(
+        image=image,
+        source_url=source_url,
+        folder_name=folder_name,
+        pull_secret=pull_secret,
+        filter_options=filter_options,
+    )
+    assert run_command(
+        command=shlex.split(base_command),
+        verify_stderr=False,
+    )[0]
+
+    icsp_file_path = os.path.join(folder_name, "ImageContentSourcePolicy.yaml")
+    assert os.path.isfile(
+        icsp_file_path
+    ), f"ICSP file does not exist in path {icsp_file_path}"
+
+    return icsp_file_path
+
+
+def create_icsp_from_file(icsp_file_path):
+    icsp = ImageContentSourcePolicy(yaml_file=icsp_file_path)
+    icsp.deploy()
+    return icsp
+
+
+def create_icsp(icsp_name, repository_digest_mirrors):
+    icsp = ImageContentSourcePolicy(
+        name=icsp_name, repository_digest_mirrors=repository_digest_mirrors
+    )
+    icsp.deploy()
+    return icsp
+
+
+def dict_base64_encode(_dict):
+    """
+    Encoding dict in base64
+
+    Args:
+        _dict (dict): data dict to be encoded
+
+    Returns:
+        str: given _dict encoded in base64
+    """
+    return base64.b64encode(json.dumps(_dict).encode("ascii")).decode("utf-8")
+
+
+def create_update_secret(secret_data_dict, name, namespace):
+    """
+    Update existing secret or create a new secret; secret type - dockerconfigjson
+
+    Args:
+        secret_data_dict (dict): Secret data to be added/created,
+            example: {"auths":{
+                    <registry_name>:
+                        {"auth": <auth_token>,
+                        "email": <auth_email>},
+                    ...,
+                    <registry_name>:
+                        {"auth": <auth_token>,
+                        "email": <auth_email>}
+                    }
+                }
+        name (str): Secret name
+        namespace (str): Secret namespace
+
+    Returns:
+        Secret: secret object with secret_data_dict content included
+    """
+    secret = Secret(name=name, namespace=namespace)
+    secret_key = ".dockerconfigjson"
+    auths_key = "auths"
+
+    if secret.exists:
+        old_secret_data_dict = json.loads(
+            base64.b64decode(secret.instance.data[secret_key])
+        )[auths_key]
+        old_secret_data_dict.update(secret_data_dict[auths_key])
+        secret_data_encoded = dict_base64_encode(
+            _dict={auths_key: old_secret_data_dict}
+        )
+
+        ResourceEditor(
+            patches={secret: {"data": {secret_key: secret_data_encoded}}}
+        ).update()
+
+        return secret
+
+    secret.data_dict = {secret_key: dict_base64_encode(_dict=secret_data_dict)}
+
+    return secret.deploy()
```

### Comparing `openshift-python-utilities-4.13.9/ocp_utilities/must_gather.py` & `openshift-python-utilities-4.14.0/ocp_utilities/must_gather.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,8 +46,8 @@
         base_command += f" --kubeconfig {kubeconfig}"
     if script_name:
         base_command += f" -- {script_name}"
     # flag_name must be the last argument
     if flag_names:
         flag_string = "".join([f" --{flag_name}" for flag_name in flag_names])
         base_command += f" {flag_string}"
-    return run_command(command=shlex.split(base_command))[1]
+    return run_command(command=shlex.split(base_command), check=False)[1]
```

### Comparing `openshift-python-utilities-4.13.9/ocp_utilities/operators.py` & `openshift-python-utilities-4.14.0/ocp_utilities/operators.py`

 * *Files 9% similar despite different names*

```diff
@@ -118,96 +118,111 @@
     )
     if csv.exists:
         return csv
     raise ResourceNotFoundError(f"CSV {csv_name} not found in namespace: {namespace}")
 
 
 def install_operator(
-    admin_client, name, channel, source, target_namespaces=None, timeout=TIMEOUT_30MIN
+    admin_client,
+    name,
+    channel,
+    source,
+    target_namespaces=None,
+    timeout=TIMEOUT_30MIN,
+    operator_namespace=None,
 ):
     """
     Install operator on cluster.
 
     Args:
         admin_client (DynamicClient): Cluster client.
         name (str): Name of the operator to install.
         channel (str): Channel to install operator from.
         source (str): CatalogSource name.
         target_namespaces (list, optional): Target namespaces for the operator install process.
             If not provided, a namespace with te operator name will be created and used.
         timeout (int): Timeout in seconds to wait for operator to be ready.
+        operator_namespace (str, optional): Operator namespace, if not provided, operator name will be used
     """
 
+    operator_namespace = operator_namespace or name
     if target_namespaces:
         for namespace in target_namespaces:
             ns = Namespace(client=admin_client, name=namespace)
             if ns.exists:
                 continue
 
             ns.deploy(wait=True)
 
     else:
-        ns = Namespace(client=admin_client, name=name)
+        ns = Namespace(client=admin_client, name=operator_namespace)
         if not ns.exists:
             ns.deploy(wait=True)
 
     OperatorGroup(
         client=admin_client,
         name=name,
-        namespace=name,
+        namespace=operator_namespace,
         target_namespaces=target_namespaces,
     ).deploy(wait=True)
 
     subscription = Subscription(
         client=admin_client,
         name=name,
-        namespace=name,
+        namespace=operator_namespace,
         channel=channel,
         source=source,
         source_namespace="openshift-marketplace",
         install_plan_approval="Automatic",
     )
     subscription.deploy(wait=True)
     wait_for_operator_install(
         admin_client=admin_client,
         subscription=subscription,
         timeout=timeout,
     )
 
 
-def uninstall_operator(admin_client, name, timeout=TIMEOUT_30MIN):
+def uninstall_operator(
+    admin_client,
+    name,
+    timeout=TIMEOUT_30MIN,
+    operator_namespace=None,
+):
     """
     Uninstall operator on cluster.
 
     Args:
         admin_client (DynamicClient): Cluster client.
         name (str): Name of the operator to uninstall.
         timeout (int): Timeout in seconds to wait for operator to be uninstalled.
+        operator_namespace (str, optional): Operator namespace, if not provided, operator name will be used
     """
 
     csv_name = None
+    operator_namespace = operator_namespace or name
     subscription = Subscription(
         client=admin_client,
         name=name,
-        namespace=name,
+        namespace=operator_namespace,
     )
     if subscription.exists:
         csv_name = subscription.instance.status.installedCSV
         subscription.clean_up()
 
     OperatorGroup(
         client=admin_client,
         name=name,
-        namespace=name,
+        namespace=operator_namespace,
     ).clean_up()
 
     for _operator in Operator.get(dyn_client=admin_client):
         if _operator.name.startswith(name):
             # operator name convention is <name>.<namespace>
-            namespace = name.split(".")[-1]
+            namespace = operator_namespace or name.split(".")[-1]
             ns = Namespace(client=admin_client, name=namespace)
             if ns.exists:
                 ns.clean_up()
 
     if csv_name:
         csv = ClusterServiceVersion(
             client=admin_client,
```

### Comparing `openshift-python-utilities-4.13.9/ocp_utilities/utils.py` & `openshift-python-utilities-4.14.0/ocp_utilities/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,38 +57,44 @@
         LOGGER.error(error_msg)
         return False, out_decoded, err_decoded
 
     return True, out_decoded, err_decoded
 
 
 def run_ssh_commands(
-    host, commands, get_pty=False, check_rc=True, timeout=TIMEOUT_30MIN
+    host,
+    commands,
+    get_pty=False,
+    check_rc=True,
+    timeout=TIMEOUT_30MIN,
+    tcp_timeout=None,
 ):
     """
     Run commands via SSH
 
     Args:
         host (Host): rrmngmnt host to execute the commands from.
         commands (list): List of multiple command lists [[cmd1, cmd2, cmd3]] or a list with a single command [cmd]
             Examples:
                  ["sudo", "reboot"], [["sleep", "5"], ["date"]]
 
         get_pty (bool): get_pty parameter for remote session (equivalent to -t argument for ssh)
         check_rc (bool): if True checks command return code and raises if rc != 0
         timeout (int): ssh exec timeout
+        tcp_timeout (float): an optional timeout (in seconds) for the TCP connect
 
     Returns:
         list: List of commands output.
 
     Raise:
         CommandExecFailed: If command failed to execute.
     """
     results = []
     commands = commands if isinstance(commands[0], list) else [commands]
-    with host.executor().session() as ssh_session:
+    with host.executor().session(timeout=tcp_timeout) as ssh_session:
         for cmd in commands:
             rc, out, err = ssh_session.run_cmd(
                 cmd=cmd, get_pty=get_pty, timeout=timeout
             )
             LOGGER.info(f"[SSH][{host.fqdn}] Executed: {' '.join(cmd)}")
             if rc and check_rc:
                 raise CommandExecFailed(name=cmd, err=err)
```

### Comparing `openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/PKG-INFO` & `openshift-python-utilities-4.14.0/openshift_python_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.13.9
+Version: 4.14.0
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.13.9/pyproject.toml` & `openshift-python-utilities-4.14.0/pyproject.toml`

 * *Files identical despite different names*

