# Comparing `tmp/wf_video_io-3.2.3.tar.gz` & `tmp/wf_video_io-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.2.3.tar", max compression
+gzip compressed data, was "wf_video_io-3.2.4.tar", max compression
```

## Comparing `wf_video_io-3.2.3.tar` & `wf_video_io-3.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.2.3/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.2.3/README.md
--rw-r--r--   0        0        0     1162 2023-05-15 18:29:11.418209 wf_video_io-3.2.3/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.2.3/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.2.3/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    14986 2023-05-15 17:34:04.908392 wf_video_io-3.2.3/video_io/client/core.py
--rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.2.3/video_io/client/errors.py
--rw-r--r--   0        0        0     3787 2023-05-15 17:34:04.829824 wf_video_io-3.2.3/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.2.3/video_io/config.py
--rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.2.3/video_io/core.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.2.3/video_io/log_retry.py
--rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.2.3/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.2.3/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.2.3/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.2.4/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.2.4/README.md
+-rw-r--r--   0        0        0     1162 2023-05-23 17:03:34.651366 wf_video_io-3.2.4/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.2.4/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.2.4/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    15027 2023-05-23 16:51:13.034649 wf_video_io-3.2.4/video_io/client/core.py
+-rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.2.4/video_io/client/errors.py
+-rw-r--r--   0        0        0     3426 2023-05-23 17:01:01.553631 wf_video_io-3.2.4/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.2.4/video_io/config.py
+-rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.2.4/video_io/core.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.2.4/video_io/log_retry.py
+-rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.2.4/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.2.4/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.2.4/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.2.4/PKG-INFO
```

### Comparing `wf_video_io-3.2.3/LICENSE` & `wf_video_io-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.3/pyproject.toml` & `wf_video_io-3.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-video-io"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.2.3"
+version = "3.2.4"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.2.3/video_io/client/core.py` & `wf_video_io-3.2.4/video_io/client/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,14 +285,16 @@
         results = []
         request["files"] = files
         request["data"] = {"videos": json.dumps(videos)}
         try:
             request = requests.Request(**request)
             r = request.prepare()
             response = self.request_session.send(r)
+            response.raise_for_status()
+
             for i, vr in enumerate(response.json()):
                 results.append(
                     {
                         "path": videos[i]["meta"]["path"],
                         "uploaded": True,
                         "id": vr["id"],
                         "disposition": "ok"
```

### Comparing `wf_video_io-3.2.3/video_io/client/utils.py` & `wf_video_io-3.2.4/video_io/client/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import re
 import subprocess
 
+import ffmpeg
 from tenacity import retry, wait_random, stop_after_attempt
 from auth0.v3.authentication import GetToken
 from cachetools.func import ttl_cache
 import jmespath
 
 
 @ttl_cache(ttl=60 * 60 * 4)
@@ -24,32 +25,17 @@
     api_token = token["access_token"]
     expires_in = token["expires_in"]
     return api_token, expires_in
 
 
 @ttl_cache(ttl=60 * 60 * 4)
 def get_video_file_details(path):
-    # check for meta-file if it exists load that and return it's contents.
+    # check for video file if it exists load that and return its contents.
     # if not then run ffprobe and return a new meta document
-    ffprobe_out = subprocess.run(
-        [
-            "ffprobe",
-            "-v",
-            "error",
-            "-show_entries",
-            "format=duration:stream=nb_read_frames,r_frame_rate,codec_type",
-            "-count_frames",
-            "-of",
-            "json=compact=1",
-            path,
-        ],
-        capture_output=True,
-        check=True,
-    )
-    return json.loads(ffprobe_out.stdout)
+    return ffmpeg.probe(path, timeout=5)
 
 
 CACHE_PATH_FILE = re.compile(
     "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})/(?P<file>.*)$"
 )
 CACHE_PATH_HOUR = re.compile(
     "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})$"
```

### Comparing `wf_video_io-3.2.3/video_io/config.py` & `wf_video_io-3.2.4/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.3/video_io/core.py` & `wf_video_io-3.2.4/video_io/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.3/video_io/utils.py` & `wf_video_io-3.2.4/video_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.3/video_io/video_reader.py` & `wf_video_io-3.2.4/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.3/setup.py` & `wf_video_io-3.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.2.3',
+    'version': '3.2.4',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.2.3/PKG-INFO` & `wf_video_io-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.2.3
+Version: 3.2.4
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

