# Comparing `tmp/wop-2.4.0.tar.gz` & `tmp/wop-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\rlafage\workspace\WhatsOpt-CLI\dist\.tmp-wijuiq1d\wop-2.4.0.tar", last modified: Mon May 15 13:06:20 2023, max compression
+gzip compressed data, was "dist\wop-2.5.0.tar", last modified: Tue May 23 08:11:06 2023, max compression
```

## Comparing `wop-2.4.0.tar` & `wop-2.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.503549 wop-2.4.0/
--rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.4.0/LICENSE
--rw-rw-rw-   0        0        0      851 2023-05-15 13:06:20.503549 wop-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 13:06:20.503549 wop-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.472293 wop-2.4.0/tests/
--rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_convert_utils.py
--rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.4.0/tests/test_mooptimization.py
--rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_push_command.py
--rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_push_utils.py
--rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_upload_utils.py
--rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_utils.py
--rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.4.0/tests/test_whatsopt_client.py
--rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_wop.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.487925 wop-2.4.0/whatsopt/
--rw-rw-rw-   0        0        0       23 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/__init__.py
--rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.4.0/whatsopt/convert_utils.py
--rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.4.0/whatsopt/logging.py
--rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.4.0/whatsopt/mooptimization.py
--rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.4.0/whatsopt/optimization.py
--rw-rw-rw-   0        0        0      232 2023-04-12 16:39:47.000000 wop-2.4.0/whatsopt/publish_utils.py
--rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.4.0/whatsopt/push_command.py
--rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.4.0/whatsopt/push_utils.py
--rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.4.0/whatsopt/show_utils.py
--rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.4.0/whatsopt/upload_utils.py
--rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/utils.py
--rw-rw-rw-   0        0        0    40369 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/whatsopt_client.py
--rw-rw-rw-   0        0        0    13166 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/wop.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.503549 wop-2.4.0/wop.egg-info/
--rw-rw-rw-   0        0        0      851 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.4.0/wop.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.900708 wop-2.5.0/
+-rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0      851 2023-05-23 08:11:06.900708 wop-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:11:06.900708 wop-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.867009 wop-2.5.0/tests/
+-rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_convert_utils.py
+-rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.5.0/tests/test_mooptimization.py
+-rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_push_command.py
+-rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_push_utils.py
+-rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_upload_utils.py
+-rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.5.0/tests/test_whatsopt_client.py
+-rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_wop.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.890628 wop-2.5.0/whatsopt/
+-rw-rw-rw-   0        0        0       23 2023-05-23 08:10:57.000000 wop-2.5.0/whatsopt/__init__.py
+-rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.5.0/whatsopt/convert_utils.py
+-rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.5.0/whatsopt/logging.py
+-rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.5.0/whatsopt/mooptimization.py
+-rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.5.0/whatsopt/optimization.py
+-rw-rw-rw-   0        0        0      232 2023-04-12 16:39:47.000000 wop-2.5.0/whatsopt/publish_utils.py
+-rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.5.0/whatsopt/push_command.py
+-rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.5.0/whatsopt/push_utils.py
+-rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.5.0/whatsopt/show_utils.py
+-rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.5.0/whatsopt/upload_utils.py
+-rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.5.0/whatsopt/utils.py
+-rw-rw-rw-   0        0        0    40617 2023-05-23 08:10:57.000000 wop-2.5.0/whatsopt/whatsopt_client.py
+-rw-rw-rw-   0        0        0    13395 2023-05-23 08:10:57.000000 wop-2.5.0/whatsopt/wop.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.900708 wop-2.5.0/wop.egg-info/
+-rw-rw-rw-   0        0        0      851 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.5.0/wop.egg-info/zip-safe
```

### Comparing `wop-2.4.0/LICENSE` & `wop-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/PKG-INFO` & `wop-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.4.0
+Version: 2.5.0
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.4.0/README.md` & `wop-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/setup.py` & `wop-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/tests/test_convert_utils.py` & `wop-2.5.0/tests/test_convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/tests/test_push_command.py` & `wop-2.5.0/tests/test_push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/tests/test_push_utils.py` & `wop-2.5.0/tests/test_push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/tests/test_upload_utils.py` & `wop-2.5.0/tests/test_upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/tests/test_utils.py` & `wop-2.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/tests/test_wop.py` & `wop-2.5.0/tests/test_wop.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/convert_utils.py` & `wop-2.5.0/whatsopt/convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/mooptimization.py` & `wop-2.5.0/whatsopt/mooptimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/optimization.py` & `wop-2.5.0/whatsopt/optimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/push_command.py` & `wop-2.5.0/whatsopt/push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/push_utils.py` & `wop-2.5.0/whatsopt/push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/show_utils.py` & `wop-2.5.0/whatsopt/show_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/upload_utils.py` & `wop-2.5.0/whatsopt/upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/utils.py` & `wop-2.5.0/whatsopt/utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.4.0/whatsopt/whatsopt_client.py` & `wop-2.5.0/whatsopt/whatsopt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,15 +578,15 @@
             state = {
                 "whatsopt_url": self._url,
                 "analysis_id": mda_id,
                 "framework": framework,
                 "pull_mode": MODE_PACKAGE if options.get("--package") else MODE_PLAIN,
             }
             save_state(state)
-            log(msg)
+            info(msg)
 
     def pull_mda_json(self, mda_id):
         url = self.endpoint(f"/api/v1/analyses/{mda_id}.wopjson")
         resp = self.session.get(url, headers=self.headers, stream=True)
         resp.raise_for_status()
         print(json.dumps(resp.json()))
 
@@ -924,20 +924,20 @@
         if not is_package_mode():
             error("Package mode is required!")
             exit(-1)
         self._update_mda_base()
         filename = build_package()
         return filename
 
-    def fetch(self, target_id=None, options={}):
+    def fetch(self, source_id=None, options={}):
         if not is_package_mode():
             error("Package mode is required!")
             exit(-1)
         mda_id = get_analysis_id()
-        param = f"?src_id={target_id}"
+        param = f"?src_id={source_id}"
         format_query = "mda_pkg_content"
         url = self.endpoint(
             f"/api/v1/analyses/{mda_id}/exports/new.{format_query}{param}"
         )
         resp = self.session.get(url, headers=self.headers, stream=True)
         if resp.ok:
             name = None
@@ -947,14 +947,18 @@
                 for chunk in resp.iter_content(chunk_size=128):
                     fd.write(chunk)
                 name = fd.name
             zipf = zipfile.ZipFile(name, "r")
             tempdir = tempfile.mkdtemp(suffix="wop", dir=tempfile.tempdir)
             zipf.extractall(tempdir)
             filenames = zipf.namelist()
+            if not filenames:
+                warn(f"No package found for Analysis #{source_id}")
+                log("Nothing to do")
+                return
             zipf.close()
 
             file_to_move = {}
             for f in filenames:
                 file_to = f
                 file_to_move[file_to] = True
                 if os.path.exists(file_to):
@@ -969,58 +973,61 @@
                             f"File {file_to} in the way: remove it or use --force to override"
                         )
                         file_to_move[file_to] = False
                 else:
                     log(f"Fetch {file_to}")
             if not options.get("--dry-run"):
                 move_files(file_to_move, tempdir)
-                log(f"Analysis #{target_id} fetched")
+                info(f"Analysis #{source_id} disciplines fetched")
         else:
-            error(f"Error while fetching Analysis #{target_id}")
-            resp.raise_for_status()
+            error(f"Error while fetching disciplines of Analysis #{source_id}")
+            error(resp.json().get("message"))
 
-    def merge(self, target_id=None, options={}):
+    def merge(self, source_id, options={}):
         if not is_package_mode():
             error("Package mode is required!")
             exit(-1)
         current_id = get_analysis_id()
         url = self.endpoint(f"/api/v1/analyses/{current_id}")
         params = {
             "analysis": {
-                "import": {"analysis": target_id},
+                "import": {"analysis": source_id},
             },
             "requested_at": str(datetime.now()),
         }
         if options.get("--dry-run"):
             self.get_status()
-            url = self.endpoint("/api/v1/analyses/{}".format(target_id))
+            url = self.endpoint("/api/v1/analyses/{}".format(source_id))
             resp = self.session.get(url, headers=self.headers)
-            log(f"Analysis #{target_id} #{resp.json()} is selected to be merged")
+            log(f"Analysis #{source_id} #{resp.json()} is selected to be merged")
         else:
             resp = self.session.put(url, headers=self.headers, json=params)
         if resp.ok:
-            self.fetch(target_id, options)
-            self._update_mda_base(options.get("--dry-run"), options.get("--force"))
             if not options.get("--dry-run"):
-                info(f"Analysis #{target_id} successfully merged")
+                info(f"Analysis #{source_id} merged")
         elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-            error(f"Error while merging Analysis #{target_id}.")
+            error(f"Error while merging Analysis #{source_id}.")
             error(
                 f"    Check analyses, maybe they are not compatible (same variable produced by different disciplines)"
             )
         elif resp.status_code == HTTPStatus.FORBIDDEN:
-            error(f"Error while merging Analysis #{target_id}.")
+            error(f"Error while merging Analysis #{source_id}.")
             error(
                 f"    You are not authorized to update the current analysis: either you do not own it or"
                 f" current analysis is already packaged or operated"
             )
         else:
-            error(f"Error while merging Analysis #{target_id}")
+            error(f"Error while merging Analysis #{source_id}")
             resp.raise_for_status()
 
+    def pull_source_mda(self, source_id, options={}):
+        self.merge(source_id, options)
+        self.fetch(source_id, options)
+        self._update_mda_base(options.get("--dry-run"))
+
     def _update_mda_base(self, dry_run=False, force=False):
         update_options = {
             "--dry-run": dry_run,
             "--force": force,
             "--server": False,
             "--egmdo": False,
             "--run-ops": False,
```

### Comparing `wop-2.4.0/whatsopt/wop.py` & `wop-2.5.0/whatsopt/wop.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import click
 from whatsopt import __version__
+from whatsopt.utils import get_analysis_id
 from .whatsopt_client import WhatsOpt, EXTRANET_SERVER_URL
 from logging import error
 
 DEFAULT_PUSH_DEPTH = 2
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
@@ -191,16 +192,16 @@
 @click.option(
     "--gemseo/--openmdao",
     default=False,
     help="pull analysis as GEMSEO source code (default OpenMDAO)",
 )
 @click.option(
     "--package/--plain",
-    default=False,
-    help="pull analysis as Python package (default plain)",
+    default=True,
+    help="pull analysis as Python package (default) or plain mode (--plain)",
 )
 @click.argument("analysis_id")
 @click.pass_context
 def pull(
     ctx,
     dry_run,
     force,
@@ -232,15 +233,19 @@
             wop.pull_project_json(analysis_id)
         else:
             wop.pull_mda_json(analysis_id)
     else:
         if project_id:
             error("Bad option --project-id which works only with option --json enabled")
             exit(-1)
-        wop.pull_mda(analysis_id, options)
+        current_id = get_analysis_id()
+        if current_id and analysis_id != current_id:
+            wop.merge_fetch_mda(analysis_id, options)
+        else:
+            wop.pull_mda(analysis_id, options)
 
 
 @wop.command()
 @click.option(
     "-n",
     "--dry-run",
     is_flag=True,
@@ -474,20 +479,20 @@
     is_flag=True,
     default=False,
     help="print analysis fetch info without actually fetching",
 )
 @click.option(
     "-f", "--force", is_flag=True, default=False, help="overwrite existing files"
 )
-@click.argument("target_id")
+@click.argument("source_id")
 @click.pass_context
-def fetch(ctx, target_id, dry_run, force):
+def fetch(ctx, source_id, dry_run, force):
     """Fetch package content of the given analysis specified by its identifier"""
     options = {"--dry-run": dry_run, "--force": force}
-    WhatsOpt(**ctx.obj).login().fetch(target_id, options)
+    WhatsOpt(**ctx.obj).login().fetch(source_id, options)
 
 
 @wop.command()
 @click.argument("analysis_id")
 @click.pass_context
 @click.option(
     "-n",
```

### Comparing `wop-2.4.0/wop.egg-info/PKG-INFO` & `wop-2.5.0/wop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.4.0
+Version: 2.5.0
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.4.0/wop.egg-info/SOURCES.txt` & `wop-2.5.0/wop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

