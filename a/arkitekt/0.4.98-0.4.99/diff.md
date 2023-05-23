# Comparing `tmp/arkitekt-0.4.98.tar.gz` & `tmp/arkitekt-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkitekt-0.4.98.tar", max compression
+gzip compressed data, was "arkitekt-0.4.99.tar", max compression
```

## Comparing `arkitekt-0.4.98.tar` & `arkitekt-0.4.99.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.98/arkitekt/__init__.py
--rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.98/arkitekt/apps/__init__.py
--rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.98/arkitekt/apps/connected.py
--rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.98/arkitekt/apps/default.py
--rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/apps/fakts.py
--rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/apps/fluss.py
--rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/apps/herre.py
--rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.98/arkitekt/apps/mikro.py
--rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.98/arkitekt/apps/rekuest.py
--rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.98/arkitekt/apps/unlok.py
--rw-r--r--   0        0        0    12107 2023-05-02 10:57:58.871349 arkitekt-0.4.98/arkitekt/builders.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.98/arkitekt/cli/__init__.py
--rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.98/arkitekt/cli/build.py
--rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.98/arkitekt/cli/configs/introspect.yaml
--rw-r--r--   0        0        0    11706 2023-04-28 14:16:38.131941 arkitekt-0.4.98/arkitekt/cli/configs/latest.yaml
--rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.98/arkitekt/cli/configs/minimal.yaml
--rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.98/arkitekt/cli/deploy.py
--rw-r--r--   0        0        0     7327 2023-05-02 09:22:57.877413 arkitekt-0.4.98/arkitekt/cli/dev.py
--rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/cli/gen.py
--rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.98/arkitekt/cli/init.py
--rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.98/arkitekt/cli/inspect.py
--rw-r--r--   0        0        0    22346 2023-05-02 08:33:52.316141 arkitekt-0.4.98/arkitekt/cli/main.py
--rw-r--r--   0        0        0     2420 2023-05-02 08:31:56.092091 arkitekt-0.4.98/arkitekt/cli/run.py
--rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/cli/scan.py
--rw-r--r--   0        0        0    24496 2023-05-02 10:57:15.091215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/fluss.schema.graphql
--rw-r--r--   0        0        0   118448 2023-05-02 10:57:15.323216 arkitekt-0.4.98/arkitekt/cli/schemas/latest/gucker.schema.graphql
--rw-r--r--   0        0        0     4820 2023-05-02 10:57:15.127215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/kuay.schema.graphql
--rw-r--r--   0        0        0   118448 2023-05-02 10:57:14.919215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/mikro.schema.graphql
--rw-r--r--   0        0        0    51282 2023-05-02 10:57:15.015215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/rekuest.schema.graphql
--rw-r--r--   0        0        0     9948 2023-05-02 10:57:15.167215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/unlok.schema.graphql
--rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.98/arkitekt/cli/templates/simple.py
--rw-r--r--   0        0        0     1326 2023-05-02 08:14:53.195649 arkitekt-0.4.98/arkitekt/cli/types.py
--rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.98/arkitekt/cli/ui.py
--rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.98/arkitekt/cli/utils.py
--rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/deployers/port.py
--rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.98/arkitekt/healthz.py
--rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.98/arkitekt/qt/__init__.py
--rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.98/arkitekt/qt/assets/dark/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.98/arkitekt/qt/assets/dark/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.98/arkitekt/qt/assets/dark/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/dark/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/dark/red pulse.gif
--rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/light/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/light/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/light/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.98/arkitekt/qt/assets/light/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.98/arkitekt/qt/assets/light/red pulse.gif
--rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/qt/magic_bar.py
--rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.98/arkitekt/qt/utils.py
--rw-r--r--   0        0        0        0 2023-05-02 08:15:03.535653 arkitekt-0.4.98/arkitekt/runners.py
--rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.98/arkitekt/tqdm.py
--rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.98/arkitekt/utils.py
--rw-r--r--   0        0        0     2001 2023-05-02 11:00:28.631822 arkitekt-0.4.98/pyproject.toml
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.98/PKG-INFO
+-rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.99/arkitekt/__init__.py
+-rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.99/arkitekt/apps/__init__.py
+-rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.99/arkitekt/apps/connected.py
+-rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.99/arkitekt/apps/default.py
+-rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.99/arkitekt/apps/fakts.py
+-rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.99/arkitekt/apps/fluss.py
+-rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.99/arkitekt/apps/herre.py
+-rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.99/arkitekt/apps/mikro.py
+-rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.99/arkitekt/apps/rekuest.py
+-rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.99/arkitekt/apps/unlok.py
+-rw-r--r--   0        0        0    12107 2023-05-02 10:57:58.871349 arkitekt-0.4.99/arkitekt/builders.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.99/arkitekt/cli/__init__.py
+-rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.99/arkitekt/cli/build.py
+-rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.99/arkitekt/cli/configs/introspect.yaml
+-rw-r--r--   0        0        0    11706 2023-04-28 14:16:38.131941 arkitekt-0.4.99/arkitekt/cli/configs/latest.yaml
+-rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.99/arkitekt/cli/configs/minimal.yaml
+-rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.99/arkitekt/cli/deploy.py
+-rw-r--r--   0        0        0     7327 2023-05-02 09:22:57.877413 arkitekt-0.4.99/arkitekt/cli/dev.py
+-rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.99/arkitekt/cli/gen.py
+-rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.99/arkitekt/cli/init.py
+-rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.99/arkitekt/cli/inspect.py
+-rw-r--r--   0        0        0    22217 2023-05-02 12:19:25.323819 arkitekt-0.4.99/arkitekt/cli/main.py
+-rw-r--r--   0        0        0     2420 2023-05-02 12:19:36.795857 arkitekt-0.4.99/arkitekt/cli/run.py
+-rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.99/arkitekt/cli/scan.py
+-rw-r--r--   0        0        0    24496 2023-05-02 10:57:15.091215 arkitekt-0.4.99/arkitekt/cli/schemas/latest/fluss.schema.graphql
+-rw-r--r--   0        0        0   118448 2023-05-02 10:57:15.323216 arkitekt-0.4.99/arkitekt/cli/schemas/latest/gucker.schema.graphql
+-rw-r--r--   0        0        0     4820 2023-05-02 10:57:15.127215 arkitekt-0.4.99/arkitekt/cli/schemas/latest/kuay.schema.graphql
+-rw-r--r--   0        0        0   118448 2023-05-02 10:57:14.919215 arkitekt-0.4.99/arkitekt/cli/schemas/latest/mikro.schema.graphql
+-rw-r--r--   0        0        0    51282 2023-05-02 10:57:15.015215 arkitekt-0.4.99/arkitekt/cli/schemas/latest/rekuest.schema.graphql
+-rw-r--r--   0        0        0     9948 2023-05-02 10:57:15.167215 arkitekt-0.4.99/arkitekt/cli/schemas/latest/unlok.schema.graphql
+-rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.99/arkitekt/cli/templates/simple.py
+-rw-r--r--   0        0        0     1326 2023-05-02 08:14:53.195649 arkitekt-0.4.99/arkitekt/cli/types.py
+-rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.99/arkitekt/cli/ui.py
+-rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.99/arkitekt/cli/utils.py
+-rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.99/arkitekt/deployers/port.py
+-rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.99/arkitekt/healthz.py
+-rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.99/arkitekt/qt/__init__.py
+-rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.99/arkitekt/qt/assets/dark/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.99/arkitekt/qt/assets/dark/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.99/arkitekt/qt/assets/dark/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.99/arkitekt/qt/assets/dark/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.99/arkitekt/qt/assets/dark/red pulse.gif
+-rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.99/arkitekt/qt/assets/light/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.99/arkitekt/qt/assets/light/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.99/arkitekt/qt/assets/light/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.99/arkitekt/qt/assets/light/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.99/arkitekt/qt/assets/light/red pulse.gif
+-rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.99/arkitekt/qt/magic_bar.py
+-rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.99/arkitekt/qt/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 08:15:03.535653 arkitekt-0.4.99/arkitekt/runners.py
+-rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.99/arkitekt/tqdm.py
+-rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.99/arkitekt/utils.py
+-rw-r--r--   0        0        0     2001 2023-05-02 12:19:38.959864 arkitekt-0.4.99/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.99/PKG-INFO
```

### Comparing `arkitekt-0.4.98/arkitekt/apps/connected.py` & `arkitekt-0.4.99/arkitekt/apps/connected.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/apps/default.py` & `arkitekt-0.4.99/arkitekt/apps/default.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/apps/fluss.py` & `arkitekt-0.4.99/arkitekt/apps/fluss.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/apps/mikro.py` & `arkitekt-0.4.99/arkitekt/apps/mikro.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/apps/rekuest.py` & `arkitekt-0.4.99/arkitekt/apps/rekuest.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/apps/unlok.py` & `arkitekt-0.4.99/arkitekt/apps/unlok.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/builders.py` & `arkitekt-0.4.99/arkitekt/builders.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/build.py` & `arkitekt-0.4.99/arkitekt/cli/build.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/configs/introspect.yaml` & `arkitekt-0.4.99/arkitekt/cli/configs/introspect.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/configs/latest.yaml` & `arkitekt-0.4.99/arkitekt/cli/configs/latest.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/configs/minimal.yaml` & `arkitekt-0.4.99/arkitekt/cli/configs/minimal.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/deploy.py` & `arkitekt-0.4.99/arkitekt/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/dev.py` & `arkitekt-0.4.99/arkitekt/cli/dev.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/gen.py` & `arkitekt-0.4.99/arkitekt/cli/gen.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/init.py` & `arkitekt-0.4.99/arkitekt/cli/init.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/inspect.py` & `arkitekt-0.4.99/arkitekt/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/main.py` & `arkitekt-0.4.99/arkitekt/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,32 +199,29 @@
     "--url",
     help="The fakts url for connection",
     envvar="FAKTS_URL",
     default="http://lok:8000",
 )
 @with_token
 @with_instance_id
-@with_version
 @with_skip_cache
 def port(url, token, instance, version, nocache=False):
     """Runs the arkitekt app"""
 
     from arkitekt.cli.run import run_port
 
     manifest = load_manifest()
     if not manifest:
         raise click.ClickException(
             "No manifest found. Please run `arkitekt init` first before deploying an arkitekt app."
         )
 
     asyncio.run(
         run_port(
-            entrypoint=manifest.entrypoint,
-            identifier=manifest.identifier,
-            version=version or manifest.version,
+            manifest,
             url=url,
             token=token,
             instance_id=instance,
             nocache=nocache,
         )
     )
```

### Comparing `arkitekt-0.4.98/arkitekt/cli/run.py` & `arkitekt-0.4.99/arkitekt/cli/run.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/scan.py` & `arkitekt-0.4.99/arkitekt/cli/scan.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/schemas/latest/fluss.schema.graphql` & `arkitekt-0.4.99/arkitekt/cli/schemas/latest/fluss.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/schemas/latest/gucker.schema.graphql` & `arkitekt-0.4.99/arkitekt/cli/schemas/latest/gucker.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/schemas/latest/kuay.schema.graphql` & `arkitekt-0.4.99/arkitekt/cli/schemas/latest/kuay.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/schemas/latest/mikro.schema.graphql` & `arkitekt-0.4.99/arkitekt/cli/schemas/latest/mikro.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/schemas/latest/rekuest.schema.graphql` & `arkitekt-0.4.99/arkitekt/cli/schemas/latest/rekuest.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/schemas/latest/unlok.schema.graphql` & `arkitekt-0.4.99/arkitekt/cli/schemas/latest/unlok.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/types.py` & `arkitekt-0.4.99/arkitekt/cli/types.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/cli/ui.py` & `arkitekt-0.4.99/arkitekt/cli/ui.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/healthz.py` & `arkitekt-0.4.99/arkitekt/healthz.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/dark/gear.png` & `arkitekt-0.4.99/arkitekt/qt/assets/dark/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/dark/green pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/dark/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/dark/orange pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/dark/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/dark/pink pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/dark/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/dark/red pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/dark/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/light/gear.png` & `arkitekt-0.4.99/arkitekt/qt/assets/light/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/light/green pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/light/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/light/orange pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/light/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/light/pink pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/light/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/assets/light/red pulse.gif` & `arkitekt-0.4.99/arkitekt/qt/assets/light/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/qt/magic_bar.py` & `arkitekt-0.4.99/arkitekt/qt/magic_bar.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/tqdm.py` & `arkitekt-0.4.99/arkitekt/tqdm.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/arkitekt/utils.py` & `arkitekt-0.4.99/arkitekt/utils.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.98/pyproject.toml` & `arkitekt-0.4.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arkitekt"
-version = "0.4.98"
+version = "0.4.99"
 description = "client for the arkitekt platform"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "arkitekt" }]
 
 [tool.poetry.dependencies]
 python = "^3.8, <=3.12"
```

### Comparing `arkitekt-0.4.98/PKG-INFO` & `arkitekt-0.4.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkitekt
-Version: 0.4.98
+Version: 0.4.99
 Summary: client for the arkitekt platform
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

