# Comparing `tmp/vantage6-3.8.8rc3.tar.gz` & `tmp/vantage6-3.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-3.8.8rc3.tar", last modified: Mon May 22 13:38:29 2023, max compression
+gzip compressed data, was "vantage6-3.9.0rc2.tar", last modified: Tue May  9 13:37:05 2023, max compression
```

## Comparing `vantage6-3.8.8rc3.tar` & `vantage6-3.9.0rc2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.120133 vantage6-3.8.8rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-22 13:38:29.120133 vantage6-3.8.8rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 13:38:29.120133 vantage6-3.8.8rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.116133 vantage6-3.8.8rc3/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.116133 vantage6-3.8.8rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.116133 vantage6-3.8.8rc3/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.120133 vantage6-3.8.8rc3/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/rabbitmq/rabbitmq.config
--rw-r--r--   0 runner    (1001) docker     (123)    29693 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 13:38:16.000000 vantage6-3.8.8rc3/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:29.116133 vantage6-3.8.8rc3/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-22 13:38:29.000000 vantage6-3.8.8rc3/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-22 13:38:29.000000 vantage6-3.8.8rc3/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:29.000000 vantage6-3.8.8rc3/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 13:38:29.000000 vantage6-3.8.8rc3/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-22 13:38:29.000000 vantage6-3.8.8rc3/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 13:38:29.000000 vantage6-3.8.8rc3/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.326882 vantage6-3.9.0rc2/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.322882 vantage6-3.9.0rc2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.326882 vantage6-3.9.0rc2/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37859 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/rabbitmq.config
+-rw-r--r--   0 runner    (1001) docker     (123)    29886 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.326882 vantage6-3.9.0rc2/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-3.8.8rc3/PKG-INFO` & `vantage6-3.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.8.8rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc2 Summary: vantage6
 command line interface Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-3.8.8rc3/setup.py` & `vantage6-3.9.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_description_content_type="text/markdown",
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'click==8.1.3',
         'colorama==0.4.6',
-        'docker==6.1.2',
+        'docker==6.0.1',
         'ipython==8.10.0',
         'questionary==1.10.0',
         'schema==0.7.5',
         'SQLAlchemy==1.4.46',
         f'vantage6-common == {version_ns["__version__"]}',
         f'vantage6-client == {version_ns["__version__"]}',
     ],
```

### Comparing `vantage6-3.8.8rc3/tests_cli/test_node_cli.py` & `vantage6-3.9.0rc2/tests_cli/test_node_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     cli_node_new_configuration,
     cli_node_files,
     cli_node_start,
     cli_node_stop,
     cli_node_attach,
     cli_node_create_private_key,
     cli_node_clean,
-    print_log_worker,
-    create_client_and_authenticate,
+    _print_log_worker,
+    _create_client_and_authenticate,
 )
 
 
 class NodeCLITest(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
@@ -246,15 +246,15 @@
             result.output,
             "[info ] - Stopped the vantage6-iknl-user Node.\n"
         )
 
         self.assertEqual(result.exit_code, 0)
 
     @patch("vantage6.cli.node.time")
-    @patch("vantage6.cli.node.print_log_worker")
+    @patch("vantage6.cli.node._print_log_worker")
     @patch("docker.DockerClient.containers")
     @patch("vantage6.cli.node.check_docker_running", return_value=True)
     def test_attach(self, check_docker, containers, log_worker, time_):
         """Attach docker logs without errors."""
         container1 = MagicMock()
         container1.name = f"{APPNAME}-iknl-user"
         containers.list.return_value = [container1]
@@ -288,15 +288,15 @@
 
         runner = CliRunner()
         result = runner.invoke(cli_node_clean)
 
         # check exit code
         self.assertEqual(result.exit_code, 0)
 
-    @patch("vantage6.cli.node.create_client_and_authenticate")
+    @patch("vantage6.cli.node._create_client_and_authenticate")
     @patch("vantage6.cli.node.NodeContext")
     def test_create_private_key(self, context, client):
         context.config_exists.return_value = True
         context.return_value.type_data_folder.return_value = Path(".")
         client.return_value = MagicMock(
             whoami=MagicMock(organization_name="Test")
         )
@@ -305,15 +305,15 @@
 
         result = runner.invoke(cli_node_create_private_key,
                                ["--name", "application"])
 
         self.assertEqual(result.exit_code, 0)
 
     @patch("vantage6.cli.node.RSACryptor")
-    @patch("vantage6.cli.node.create_client_and_authenticate")
+    @patch("vantage6.cli.node._create_client_and_authenticate")
     @patch("vantage6.cli.node.NodeContext")
     def test_create_private_key_overwite(self, context, client, cryptor):
         context.config_exists.return_value = True
         context.return_value.type_data_folder.return_value = Path(".")
         client.return_value = MagicMock(
             whoami=MagicMock(organization_name="Test")
         )
@@ -377,19 +377,19 @@
 
         runner = CliRunner()
         result = runner.invoke(cli_node_clean)
 
         # check exit code
         self.assertEqual(result.exit_code, 1)
 
-    def test_print_log_worker(self):
+    def test__print_log_worker(self):
         stream = BytesIO("Hello!".encode(STRING_ENCODING))
         temp_stdout = StringIO()
         with contextlib.redirect_stdout(temp_stdout):
-            print_log_worker(stream)
+            _print_log_worker(stream)
         output = temp_stdout.getvalue().strip()
         self.assertEqual(output, "Hello!")
 
     @patch("vantage6.cli.node.info")
     @patch("vantage6.cli.node.debug")
     @patch("vantage6.cli.node.error")
     @patch("vantage6.cli.node.Client")
@@ -402,22 +402,22 @@
                 "port": 5000,
                 "api_path": ""
             }
         )
 
         # should not trigger an exception
         try:
-            create_client_and_authenticate(ctx)
+            _create_client_and_authenticate(ctx)
         except Exception:
             self.fail("Raised an exception!")
 
         # client raises exception
         client.side_effect = Exception("Boom!")
         with self.assertRaises(Exception):
-            create_client_and_authenticate(ctx)
+            _create_client_and_authenticate(ctx)
 
     # TODO this function has been moved to the common package. A test should
     # be added there instead of here
     # @patch("vantage6.cli.node.error")
     # def test_check_docker(self, error):
     #     docker = MagicMock()
     #     try:
```

### Comparing `vantage6-3.8.8rc3/tests_cli/test_server_cli.py` & `vantage6-3.9.0rc2/tests_cli/test_server_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         runner = CliRunner()
         result = runner.invoke(cli_server_files, ["--name", "iknl"])
 
         self.assertIsNone(result.exception)
         self.assertEqual(result.exit_code, 0)
 
     @patch("docker.DockerClient.containers")
-    @patch("vantage6.cli.server.print_log_worker")
+    @patch("vantage6.cli.server._print_log_worker")
     @patch("vantage6.cli.server.click.Path")
     @patch("vantage6.cli.server.check_docker_running", return_value=True)
     @patch("vantage6.cli.server.ServerContext")
     def test_import(self, context, docker_check, click_path, log, containers):
         """Import entities without errors."""
         click_path.return_value = MagicMock()
```

### Comparing `vantage6-3.8.8rc3/tests_cli/test_wizard.py` & `vantage6-3.9.0rc2/tests_cli/test_wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def test_server_wizard(self):
 
         with patch(f"{module_path}.q") as q:
             q.prompt.side_effect = self.prompts
             q.confirm.return_value.ask.side_effect = [True, True, True, True]
 
-            config = server_configuration_questionaire("", "vantage6")
+            config = server_configuration_questionaire("vantage6")
 
             keys = ["description", "ip", "port", "api_path", "uri",
                     "allow_drop_all", "jwt_secret_key", "logging",
                     "vpn_server", "rabbitmq_uri", "two_factor_auth"]
 
             for key in keys:
                 self.assertIn(key, config)
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/_version.py` & `vantage6-3.9.0rc2/vantage6/cli/_version.py`

 * *Files 14% similar despite different names*

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
 pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/configuration_wizard.py` & `vantage6-3.9.0rc2/vantage6/cli/configuration_wizard.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,30 @@
 from vantage6.cli.context import NodeContext, ServerContext
 from vantage6.cli.configuration_manager import (
     NodeConfigurationManager,
     ServerConfigurationManager
 )
 
 
-def node_configuration_questionaire(dirs, instance_name):
-    """Questionary to generate a config file for the node instance."""
+def node_configuration_questionaire(dirs: dict, instance_name: str) -> dict:
+    """
+    Questionary to generate a config file for the node instance.
 
+    Parameters
+    ----------
+    dirs : dict
+        Dictionary with the directories of the node instance.
+    instance_name : str
+        Name of the node instance.
+
+    Returns
+    -------
+    dict
+        Dictionary with the new node configuration
+    """
     config = q.prompt([
         {
             "type": "text",
             "name": "api_key",
             "message": "Enter given api-key:"
         },
         {
@@ -83,15 +96,14 @@
         config['vpn_subnet'] = q.text(
             message="Subnet of the VPN server you want to connect to:",
             default='10.76.0.0/16'
         ).ask()
 
     config["logging"] = {
         "level": res,
-        "file": f"{instance_name}.log",
         "use_console": True,
         "backup_count": 5,
         "max_size": 1024,
         "format": "%(asctime)s - %(name)-14s - %(levelname)-8s - %(message)s",
         "datefmt": "%Y-%m-%d %H:%M:%S"
     }
 
@@ -104,16 +116,28 @@
         "enabled": encryption == "true",
         "private_key": private_key
     }
 
     return config
 
 
-def server_configuration_questionaire(dirs, instance_name):
-    """Questionary to generate a config file for the node instance."""
+def server_configuration_questionaire(instance_name: str) -> dict:
+    """
+    Questionary to generate a config file for the node instance.
+
+    Parameters
+    ----------
+    instance_name : str
+        Name of the node instance.
+
+    Returns
+    -------
+    dict
+        Dictionary with the new server configuration
+    """
 
     config = q.prompt([
         {
             "type": "text",
             "name": "description",
             "message": "Enter a human-readable description:"
         },
@@ -218,26 +242,45 @@
         "format": "%(asctime)s - %(name)-14s - %(levelname)-8s - %(message)s",
         "datefmt": "%Y-%m-%d %H:%M:%S"
     }
 
     return config
 
 
-def configuration_wizard(type_, instance_name, environment, system_folders):
+def configuration_wizard(type_: str, instance_name: str, environment: str,
+                         system_folders: bool) -> Path:
+    """
+    Create a configuration file for a node or server instance.
 
+    Parameters
+    ----------
+    type_ : str
+        Type of the instance. Either "node" or "server"
+    instance_name : str
+        Name of the instance
+    environment : str
+        Name of the environment
+    system_folders : bool
+        Whether to use the system folders or not
+
+    Returns
+    -------
+    Path
+        Path to the configuration file
+    """
     # for defaults and where to save the config
     dirs = NodeContext.instance_folders(type_, instance_name, system_folders)
 
     # invoke questionaire to create configuration file
     if type_ == "node":
         conf_manager = NodeConfigurationManager
         config = node_configuration_questionaire(dirs, instance_name)
     else:
         conf_manager = ServerConfigurationManager
-        config = server_configuration_questionaire(dirs, instance_name)
+        config = server_configuration_questionaire(instance_name)
 
     # in the case of an environment we need to add it to the current
     # configuration. In the case of application we can simply overwrite this
     # key (although there might be environments present)
     config_file = Path(dirs.get("config")) / (instance_name + ".yaml")
 
     if Path(config_file).exists():
@@ -247,18 +290,31 @@
 
     config_manager.put(environment, config)
     config_manager.save(config_file)
 
     return config_file
 
 
-def select_configuration_questionaire(type_, system_folders):
-    """Ask which configuration the user wants to use
+def select_configuration_questionaire(
+        type_: str, system_folders: bool) -> tuple[str, str]:
+    """
+    Ask which configuration the user wants to use. It shows only configurations
+    that are in the default folder.
 
-    It shows only configurations that are in the default folder.
+    Parameters
+    ----------
+    type_ : str
+        Type of the instance. Either "node" or "server"
+    system_folders : bool
+        Whether to use the system folders or not
+
+    Returns
+    -------
+    tuple[str, str]
+        Name of the configuration and the environment
     """
     context = NodeContext if type_ == "node" else ServerContext
     configs, f = context.available_configurations(system_folders)
 
     # each collection (file) can contain multiple configs. (e.g. test,
     # dev)
     choices = []
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/context.py` & `vantage6-3.9.0rc2/vantage6/cli/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 # TODO BvB 2023-01-10 we should have a look at all context classes and define
 # them in the same place. Now the DockerNodeContext is defined in the node, but
 # the server only has a TestServerContext there. This should be made consistent
 from __future__ import annotations
 
 import os.path
 
-from typing import Tuple
 from pathlib import Path
 
 from sqlalchemy.engine.url import make_url
 
 from vantage6.common.context import AppContext
 from vantage6.common.globals import APPNAME
 from vantage6.cli.configuration_manager import (NodeConfigurationManager,
@@ -77,38 +76,30 @@
         -------
         str
             string representation of the database uri
         """
         uri = os.environ.get("VANTAGE6_DB_URI") or self.config['uri']
         url = make_url(uri)
 
-        if url.host is None and not os.path.isabs(url.database):
-            # We're dealing with a relative path here of a local database, when
-            # we're running the server outside of docker. Therefore we need to
-            # prepend the data directory to the database name, but after the
-            # driver name (e.g. sqlite:////db.sqlite ->
-            # sqlite:////data_dir>/db.sqlite)
-
-            # find index of database name
-            idx_db_name = str(url).find(url.database)
-
-            # add the datadir to the right location in the database uri
-            return str(url)[:idx_db_name] + str(self.data_dir / url.database)
+        if (url.host is None) and (not os.path.isabs(url.database)):
+            # We're dealing with a relative path here.
+            url.database = str(self.data_dir / url.database)
+            uri = str(url)
 
         return uri
 
     @property
     def docker_container_name(self) -> str:
         """
-        Unique name of the docker container.
+        Name of the docker container that the server is running in.
 
         Returns
         -------
         str
-            Unique docker container name
+            Server's docker container name
         """
         return f"{APPNAME}-{self.name}-{self.scope}-server"
 
     @classmethod
     def from_external_config_file(
             cls, path: str, environment: str = S_ENV,
             system_folders: bool = S_FOL) -> ServerContext:
@@ -163,26 +154,26 @@
         """
         return super().config_exists("server", instance_name,
                                      environment=environment,
                                      system_folders=system_folders)
 
     @classmethod
     def available_configurations(cls, system_folders: bool = S_FOL) \
-            -> Tuple[list, list]:
+            -> tuple[list, list]:
         """
         Find all available server configurations in the default folders.
 
         Parameters
         ----------
         system_folders : bool, optional
             System wide or user configuration, by default S_FOL
 
         Returns
         -------
-        Tuple[List, List]
+        tuple[list, list]
             The first list contains validated configuration files, the second
             list contains invalid configuration files.
         """
         return super().available_configurations("server", system_folders)
 
 
 class NodeContext(AppContext):
@@ -267,70 +258,70 @@
         """
         return super().config_exists("node", instance_name,
                                      environment=environment,
                                      system_folders=system_folders)
 
     @classmethod
     def available_configurations(cls, system_folders: bool = N_FOL) \
-            -> Tuple[list, list]:
+            -> tuple[list, list]:
         """
         Find all available server configurations in the default folders.
 
         Parameters
         ----------
         system_folders : bool, optional
             System wide or user configuration, by default N_FOL
 
         Returns
         -------
-        Tuple[List, List]
+        tuple[list, list]
             The first list contains validated configuration files, the second
             list contains invalid configuration files.
         """
         return super().available_configurations("node", system_folders)
 
     @staticmethod
     def type_data_folder(system_folders: bool = N_FOL) -> Path:
         """
         Obtain OS specific data folder where to store node specific data.
 
         Parameters
         ----------
         system_folders : bool, optional
-            System wide or user configuration, by default N_FOL
+            System wide or user configuration
 
         Returns
         -------
         Path
             Path to the data folder
         """
         return AppContext.type_data_folder("node", system_folders)
 
     @property
-    def databases(self):
+    def databases(self) -> dict:
         """
         Dictionary of local databases that are available for this node.
 
         Returns
         -------
         dict
             dictionary with database names as keys and their corresponding
             paths as values.
         """
         return self.config["databases"]
 
     @property
     def docker_container_name(self) -> str:
         """
-        Unique Docker container name of the node.
+        Docker container name of the node.
 
         Returns
         -------
         str
-            Unique Docker container name
+            Node's Docker container name
         """
         return f"{APPNAME}-{self.name}-{self.scope}"
 
     @property
     def docker_network_name(self) -> str:
         """
         Private Docker network name which is unique for this node.
@@ -377,21 +368,40 @@
     def docker_ssh_volume_name(self) -> str:
         """
         Docker volume in which the SSH configuration is stored.
 
         Returns
         -------
         str
-            Docker voluem name
+            Docker volume name
         """
         return os.environ.get(
             'SSH_TUNNEL_VOLUME_NAME',
             f"{self.docker_container_name}-ssh-vol"
         )
 
+    @property
+    def docker_squid_volume_name(self) -> str:
+        """
+        Docker volume in which the SSH configuration is stored.
+
+        Returns
+        -------
+        str
+            Docker volume name
+        """
+        return os.environ.get(
+            'SSH_SQUID_VOLUME_NAME',
+            f"{self.docker_container_name}-squid-vol"
+        )
+
+    @property
+    def proxy_log_file(self):
+        return self.log_file_name(type_="proxy_server")
+
     def docker_temporary_volume_name(self, run_id: int) -> str:
         """
         Docker volume in which temporary data is stored. Temporary data is
         linked to a specific run. Multiple algorithm containers can have the
         same run id, and therefore the share same temporary volume.
 
         Parameters
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/globals.py` & `vantage6-3.9.0rc2/vantage6/cli/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.8rc3/vantage6/cli/node.py` & `vantage6-3.9.0rc2/vantage6/cli/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,24 @@
     * vnode start
     * vnode stop
     * vnode attach
     * vnode clean
     * vnode remove
     * vnode version
     * vnode create-private-key
-
-
 """
 import click
 import sys
 import questionary as q
 import docker
 import time
 import os.path
 import itertools
 
-from typing import Iterable, Tuple, List
+from typing import Iterable
 from pathlib import Path
 from threading import Thread
 from colorama import Fore, Style
 
 from vantage6.common import (
     warning, error, info, debug,
     bytes_to_base64s, check_config_writeable,
@@ -78,15 +76,15 @@
     """
     Lists all nodes in the default configuration directories.
     """
 
     client = docker.from_env()
     check_docker_running()
 
-    running_node_names = find_running_node_names(client)
+    running_node_names = _find_running_node_names(client)
 
     header = \
         "\nName"+(21*" ") + \
         "Environments"+(20*" ") + \
         "Status"+(10*" ") + \
         "System/User"
 
@@ -213,15 +211,15 @@
     name : str
         Name of the configuration file.
     environment : str
         DTAP environment to use.
     system_folders : bool
         Is this configuration stored in the system or in the user folders.
     """
-    name, environment = select_node(name, environment, system_folders)
+    name, environment = _select_node(name, environment, system_folders)
 
     # create node context
     ctx = NodeContext(name, environment=environment,
                       system_folders=system_folders)
 
     # return path of the configuration
     info(f"Configuration file = {ctx.config_file}")
@@ -367,23 +365,25 @@
         info(" ... success!")
 
     info("Creating Docker data volume")
 
     data_volume = docker_client.volumes.create(ctx.docker_volume_name)
     vpn_volume = docker_client.volumes.create(ctx.docker_vpn_volume_name)
     ssh_volume = docker_client.volumes.create(ctx.docker_ssh_volume_name)
+    squid_volume = docker_client.volumes.create(ctx.docker_squid_volume_name)
 
     info("Creating file & folder mounts")
     # FIXME: should obtain mount points from DockerNodeContext
     mounts = [
         # (target, source)
         ("/mnt/log", str(ctx.log_dir)),
         ("/mnt/data", data_volume.name),
         ("/mnt/vpn", vpn_volume.name),
         ("/mnt/ssh", ssh_volume.name),
+        ("/mnt/squid", squid_volume.name),
         ("/mnt/config", str(ctx.config_dir)),
         ("/var/run/docker.sock", "/var/run/docker.sock"),
     ]
 
     if mount_src:
         # If mount_src is a relative path, docker will consider it a volume.
         mount_src = os.path.abspath(mount_src)
@@ -521,15 +521,15 @@
         tty=True
     )
 
     info(f"Success! container id = {container}")
 
     if attach:
         logs = container.attach(stream=True, logs=True)
-        Thread(target=print_log_worker, args=(logs,), daemon=True).start()
+        Thread(target=_print_log_worker, args=(logs,), daemon=True).start()
         while True:
             try:
                 time.sleep(1)
             except KeyboardInterrupt:
                 info("Closing log file. Keyboard Interrupt.")
                 info("Note that your node is still running! Shut it down with "
                      f"'{Fore.RED}vnode stop{Style.RESET_ALL}'")
@@ -561,15 +561,15 @@
         If set to true, all running nodes will be stopped.
     force : bool
         If set to true, the node will not be stopped gracefully.
     """
     client = docker.from_env()
     check_docker_running()
 
-    running_node_names = find_running_node_names(client)
+    running_node_names = _find_running_node_names(client)
 
     if not running_node_names:
         warning("No nodes are currently running.")
         return
 
     if force:
         warning('Forcing the node to stop will not terminate helper '
@@ -623,27 +623,31 @@
         Name of the configuration file.
     system_folders : bool
         Wether this configuration stored in the system or in the user folders.
     """
     client = docker.from_env()
     check_docker_running()
 
-    running_node_names = find_running_node_names(client)
+    running_node_names = _find_running_node_names(client)
+
+    if not running_node_names:
+        warning("No nodes are currently running. Cannot show any logs!")
+        return
 
     if not name:
         name = q.select("Select the node you wish to inspect:",
                         choices=running_node_names).ask()
     else:
         post_fix = "system" if system_folders else "user"
         name = f"{APPNAME}-{name}-{post_fix}"
 
     if name in running_node_names:
         container = client.containers.get(name)
         logs = container.attach(stream=True, logs=True)
-        Thread(target=print_log_worker, args=(logs,), daemon=True).start()
+        Thread(target=_print_log_worker, args=(logs,), daemon=True).start()
         while True:
             try:
                 time.sleep(1)
             except KeyboardInterrupt:
                 info("Closing log file. Keyboard Interrupt.")
                 info("Note that your node is still running! Shut it down with "
                      f"'{Fore.RED}vnode stop{Style.RESET_ALL}'")
@@ -693,15 +697,15 @@
     """
     NodeContext.LOGGING_ENABLED = False
     if config:
         name = Path(config).stem
         ctx = NodeContext(name, environment, system_folders, config)
     else:
         # retrieve context
-        name, environment = select_node(name, environment, system_folders)
+        name, environment = _select_node(name, environment, system_folders)
 
         # raise error if config could not be found
         if not NodeContext.config_exists(name, environment, system_folders):
             error(
                 f"The configuration {Fore.RED}{name}{Style.RESET_ALL} with "
                 f"environment {Fore.RED}{environment}{Style.RESET_ALL} could "
                 f"not be found."
@@ -710,15 +714,15 @@
 
         # Create node context
         ctx = NodeContext(name, environment, system_folders)
 
     # Authenticate with the server to obtain organization name if it wasn't
     # provided
     if organization_name is None:
-        client = create_client_and_authenticate(ctx)
+        client = _create_client_and_authenticate(ctx)
         organization_name = client.whoami.organization_name
 
     # create directory where private key goes if it doesn't exist yet
     ctx.type_data_folder(system_folders).mkdir(parents=True, exist_ok=True)
 
     # generate new key, and save it
     filename = f"privkey_{organization_name}.pem"
@@ -770,15 +774,15 @@
     if upload:
         info(
             "Uploading public key to the server. "
             "This will overwrite any previously existing key!"
         )
 
         if 'client' not in locals():
-            client = create_client_and_authenticate(ctx)
+            client = _create_client_and_authenticate(ctx)
 
         # TODO what happens if the user doesn't have permission to upload key?
         # Does that lead to an exception or not?
         try:
             client.request(
                 f"/organization/{client.whoami.organization_id}",
                 method="patch",
@@ -856,21 +860,21 @@
     environment : str
         DTAP environment, note that regardless of the environment, the entire
         configuration is deleted
     system_folders : bool
         If True, use system folders, otherwise use user folders
     """
     # select configuration name if none supplied
-    name, environment = select_node(name, environment, system_folders)
+    name, environment = _select_node(name, environment, system_folders)
 
     client = docker.from_env()
     check_if_docker_daemon_is_running(client)
 
     # check if node is still running, otherwise don't allow deleting it
-    running_node_names = find_running_node_names(client)
+    running_node_names = _find_running_node_names(client)
 
     post_fix = "system" if system_folders else "user"
     node_container_name = f"{APPNAME}-{name}-{post_fix}"
     if node_container_name in running_node_names:
         error(f"Node {name} is still running! Please stop the node before "
               "deleting it.")
         exit(1)
@@ -896,25 +900,25 @@
         # remove docker vpn volume
         if vol.name == ctx.docker_vpn_volume_name:
             info(f"Deleting VPN docker volume {vol.name}")
             vol.remove()
 
     # remove the VPN configuration file
     vpn_config_file = os.path.join(ctx.data_dir, 'vpn', VPN_CONFIG_FILE)
-    remove_file(vpn_config_file, 'VPN configuration')
+    _remove_file(vpn_config_file, 'VPN configuration')
 
     # remove the config file
-    remove_file(ctx.config_file, 'configuration')
+    _remove_file(ctx.config_file, 'configuration')
 
     # remove the log file. As this process opens the log file above, the log
     # handlers need to be closed before deleting
     info(f"Removing log file {ctx.log_file}")
     for handler in itertools.chain(ctx.log.handlers, ctx.log.root.handlers):
         handler.close()
-    remove_file(ctx.log_file, 'log')
+    _remove_file(ctx.log_file, 'log')
 
 
 #
 #   version
 #
 @cli_node.command(name='version')
 @click.option("-n", "--name", default=None, help="configuration name")
@@ -930,15 +934,15 @@
         Configuration name
     system_folders : bool
         If True, use system folders, otherwise use user folders
     """
     client = docker.from_env()
     check_docker_running()
 
-    running_node_names = find_running_node_names(client)
+    running_node_names = _find_running_node_names(client)
 
     if not name:
         if not running_node_names:
             error("No nodes are running! You can only check the version for "
                   "nodes that are running")
             exit(1)
         name = q.select("Select the node you wish to inspect:",
@@ -962,20 +966,32 @@
 @cli_node.command(name='set-api-key')
 @click.option("-n", "--name", default=None, help="configuration name")
 @click.option("--api-key", default=None, help="New API key")
 @click.option('-e', '--environment', default=N_ENV,
               help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=N_FOL)
-def cli_node_set_api_key(name, api_key, environment, system_folders):
+def cli_node_set_api_key(name: str, api_key: str, environment: str,
+                         system_folders: bool) -> None:
     """
     Put a new API key into the node configuration file
+
+    Parameters
+    ----------
+    name : str
+        Node configuration name
+    api_key : str
+        New API key
+    environment : str
+        DTAP environment
+    system_folders : bool
+        If True, use system folders, otherwise use user folders
     """
     # select name and environment
-    name, environment = select_node(name, environment, system_folders)
+    name, environment = _select_node(name, environment, system_folders)
 
     # Check that we can write in the config folder
     if not check_config_writeable(system_folders):
         error("Your user does not have write access to all folders. Exiting")
         exit(1)
 
     if not api_key:
@@ -991,29 +1007,28 @@
     conf_mgr.put(environment, ctx.config)
     conf_mgr.save(ctx.config_file)
     info("Your new API key has been uploaded to the config file "
          f"{ctx.config_file}.")
 
 
 #  helper functions
-def print_log_worker(logs_stream: Iterable[bytes]) -> None:
+def _print_log_worker(logs_stream: Iterable[bytes]) -> None:
     """
     Print the logs from the logs stream.
 
     Parameters
     ----------
     logs_stream : Iterable[bytes]
         Output of the container.attach() method
     """
-
     for log in logs_stream:
         print(log.decode(STRING_ENCODING), end="")
 
 
-def create_client_and_authenticate(ctx: NodeContext) -> Client:
+def _create_client_and_authenticate(ctx: NodeContext) -> Client:
     """
     Generate a client and authenticate with the server.
 
     Parameters
     ----------
     ctx : NodeContext
         Context of the node loaded from the configuration file
@@ -1040,23 +1055,23 @@
         error("Could not authenticate with server!")
         debug(e)
         exit(1)
 
     return client
 
 
-def select_node(name: str, environment: str, system_folders: bool) \
-        -> Tuple[str, str]:
+def _select_node(name: str, environment: str, system_folders: bool) \
+        -> tuple[str, str]:
     """
     Let user select node through questionnaire if name/environment is not
     given.
 
     Returns
     -------
-    Tuple[str, str]
+    tuple[str, str]
         name, environment of the configuration file
     """
     name, environment = (name, environment) if name else \
         select_configuration_questionaire("node", system_folders)
 
     # raise error if config could not be found
     if not NodeContext.config_exists(name, environment, system_folders):
@@ -1065,34 +1080,34 @@
             f"environment {Fore.RED}{environment}{Style.RESET_ALL} could "
             f"not be found."
         )
         exit(1)
     return name, environment
 
 
-def find_running_node_names(client: docker.DockerClient) -> List[str]:
+def _find_running_node_names(client: docker.DockerClient) -> list[str]:
     """
     Returns a list of names of running nodes.
 
     Parameters
     ----------
     client : docker.DockerClient
         Docker client instance
 
     Returns
     -------
-    List[str]
+    list[str]
         List of names of running nodes
     """
     running_nodes = client.containers.list(
         filters={"label": f"{APPNAME}-type=node"})
     return [node.name for node in running_nodes]
 
 
-def remove_file(file: str, file_type: str) -> None:
+def _remove_file(file: str, file_type: str) -> None:
     """
     Remove a file if it exists.
 
     Parameters
     ----------
     file : str
         absolute path to the file to be deleted
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/rabbitmq/__init__.py` & `vantage6-3.9.0rc2/vantage6/cli/rabbitmq/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """RabbitMQ utilities."""
-from typing import Dict
 
 from vantage6.common import is_ip_address
 
 
-def split_rabbitmq_uri(rabbit_uri: str) -> Dict:
-    """Get details (user, pass, host, vhost, port) from a RabbitMQ uri.
+def split_rabbitmq_uri(rabbit_uri: str) -> dict:
+    """
+    Get details (user, pass, host, vhost, port) from a RabbitMQ uri.
 
     Parameters
     ----------
     rabbit_uri: str
         URI of RabbitMQ service ('amqp://$user:$pass@$host:$port/$vhost')
 
     Returns
     -------
-    Dict[str]
+    dict[str]
         The vhost defined in the RabbitMQ URI
     """
     (user_details, location_details) = rabbit_uri.split('@', 1)
     (user, password) = user_details.split('/')[-1].split(':', 1)
     (host, remainder) = location_details.split(':', 1)
     port, vhost = remainder.split('/', 1)
     return {
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/rabbitmq/definitions.py` & `vantage6-3.9.0rc2/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.8rc3/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-3.9.0rc2/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import shutil
 import base64
 import hashlib
 import time
 
 from pathlib import Path
-from typing import Dict
 
 from vantage6.common.globals import APPNAME
 from vantage6.common import debug, info, error
 from vantage6.common.docker.addons import get_container
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.cli.context import ServerContext
 from vantage6.cli.rabbitmq.definitions import RABBITMQ_DEFINITIONS
@@ -22,27 +21,26 @@
 RABBIT_CONFIG = 'rabbitmq.config'
 RABBIT_DIR = 'rabbitmq'
 
 
 class RabbitMQManager:
     """
     Manages the RabbitMQ docker container
+
+    Parameters
+    ----------
+    ctx: ServerContext
+        Configuration object
+    queue_uri: str
+        URI where the RabbitMQ instance should be running
+    network_mgr: NetworkManager
+        Network manager for network in which server container resides
     """
     def __init__(self, ctx: ServerContext, network_mgr: NetworkManager,
                  image: str = None) -> None:
-        """
-        Parameters
-        ----------
-        ctx: ServerContext
-            Configuration object
-        queue_uri: str
-            URI where the RabbitMQ instance should be running
-        network_mgr: NetworkManager
-            Network manager for network in which server container resides
-        """
         self.ctx = ctx
         self.queue_uri = self.ctx.config.get('rabbitmq_uri')
         rabbit_splitted = split_rabbitmq_uri(self.queue_uri)
         self.rabbit_user = rabbit_splitted['user']
         self.rabbit_pass = rabbit_splitted['password']
         self.vhost = rabbit_splitted['vhost']
         self.port = rabbit_splitted['port']
@@ -125,19 +123,24 @@
             Whether the container has fully initialized RabbitMQ or not
         """
         response = self.rabbit_container.exec_run(
             cmd="rabbitmqctl status --formatter json"
         )
         return response.exit_code == 0
 
-    def _get_volumes(self) -> Dict:
+    def _get_volumes(self) -> dict:
         """
         Prepare the volumes for the RabbitMQ container. The RabbitMQ should
         set up the right vhost and users to allow the server to communicate
         with RabbitMQ as configured.
+
+        Returns
+        -------
+        dict
+            Dictionary with the volumes to mount in the RabbitMQ container
         """
         # default RabbitMQ configuration: replace the user/password with the
         # credentials from the configuraiton
         rabbit_definitions = self._get_rabbitmq_definitions()
 
         # write the RabbitMQ definition to file(s)
         with open(self.definitions_file, 'w') as f:
@@ -162,15 +165,15 @@
                 'bind': '/etc/rabbitmq/rabbitmq.config', 'mode': 'ro'
             },
             rabbit_data_dir: {
                 'bind': '/var/lib/rabbitmq', 'mode': 'rw'
             }
         }
 
-    def _get_rabbitmq_definitions(self) -> Dict:
+    def _get_rabbitmq_definitions(self) -> dict:
         """
         Get startup definitions (users/vhosts etc) for RabbitMQ container
 
         Returns
         -------
         Dict:
             dictionary with all users/vhosts etc that must be generated on
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/server.py` & `vantage6-3.9.0rc2/vantage6/cli/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 import questionary as q
 import docker
 import os
 import time
 import subprocess
 
-from typing import Callable, Type, Iterable
+from typing import Iterable
 from threading import Thread
 from functools import wraps
 from colorama import (Fore, Style)
 from sqlalchemy.engine.url import make_url
 from docker.client import DockerClient
 
 from vantage6.common import (info, warning, error, debug as debug_msg,
@@ -36,15 +36,15 @@
     configuration_wizard
 )
 from vantage6.cli.utils import check_config_name_allowed
 from vantage6.cli.rabbitmq.queue_manager import RabbitMQManager
 from vantage6.cli import __version__, rabbitmq
 
 
-def click_insert_context(func: Callable) -> Callable:
+def click_insert_context(func: callable) -> callable:
     """
     Supply the Click function with additional context parameters. The context
     is then passed to the function as the first argument.
 
     Parameters
     ----------
     func : Callable
@@ -63,15 +63,15 @@
                   default=DEFAULT_SERVER_ENVIRONMENT,
                   help='configuration environment to use')
     @click.option('--system', 'system_folders', flag_value=True)
     @click.option('--user', 'system_folders', flag_value=False,
                   default=DEFAULT_SERVER_SYSTEM_FOLDERS)
     @wraps(func)
     def func_with_context(name: str, config: str, environment: str,
-                          system_folders: bool, *args, **kwargs) -> Callable:
+                          system_folders: bool, *args, **kwargs) -> callable:
         """
         Decorator function that adds the context to the function.
 
         Parameters
         ----------
         name : str
             name of the configuration you want to use.
@@ -103,15 +103,15 @@
                 name, environment = select_configuration_questionaire(
                     "server", system_folders
                 )
             except Exception:
                 error("No configurations could be found!")
                 exit(1)
 
-        ctx = get_server_context(name, environment, system_folders)
+        ctx = _get_server_context(name, environment, system_folders)
         return func(ctx, *args, **kwargs)
 
     return func_with_context
 
 
 @click.group(name='server')
 def cli_server() -> None:
@@ -130,23 +130,23 @@
 @click.option('--keep/--auto-remove', default=False,
               help="Keep image after finishing")
 @click.option('--mount-src', default='',
               help="mount vantage6-master package source")
 @click.option('--attach/--detach', default=False,
               help="Attach server logs to the console after start")
 @click_insert_context
-def cli_server_start(ctx: Type[ServerContext], ip: str, port: int, image: str,
+def cli_server_start(ctx: ServerContext, ip: str, port: int, image: str,
                      rabbitmq_image: str, keep: bool, mount_src: str,
                      attach: bool) -> None:
     """
     Start the server in a Docker container.
 
     Parameters
     ----------
-    ctx : Type[ServerContext]
+    ctx : ServerContext
         Server context object
     ip : str
         ip interface to listen on
     port : int
         port to listen on
     image : str
         Server Docker image to use
@@ -284,15 +284,15 @@
         network=server_network_mgr.network_name
     )
 
     info(f"Success! container id = {container.id}")
 
     if attach:
         logs = container.attach(stream=True, logs=True, stdout=True)
-        Thread(target=print_log_worker, args=(logs,), daemon=True).start()
+        Thread(target=_print_log_worker, args=(logs,), daemon=True).start()
         while True:
             try:
                 time.sleep(1)
             except KeyboardInterrupt:
                 info("Closing log file. Keyboard Interrupt.")
                 info("Note that your server is still running! Shut it down "
                      f"with {Fore.RED}vserver stop{Style.RESET_ALL}")
@@ -359,15 +359,15 @@
 
 
 #
 #   files
 #
 @cli_server.command(name='files')
 @click_insert_context
-def cli_server_files(ctx: Type[ServerContext]) -> None:
+def cli_server_files(ctx: ServerContext) -> None:
     """
     List files locations of a server instance.
 
     Parameters
     ----------
     ctx : Type[ServerContext]
         Server context object
@@ -423,15 +423,15 @@
         error(e)
         exit(1)
 
     # Check that we can write in this folder
     if not check_config_writeable(system_folders):
         error("Your user does not have write access to all folders. Exiting")
         info(f"Create a new server using '{Fore.GREEN}vserver new "
-             f"--user{Style.RESET_ALL}' instead!")
+             "--user{Style.RESET_ALL}' instead!")
         exit(1)
 
     # create config in ctx location
     cfg_file = configuration_wizard("server", name, environment=environment,
                                     system_folders=system_folders)
     info(f"New configuration created: {Fore.GREEN}{cfg_file}{Style.RESET_ALL}")
 
@@ -450,22 +450,22 @@
 @click.option('--drop-all', is_flag=True, default=False)
 @click.option('-i', '--image', default=None, help="Node Docker image to use")
 @click.option('--mount-src', default='',
               help="mount vantage6-master package source")
 @click.option('--keep/--auto-remove', default=False,
               help="Keep image after finishing")
 @click_insert_context
-def cli_server_import(ctx: Type[ServerContext], file_: str, drop_all: bool,
+def cli_server_import(ctx: ServerContext, file_: str, drop_all: bool,
                       image: str, mount_src: str, keep: bool) -> None:
     """
     Batch import organizations/collaborations/users and tasks.
 
     Parameters
     ----------
-    ctx : Type[ServerContext]
+    ctx : ServerContext
         Server context object
     file_ : str
         Yaml file containing the vantage6 formatted data to import
     drop_all : bool
         Wether to drop all data before importing
     image : str
         Node Docker image to use which contains the import script
@@ -563,25 +563,25 @@
             "name": ctx.config_file_name
         },
         environment=environment_vars,
         auto_remove=not keep,
         tty=True
     )
     logs = container.logs(stream=True, stdout=True)
-    Thread(target=print_log_worker, args=(logs,), daemon=False).start()
+    Thread(target=_print_log_worker, args=(logs,), daemon=False).start()
 
     info(f"Success! container id = {container.id}")
 
 
 #
 #   shell
 #
 @cli_server.command(name='shell')
 @click_insert_context
-def cli_server_shell(ctx: Type[ServerContext]) -> None:
+def cli_server_shell(ctx: ServerContext) -> None:
     """
     Run an iPython shell in the server container and attach the ORM. This
     can be used to modify the database.
 
     Parameters
     ----------
     ctx : Type[ServerContext]
@@ -699,15 +699,15 @@
     else:
         post_fix = "system" if system_folders else "user"
         name = f"{APPNAME}-{name}-{post_fix}-server"
 
     if name in running_server_names:
         container = client.containers.get(name)
         logs = container.attach(stream=True, logs=True, stdout=True)
-        Thread(target=print_log_worker, args=(logs,), daemon=True).start()
+        Thread(target=_print_log_worker, args=(logs,), daemon=True).start()
         while True:
             try:
                 time.sleep(1)
             except KeyboardInterrupt:
                 info("Closing log file. Keyboard Interrupt.")
                 info("Note that your server is still running! Shut it down "
                      f"with {Fore.RED}vserver stop{Style.RESET_ALL}")
@@ -720,15 +720,15 @@
 #   version
 #
 @cli_server.command(name='version')
 @click.option("-n", "--name", default=None, help="configuration name")
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False,
               default=DEFAULT_SERVER_SYSTEM_FOLDERS)
-def cli_server_version(name: str, system_folders: bool):
+def cli_server_version(name: str, system_folders: bool) -> None:
     """
     Print the version of the vantage6 services.
 
     Parameters
     ----------
     name : str
         Name of the server to inspect
@@ -762,19 +762,28 @@
     else:
         error(f"Server {name} is not running! Cannot provide version...")
 
 
 #
 # helper functions
 #
-def get_server_context(name: str, environment: str, system_folders: bool) \
+def _get_server_context(name: str, environment: str, system_folders: bool) \
         -> ServerContext:
     """
     Load the server context from the configuration file.
 
+    Parameters
+    ----------
+    name : str
+        Name of the server to inspect
+    environment : str
+        DTAP environment to use
+    system_folders : bool
+        Wether to use system folders or if False, the user folders
+
     Returns
     -------
     ServerContext
         Server context object
     """
     if not ServerContext.config_exists(name, environment, system_folders):
         scope = "system" if system_folders else "user"
@@ -847,15 +856,15 @@
     info(f"Stopped the {Fore.GREEN}{container_name}{Style.RESET_ALL} server.")
 
     # find the configuration name from the docker container name
     # server name is formatted as f"{APPNAME}-{self.name}-{self.scope}-server"
     scope = "system" if system_folders else "user"
     config_name = get_server_config_name(container_name, scope)
 
-    ctx = get_server_context(config_name, environment, system_folders)
+    ctx = _get_server_context(config_name, environment, system_folders)
 
     # delete the server network
     network_name = f"{APPNAME}-{ctx.name}-{ctx.scope}-network"
     network = get_network(client, name=network_name)
     delete_network(network, kill_containers=False)
 
     # kill RabbitMQ if it exists and no other servers are using to it (i.e. it
@@ -868,15 +877,15 @@
         if rabbit_container and \
                 get_num_nonempty_networks(rabbit_container) == 0:
             remove_container(rabbit_container, kill=True)
             info(f"Stopped the {Fore.GREEN}{rabbit_container_name}"
                  f"{Style.RESET_ALL} container.")
 
 
-def print_log_worker(logs_stream: Iterable[bytes]) -> None:
+def _print_log_worker(logs_stream: Iterable[bytes]) -> None:
     """
     Print the logs from the docker container to the terminal.
 
     Parameters
     ----------
     logs_stream : Iterable[bytes]
         Output of the `container.attach(.)` method
```

### Comparing `vantage6-3.8.8rc3/vantage6/cli/utils.py` & `vantage6-3.9.0rc2/vantage6/cli/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 Utility functions for the CLI
 """
 from __future__ import annotations
 
 import re
 import docker
 
-from typing import Type
-
 from vantage6.common import error
 
 
 def check_config_name_allowed(name: str) -> None:
     """
     Check if configuration name is allowed
 
@@ -25,21 +23,21 @@
               "characters: a-zA-Z0-9_.-")
         # FIXME: FM, 2023-01-03: I dont think this is a good side effect. This
         # should be handled by the caller.
         exit(1)
 
 
 def check_if_docker_daemon_is_running(
-        docker_client: Type[docker.DockerClient]) -> None:
+        docker_client: docker.DockerClient) -> None:
     """
     Check if Docker daemon is running
 
     Parameters
     ----------
-    docker_client : Type[docker.DockerClient]
+    docker_client : docker.DockerClient
         The docker client
     """
     try:
         docker_client.ping()
     except Exception:
         error("Docker socket can not be found. Make sure Docker is running.")
         exit(1)
```

### Comparing `vantage6-3.8.8rc3/vantage6.egg-info/PKG-INFO` & `vantage6-3.9.0rc2/vantage6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.8.8rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc2 Summary: vantage6
 command line interface Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-3.8.8rc3/vantage6.egg-info/SOURCES.txt` & `vantage6-3.9.0rc2/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

