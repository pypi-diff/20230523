# Comparing `tmp/task_assembly-0.1.8.tar.gz` & `tmp/task_assembly-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task_assembly-0.1.8.tar", max compression
+gzip compressed data, was "task_assembly-0.1.9.tar", max compression
```

## Comparing `task_assembly-0.1.8.tar` & `task_assembly-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1091 2022-10-31 16:16:04.454586 task_assembly-0.1.8/LICENSE
--rw-r--r--   0        0        0      560 2023-01-10 20:18:00.315730 task_assembly-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      105 2022-10-31 16:17:24.413127 task_assembly-0.1.8/README.md
--rw-r--r--   0        0        0       35 2023-01-07 00:50:03.343615 task_assembly-0.1.8/task_assembly/__init__.py
--rw-r--r--   0        0        0       30 2023-01-07 00:49:39.482793 task_assembly-0.1.8/task_assembly/__main__.py
--rw-r--r--   0        0        0    18670 2023-01-10 20:06:16.732263 task_assembly-0.1.8/task_assembly/cli.py
--rw-r--r--   0        0        0    13233 2023-01-10 00:37:41.756936 task_assembly-0.1.8/task_assembly/client.py
--rw-r--r--   0        0        0     1341 2022-04-11 22:04:25.144000 task_assembly-0.1.8/task_assembly/handlers.py
--rw-r--r--   0        0        0     2956 2023-01-07 00:47:31.619743 task_assembly-0.1.8/task_assembly/utils.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 task_assembly-0.1.8/setup.py
--rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 task_assembly-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-10-31 16:16:04.454586 task_assembly-0.1.9/LICENSE
+-rw-r--r--   0        0        0      578 2023-02-12 05:35:46.979033 task_assembly-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      105 2022-10-31 16:17:24.413127 task_assembly-0.1.9/README.md
+-rw-r--r--   0        0        0       35 2023-01-07 00:50:03.343615 task_assembly-0.1.9/task_assembly/__init__.py
+-rw-r--r--   0        0        0       30 2023-01-07 00:49:39.482793 task_assembly-0.1.9/task_assembly/__main__.py
+-rw-r--r--   0        0        0    20703 2023-02-12 02:11:32.809912 task_assembly-0.1.9/task_assembly/cli.py
+-rw-r--r--   0        0        0    12408 2023-02-11 17:10:29.745961 task_assembly-0.1.9/task_assembly/client.py
+-rw-r--r--   0        0        0     1341 2022-04-11 22:04:25.144000 task_assembly-0.1.9/task_assembly/handlers.py
+-rw-r--r--   0        0        0     3012 2023-02-11 17:07:41.644956 task_assembly-0.1.9/task_assembly/utils.py
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 task_assembly-0.1.9/setup.py
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 task_assembly-0.1.9/PKG-INFO
```

### Comparing `task_assembly-0.1.8/LICENSE` & `task_assembly-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `task_assembly-0.1.8/pyproject.toml` & `task_assembly-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task-assembly"
-version = "0.1.8"
+version = "0.1.9"
 description = "SDK and CLI for using the Task Assembly crowdwork service"
 authors = ["Dave Schultz <dave@daveschultzconsulting.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "task_assembly"}]
 
 [tool.poetry.scripts]
@@ -12,11 +12,12 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 api-client = "^1.3.1"
 larry = "^0.2.12"
 boto3 = "^1.26.0"
 tabulate = "^0.9.0"
+toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `task_assembly-0.1.8/task_assembly/cli.py` & `task_assembly-0.1.9/task_assembly/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import os.path
 import posixpath
+from pathlib import Path
 from datetime import datetime
 
 import larry as lry
 import argparse
+import toml
 import csv
 
 from botocore.exceptions import ClientError
 from tabulate import tabulate
 
 from .client import AssemblyClient
 from .utils import REV_TASK_DEFINITION_ARG_MAP
@@ -59,18 +61,20 @@
             definition.pop("GoldAnswers")
         if definition_file:
             with open(definition_file, "w") as fp:
                 json.dump(definition, fp, indent=4)
         else:
             print(json.dumps(definition, indent=4))
 
-    def create_task(self, definition_file, assignments, sandbox, values, max_assignments, quals):
+    def create_task(self, definition_file, assignments, sandbox, values, max_assignments, quals,
+                    use_computed_result=False):
         definition = self.read_definition(definition_file)
         params = {
-            "definition_id": definition["DefinitionId"]
+            "definition_id": definition["DefinitionId"],
+            "use_computed_result": use_computed_result
         }
         if assignments:
             params["default_assignments"] = assignments
         if max_assignments:
             params["max_assignments"] = max_assignments
         if sandbox:
             params["sandbox"] = True
@@ -313,18 +317,21 @@
         fieldnames = dict.fromkeys(results[0].keys())
         for result in results:
             fieldnames.update(dict.fromkeys(result.keys()))
         return list(fieldnames.keys())
 
 def main():
     parser = argparse.ArgumentParser("Task Assembly CLI")
+    parser.add_argument("--profile")
     subparsers = parser.add_subparsers(dest="command", required=True)
 
     c_parser = subparsers.add_parser("configure")
     c_parser.add_argument("--key")
+    c_parser.add_argument("--key_secret")
+    c_parser.add_argument("--aws_profile")
     c_parser.add_argument("--validate", action="store_true")
 
     ctt_parser = subparsers.add_parser("create_task_type")
     ctt_parser.add_argument("name")
     ctt_parser.set_defaults(func=CLI.create_task_type)
 
     ctd_parser = subparsers.add_parser("create_task_definition")
@@ -344,14 +351,15 @@
     ct_parser = subparsers.add_parser("create_task")
     ct_parser.add_argument("values", type=str, nargs="*")
     ct_parser.add_argument("--assignments", type=int)
     ct_parser.add_argument("--sandbox", action="store_true")
     ct_parser.add_argument("--definition_file", default="definition.json")
     ct_parser.add_argument("--max_assignments", type=int)
     ct_parser.add_argument("--quals", type=str)
+    ct_parser.add_argument("--use_computed_result", action="store_true")
     ct_parser.set_defaults(func=CLI.create_task)
 
     gt_parser = subparsers.add_parser("get_task")
     gt_parser.add_argument("task_id")
     gt_parser.add_argument("--include_assignments", action="store_true")
     gt_parser.set_defaults(func=CLI.get_task)
 
@@ -409,27 +417,72 @@
     rsb_parser = subparsers.add_parser("resolve_batch")
     rsb_parser.add_argument("batch_id")
     rsb_parser.add_argument("--extend", action="store_true")
     rsb_parser.set_defaults(func=CLI.resolve_batch)
 
     args = parser.parse_args()
 
-    if args.command == "configure" and args.key:
-        with open("api-key.txt", "w") as fp:
-            fp.write(args.key)
+    ta_dir = Path.home().joinpath(".taskassembly")
+    ta_config = ta_dir.joinpath("config.toml")
+    profile = args.profile if args.profile else "default"
+
+    if args.command == "configure" and (args.key or args.key_secret or args.aws_profile):
+        ta_dir.mkdir(exist_ok=True)
+        config = {"version": "0.1"}
+        if ta_config.exists():
+            with open(ta_config) as fp:
+                config = toml.load(fp)
+        if profile not in config:
+            config[profile] = {}
+        pf = config[profile]
+        if "credentials" not in pf:
+            pf["credentials"] = {}
+        creds = pf["credentials"]
+        if args.key:
+            creds["api_key"] = args.key
+        if args.key_secret:
+            creds["api_key_secret"] = args.key_secret
+        if args.aws_profile:
+            creds["aws_profile"] = args.aws_profile
+        with open(ta_config, "w") as fp:
+            toml.dump(config, fp)
         if not args.validate:
             exit(0)
 
-    if not os.path.exists("api-key.txt"):
-        print("No api-key.txt file found. Please run the configure command first.")
+    if not ta_config.exists():
+        print("No configuration file found. Please run the 'configure' command first.")
+        exit(1)
+
+    with open(ta_config) as fp:
+        config = toml.load(fp)
+        profile_config = config.get(profile)
+    if not profile_config:
+        print(f"No configuration found for {profile} profile")
+        exit(1)
+    profile_credentials = profile_config["credentials"]
+    if profile_credentials.get("aws_profile"):
+        lry.set_session(profile_name=profile_credentials.get("aws_profile"))
+    api_key = None
+    if "api_key" in profile_credentials:
+        api_key = profile_credentials.get("api_key")
+    elif "api_key_secret" in profile_credentials:
+        sm = lry.session().client('secretsmanager')
+        response = sm.get_secret_value(SecretId=profile_credentials["api_key_secret"])
+        secret_value = response["SecretString"]
+        try:
+            secrets = json.loads(secret_value)
+            api_key = secrets["api_key"]
+        except:
+            api_key = secret_value
+
+    if api_key is None:
+        print("Missing api key value")
         exit(1)
 
-    with open("api-key.txt") as fp:
-        api_key = fp.read().strip()
-        client = AssemblyClient(api_key)
+    client = AssemblyClient(api_key)
     cli = CLI(client)
 
     if args.command == "configure" and args.validate:
         response = client.validate()
         print(f"Organization: {response['Organization']['Name']}")
         print(f"AWS Account: {response['AWSAccountId']}")
         print(f"MTurk connection status: {'SUCCESS' if response.get('MTurk') else 'FAILED'}")
```

### Comparing `task_assembly-0.1.8/task_assembly/client.py` & `task_assembly-0.1.9/task_assembly/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,43 +70,23 @@
             keywords=None,
             qualification_requirements=None,
             render_handler=None,
             submission_handlers=None,
             consolidation_handlers=None,
             callback_handlers=None,
             scoring_handler=None,
+            computed_result_handler=None,
             gold_answers=None,
             test_policy=None,
     ):
         url = self.ENDPOINT + "/taskDefinition/create"
         params = self._map_parameters(
             locals(),
             self.create_task_definition.actual_kwargs,
-            {
-                "name": "Name",
-                "task_type_id": "TaskType",
-                "template": "Template",
-                "title": "Title",
-                "description": "Description",
-                "reward_cents": "RewardCents",
-                "lifetime": "Lifetime",
-                "assignment_duration": "AssignmentDuration",
-                "default_assignments": "DefaultAssignments",
-                "max_assignments": "MaxAssignments",
-                "auto_approval_delay": "AutoApprovalDelay",
-                "keywords": "Keywords",
-                "qualification_requirements": "QualificationRequirements",
-                "render_handler": "RenderHandler",
-                "submission_handlers": "SubmissionHandlers",
-                "consolidation_handlers": "ConsolidationHandlers",
-                "scoring_handler": "ScoringHandler",
-                "callback_handlers": "CallbackHandlers",
-                "gold_answers": "GoldAnswers",
-                "test_policy": "TestPolicy",
-            },
+            TASK_DEFINITION_ARG_MAP
         )
         if isinstance(params.get("Template"), io.IOBase):
             params["Template"] = params["Template"].read()
         return self.post(url, data=params)
 
     @_arg_decorator
     def update_task_definition(
@@ -126,14 +106,15 @@
             qualification_requirements=None,
             load_handler=None,
             render_handler=None,
             submission_handlers=None,
             consolidation_handlers=None,
             callback_handlers=None,
             scoring_handler=None,
+            computed_result_handler=None,
             gold_answers=None,
             test_policy=None,
             result_layout=None,
             handler_code=None
     ):
         url = self.ENDPOINT + "/taskDefinition/update"
         params = self._map_parameters(
@@ -164,28 +145,30 @@
             self,
             definition_id,
             data,
             sandbox=False,
             default_assignments=None,
             max_assignments=None,
             sfn_token=None,
-            qualification_requirements=None
+            qualification_requirements=None,
+            use_computed_result=None
     ):
         url = self.ENDPOINT + "/task/create"
         params = self._map_parameters(
             locals(),
             self.create_task.actual_kwargs,
             {
                 "definition_id": "DefinitionId",
                 "data": "Data",
                 "sandbox": "Sandbox",
                 "default_assignments": "DefaultAssignments",
                 "max_assignments": "MaxAssignments",
                 "sfn_token": "SFNToken",
-                "qualification_requirements": "QualificationRequirements"
+                "qualification_requirements": "QualificationRequirements",
+                "use_computed_result": "UseComputedResult"
             },
         )
         return self.post(url, data=params)["TaskId"]
 
     @_arg_decorator
     def render_task(self, definition_id, data):
         url = self.ENDPOINT + "/task/render"
```

### Comparing `task_assembly-0.1.8/task_assembly/handlers.py` & `task_assembly-0.1.9/task_assembly/handlers.py`

 * *Files identical despite different names*

### Comparing `task_assembly-0.1.8/task_assembly/utils.py` & `task_assembly-0.1.9/task_assembly/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "qualification_requirements": "QualificationRequirements",
     "load_handler": "LoadHandler",
     "render_handler": "RenderHandler",
     "submission_handlers": "SubmissionHandlers",
     "consolidation_handlers": "ConsolidationHandlers",
     "scoring_handler": "ScoringHandler",
     "callback_handlers": "CallbackHandlers",
+    "computed_result_handler": "ComputedResultHandler",
     "handler_code": "HandlerCode",
     "gold_answers": "GoldAnswers",
     "test_policy": "TestPolicy",
     "result_layout": "ResultLayout"
 }
 REV_TASK_DEFINITION_ARG_MAP = {v: k for k, v in TASK_DEFINITION_ARG_MAP.items()}
```

### Comparing `task_assembly-0.1.8/setup.py` & `task_assembly-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['api-client>=1.3.1,<2.0.0',
  'boto3>=1.26.0,<2.0.0',
  'larry>=0.2.12,<0.3.0',
- 'tabulate>=0.9.0,<0.10.0']
+ 'tabulate>=0.9.0,<0.10.0',
+ 'toml>=0.10.2,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['task-assembly = task_assembly.cli:main']}
 
 setup_kwargs = {
     'name': 'task-assembly',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'SDK and CLI for using the Task Assembly crowdwork service',
     'long_description': '# Task Assembly Client\nTools for working with the Task Assembly service for managing crowdwork projects.\n',
     'author': 'Dave Schultz',
     'author_email': 'dave@daveschultzconsulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `task_assembly-0.1.8/PKG-INFO` & `task_assembly-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task-assembly
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK and CLI for using the Task Assembly crowdwork service
 License: MIT
 Author: Dave Schultz
 Author-email: dave@daveschultzconsulting.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,12 +12,13 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: api-client (>=1.3.1,<2.0.0)
 Requires-Dist: boto3 (>=1.26.0,<2.0.0)
 Requires-Dist: larry (>=0.2.12,<0.3.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Task Assembly Client
 Tools for working with the Task Assembly service for managing crowdwork projects.
```

