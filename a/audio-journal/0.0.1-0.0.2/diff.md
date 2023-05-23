# Comparing `tmp/audio-journal-0.0.1.tar.gz` & `tmp/audio-journal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-journal-0.0.1.tar", last modified: Fri May 19 23:11:50 2023, max compression
+gzip compressed data, was "audio-journal-0.0.2.tar", last modified: Tue May 23 21:11:08 2023, max compression
```

## Comparing `audio-journal-0.0.1.tar` & `audio-journal-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-19 23:11:50.523545 audio-journal-0.0.1/
--rw-r--r--   0 kyle       (501) staff       (20)    11337 2023-05-18 23:36:04.000000 audio-journal-0.0.1/LICENSE
--rw-r--r--   0 kyle       (501) staff       (20)      111 2023-05-18 23:36:04.000000 audio-journal-0.0.1/MANIFEST.in
--rw-r--r--   0 kyle       (501) staff       (20)     2213 2023-05-19 23:11:50.523371 audio-journal-0.0.1/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)     1391 2023-05-19 23:05:51.000000 audio-journal-0.0.1/README.md
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-19 23:11:50.522506 audio-journal-0.0.1/audio_journal/
--rw-r--r--   0 kyle       (501) staff       (20)       22 2023-05-19 23:07:38.000000 audio-journal-0.0.1/audio_journal/__init__.py
--rw-r--r--   0 kyle       (501) staff       (20)      433 2023-05-19 23:07:38.000000 audio-journal-0.0.1/audio_journal/_modidx.py
--rw-r--r--   0 kyle       (501) staff       (20)      645 2023-05-19 23:07:38.000000 audio-journal-0.0.1/audio_journal/main.py
--rw-r--r--   0 kyle       (501) staff       (20)     5384 2023-05-19 22:53:56.000000 audio-journal-0.0.1/audio_journal/old_main.py
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-19 23:11:50.523223 audio-journal-0.0.1/audio_journal.egg-info/
--rw-r--r--   0 kyle       (501) staff       (20)     2213 2023-05-19 23:11:50.000000 audio-journal-0.0.1/audio_journal.egg-info/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      410 2023-05-19 23:11:50.000000 audio-journal-0.0.1/audio_journal.egg-info/SOURCES.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-19 23:11:50.000000 audio-journal-0.0.1/audio_journal.egg-info/dependency_links.txt
--rw-r--r--   0 kyle       (501) staff       (20)      115 2023-05-19 23:11:50.000000 audio-journal-0.0.1/audio_journal.egg-info/entry_points.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-18 23:47:02.000000 audio-journal-0.0.1/audio_journal.egg-info/not-zip-safe
--rw-r--r--   0 kyle       (501) staff       (20)       85 2023-05-19 23:11:50.000000 audio-journal-0.0.1/audio_journal.egg-info/requires.txt
--rw-r--r--   0 kyle       (501) staff       (20)       14 2023-05-19 23:11:50.000000 audio-journal-0.0.1/audio_journal.egg-info/top_level.txt
--rw-r--r--   0 kyle       (501) staff       (20)     1086 2023-05-19 22:06:31.000000 audio-journal-0.0.1/settings.ini
--rw-r--r--   0 kyle       (501) staff       (20)       38 2023-05-19 23:11:50.523579 audio-journal-0.0.1/setup.cfg
--rw-r--r--   0 kyle       (501) staff       (20)     2596 2023-05-18 23:36:04.000000 audio-journal-0.0.1/setup.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:11:08.207532 audio-journal-0.0.2/
+-rw-r--r--   0 kyle       (501) staff       (20)    11337 2023-05-18 23:36:04.000000 audio-journal-0.0.2/LICENSE
+-rw-r--r--   0 kyle       (501) staff       (20)      111 2023-05-18 23:36:04.000000 audio-journal-0.0.2/MANIFEST.in
+-rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:11:08.207385 audio-journal-0.0.2/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      104 2023-05-20 00:13:01.000000 audio-journal-0.0.2/README.md
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:11:08.206307 audio-journal-0.0.2/audio_journal/
+-rw-r--r--   0 kyle       (501) staff       (20)       22 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/__init__.py
+-rw-r--r--   0 kyle       (501) staff       (20)     2324 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/_modidx.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1200 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/config.py
+-rw-r--r--   0 kyle       (501) staff       (20)      807 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/main.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1786 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/notion.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1923 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/record.py
+-rw-r--r--   0 kyle       (501) staff       (20)      956 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/sounds.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1393 2023-05-23 19:48:37.000000 audio-journal-0.0.2/audio_journal/transcribe.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:11:08.207207 audio-journal-0.0.2/audio_journal.egg-info/
+-rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:11:08.000000 audio-journal-0.0.2/audio_journal.egg-info/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      508 2023-05-23 21:11:08.000000 audio-journal-0.0.2/audio_journal.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-23 21:11:08.000000 audio-journal-0.0.2/audio_journal.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle       (501) staff       (20)      115 2023-05-23 21:11:08.000000 audio-journal-0.0.2/audio_journal.egg-info/entry_points.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-18 23:47:02.000000 audio-journal-0.0.2/audio_journal.egg-info/not-zip-safe
+-rw-r--r--   0 kyle       (501) staff       (20)       76 2023-05-23 21:11:08.000000 audio-journal-0.0.2/audio_journal.egg-info/requires.txt
+-rw-r--r--   0 kyle       (501) staff       (20)       14 2023-05-23 21:11:08.000000 audio-journal-0.0.2/audio_journal.egg-info/top_level.txt
+-rw-r--r--   0 kyle       (501) staff       (20)     1077 2023-05-23 21:11:04.000000 audio-journal-0.0.2/settings.ini
+-rw-r--r--   0 kyle       (501) staff       (20)       38 2023-05-23 21:11:08.207569 audio-journal-0.0.2/setup.cfg
+-rw-r--r--   0 kyle       (501) staff       (20)     2596 2023-05-18 23:36:04.000000 audio-journal-0.0.2/setup.py
```

### Comparing `audio-journal-0.0.1/LICENSE` & `audio-journal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.1/settings.ini` & `audio-journal-0.0.2/settings.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = audio-journal
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = audio_journal
@@ -34,10 +34,10 @@
 description = CLI tool to transcribe audio and store it in Notion
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = smith-kyle
 
 ### Optional ###
-requirements = keyboard sounddevice notion_client openai-whisper load_dotenv soundfile pydub
+requirements = sounddevice notion_client openai-whisper load_dotenv soundfile pydub
 # dev_requirements = 
 console_scripts = audio_journal_start=audio_journal.main:start
```

### Comparing `audio-journal-0.0.1/setup.py` & `audio-journal-0.0.2/setup.py`

 * *Files identical despite different names*

