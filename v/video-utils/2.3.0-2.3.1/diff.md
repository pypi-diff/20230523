# Comparing `tmp/video_utils-2.3.0.tar.gz` & `tmp/video_utils-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_utils-2.3.0.tar", max compression
+gzip compressed data, was "video_utils-2.3.1.tar", max compression
```

## Comparing `video_utils-2.3.0.tar` & `video_utils-2.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-23 10:41:51.500130 video_utils-2.3.0/LICENSE.md
--rw-r--r--   0        0        0     1368 2023-05-23 10:41:51.500130 video_utils-2.3.0/README.md
--rw-r--r--   0        0        0      744 2023-05-23 10:41:51.500130 video_utils-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      166 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/__init__.py
--rw-r--r--   0        0        0     1627 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/codec.py
--rw-r--r--   0        0        0      259 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/colour.py
--rw-r--r--   0        0        0     5367 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/fileMap.py
--rw-r--r--   0        0        0      868 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/parse_episode.py
--rw-r--r--   0        0        0     1549 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/validators.py
--rw-r--r--   0        0        0     3437 2023-05-23 10:41:51.504130 video_utils-2.3.0/video_utils/video.py
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 video_utils-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-23 11:07:11.915122 video_utils-2.3.1/LICENSE.md
+-rw-r--r--   0        0        0     1368 2023-05-23 11:07:11.915122 video_utils-2.3.1/README.md
+-rw-r--r--   0        0        0      744 2023-05-23 11:07:11.915122 video_utils-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/__init__.py
+-rw-r--r--   0        0        0     1802 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/codec.py
+-rw-r--r--   0        0        0      274 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/colour.py
+-rw-r--r--   0        0        0     5661 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/fileMap.py
+-rw-r--r--   0        0        0      962 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/parse_episode.py
+-rw-r--r--   0        0        0     1549 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/validators.py
+-rw-r--r--   0        0        0     3811 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/video.py
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 video_utils-2.3.1/PKG-INFO
```

### Comparing `video_utils-2.3.0/LICENSE.md` & `video_utils-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.0/README.md` & `video_utils-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.0/pyproject.toml` & `video_utils-2.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video_utils"
-version = "2.3.0"
+version = "2.3.1"
 description = "This library is used for lots of shared functionality around parsing TV shows and movies"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `video_utils-2.3.0/video_utils/codec.py` & `video_utils-2.3.1/video_utils/codec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,52 @@
+from typing import Optional
+
 # TODO: Add automatic creation of additional info about codecs to here instead of validators?
 
 # Key is the codec format returned by MediaInfo
 CODEC_DATA = {
     "AV1": {"ffmpeg_names": {"software": "libaom-av1"}, "pretty_name": "av1"},
     "HEVC": {"ffmpeg_names": {"software": "libx265", "nvidia": "hevc_nvenc", "intel": "hevc_qsv"}, "pretty_name": "x265"},
     "AVC": {"ffmpeg_names": {"software": "h264", "nvidia": "h264_nvenc", "intel": "h264_qsv"}, "pretty_name": "x264"},
     "AAC": {"ffmpeg_names": {"software": "aac"}, "pretty_name": "aac"},
 }
 
 
 class Codec:
-
-    def __init__(self, format_name, ffmpeg_name=None, pretty_name=None):
+    def __init__(
+        self,
+        format_name: str,
+        ffmpeg_name: Optional[str] = None,
+        pretty_name: Optional[str] = None
+    ) -> None:
         self.format_name = format_name
         self._ffmpeg_name = ffmpeg_name
         self.pretty_name = pretty_name
         self._autodetect()
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Codec):
             # don't attempt to compare against unrelated types
             return NotImplemented
 
         return self.format_name == other.format_name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<Codec format_name={self.format_name}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.__repr__()
 
-    def _autodetect(self):
+    def _autodetect(self) -> None:
         try:
             self._data = CODEC_DATA[self.format_name]
             self.pretty_name = self.pretty_name if self.pretty_name else self._data["pretty_name"]
         except KeyError:
             pass  # No match found
 
-    def get_ffmpeg_name(self, encoder="software"):
+    def get_ffmpeg_name(self, encoder: str = "software") -> Optional[str]:
         if self._ffmpeg_name:
             return self._ffmpeg_name
         try:
             return self._data["ffmpeg_names"][encoder]
         except:
             return None
```

### Comparing `video_utils-2.3.0/video_utils/fileMap.py` & `video_utils-2.3.1/video_utils/fileMap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,73 @@
-#!/usr/bin/env python3
-
 from copy import deepcopy
 import logging
 import os
 from os import path
 import hashlib
 import pickle
 from rich.progress import track
+from typing import Dict, List
 
 from .colour import colour
 from .validators import Filter
 from .video import Video
 
 log = logging.getLogger(__name__)
 
 
 class FileMap:
-    def __init__(self, directory, update=True, use_cache=True, progress_bar=True):
+    def __init__(self, directory: str, update: bool = True, use_cache: bool = True, progress_bar: bool = True):
         """
         update and use_cache values are only honoured on object initialization
         """
-        self.directory = directory
-        self._update = update
-        self._use_cache = use_cache
-        self._progress_bar = progress_bar
-        self.contents = {}
-        self._validate_settings(update=self.update, use_cache=self.use_cache)
+        self.directory: str = directory
+        self._update: bool = update
+        self._use_cache: bool = use_cache
+        self._progress_bar: bool = progress_bar
+        self.contents: Dict[str, List[Video]] = {}
+        self._validate_settings(update=self._update, use_cache=self._use_cache)
 
     @property
-    def directory(self):
+    def directory(self) -> str:
         return self._directory
 
     @directory.setter
-    def directory(self, value):
+    def directory(self, value: str) -> None:
         self._directory = path.realpath(value)
 
     @property
-    def update(self):
+    def update(self) -> bool:
         return self._update
 
     @update.setter
-    def update(self, value):
+    def update(self, value: bool) -> None:
         self._validate_settings(update=value, use_cache=self.use_cache)
         self._update = value
 
     @property
-    def use_cache(self):
+    def use_cache(self) -> bool:
         return self._use_cache
 
     @use_cache.setter
-    def use_cache(self, value):
+    def use_cache(self, value: bool) -> None:
         self._validate_settings(update=self.update, use_cache=value)
         self._use_cache = value
 
-    def _validate_settings(self, update, use_cache):
+    def _validate_settings(self, update: bool, use_cache: bool) -> None:
         if not update and not use_cache:
-            raise AttributeError(
-                "At least one of update or use_cache must be True")
+            raise AttributeError("At least one of update or use_cache must be True")
 
-    def load(self):
+    def load(self) -> None:
         storage = _FileMapStorage(self.directory)
         self.contents = storage.load(self.use_cache)
         if self.update:
             self._update_content()
         storage.save(self.contents)
 
-    def _update_content(self):
+    def _update_content(self) -> None:
         """
         Update the contents of this filemap
         """
         log.debug("Updating contents...")
         filter = Filter()
         if self.use_cache:
             self._prune_missing_files()
@@ -81,40 +79,40 @@
 
             if self._progress_bar:
                 video_files = track(video_files)
 
             for video_file in video_files:
                 self._update_video(dir_path, video_file)
 
-    def _update_video(self, dir_path, video_name):
+    def _update_video(self, dir_path: str, video_name: str) -> None:
         if dir_path not in self.contents:
             self.contents[dir_path] = []
 
         video = Video(name=video_name, dir_path=dir_path)
         if video in self.contents[dir_path]:
             log.debug(
                 f"Video ({video.full_path} already in cache. Checking for updates and replacing...)")
             video = next(i for i in self.contents[dir_path] if i == video)
             self.contents[dir_path].remove(video)
         video.refresh()
         self.contents[dir_path].append(video)
 
-    def _video_needs_refreshing(self, video):
+    def _video_needs_refreshing(self, video: Video) -> None:
         pass
 
     def _file_tree(self):
         if path.isfile(self.directory):
             log.debug("Provided directory is a file, not a directory")
             file_tree = [(path.dirname(self.directory), [],
                           [path.basename(self.directory)])]
         else:
             file_tree = os.walk(self.directory, followlinks=True)
         return file_tree
 
-    def _prune_missing_files(self):
+    def _prune_missing_files(self) -> None:
         log.info(colour("blue", "Checking for missing/deleted files..."))
         # Can't mutate the original while we iterate through it
         contents_copy = deepcopy(self.contents)
         for dir_path in contents_copy:
             log.info(colour("blue", f"Processing directory {dir_path}"))
 
             if not path.exists(dir_path):
@@ -129,34 +127,34 @@
             for video in sub_directory:
                 if not path.exists(video.full_path):
                     log.debug("Removing %s from cache" % video.full_path)
                     self.contents[dir_path].remove(video)
 
 
 class _FileMapStorage:
-    def __init__(self, directory):
+    def __init__(self, directory: str) -> None:
         self.directory = directory
 
-    def load(self, use_cache=True):
+    def load(self, use_cache: bool = True) -> Dict[str, List[Video]]:
         data = {}
         if use_cache:
             if path.exists(self.storage_path):
                 log.debug("Loading from cache...")
                 try:
                     with open(self.storage_path, 'rb') as f:
                         data = pickle.load(f)
                 except EOFError:
                     log.error(
                         f"Failed to load cache! Likely a corrupt cache file ({self.storage_path}). Ignoring cache...")
         return data
 
-    def save(self, data):
+    def save(self, data: Dict[str, List[Video]]) -> None:
         log.debug("Saving out filemap...")
         with open(self.storage_path, 'wb') as f:
             pickle.dump(data, f)
 
     @property
-    def storage_path(self):
+    def storage_path(self) -> str:
         storage_path = path.join(path.expanduser("~"), ".local", "share", "video_utils")
         os.makedirs(storage_path, exist_ok=True)
         name = hashlib.md5(bytes(self.directory, 'ascii')).hexdigest()
         return path.join(storage_path, name)
```

### Comparing `video_utils-2.3.0/video_utils/parse_episode.py` & `video_utils-2.3.1/video_utils/parse_episode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 import re
 import logging
+from typing import Optional, Tuple, Dict
 
 log = logging.getLogger(__name__)
 
 
-def _split_data(filename):
+def _split_data(filename: str) -> Tuple[str, str, str, str]:
     results = re.findall(
         r"(.*?)\ ?(?:\-\ ?)?\[?(?:[Ss](?=\d+[eE]\d+))?(\d+)[XxeE](\d+)\]?(?:\ ?\-)?\ ?(.*)", filename)
     if results:
         return results[0]
-    return (None, None, None, None)
+    raise ValueError
 
 
-def parse_episode(filename):
+def parse_episode(filename: str) -> Dict[str, Optional[str]]:
     shortname = os.path.basename(filename)
     shortname = os.path.splitext(shortname)[0]
     showName, season, episode, episodeName = _split_data(shortname)
+
     try:
         season = int(season)
         episode = int(episode)
     except TypeError:
         log.debug("Failed to parse season or episode number")
     result = {
         "showName": showName,
```

### Comparing `video_utils-2.3.0/video_utils/validators.py` & `video_utils-2.3.1/video_utils/validators.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.0/video_utils/video.py` & `video_utils-2.3.1/video_utils/video.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 import logging
 import os
 from os import path
-from typing import List
+from typing import List, Optional
 
 from pymediainfo import MediaInfo
 from iso639 import to_iso639_2
 
 from .validators import Validator
 from .codec import Codec
 
 log = logging.getLogger(__name__)
 
 
 class Video:
-    def __init__(self, name, dir_path, codec=None, quality=None, size=None, video_track=None, audio_tracks=None, text_tracks=None):
+    def __init__(
+        self,
+        name: str,
+        dir_path: str,
+        codec: Optional[Codec] = None,
+        quality: Optional[str] = None,
+        size: Optional[int] = None,
+        video_track: Optional[object] = None,
+        audio_tracks: Optional[List[object]] = None,
+        text_tracks: Optional[List[object]] = None,
+    ):
         self.name = name
         self.dir_path = dir_path
         self.codec = codec
         self.quality = quality
         self.size = size
         self.video_track = video_track
         self.audio_tracks = audio_tracks
         self.text_tracks = text_tracks
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Video):
             # don't attempt to compare against unrelated types
             return NotImplemented
 
         return self.full_path == other.full_path
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<Video name={self.name} codec={self.codec} quality={self.quality}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.__repr__()
 
     @property
     def subtitle_languages(self) -> List[str]:
         if self.text_tracks:
             return [to_iso639_2(x.language) for x in self.text_tracks]
         return []
@@ -49,52 +59,52 @@
         return []
 
     @property
     def dir_path(self) -> str:
         return self._dir_path
 
     @dir_path.setter
-    def dir_path(self, value):
+    def dir_path(self, value: str) -> None:
         self._dir_path = path.realpath(value)
 
     @property
     def full_path(self) -> str:
         return path.join(self.dir_path, self.name)
 
     @property
-    def codec(self):
+    def codec(self) -> Optional[Codec]:
         return self._codec
 
     @codec.setter
-    def codec(self, value):
+    def codec(self, value: Optional[Codec]) -> None:
         if value is not None and not isinstance(value, Codec):
             raise TypeError("An object of type Codec must be specified")
         self._codec = value
 
     @property
-    def quality(self):
+    def quality(self) -> Optional[str]:
         return self._quality
 
     @quality.setter
-    def quality(self, value):
+    def quality(self, value: Optional[str]) -> None:
         if value is None:
             value = "Unknown"
         Validator().quality(value)
         self._quality = value
 
-    def _needs_refresh(self):
+    def _needs_refresh(self) -> bool:
         if self.size != self._get_size():
             return True
         log.debug(f"Skipping refresh on '{self.full_path}'")
         return False
 
-    def _get_size(self):
+    def _get_size(self) -> int:
         return os.stat(self.full_path).st_size
 
-    def refresh(self):
+    def refresh(self) -> None:
         """
         Reads the metadata for the given filename and path from the filesystem and saves it to this instance
         """
         if self._needs_refresh():
             log.debug(f"Refreshing data for video: {self.full_path}")
             self.size = self._get_size()
             metadata = MediaInfo.parse(self.full_path)
```

### Comparing `video_utils-2.3.0/PKG-INFO` & `video_utils-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-utils
-Version: 2.3.0
+Version: 2.3.1
 Summary: This library is used for lots of shared functionality around parsing TV shows and movies
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

