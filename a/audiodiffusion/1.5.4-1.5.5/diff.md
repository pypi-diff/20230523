# Comparing `tmp/audiodiffusion-1.5.4.tar.gz` & `tmp/audiodiffusion-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiodiffusion-1.5.4.tar", last modified: Wed May 17 15:16:42 2023, max compression
+gzip compressed data, was "audiodiffusion-1.5.5.tar", last modified: Tue May 23 13:40:14 2023, max compression
```

## Comparing `audiodiffusion-1.5.4.tar` & `audiodiffusion-1.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.4/LICENSE
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.4/README.md
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-17 15:16:42.695539 audiodiffusion-1.5.4/audiodiffusion/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-05-17 15:13:51.000000 audiodiffusion-1.5.4/audiodiffusion/__init__.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     3490 2022-12-24 15:06:00.000000 audiodiffusion-1.5.4/audiodiffusion/audio_encoder.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5680 2023-05-17 15:12:31.000000 audiodiffusion-1.5.4/audiodiffusion/mel.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    10809 2023-04-22 08:29:21.000000 audiodiffusion-1.5.4/audiodiffusion/pipeline_audio_diffusion.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.4/audiodiffusion/utils.py
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/audiodiffusion.egg-info/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/SOURCES.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/dependency_links.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/not-zip-safe
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/requires.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/top_level.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.4/pyproject.toml
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/setup.cfg
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.4/setup.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-23 13:40:14.824090 audiodiffusion-1.5.5/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.5/LICENSE
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-23 13:40:14.824090 audiodiffusion-1.5.5/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.5/README.md
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-23 13:40:14.816090 audiodiffusion-1.5.5/audiodiffusion/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-05-23 13:39:29.000000 audiodiffusion-1.5.5/audiodiffusion/__init__.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     3738 2023-05-23 13:33:43.000000 audiodiffusion-1.5.5/audiodiffusion/audio_encoder.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5680 2023-05-17 15:12:31.000000 audiodiffusion-1.5.5/audiodiffusion/mel.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    10809 2023-04-22 08:29:21.000000 audiodiffusion-1.5.5/audiodiffusion/pipeline_audio_diffusion.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.5/audiodiffusion/utils.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-23 13:40:14.820090 audiodiffusion-1.5.5/audiodiffusion.egg-info/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/not-zip-safe
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/requires.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.5/pyproject.toml
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-05-23 13:40:14.824090 audiodiffusion-1.5.5/setup.cfg
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.5/setup.py
```

### Comparing `audiodiffusion-1.5.4/LICENSE` & `audiodiffusion-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.4/PKG-INFO` & `audiodiffusion-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.4
+Version: 1.5.5
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

### Comparing `audiodiffusion-1.5.4/README.md` & `audiodiffusion-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.4/audiodiffusion/__init__.py` & `audiodiffusion-1.5.5/audiodiffusion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from librosa.beat import beat_track
 from PIL import Image
 from tqdm.auto import tqdm
 
 # from diffusers import AudioDiffusionPipeline
 from .pipeline_audio_diffusion import AudioDiffusionPipeline
 
-VERSION = "1.5.4"
+VERSION = "1.5.5"
 
 
 class AudioDiffusion:
     def __init__(
         self,
         model_id: str = "teticio/audio-diffusion-256",
         cuda: bool = torch.cuda.is_available(),
```

### Comparing `audiodiffusion-1.5.4/audiodiffusion/audio_encoder.py` & `audiodiffusion-1.5.5/audiodiffusion/audio_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,30 +78,36 @@
         for conv_block in self.conv_blocks:
             x = conv_block(x)
         x = self.dense_block(x)
         x = self.embedding(x)
         return x
 
     @torch.no_grad()
-    def encode(self, audio_files):
+    def encode(self, audio_files, pool="average"):
         self.eval()
         y = []
         for audio_file in audio_files:
             self.mel.load_audio(audio_file)
             x = [
                 np.expand_dims(
                     np.frombuffer(self.mel.audio_slice_to_image(slice).tobytes(), dtype="uint8").reshape(
                         (self.mel.y_res, self.mel.x_res)
                     )
                     / 255,
                     axis=0,
                 )
                 for slice in range(self.mel.get_number_of_slices())
             ]
-            y += [torch.mean(self(torch.Tensor(x)), dim=0)]
+            y += [self(torch.Tensor(x))]
+            if pool == "average":
+                y[-1] = torch.mean(y[-1], dim=0)
+            elif pool == "max":
+                y[-1] = torch.max(y[-1], dim=0)
+            else:
+                assert pool is None, f"Unknown pooling method {pool}"
         return torch.stack(y)
 
 
 # from diffusers import Mel
 # from audiodiffusion.audio_encoder import AudioEncoder
 # audio_encoder = AudioEncoder.from_pretrained("teticio/audio-encoder")
 # audio_encoder.encode(['/home/teticio/Music/liked/Agua Re - Holy Dance - Large Sound Mix.mp3'])
```

### Comparing `audiodiffusion-1.5.4/audiodiffusion/mel.py` & `audiodiffusion-1.5.5/audiodiffusion/mel.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.4/audiodiffusion/pipeline_audio_diffusion.py` & `audiodiffusion-1.5.5/audiodiffusion/pipeline_audio_diffusion.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.4/audiodiffusion/utils.py` & `audiodiffusion-1.5.5/audiodiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.4/audiodiffusion.egg-info/PKG-INFO` & `audiodiffusion-1.5.5/audiodiffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.4
+Version: 1.5.5
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

