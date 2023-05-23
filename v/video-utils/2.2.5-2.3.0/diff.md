# Comparing `tmp/video_utils-2.2.5.tar.gz` & `tmp/video_utils-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_utils-2.2.5.tar", max compression
+gzip compressed data, was "video_utils-2.3.0.tar", max compression
```

## Comparing `video_utils-2.2.5.tar` & `video_utils-2.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-15 13:34:03.040912 video_utils-2.2.5/LICENSE.md
--rw-r--r--   0        0        0      917 2023-05-15 13:34:03.040912 video_utils-2.2.5/README.md
--rw-r--r--   0        0        0      726 2023-05-15 13:34:03.040912 video_utils-2.2.5/pyproject.toml
--rw-r--r--   0        0        0      166 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/__init__.py
--rw-r--r--   0        0        0     1627 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/codec.py
--rw-r--r--   0        0        0      259 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/colour.py
--rw-r--r--   0        0        0     5355 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/fileMap.py
--rw-r--r--   0        0        0      868 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/parse_episode.py
--rw-r--r--   0        0        0     1549 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/validators.py
--rw-r--r--   0        0        0     2649 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/video.py
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 video_utils-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-23 10:41:51.500130 video_utils-2.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1368 2023-05-23 10:41:51.500130 video_utils-2.3.0/README.md
+-rw-r--r--   0        0        0      744 2023-05-23 10:41:51.500130 video_utils-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/__init__.py
+-rw-r--r--   0        0        0     1627 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/codec.py
+-rw-r--r--   0        0        0      259 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/colour.py
+-rw-r--r--   0        0        0     5367 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/fileMap.py
+-rw-r--r--   0        0        0      868 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/parse_episode.py
+-rw-r--r--   0        0        0     1549 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/validators.py
+-rw-r--r--   0        0        0     3437 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/video.py
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 video_utils-2.3.0/PKG-INFO
```

### Comparing `video_utils-2.2.5/LICENSE.md` & `video_utils-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.5/README.md` & `video_utils-2.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # Video Utils
 
-![Test Status](https://github.com/justin8/video_utils/workflows/Tests/badge.svg?branch=master)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/video_utils)](https://pypi.org/project/video_utils/) [![PyPI version](https://badge.fury.io/py/video_utils.svg)](https://badge.fury.io/py/video_utils)
+
+[![Workflow](https://github.com/justin8/video_utils/actions/workflows/workflow.yml/badge.svg)](https://github.com/justin8/video_utils/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/justin8/video_utils/branch/master/graph/badge.svg)](https://codecov.io/gh/justin8/video_utils)
+[![Downloads](https://pepy.tech/badge/video_utils/month)](https://pepy.tech/project/video_utils)
 
 This library provides utilities for dealing with TV show and Movie files and the metadata around them.
 
 ## Example Usage
 
 ```python
 from video_utils import FileMap
 
-f = FileMap("/path/to/videos")
-f.load() # By default, this will load the cached metadata, and then update files that have changed in size
+def run():
+    f = FileMap("/path/to/videos")
+    f.load() # By default, this will load the cached metadata, and then update files that have changed in size
+
+    for directory in f.contents:
+        for video in f.contents[directory]:
+            codec = video.codec
+            print(codec.pretty_name) # x265
+            print(video.quality) # 1080p
+            print(video.full_path)
+            print(video.size) # in bytes
+            print(video)
+            video.refresh() # force a refresh of the video metadata, will only occur if filesize has changed.
 
-for directory in f.contents:
-    for video in f.contents[directory]:
-        codec = video.codec
-        print(codec.pretty_name) # x265
-        print(video.quality) # 1080p
-        print(video.full_path)
-        print(video.size) # in bytes
-        print(video)
-        video.refresh() # force a refresh of the video metadata, will only occur if filesize has changed.
+run()
 ```
```

### Comparing `video_utils-2.2.5/pyproject.toml` & `video_utils-2.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "video_utils"
-version = "2.2.5"
+version = "2.3.0"
 description = "This library is used for lots of shared functionality around parsing TV shows and movies"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3 :: Only"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 colorama = "^0.4.6"
 pymediainfo = "^6.0.1"
-tqdm = "^4.65.0"
 ffmpy = "^0.3.0"
+rich = "^13.3.5"
+iso639 = "^0.1.4"
 
 [tool.poetry.dev-dependencies]
 coverage = "^7.2.5"
 mock = "^5.0.2"
 pytest = "^7.3.1"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
```

### Comparing `video_utils-2.2.5/video_utils/codec.py` & `video_utils-2.3.0/video_utils/codec.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.5/video_utils/fileMap.py` & `video_utils-2.3.0/video_utils/fileMap.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from copy import deepcopy
 import logging
 import os
 from os import path
 import hashlib
 import pickle
-from tqdm import tqdm
+from rich.progress import track
 
 from .colour import colour
 from .validators import Filter
 from .video import Video
 
 log = logging.getLogger(__name__)
 
@@ -76,15 +76,15 @@
         for dir_path, dir_names, file_names in self._file_tree():
             log.info(colour("green", "Working in directory: %s" % dir_path))
 
             video_files = filter.only_videos(file_names)
             log.debug("Total videos in %s: %s" % (dir_path, len(video_files)))
 
             if self._progress_bar:
-                video_files = tqdm(video_files)
+                video_files = track(video_files)
 
             for video_file in video_files:
                 self._update_video(dir_path, video_file)
 
     def _update_video(self, dir_path, video_name):
         if dir_path not in self.contents:
             self.contents[dir_path] = []
@@ -120,15 +120,15 @@
             if not path.exists(dir_path):
                 log.debug("Removing %s from cache" % dir_path)
                 del self.contents[dir_path]
                 continue
 
             sub_directory = contents_copy[dir_path]
             if self._progress_bar:
-                sub_directory = tqdm(sub_directory)
+                sub_directory = track(sub_directory)
 
             for video in sub_directory:
                 if not path.exists(video.full_path):
                     log.debug("Removing %s from cache" % video.full_path)
                     self.contents[dir_path].remove(video)
```

### Comparing `video_utils-2.2.5/video_utils/parse_episode.py` & `video_utils-2.3.0/video_utils/parse_episode.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.5/video_utils/validators.py` & `video_utils-2.3.0/video_utils/validators.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.5/video_utils/video.py` & `video_utils-2.3.0/video_utils/video.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import logging
 import os
 from os import path
+from typing import List
 
 from pymediainfo import MediaInfo
+from iso639 import to_iso639_2
 
 from .validators import Validator
 from .codec import Codec
 
 log = logging.getLogger(__name__)
 
 
 class Video:
-    def __init__(self, name, dir_path, codec=None, quality=None, size=None):
+    def __init__(self, name, dir_path, codec=None, quality=None, size=None, video_track=None, audio_tracks=None, text_tracks=None):
         self.name = name
         self.dir_path = dir_path
         self.codec = codec
         self.quality = quality
         self.size = size
+        self.video_track = video_track
+        self.audio_tracks = audio_tracks
+        self.text_tracks = text_tracks
 
     def __eq__(self, other):
         if not isinstance(other, Video):
             # don't attempt to compare against unrelated types
             return NotImplemented
 
         return self.full_path == other.full_path
@@ -28,23 +33,35 @@
     def __repr__(self):
         return f"<Video name={self.name} codec={self.codec} quality={self.quality}>"
 
     def __str__(self):
         return self.__repr__()
 
     @property
-    def dir_path(self):
+    def subtitle_languages(self) -> List[str]:
+        if self.text_tracks:
+            return [to_iso639_2(x.language) for x in self.text_tracks]
+        return []
+
+    @property
+    def audio_languages(self) -> List[str]:
+        if self.audio_tracks:
+            return [to_iso639_2(x.language) for x in self.audio_tracks]
+        return []
+
+    @property
+    def dir_path(self) -> str:
         return self._dir_path
 
     @dir_path.setter
     def dir_path(self, value):
         self._dir_path = path.realpath(value)
 
     @property
-    def full_path(self):
+    def full_path(self) -> str:
         return path.join(self.dir_path, self.name)
 
     @property
     def codec(self):
         return self._codec
 
     @codec.setter
@@ -77,16 +94,20 @@
         """
         Reads the metadata for the given filename and path from the filesystem and saves it to this instance
         """
         if self._needs_refresh():
             log.debug(f"Refreshing data for video: {self.full_path}")
             self.size = self._get_size()
             metadata = MediaInfo.parse(self.full_path)
-            for track in metadata.tracks:
-                if track.track_type == "Video":
-                    self.quality = Validator().quality_similar_to(track)
-                    self.codec = Codec(format_name=track.format, )
-                    break
+            self.audio_tracks = metadata.audio_tracks  # type: ignore
+            self.text_tracks = metadata.text_tracks  # type: ignore
+            try:
+                self.video_track = metadata.video_tracks[0]  # type: ignore
+            except IndexError:
+                raise RuntimeError
+
+            self.quality = Validator().quality_similar_to(self.video_track)
+            self.codec = Codec(format_name=self.video_track.format)
             if self.quality == "Unknown":
                 error_message = f"Failed to parse track metadata from {self.full_path}"
                 log.error(error_message)
                 raise RuntimeError(error_message)
```

