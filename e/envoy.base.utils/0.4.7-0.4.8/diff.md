# Comparing `tmp/envoy.base.utils-0.4.7.tar.gz` & `tmp/envoy.base.utils-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.base.utils-0.4.7.tar", last modified: Sun Apr 30 17:55:05 2023, max compression
+gzip compressed data, was "envoy.base.utils-0.4.8.tar", last modified: Sat May 20 17:37:48 2023, max compression
```

## Comparing `envoy.base.utils-0.4.7.tar` & `envoy.base.utils-0.4.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.315741 envoy.base.utils-0.4.7/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.315741 envoy.base.utils-0.4.7/envoy/base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/envoy/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/envoy/base/utils/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/data_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/data_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/jinja_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/parallel_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project_data_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.315741 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.765567 envoy.base.utils-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-20 17:37:48.765567 envoy.base.utils-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.761567 envoy.base.utils-0.4.8/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.761567 envoy.base.utils-0.4.8/envoy/base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.761567 envoy.base.utils-0.4.8/envoy/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.765567 envoy.base.utils-0.4.8/envoy/base/utils/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.765567 envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/abstract/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/data_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/data_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/jinja_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/parallel_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/project_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/project_data_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/project_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy/base/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:37:48.761567 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/envoy.base.utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:37:48.765567 envoy.base.utils-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-20 17:37:48.000000 envoy.base.utils-0.4.8/setup.py
```

### Comparing `envoy.base.utils-0.4.7/backend_shim.py` & `envoy.base.utils-0.4.8/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/__init__.py` & `envoy.base.utils-0.4.8/envoy/base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/changelog.py` & `envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/inventory.py` & `envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/inventory.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/project.py` & `envoy.base.utils-0.4.8/envoy/base/utils/abstract/project/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import asyncio
 import json
 import pathlib
 from concurrent import futures
+from datetime import datetime
 from functools import cached_property
 from typing import (
     AsyncGenerator, List, Mapping, Optional,
     Tuple, Type, Union)
 
 import aiohttp
 from packaging import version as _version
@@ -234,37 +235,47 @@
     def is_current(self, version: _version.Version) -> bool:
         return (
             self.version.base_version
             == version.base_version)
 
     async def publish(
             self,
+            dry_run: bool = False,
             assets: Optional[pathlib.Path] = None,
             commitish: Optional[str] = None,
             dev: Optional[bool] = None,
             latest: Optional[bool] = None) -> typing.ProjectPublishResultDict:
-        if not dev and self.is_dev:
+        if not dev and self.is_dev and not dry_run:
             raise _github.exceptions.TagError(
                 f"Cannot tag a dev version: {self.version}")
         commitish = (
             commitish
             if commitish
             else (self.main_branch
                   if self.is_main
                   else f"release/v{self.minor_version}"))
+        latest = latest or (self.is_main and not self.is_dev)
+        if dry_run:
+            return dict(
+                commitish=commitish,
+                date=datetime.now().strftime("%m/%d/%Y %H:%M:%S"),
+                tag_name=f"v{self.version}",
+                url=f"test://releases/v{self.version}",
+                dry_run=" (dry run)")
         release = await self.repo.create_release(
             commitish,
             f"v{self.version}",
-            latest=latest or (self.is_main and not self.is_dev))
+            latest=latest)
         # TODO: add asset upload
         return dict(
             commitish=release["target_commitish"],
             date=release["published_at"],
             tag_name=release["tag_name"],
-            url=release["html_url"])
+            url=release["html_url"],
+            dry_run="")
 
     async def release(self) -> typing.ProjectReleaseResultDict:
         if not self.is_dev:
             raise exceptions.ReleaseError(
                 "Project is not set to dev")
         self.write_version(self.version)
         date = self.changelogs.datestamp
```

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/abstract/protobuf.py` & `envoy.base.utils-0.4.8/envoy/base/utils/abstract/protobuf.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/data_env.py` & `envoy.base.utils-0.4.8/envoy/base/utils/data_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/interface.py` & `envoy.base.utils-0.4.8/envoy/base/utils/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/jinja_env.py` & `envoy.base.utils-0.4.8/envoy/base/utils/jinja_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/parallel_runner.py` & `envoy.base.utils-0.4.8/envoy/base/utils/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/project.py` & `envoy.base.utils-0.4.8/envoy/base/utils/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/project_runner.py` & `envoy.base.utils-0.4.8/envoy/base/utils/project_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ENV_GITHUB_TOKEN = 'GITHUB_TOKEN'
 NOTIFY_MSGS: frozendict = frozendict(
     release=(
         "Release created ({change[release][version]}): "
         "{change[release][date]}"),
     dev="Repo set to dev ({change[dev][version]})",
     sync="Repo synced",
-    publish="Repo published")
+    publish="Repo published{change[publish][dry_run]}")
 COMMIT_MSGS: frozendict = frozendict(
     release="repo: Release `{change[release][version]}`",
     dev="repo: Dev `{change[dev][version]}`",
     sync="repo: Sync")
 
 
 class BaseProjectRunner(runner.Runner):
@@ -86,15 +86,15 @@
             choices=["sync", "release", "dev", "publish"])
         parser.add_argument("path", default=".")
         parser.add_argument("--github_token")
         parser.add_argument("--nosync", action="store_true")
         parser.add_argument("--nocommit", action="store_true")
         parser.add_argument("--patch", action="store_true")
         parser.add_argument("--repo", default="")
-
+        parser.add_argument("--dry-run", action="store_true")
         parser.add_argument("--publish-assets", default="")
         parser.add_argument("--publish-commitish", default="")
         parser.add_argument("--publish-dev", action="store_true")
         parser.add_argument("--publish-latest", action="store_true")
         parser.add_argument("--publish-generate-notes", action="store_true")
 
     async def commit(
@@ -106,14 +106,15 @@
         self.log.info(f"[git] commit: \"{msg}\"")
 
     async def handle_action(self) -> typing.ProjectChangeDict:
         change: typing.ProjectChangeDict = {}
         if self.command == "publish":
             return dict(
                 publish=await self.run_publish(
+                    dry_run=self.args.dry_run,
                     assets=self.args.publish_assets,
                     commitish=self.args.publish_commitish,
                     dev=self.args.publish_dev,
                     latest=self.args.publish_latest))
         if self.command == "dev":
             change["dev"] = await self.run_dev()
         if self.command == "release":
```

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/tar.py` & `envoy.base.utils-0.4.8/envoy/base/utils/tar.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/typing.py` & `envoy.base.utils-0.4.8/envoy/base/utils/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 
 class ProjectPublishResultDict(TypedDict):
     commitish: str
     date: str
     tag_name: str
     url: str
+    dry_run: str
 
 
 class ProjectChangeDict(TypedDict, total=False):
     dev: ProjectDevResultDict
     publish: ProjectPublishResultDict
     release: ProjectReleaseResultDict
     sync: ProjectSyncResultDict
```

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/utils.py` & `envoy.base.utils-0.4.8/envoy/base/utils/utils.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy/base/utils/yaml.py` & `envoy.base.utils-0.4.8/envoy/base/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/envoy.base.utils.egg-info/SOURCES.txt` & `envoy.base.utils-0.4.8/envoy.base.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.7/setup.py` & `envoy.base.utils-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     },
     'packages': (
         'envoy.base.utils',
         'envoy.base.utils.abstract',
         'envoy.base.utils.abstract.project',
     ),
     'python_requires': '>=3.10.0',
-    'url': 'https://github.com/envoyproxy/pytooling/tree/main/envoy.base.utils',
-    'version': '0.4.7',
+    'url': 'https://github.com/envoyproxy/toolshed/tree/main/envoy.base.utils',
+    'version': '0.4.8',
 })
```

