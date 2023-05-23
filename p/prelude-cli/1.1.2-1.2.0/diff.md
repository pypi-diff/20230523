# Comparing `tmp/prelude-cli-1.1.2.tar.gz` & `tmp/prelude-cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.1.2.tar", last modified: Tue May 16 20:32:48 2023, max compression
+gzip compressed data, was "prelude-cli-1.2.0.tar", last modified: Tue May 23 20:19:01 2023, max compression
```

## Comparing `prelude-cli-1.1.2.tar` & `prelude-cli-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:32:48.747558 prelude-cli-1.1.2/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.1.2/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.1.2/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-16 20:32:48.747625 prelude-cli-1.1.2/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.1.2/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:32:48.744818 prelude-cli-1.1.2/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.1.2/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.1.2/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.1.2/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:32:48.745690 prelude-cli-1.1.2/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.1.2/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      241 2023-05-04 16:11:50.000000 prelude-cli-1.1.2/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:32:48.747338 prelude-cli-1.1.2/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.1.2/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4956 2023-05-16 20:26:27.000000 prelude-cli-1.1.2/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.1.2/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     5021 2023-05-04 16:11:50.000000 prelude-cli-1.1.2/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3494 2023-05-12 13:56:19.000000 prelude-cli-1.1.2/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2246 2023-05-03 13:30:52.000000 prelude-cli-1.1.2/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.1.2/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:32:48.745458 prelude-cli-1.1.2/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-16 20:32:48.000000 prelude-cli-1.1.2/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-05-16 20:32:48.000000 prelude-cli-1.1.2/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-16 20:32:48.000000 prelude-cli-1.1.2/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-05-16 20:32:48.000000 prelude-cli-1.1.2/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-05-16 20:32:48.000000 prelude-cli-1.1.2/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-05-16 20:32:48.000000 prelude-cli-1.1.2/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.1.2/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-05-16 20:32:48.747856 prelude-cli-1.1.2/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.502207 prelude-cli-1.2.0/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 20:19:01.502254 prelude-cli-1.2.0/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.0/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.499610 prelude-cli-1.2.0/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.0/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.0/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.500500 prelude-cli-1.2.0/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      241 2023-05-04 16:11:50.000000 prelude-cli-1.2.0/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.501992 prelude-cli-1.2.0/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3241 2023-05-18 20:31:39.000000 prelude-cli-1.2.0/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.0/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     7272 2023-05-23 15:18:07.000000 prelude-cli-1.2.0/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3478 2023-05-18 20:31:39.000000 prelude-cli-1.2.0/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.0/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.0/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.500319 prelude-cli-1.2.0/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-05-23 20:19:01.502457 prelude-cli-1.2.0/setup.cfg
```

### Comparing `prelude-cli-1.1.2/LICENSE` & `prelude-cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.1.2/PKG-INFO` & `prelude-cli-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.1.2
+Version: 1.2.0
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.1.2/prelude_cli/cli.py` & `prelude-cli-1.2.0/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.1.2/prelude_cli/views/configure.py` & `prelude-cli-1.2.0/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.1.2/prelude_cli/views/detect.py` & `prelude-cli-1.2.0/prelude_cli/views/detect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import click
+import asyncio 
 
 from rich import print_json
+from pathlib import Path, PurePath
 from datetime import datetime, timedelta
 
 from prelude_sdk.models.codes import RunCode
 from prelude_cli.views.shared import handle_api_error, Spinner
+from prelude_sdk.controllers.iam_controller import IAMController
 from prelude_sdk.controllers.detect_controller import DetectController
 
 
 @click.group()
 @click.pass_context
 def detect(ctx):
     """ Continuous security testing """
@@ -22,28 +25,62 @@
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default='')
 @click.option('-i', '--endpoint_id', help='update a specific endpoint_id with the provided values', type=str, default='')
 @click.pass_obj
 @handle_api_error
 def register_endpoint(controller, host, serial_num, edr_id, tags, endpoint_id):
     """ Register a new endpoint """
     with Spinner():
-        token = controller.register_endpoint(host=host, serial_num=serial_num, edr_id=edr_id, tags=tags, endpoint_id=endpoint_id)
-    click.secho(token)
+        token = controller.register_endpoint(
+            host=host, 
+            serial_num=serial_num, 
+            edr_id=edr_id, 
+            tags=tags, 
+            endpoint_id=endpoint_id
+        )
+        click.secho(token)
 
 
 @detect.command('tests')
 @click.pass_obj
 @handle_api_error
 def list_tests(controller):
     """ List all security tests """
     with Spinner():
         data = controller.list_tests()
     print_json(data=data)
 
 
+@detect.command('test')
+@click.argument('test_id')
+@click.pass_obj
+@handle_api_error
+def get_test(controller, test_id):
+    """ List properties for a test """
+    with Spinner():
+        print_json(data=controller.get_test(test_id=test_id))
+
+
+@detect.command('download')
+@click.argument('test')
+@click.pass_obj
+@handle_api_error
+def download(controller, test):
+    """ Download a test to your local environment """
+    click.secho(f'Downloading {test}')
+    Path(test).mkdir(parents=True, exist_ok=True)
+    with Spinner():
+        attachments = controller.get_test(test_id=test).get('attachments')
+
+        for attach in attachments:
+            if Path(attach).suffix:
+                code = controller.download(test_id=test, filename=attach)
+                with open(PurePath(test, attach), 'wb') as f:
+                    f.write(code)
+
+
 @detect.command('enable-test')
 @click.argument('test')
 @click.option('-t', '--tags', help='only enable for these tags (comma-separated list)', type=str, default='')
 @click.option('-r', '--run_code',
               help='provide a run_code',
               default=RunCode.DAILY.name, show_default=True,
               type=click.Choice([r.name for r in RunCode], case_sensitive=False))
@@ -92,34 +129,69 @@
 
 @detect.command('queue')
 @click.pass_obj
 @handle_api_error
 def queue(controller):
     """ List all tests in your active queue """
     with Spinner():
-        data = controller.list_queue()
-    print_json(data=data)
+        iam = IAMController(account=controller.account)
+        queue = iam.get_account().get('queue')
+        print_json(data=queue)
 
 
 @detect.command('endpoints')
 @click.option('-d', '--days', help='only show endpoints that have run at least once in the past DAYS days', default=90, type=int)
 @click.pass_obj
 @handle_api_error
 def endpoints(controller, days):
     """ List all active endpoints associated to your account """
     with Spinner():
         data = controller.list_endpoints(days=days)
     print_json(data=data)
 
 
+@detect.command('advisories')
+@click.pass_obj
+@click.option('-y', '--year', help='View advisories from a specific year', default=None, type=int)
+@handle_api_error
+def advisories(controller, year):
+    """ List all Prelude advisories """
+    with Spinner():
+        print_json(data=controller.list_advisories(year=year))
+
+
+@detect.command('clone')
+@click.pass_obj
+@handle_api_error
+def clone(controller):
+    """ Download all tests to your local environment """
+    
+    async def fetch(test):
+        click.secho(f'Cloning {test["id"]}')
+        Path(test['id']).mkdir(parents=True, exist_ok=True)
+
+        for attach in controller.get_test(test_id=test['id']).get('attachments'):
+            if Path(attach).suffix:
+                code = controller.download(test_id=test['id'], filename=attach)
+                with open(PurePath(test['id'], attach), 'wb') as f:
+                    f.write(code)
+
+    async def start_cloning():
+        await asyncio.gather(*[fetch(test) for test in detect.list_tests()])
+
+    with Spinner():
+        asyncio.run(start_cloning())
+        click.secho('Project cloned successfully', fg='green')
+
+
 @detect.command('activity')
 @click.option('-v', '--view',
               help='retrieve a specific result view',
               default='logs', show_default=True,
-              type=click.Choice(['logs', 'days', 'insights', 'probes', 'units']))
+              type=click.Choice(['logs', 'days', 'insights', 'probes', 'advisories', 'tests']))
 @click.option('-d', '--days', help='days to look back', default=30, type=int)
 @click.option('--tests', help='comma-separated list of test IDs', type=str)
 @click.option('--tags', help='comma-separated list of tags', type=str)
 @click.option('--endpoints', help='comma-separated list of endpoint IDs', type=str)
 @click.option('--dos', help='comma-separated list of DOS', type=str)
 @click.pass_obj
 @handle_api_error
```

### Comparing `prelude-cli-1.1.2/prelude_cli/views/iam.py` & `prelude-cli-1.2.0/prelude_cli/views/iam.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 
 @iam.command('account')
 @click.pass_obj
 @handle_api_error
 def describe_account(controller):
     """ Get account details """
     with Spinner():
-        data = controller.get_account()
-    print_json(data=data)
+        print_json(data=controller.get_account())
 
 
 @iam.command('create-user')
 @click.option('-d', '--days', help='days this user will remain active', default=365, type=int)
 @click.option('-p', '--permission', help='user permission level', default=Permission.SERVICE.name,
               type=click.Choice([p.name for p in Permission if p != Permission.INVALID], case_sensitive=False), show_default=True)
 @click.option('-n', '--name', help='name of user', default='', type=str)
```

### Comparing `prelude-cli-1.1.2/prelude_cli/views/partner.py` & `prelude-cli-1.2.0/prelude_cli/views/partner.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 @click.option('--user', default='', help='user identifier')
 @click.option('--secret', default='', help='secret for OAUTH use cases')
 @click.pass_obj
 @handle_api_error
 def attach_partner(controller, name, api, user, secret):
     """ Attach an EDR to Detect """
     with Spinner():
-        controller.attach(name=name, api=api, user=user, secret=secret)
+        data = controller.attach(name=name, api=api, user=user, secret=secret)
+    print_json(data=data)
 
 
 @partner.command('detach')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('name')
 @click.pass_obj
 @handle_api_error
```

### Comparing `prelude-cli-1.1.2/prelude_cli/views/shared.py` & `prelude-cli-1.2.0/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.1.2/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.2.0/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.1.2
+Version: 1.2.0
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.1.2/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.2.0/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.1.2/setup.cfg` & `prelude-cli-1.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.1.2
+version = 1.2.0
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.1.2
+	prelude-sdk == 1.2.0
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

