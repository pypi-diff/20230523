# Comparing `tmp/smb3-video-autosplitter-0.2.0.tar.gz` & `tmp/smb3-video-autosplitter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smb3-video-autosplitter-0.2.0.tar", last modified: Thu May 18 13:49:18 2023, max compression
+gzip compressed data, was "smb3-video-autosplitter-0.3.0.tar", last modified: Tue May 23 21:03:04 2023, max compression
```

## Comparing `smb3-video-autosplitter-0.2.0.tar` & `smb3-video-autosplitter-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 13:49:18.991605 smb3-video-autosplitter-0.2.0/
--rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      555 2023-05-18 13:49:18.991605 smb3-video-autosplitter-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.2.0/README.rst
--rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.2.0/requirements_test.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 13:49:18.991605 smb3-video-autosplitter-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-05-18 13:48:52.000000 smb3-video-autosplitter-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 13:49:18.985600 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/
--rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-05-18 13:42:53.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/autosplitter.py
--rw-rw-rw-   0        0        0     1390 2023-05-18 13:20:19.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/livesplit.py
--rw-rw-rw-   0        0        0      767 2023-05-18 02:14:04.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/logging.py
--rw-rw-rw-   0        0        0     1636 2023-05-18 02:21:11.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/main.py
--rw-rw-rw-   0        0        0      774 2023-05-18 02:21:26.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/opencv.py
--rw-rw-rw-   0        0        0      791 2023-05-18 13:41:47.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/settings.py
--rw-rw-rw-   0        0        0     1552 2023-05-18 02:14:40.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 13:49:18.990604 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 13:49:12.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-23 21:03:04.194235 smb3-video-autosplitter-0.3.0/
+-rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      555 2023-05-23 21:03:04.193233 smb3-video-autosplitter-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.3.0/README.rst
+-rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.3.0/requirements_test.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 21:03:04.194235 smb3-video-autosplitter-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-05-23 21:02:47.000000 smb3-video-autosplitter-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 21:03:04.187228 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/
+-rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-05-23 20:54:55.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/autosplitter.py
+-rw-rw-rw-   0        0        0     1390 2023-05-18 13:20:19.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/livesplit.py
+-rw-rw-rw-   0        0        0      767 2023-05-18 02:14:04.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/logging.py
+-rw-rw-rw-   0        0        0     1701 2023-05-23 20:47:08.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/main.py
+-rw-rw-rw-   0        0        0     1314 2023-05-23 20:46:23.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/opencv.py
+-rw-rw-rw-   0        0        0      886 2023-05-23 20:46:43.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/settings.py
+-rw-rw-rw-   0        0        0     1552 2023-05-18 02:14:40.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 21:03:04.193233 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-23 21:03:04.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-05-23 21:03:04.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 21:03:04.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-23 21:03:04.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-23 21:03:04.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 21:02:57.000000 smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/zip-safe
```

### Comparing `smb3-video-autosplitter-0.2.0/LICENSE` & `smb3-video-autosplitter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.2.0/PKG-INFO` & `smb3-video-autosplitter-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.2.0/README.rst` & `smb3-video-autosplitter-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.2.0/setup.py` & `smb3-video-autosplitter-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="smb3-video-autosplitter",
-    version="0.2.0",
+    version="0.3.0",
     description=("Ingest video data to render smb3 eh manip stimuli"),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/autosplitter.py` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/autosplitter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 video based autosplitter for smb3
 """
 from dataclasses import dataclass
 import logging
 import time
+from typing import Optional
 
 import cv2
 
 from smb3_video_autosplitter.livesplit import Livesplit
 from smb3_video_autosplitter.settings import Settings
 from smb3_video_autosplitter.util import locate_all_opencv
 
@@ -16,48 +17,72 @@
 
 @dataclass
 class Split:
     path: str
     image: any
     region: list[int, int, int, int]
     command_name: str
+    split_offset_s: Optional[float] = 0
+    split_wait_s: Optional[float] = 0
+    description: Optional[str] = None
 
 
 class Autosplitter:
     def __init__(self, settings: Settings):
         self.settings = settings
         self.initialize_splits()
         self.earliest_next_trigger_time = 0
         self.livesplit = Livesplit()
-        self.split_offset_s = (settings.split_offset_frames * 16.64) / 1000
 
     def tick(self, frame):
         if frame is None or self.earliest_next_trigger_time >= time.time():
             return
-        for split in self.splits:
+        for split in self.candidate_splits:
             results = list(
                 locate_all_opencv(
                     split.image,
                     frame,
                     region=split.region,
                     confidence=self.settings.confidence,
                 )
             )
             if results:
-                time.sleep(self.split_offset_s)
-                self.earliest_next_trigger_time = (
-                    time.time() + self.settings.split_dedupe_wait_s
-                )
-                LOGGER.info(
-                    f"Splitting after {split.path} observed {len(results)} times at {list(map(str, results))}"
-                )
-                self.livesplit.send(split.command_name)
+                if self.settings.sequential:
+                    self.splits.pop(0)
+                self.handle_split_image_found(split, results)
+
+    def handle_split_image_found(self, split: Split, results):
+        sleep_duration = (
+            split.split_offset_s
+            if split.split_offset_s
+            else self.settings.split_offset_s_default
+        )
+        time.sleep(sleep_duration)
+        split_wait_s = (
+            split.split_wait_s
+            if split.split_wait_s
+            else self.settings.split_wait_s_default
+        )
+        self.earliest_next_trigger_time = time.time() + split_wait_s
+        LOGGER.info(
+            f"Splitting after {split.path} observed {len(results)} times at {list(map(str, results))}"
+        )
+        self.livesplit.send(split.command_name)
 
     def initialize_splits(self):
         self.splits: list[Split] = []
         for split in self.settings.splits:
             image = cv2.imread(split.path)
             region = [split.x, split.y, split.width, split.height]
             self.splits.append(Split(split.path, image, region, split.command_name))
 
+    @property
+    def candidate_splits(self):
+        if self.settings.sequential:
+            return [self.splits[0]]
+        return self.splits
+
+    def reset(self):
+        self.initialize_splits()
+
     def terminate(self):
         self.livesplit.terminate()
```

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/livesplit.py` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/livesplit.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/logging.py` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/logging.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/main.py` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,19 @@
 
 def main():
     initialize_logging(
         file_log_level=SETTINGS.file_log_level,
         console_log_level=SETTINGS.console_log_level,
     )
     print_camera_info()
-    opencv = OpenCV(SETTINGS.video_capture_source, SETTINGS.show_capture_video)
+    opencv = OpenCV(
+        SETTINGS.video_capture_source,
+        SETTINGS.show_capture_video,
+        SETTINGS.write_capture_video,
+    )
     try:
         autosplitter = Autosplitter(SETTINGS)
     except LivesplitConnectFailedException:
         LOGGER.warning("Failed to connect to livesplit, is it running?")
         exit()
     while True:
         opencv.tick()
```

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/opencv.py` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/opencv.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,34 @@
-from pygrabber.dshow_graph import FilterGraph
+from pygrabber.dshow_graph import FilterGraph, FilterType
 import cv2
 
 
 class OpenCV:
-    def __init__(self, video_capture_source, show_capture_video=False):
+    def __init__(
+        self, video_capture_source, show_capture_video=False, write_capture_video=False
+    ):
         self.show_capture_video = show_capture_video
+        self.write_capture_video = write_capture_video
         self.graph = FilterGraph()
         self.graph.add_video_input_device(video_capture_source)
         self.graph.add_sample_grabber(self.on_frame_received)
         self.graph.add_null_render()
         self.graph.prepare_preview_graph()
         self.graph.run()
         self.frame = None
+        if write_capture_video:
+            video_input = self.graph.filters[FilterType.video_input]
+            width, height = video_input.get_current_format()
+            self.output_video = cv2.VideoWriter(
+                "capture.avi", cv2.VideoWriter_fourcc(*"MPEG"), 60, (width, height)
+            )
 
     def tick(self):
         self.graph.grab_frame()
         if self.show_capture_video and self.frame is not None:
             cv2.imshow("capture", self.frame)
             _ = cv2.waitKey(1)
+        if self.write_capture_video and self.frame is not None:
+            self.output_video.write(self.frame)
 
     def on_frame_received(self, frame):
         self.frame = frame
```

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/util.py` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter/util.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/PKG-INFO` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/SOURCES.txt` & `smb3-video-autosplitter-0.3.0/smb3_video_autosplitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

