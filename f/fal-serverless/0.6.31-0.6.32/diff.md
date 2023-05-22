# Comparing `tmp/fal_serverless-0.6.31.tar.gz` & `tmp/fal_serverless-0.6.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.31.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.32.tar", max compression
```

## Comparing `fal_serverless-0.6.31.tar` & `fal_serverless-0.6.32.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      213 2023-05-08 12:43:58.060579 fal_serverless-0.6.31/README.md
--rw-r--r--   0        0        0      998 2023-05-08 12:44:13.456756 fal_serverless-0.6.31/pyproject.toml
--rw-r--r--   0        0        0      335 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    17406 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2532 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    12772 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      172 2023-05-08 12:44:07.892691 fal_serverless-0.6.31/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     2122 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    15210 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     5335 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 fal_serverless-0.6.31/setup.py
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 fal_serverless-0.6.31/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/README.md
+-rw-r--r--   0        0        0      997 2023-05-22 22:27:48.446837 fal_serverless-0.6.32/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    17062 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2532 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    15093 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      158 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    15875 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     5335 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 fal_serverless-0.6.32/setup.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 fal_serverless-0.6.32/PKG-INFO
```

### Comparing `fal_serverless-0.6.31/pyproject.toml` & `fal_serverless-0.6.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.31"
+version = "0.6.32"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
 isolate = {version = "0.12.0", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = "0.3.5.1"
-isolate-proto = "^0.0.27"
+isolate-proto = "0.0.28"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "^2.9.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
```

### Comparing `fal_serverless-0.6.31/src/fal_serverless/api.py` & `fal_serverless-0.6.32/src/fal_serverless/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import inspect
 import os
-import time
 from collections import defaultdict
 from concurrent.futures import Future, ThreadPoolExecutor
 from dataclasses import dataclass, field, replace
 from functools import partial, wraps
 from typing import Any, Callable, ClassVar, Dict, Generic, Iterator, TypeVar, cast
 
 import dill
@@ -186,54 +185,45 @@
 def _handle_grpc_error():
     def decorator(fn):
         @wraps(fn)
         def handler(*args, **kwargs):
             """
             Wraps grpc errors as fal Serverless Errors.
             """
-            max_retries = 3
-            max_wait_time = 1
-            for i in range(max_retries):
-                try:
-                    return fn(*args, **kwargs)
-                except grpc.RpcError as e:
-                    if e.code() == grpc.StatusCode.UNAVAILABLE:
-                        print("Could not reach fal Serverless host. Trying again.")
-                        time.sleep(max_wait_time)
-
-                        # Reached max retries
-                        if i + 1 == max_retries:
-                            raise FalServerlessError(
-                                "Could not reach fal Serverless host. "
-                                "This is most likely a transient problem. "
-                                "Please, try again."
-                            )
-                    elif e.details().endswith("died with <Signals.SIGKILL: 9>.`."):
-                        raise FalServerlessError(
-                            "Isolated function crashed. "
-                            "This is likely due to resource overflow. "
-                            "You can try again by setting a bigger `machine_type`"
-                        )
-
-                    elif e.code() == grpc.StatusCode.INVALID_ARGUMENT and (
-                        "The function function could not be deserialized" in e.details()
-                    ):
-                        raise FalMissingDependencyError(e.details())
-                    else:
-                        raise FalServerlessError(e.details())
+            try:
+                return fn(*args, **kwargs)
+            except grpc.RpcError as e:
+                if e.code() == grpc.StatusCode.UNAVAILABLE:
+                    raise FalServerlessError(
+                        "Could not reach fal Serverless host. "
+                        "This is most likely a transient problem. "
+                        "Please, try again."
+                    )
+                elif e.details().endswith("died with <Signals.SIGKILL: 9>.`."):
+                    raise FalServerlessError(
+                        "Isolated function crashed. "
+                        "This is likely due to resource overflow. "
+                        "You can try again by setting a bigger `machine_type`"
+                    )
+
+                elif e.code() == grpc.StatusCode.INVALID_ARGUMENT and (
+                    "The function function could not be deserialized" in e.details()
+                ):
+                    raise FalMissingDependencyError(e.details())
+                else:
+                    raise FalServerlessError(e.details())
 
         return handler
 
     return decorator
 
 
 def find_missing_dependencies(
     func: Callable[..., Any], env: dict
 ) -> Iterator[tuple[str, list[str]]]:
-
     if env["kind"] != "virtualenv":
         return
 
     used_modules = defaultdict(list)
     scope = {**dill.detect.globalvars(func, recurse=True), **dill.detect.freevars(func)}  # type: ignore
 
     for name, obj in scope.items():
@@ -285,14 +275,15 @@
 
     @_handle_grpc_error()
     def register(
         self,
         func: Callable[..., ReturnT],
         options: Options,
         application_name: str | None = None,
+        application_is_public: bool = False,
     ) -> str | None:
         environment_options = options.environment.copy()
         environment_options.setdefault("python_version", active_python())
         environments = [self._connection.define_environment(**environment_options)]
 
         machine_type = options.host.get(
             "machine_type", FAL_SERVERLESS_DEFAULT_MACHINE_TYPE
@@ -305,14 +296,15 @@
 
         partial_func = _execution_controller(func, tuple(), {})
 
         for partial_result in self._connection.register(
             partial_func,
             environments,
             application_name=application_name,
+            application_is_public=application_is_public,
             machine_requirements=machine_requirements,
         ):
             for log in partial_result.logs:
                 self._log_printer.print(log)
 
             if partial_result.result:
                 return partial_result.result.application_id
```

### Comparing `fal_serverless-0.6.31/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.32/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.32/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.32/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/cli.py` & `fal_serverless-0.6.32/src/fal_serverless/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import datetime
 import operator
 from sys import argv
+from typing import Literal
 from uuid import uuid4
 
 import click
 import fal_serverless.auth as auth
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
@@ -73,26 +74,67 @@
                     console.print()
                     console.print(
                         f"The [markdown.code]invocation_id[/] for this operation is: [white]{invocation_id}[/]"
                     )
                 else:
                     self._exception_handler.handle(exception)
 
+    def add_command(
+        self,
+        cmd: click.Command,
+        name: str | None = None,
+        aliases: list[str] | None = None,
+    ) -> None:
+        name = name or cmd.name
+        assert name, "Command must have a name"
+
+        if not aliases:
+            aliases = []
+
+        if aliases:
+            # Add aliases to the help text
+            aliases_str = "Alias: " + ", ".join([name, *aliases])
+            cmd.help = (cmd.help or "") + "\n\nAlias: " + ", ".join([name, *aliases])
+            cmd.short_help = (
+                (cmd.short_help or "") + "(Alias: " + ", ".join(aliases) + ")"
+            )
+
+        super().add_command(cmd, name)
+        alias_cmd = AliasCommand(cmd)
+
+        for alias in aliases:
+            self.add_command(alias_cmd, alias)
+
+
+class AliasCommand(click.Command):
+    def __init__(self, wrapped):
+        self._wrapped = wrapped
+
+    def __getattribute__(self, __name: str):
+        if __name == "_wrapped":
+            # To be able to call `self._wrapped` below
+            return super().__getattribute__(__name)
+
+        if __name == "hidden":
+            return True
+
+        return self._wrapped.__getattribute__(__name)
+
 
 @click.group(cls=MainGroup)
 @click.option(
     "--debug", is_flag=True, help="Enable detailed errors and verbose logging."
 )
 @click.version_option()
 def cli(debug):
     pass
 
 
 ###### Auth group ######
-@cli.group("auth")
+@click.group
 def auth_cli():
     pass
 
 
 @auth_cli.command(name="login")
 def auth_login():
     auth.login()
@@ -113,15 +155,15 @@
     """
     To test auth.
     """
     print(f"Hello, {auth.USER.info['name']} - '{auth.USER.info['sub']}'")
 
 
 ###### Key group ######
-@cli.group("key")
+@click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def key_cli(ctx, host: str, port: str):
     ctx.obj = sdk.FalServerlessClient(f"{host}:{port}")
 
 
@@ -157,15 +199,15 @@
 @click.pass_obj
 def key_revoke(client: sdk.FalServerlessClient, key_id: str):
     with client.connect() as connection:
         connection.revoke_user_key(key_id)
 
 
 ###### Usage group ######
-@cli.group("usage")
+@click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def usage_cli(ctx, host: str, port: str):
     ctx.obj = sdk.FalServerlessClient(f"{host}:{port}")
 
 
@@ -192,31 +234,39 @@
                 str(ws.duration),
             )
 
     console.print(table)
 
 
 ##### Function group #####
-@cli.group("function")
+@click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def function_cli(ctx, host: str, port: str):
     ctx.obj = api.FalServerlessHost(f"{host}:{port}")
 
 
 @function_cli.command("serve")
 @click.option("--alias", default=None)
+@click.option(
+    "--auth",
+    "auth_mode",
+    # TODO: handle shared auth mode
+    type=click.Choice(["public", "private"]),
+    default="private",
+)
 @click.argument("file_path", required=True)
 @click.argument("function_name", required=True)
 @click.pass_obj
 def register_application(
     host: api.FalServerlessHost,
     file_path: str,
     function_name: str,
+    auth_mode: Literal["public", "private"],
     alias: str | None = None,
 ):
     import runpy
 
     module = runpy.run_path(file_path)
     isolated_function = module[function_name]
     gateway_options = isolated_function.options.gateway
@@ -224,14 +274,15 @@
         raise api.FalServerlessError(
             "One of `serve` or `exposed-port` options needs to be specified in the isolated annotation to register a function"
         )
     id = host.register(
         func=isolated_function.func,
         options=isolated_function.options,
         application_name=alias,
+        application_is_public=auth_mode == "public",
     )
     if id:
         # TODO: should we centralize this URL format?
         gateway_host = host.url.replace("api.", "gateway.")
 
         # Encode since user_id can contain special characters
         user_id = auth.USER.info["sub"].split("|")[1]
@@ -247,120 +298,148 @@
 
 @function_cli.command("schedule")
 @click.argument("cron_string", required=True)
 @click.argument("file_path", required=True)
 @click.argument("function_name", required=True)
 @click.pass_obj
 def register_schedulded(
-    client: api.FalServerlessHost, cron_string: str, file_path: str, function_name: str
+    host: api.FalServerlessHost, cron_string: str, file_path: str, function_name: str
 ):
     import runpy
 
     module = runpy.run_path(file_path)
     isolated_function = module[function_name]
 
-    cron_id = client.schedule(
+    cron_id = host.schedule(
         func=isolated_function.func, cron=cron_string, options=isolated_function.options
     )
     if cron_id:
         console.print(cron_id)
 
 
 @function_cli.command("logs")
 @click.argument("url", required=True)
 @click.argument("call_id", required=True)
 @click.pass_obj
-def get_logs(client: api.FalServerlessHost, url: str, call_id: str):
+def get_logs(host: api.FalServerlessHost, url: str, call_id: str):
     logs = parse_logs(f"/data/logs/gateway/{url}/{call_id}")
     log_printer = IsolateLogPrinter(debug=True)
     for log in logs:
         log_printer.print_dict(log)
 
 
 @function_cli.command("calls")
 @click.argument("url", required=True)
 @click.pass_obj
-def get_function_call_ids(client: api.FalServerlessHost, url: str):
+def get_function_call_ids(host: api.FalServerlessHost, url: str):
     # This will only return a list calls that we have logs for.
     calls = list_children(f"/data/logs/gateway/{url}")
     calls.sort(key=operator.itemgetter("updated_time"))
     for call in calls:
         name = call["name"].split(".")[0]
         timestamp = datetime.datetime.fromtimestamp(call["updated_time"])
         timestamp_str = timestamp.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
         console.print(f"{timestamp_str}: {name}")
 
 
+##### Alias group #####
+@click.group
+@click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
+@click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
+@click.pass_context
+def alias_cli(ctx, host: str, port: str):
+    ctx.obj = api.FalServerlessClient(f"{host}:{port}")
+
+
+@alias_cli.command("list")
+@click.pass_obj
+def alias_list(client: api.FalServerlessClient):
+    with client.connect() as connection:
+        table = Table(title="Function Aliases")
+        table.add_column("Alias")
+        table.add_column("Revision")
+        table.add_column("Auth")
+
+        for app_alias in connection.list_aliases():
+            table.add_row(
+                app_alias.alias,
+                app_alias.revision,
+                "public" if app_alias.public else "private",
+            )
+
+    console.print(table)
+
+
 ##### Crons group #####
-@cli.group("crons")
+@click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def crons_cli(ctx, host: str, port: str):
     ctx.obj = api.FalServerlessHost(f"{host}:{port}")
 
 
 @crons_cli.command(name="list")
 @click.pass_obj
-def list_scheduled(client: api.FalServerlessHost):
+def list_scheduled(host: api.FalServerlessHost):
     table = Table(title="Cronjobs")
     table.add_column("Cron ID")
     table.add_column("Cron")
     table.add_column("ETA next run")
     table.add_column("State")
-    for cron in client._connection.list_scheduled_runs():
+    for cron in host._connection.list_scheduled_runs():
         state_string = ["Not Active", "Active"][cron.active]
         table.add_row(cron.cron_id, cron.cron_string, str(cron.next_run), state_string)
 
     console.print(table)
 
 
 @crons_cli.command(name="activations")
 @click.argument("cron_id", required=True)
 @click.argument("limit", default=15)
 @click.pass_obj
-def list_activations(client: api.FalServerlessHost, cron_id: str, limit: int = 15):
+def list_activations(host: api.FalServerlessHost, cron_id: str, limit: int = 15):
     table = Table(title="Cron activations")
     table.add_column("Activation ID")
     table.add_column("Start Date")
     table.add_column("Finish Date")
 
-    for activation in client._connection.list_run_activations(cron_id)[:limit]:
+    for activation in host._connection.list_run_activations(cron_id)[:limit]:
         table.add_row(
             str(activation.activation_id),
             str(activation.started_at),
             str(activation.finished_at),
         )
 
     console.print(table)
 
 
 @crons_cli.command(name="logs")
 @click.argument("cron_id", required=True)
 @click.argument("activation_id", required=True)
 @click.pass_obj
-def print_logs(client: api.FalServerlessHost, cron_id: str, activation_id: str):
-    logs = client._connection.get_activation_logs(cron_id, activation_id)
+def print_logs(host: api.FalServerlessHost, cron_id: str, activation_id: str):
+    logs = host._connection.get_activation_logs(cron_id, activation_id)
     if not logs:
         console.print(f"No logs found for activation {activation_id}")
         return
     log_printer = IsolateLogPrinter(debug=True)
     for log in logs:
         log_printer.print(log)
 
 
 @crons_cli.command("cancel")
 @click.argument("cron_id", required=True)
 @click.pass_obj
-def cancel_scheduled(client: api.FalServerlessHost, cron_id: str):
-    client._connection.cancel_scheduled_run(cron_id)
+def cancel_scheduled(host: api.FalServerlessHost, cron_id: str):
+    host._connection.cancel_scheduled_run(cron_id)
     console.print("Cancelled", repr(cron_id))
 
 
-@cli.group("secrets")
+@click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def secrets_cli(ctx, host: str, port: str):
     ctx.obj = sdk.FalServerlessClient(f"{host}:{port}")
 
 
@@ -394,15 +473,16 @@
 def delete_secret(client: api.FalServerlessClient, secret_name: str):
     with client.connect() as connection:
         connection.delete_secret(secret_name)
         console.print(f"Secret '{secret_name}' has deleted")
 
 
 cli.add_command(auth_cli, name="auth")
-cli.add_command(key_cli, name="key")
-cli.add_command(function_cli, name="function")
-cli.add_command(crons_cli, name="crons")
+cli.add_command(key_cli, name="key", aliases=["keys"])
+cli.add_command(function_cli, name="function", aliases=["fn"])
+cli.add_command(alias_cli, name="alias")
+cli.add_command(crons_cli, name="cron", aliases=["crons"])
 cli.add_command(usage_cli, name="usage")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `fal_serverless-0.6.31/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.32/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.32/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.32/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.32/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.32/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.32/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.32/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/src/fal_serverless/sdk.py` & `fal_serverless-0.6.32/src/fal_serverless/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,14 +156,21 @@
 
 
 @dataclass
 class HostedRunStatus:
     state: HostedRunState
 
 
+@dataclass
+class AliasInfo:
+    alias: str
+    revision: str
+    public: bool
+
+
 @dataclass(frozen=True)
 class Cron:
     cron_id: str
     cron_string: str
     next_run: datetime
     active: bool
 
@@ -238,14 +245,23 @@
         cron_id=message.cron_id,
         cron_string=message.cron_string,
         next_run=message.next_run.ToDatetime(),
         active=message.is_active,
     )
 
 
+@from_grpc.register(isolate_proto.AliasInfo)
+def _from_grpc_alias_info(message: isolate_proto.AliasInfo) -> AliasInfo:
+    return AliasInfo(
+        alias=message.alias,
+        revision=message.revision,
+        public=message.is_public,
+    )
+
+
 @from_grpc.register(isolate_proto.RegisterApplicationResult)
 def _from_grpc_register_application_result(
     message: isolate_proto.RegisterApplicationResult,
 ) -> RegisterApplicationResult:
     return RegisterApplicationResult(
         logs=[from_grpc(log) for log in message.logs],
         result=None
@@ -368,14 +384,15 @@
         )
 
     def register(
         self,
         function: Callable[..., ResultT],
         environments: list[isolate_proto.EnvironmentDefinition],
         application_name: str | None = None,
+        application_is_public: bool = False,
         *,
         serialization_method: str = _DEFAULT_SERIALIZATION_METHOD,
         machine_requirements: MachineRequirements | None = None,
     ) -> Iterator[isolate_proto.RegisterApplicationResult]:
         wrapped_function = to_serialized_object(function, serialization_method)
         if machine_requirements:
             wrapped_requirements = isolate_proto.MachineRequirements(
@@ -386,14 +403,15 @@
             wrapped_requirements = None
 
         request = isolate_proto.RegisterApplicationRequest(
             function=wrapped_function,
             environments=environments,
             machine_requirements=wrapped_requirements,
             application_name=application_name,
+            is_public=application_is_public,
         )
         for partial_result in self.stub.RegisterApplication(request):
             yield from_grpc(partial_result)
 
     def run(
         self,
         function: Callable[..., ResultT],
@@ -433,14 +451,19 @@
             application_id=application_id, cron=cron
         )
         response: isolate_proto.RegisterApplicationResultType = self.stub.RegisterCron(
             request
         )
         return response
 
+    def list_aliases(self) -> list[AliasInfo]:
+        request = isolate_proto.ListAliasesRequest()
+        response: isolate_proto.ListAliasesResult = self.stub.ListAliases(request)
+        return [from_grpc(alias) for alias in response.aliases]
+
     def list_scheduled_runs(self) -> list[Cron]:
         request = isolate_proto.ListCronsRequest()
         response: isolate_proto.ListCronsResult = self.stub.ListCrons(request)
         return [from_grpc(cron) for cron in response.crons]
 
     def list_run_activations(self, run: str | Cron) -> list[ScheduledRunActivation]:
         request = isolate_proto.ListActivationsRequest(cron_id=_get_cron_id(run))
```

### Comparing `fal_serverless-0.6.31/src/fal_serverless/sync.py` & `fal_serverless-0.6.32/src/fal_serverless/sync.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.31/setup.py` & `fal_serverless-0.6.32/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client>=2.9.0,<3.0.0',
  'dill==0.3.5.1',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto>=0.0.27,<0.0.28',
+ 'isolate-proto==0.0.28',
  'isolate[build]==0.12.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'packaging>=21.3',
  'pathspec>=0.11.1,<0.12.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
@@ -38,15 +38,15 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.31',
+    'version': '0.6.32',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '# fal-serverless\n\nLibrary to run, serve or schedule your Python functions in the cloud with any machine type you may need.\n\nCheck out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.31/PKG-INFO` & `fal_serverless-0.6.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.31
+Version: 0.6.32
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (>=2.9.0,<3.0.0)
 Requires-Dist: dill (==0.3.5.1)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (>=0.0.27,<0.0.28)
+Requires-Dist: isolate-proto (==0.0.28)
 Requires-Dist: isolate[build] (==0.12.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

