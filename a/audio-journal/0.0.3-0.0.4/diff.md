# Comparing `tmp/audio-journal-0.0.3.tar.gz` & `tmp/audio-journal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-journal-0.0.3.tar", last modified: Tue May 23 21:16:04 2023, max compression
+gzip compressed data, was "audio-journal-0.0.4.tar", last modified: Tue May 23 21:17:12 2023, max compression
```

## Comparing `audio-journal-0.0.3.tar` & `audio-journal-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:16:04.073003 audio-journal-0.0.3/
--rw-r--r--   0 kyle       (501) staff       (20)    11337 2023-05-18 23:36:04.000000 audio-journal-0.0.3/LICENSE
--rw-r--r--   0 kyle       (501) staff       (20)      141 2023-05-23 21:15:46.000000 audio-journal-0.0.3/MANIFEST.in
--rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:16:04.072871 audio-journal-0.0.3/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      104 2023-05-20 00:13:01.000000 audio-journal-0.0.3/README.md
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:16:04.071828 audio-journal-0.0.3/audio_journal/
--rw-r--r--   0 kyle       (501) staff       (20)       22 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/__init__.py
--rw-r--r--   0 kyle       (501) staff       (20)     2324 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/_modidx.py
--rw-r--r--   0 kyle       (501) staff       (20)     1200 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/config.py
--rw-r--r--   0 kyle       (501) staff       (20)      807 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/main.py
--rw-r--r--   0 kyle       (501) staff       (20)     1786 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/notion.py
--rw-r--r--   0 kyle       (501) staff       (20)     1923 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/record.py
--rw-r--r--   0 kyle       (501) staff       (20)      956 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/sounds.py
--rw-r--r--   0 kyle       (501) staff       (20)     1393 2023-05-23 19:48:37.000000 audio-journal-0.0.3/audio_journal/transcribe.py
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:16:04.072706 audio-journal-0.0.3/audio_journal.egg-info/
--rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:16:04.000000 audio-journal-0.0.3/audio_journal.egg-info/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      508 2023-05-23 21:16:04.000000 audio-journal-0.0.3/audio_journal.egg-info/SOURCES.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-23 21:16:04.000000 audio-journal-0.0.3/audio_journal.egg-info/dependency_links.txt
--rw-r--r--   0 kyle       (501) staff       (20)      115 2023-05-23 21:16:04.000000 audio-journal-0.0.3/audio_journal.egg-info/entry_points.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-18 23:47:02.000000 audio-journal-0.0.3/audio_journal.egg-info/not-zip-safe
--rw-r--r--   0 kyle       (501) staff       (20)       76 2023-05-23 21:16:04.000000 audio-journal-0.0.3/audio_journal.egg-info/requires.txt
--rw-r--r--   0 kyle       (501) staff       (20)       14 2023-05-23 21:16:04.000000 audio-journal-0.0.3/audio_journal.egg-info/top_level.txt
--rw-r--r--   0 kyle       (501) staff       (20)     1077 2023-05-23 21:15:52.000000 audio-journal-0.0.3/settings.ini
--rw-r--r--   0 kyle       (501) staff       (20)       38 2023-05-23 21:16:04.073044 audio-journal-0.0.3/setup.cfg
--rw-r--r--   0 kyle       (501) staff       (20)     2596 2023-05-18 23:36:04.000000 audio-journal-0.0.3/setup.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.542332 audio-journal-0.0.4/
+-rw-r--r--   0 kyle       (501) staff       (20)    11337 2023-05-18 23:36:04.000000 audio-journal-0.0.4/LICENSE
+-rw-r--r--   0 kyle       (501) staff       (20)      155 2023-05-23 21:17:06.000000 audio-journal-0.0.4/MANIFEST.in
+-rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:17:12.542126 audio-journal-0.0.4/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      104 2023-05-20 00:13:01.000000 audio-journal-0.0.4/README.md
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.539747 audio-journal-0.0.4/audio_journal/
+-rw-r--r--   0 kyle       (501) staff       (20)       22 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/__init__.py
+-rw-r--r--   0 kyle       (501) staff       (20)     2324 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/_modidx.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.541359 audio-journal-0.0.4/audio_journal/beeps/
+-rw-r--r--   0 kyle       (501) staff       (20)   116188 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/error.wav
+-rw-r--r--   0 kyle       (501) staff       (20)    24274 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/start.wav
+-rw-r--r--   0 kyle       (501) staff       (20)    30708 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/stop.wav
+-rw-r--r--   0 kyle       (501) staff       (20)  1186954 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/success.wav
+-rw-r--r--   0 kyle       (501) staff       (20)     1200 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/config.py
+-rw-r--r--   0 kyle       (501) staff       (20)      807 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/main.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1786 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/notion.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1923 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/record.py
+-rw-r--r--   0 kyle       (501) staff       (20)      956 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/sounds.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1393 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/transcribe.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.540715 audio-journal-0.0.4/audio_journal.egg-info/
+-rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      629 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle       (501) staff       (20)      115 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/entry_points.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-18 23:47:02.000000 audio-journal-0.0.4/audio_journal.egg-info/not-zip-safe
+-rw-r--r--   0 kyle       (501) staff       (20)       76 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/requires.txt
+-rw-r--r--   0 kyle       (501) staff       (20)       14 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/top_level.txt
+-rw-r--r--   0 kyle       (501) staff       (20)     1077 2023-05-23 21:16:51.000000 audio-journal-0.0.4/settings.ini
+-rw-r--r--   0 kyle       (501) staff       (20)       38 2023-05-23 21:17:12.542373 audio-journal-0.0.4/setup.cfg
+-rw-r--r--   0 kyle       (501) staff       (20)     2596 2023-05-18 23:36:04.000000 audio-journal-0.0.4/setup.py
```

### Comparing `audio-journal-0.0.3/LICENSE` & `audio-journal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/PKG-INFO` & `audio-journal-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-journal
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI tool to transcribe audio and store it in Notion
 Home-page: https://github.com/smith-kyle/audio-journal
 Author: Kyle Smith
 Author-email: kyle@gitnotebooks.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `audio-journal-0.0.3/audio_journal/_modidx.py` & `audio-journal-0.0.4/audio_journal/_modidx.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/audio_journal/config.py` & `audio-journal-0.0.4/audio_journal/config.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/audio_journal/main.py` & `audio-journal-0.0.4/audio_journal/main.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/audio_journal/notion.py` & `audio-journal-0.0.4/audio_journal/notion.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/audio_journal/record.py` & `audio-journal-0.0.4/audio_journal/record.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/audio_journal/sounds.py` & `audio-journal-0.0.4/audio_journal/sounds.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/audio_journal/transcribe.py` & `audio-journal-0.0.4/audio_journal/transcribe.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.3/audio_journal.egg-info/PKG-INFO` & `audio-journal-0.0.4/audio_journal.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-journal
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI tool to transcribe audio and store it in Notion
 Home-page: https://github.com/smith-kyle/audio-journal
 Author: Kyle Smith
 Author-email: kyle@gitnotebooks.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `audio-journal-0.0.3/settings.ini` & `audio-journal-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = audio-journal
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = audio_journal
```

### Comparing `audio-journal-0.0.3/setup.py` & `audio-journal-0.0.4/setup.py`

 * *Files identical despite different names*

