# Comparing `tmp/NREL-gaps-0.3.2.tar.gz` & `tmp/NREL-gaps-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-gaps-0.3.2.tar", last modified: Thu May 18 02:11:49 2023, max compression
+gzip compressed data, was "NREL-gaps-0.3.3.tar", last modified: Mon May 22 22:12:59 2023, max compression
```

## Comparing `NREL-gaps-0.3.2.tar` & `NREL-gaps-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.411793 NREL-gaps-0.3.2/NREL_gaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.415794 NREL-gaps-0.3.2/gaps/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/gaps/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/project_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.644186 NREL-gaps-0.3.3/NREL_gaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/gaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/gaps/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/project_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/setup.py
```

### Comparing `NREL-gaps-0.3.2/LICENSE` & `NREL-gaps-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/NREL_gaps.egg-info/PKG-INFO` & `NREL-gaps-0.3.3/NREL_gaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.3.2
+Version: 0.3.3
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NREL-gaps-0.3.2/NREL_gaps.egg-info/SOURCES.txt` & `NREL-gaps-0.3.3/NREL_gaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/PKG-INFO` & `NREL-gaps-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.3.2
+Version: 0.3.3
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NREL-gaps-0.3.2/README.rst` & `NREL-gaps-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/batch.py` & `NREL-gaps-0.3.3/gaps/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/batch.py` & `NREL-gaps-0.3.3/gaps/cli/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/cli.py` & `NREL-gaps-0.3.3/gaps/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,45 +49,20 @@
                 all_commands.append(collect_configuration)
         self.command_configs = all_commands
         return self
 
     def convert_to_commands(self):
         """Convert all of the command configs into click commands."""
         for command_config in self.command_configs:
-            doc = command_config.documentation
-            name = command_config.name
-            params = [
-                click.Option(
-                    param_decls=["--config_file", "-c"],
-                    required=True,
-                    type=click.Path(exists=True),
-                    help=doc.config_help(name),
-                )
-            ]
-
-            command = _WrappedCommand(
-                name,
-                context_settings=None,
-                callback=partial(
-                    from_config,
-                    command_config=command_config,
-                ),
-                params=params,
-                help=doc.command_help(name),
-                epilog=None,
-                short_help=None,
-                options_metavar="[OPTIONS]",
-                add_help_option=True,
-                no_args_is_help=True,
-                hidden=False,
-                deprecated=False,
-            )
+            command = as_click_command(command_config)
             self.commands.append(command)
-            Pipeline.COMMANDS[name] = command
-            self.template_configs[name] = doc.template_config
+            Pipeline.COMMANDS[command_config.name] = command
+            self.template_configs[command_config.name] = (
+                command_config.documentation.template_config
+            )
         return self
 
     def add_pipeline_command(self):
         """Add pipeline command, which includes the previous commands."""
         tpc = template_pipeline_config(self.command_configs)
         pipeline = pipeline_command(tpc)
         self.commands = [pipeline] + self.commands
@@ -118,14 +93,60 @@
             .add_batch_command()
             .add_status_command()
             .add_template_command()
             .commands
         )
 
 
+def as_click_command(command_config):
+    """Convert a GAPs command configuration object into a ``click`` command.
+
+    Parameters
+    ----------
+    command_config : command configuration object
+        Instance of a class that inherits from
+        :class:`~gaps.cli.command.AbstractBaseCLICommandConfiguration`
+        (i.e. :class:`gaps.cli.command.CLICommandFromClass`,
+        :class:`gaps.cli.command.CLICommandFromFunction`, etc.).
+
+    Returns
+    -------
+    click.command
+        A ``click`` command generated from the command configuration.
+    """
+    doc = command_config.documentation
+    name = command_config.name
+    params = [
+        click.Option(
+            param_decls=["--config_file", "-c"],
+            required=True,
+            type=click.Path(exists=True),
+            help=doc.config_help(name),
+        )
+    ]
+
+    return _WrappedCommand(
+        name,
+        context_settings=None,
+        callback=partial(
+            from_config,
+            command_config=command_config,
+        ),
+        params=params,
+        help=doc.command_help(name),
+        epilog=None,
+        short_help=None,
+        options_metavar="[OPTIONS]",
+        add_help_option=True,
+        no_args_is_help=True,
+        hidden=False,
+        deprecated=False,
+    )
+
+
 def make_cli(commands, info=None):
     """Create a pipeline CLI to split execution across HPC nodes.
 
     This function generates a CLI for a package based on the input
     command configurations. Each command configuration is based around
     a function that is to be executed on one or more nodes.
```

### Comparing `NREL-gaps-0.3.2/gaps/cli/collect.py` & `NREL-gaps-0.3.3/gaps/cli/collect.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/command.py` & `NREL-gaps-0.3.3/gaps/cli/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,17 +220,17 @@
             Optional function for configuration pre-processing. The
             preprocessing step occurs before jobs are split across HPC
             nodes, and can therefore be used to calculate the
             ``split_keys`` input and/or validate that it conforms to the
             requirements layed out above. At minimum, this function
             should have "config" as the first parameter (which will
             receive the user configuration input as a dictionary) and
-            must return the updated config dictionary. This function can
-            also "request" the following arguments by including them in
-            the function signature:
+            *must* return the updated config dictionary. This function
+            can also "request" the following arguments by including them
+            in the function signature:
 
                 command_name : str
                     Name of the command being run. This is equivalent to
                     the ``name`` input above.
                 config_file : Path
                     Path to the configuration file specified by the
                     user.
@@ -468,17 +468,17 @@
             Optional function for configuration pre-processing. The
             preprocessing step occurs before jobs are split across HPC
             nodes, and can therefore be used to calculate the
             ``split_keys`` input and/or validate that it conforms to the
             requirements layed out above. At minimum, this function
             should have "config" as the first parameter (which will
             receive the user configuration input as a dictionary) and
-            must return the updated config dictionary. This function can
-            also "request" the following arguments by including them in
-            the function signature:
+            *must* return the updated config dictionary. This function
+            can also "request" the following arguments by including them
+            in the function signature:
 
                 command_name : str
                     Name of the command being run. This is equivalent to
                     the ``name`` input above.
                 config_file : Path
                     Path to the configuration file specified by the
                     user.
```

### Comparing `NREL-gaps-0.3.2/gaps/cli/config.py` & `NREL-gaps-0.3.3/gaps/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     def enable_logging(self):
         """Enable logging based on config file input."""
         self.log_directory = self.config.pop(
             "log_directory", (self.project_dir / "logs").as_posix()
         )
         self.verbose = (
             self.config.pop("log_level", "INFO") == "DEBUG"
-            or self.ctx.obj["VERBOSE"]
+            or self.ctx.obj.get("VERBOSE", False)
         )
         pipe_log_file = Path(self.log_directory) / f"{self.job_name}.log"
         init_logger(
             stream=self.ctx.obj.get("LOG_STREAM", True),
             level="DEBUG" if self.verbose else "INFO",
             file=pipe_log_file.as_posix(),
         )
```

### Comparing `NREL-gaps-0.3.2/gaps/cli/documentation.py` & `NREL-gaps-0.3.3/gaps/cli/documentation.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/execution.py` & `NREL-gaps-0.3.3/gaps/cli/execution.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/pipeline.py` & `NREL-gaps-0.3.3/gaps/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/preprocessing.py` & `NREL-gaps-0.3.3/gaps/cli/preprocessing.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/status.py` & `NREL-gaps-0.3.3/gaps/cli/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/cli/templates.py` & `NREL-gaps-0.3.3/gaps/cli/templates.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/collection.py` & `NREL-gaps-0.3.3/gaps/collection.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/config.py` & `NREL-gaps-0.3.3/gaps/config.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/exceptions.py` & `NREL-gaps-0.3.3/gaps/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/hpc.py` & `NREL-gaps-0.3.3/gaps/hpc.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/legacy.py` & `NREL-gaps-0.3.3/gaps/legacy.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/log.py` & `NREL-gaps-0.3.3/gaps/log.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/pipeline.py` & `NREL-gaps-0.3.3/gaps/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/project_points.py` & `NREL-gaps-0.3.3/gaps/project_points.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/status.py` & `NREL-gaps-0.3.3/gaps/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/utilities.py` & `NREL-gaps-0.3.3/gaps/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/gaps/warnings.py` & `NREL-gaps-0.3.3/gaps/warnings.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.2/setup.py` & `NREL-gaps-0.3.3/setup.py`

 * *Files identical despite different names*

