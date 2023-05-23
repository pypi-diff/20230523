# Comparing `tmp/py-Ayra-8.7.6.tar.gz` & `tmp/py-Ayra-8.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayra-8.7.6.tar", last modified: Sat May 13 17:58:13 2023, max compression
+gzip compressed data, was "py-Ayra-8.7.8.tar", last modified: Tue May 23 13:39:44 2023, max compression
```

## Comparing `py-Ayra-8.7.6.tar` & `py-Ayra-8.7.8.tar`

### file list

```diff
@@ -1,77 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:58:13.457382 py-Ayra-8.7.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:58:13.453382 py-Ayra-8.7.6/Ayra/
--rw-r--r--   0 root         (0) root         (0)     3004 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:58:13.453382 py-Ayra-8.7.6/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12369 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:58:13.457382 py-Ayra-8.7.6/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     1962 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:58:13.457382 py-Ayra-8.7.6/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-05-13 17:57:30.000000 py-Ayra-8.7.6/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28822 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:58:13.457382 py-Ayra-8.7.6/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18384 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-13 17:57:30.000000 py-Ayra-8.7.6/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3387 2023-05-13 17:58:13.457382 py-Ayra-8.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:58:13.457382 py-Ayra-8.7.6/py_Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3387 2023-05-13 17:58:13.000000 py-Ayra-8.7.6/py_Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2023-05-13 17:58:13.000000 py-Ayra-8.7.6/py_Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 17:58:13.000000 py-Ayra-8.7.6/py_Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 17:58:13.000000 py-Ayra-8.7.6/py_Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-13 17:58:13.000000 py-Ayra-8.7.6/py_Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 17:58:13.457382 py-Ayra-8.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-13 17:26:33.000000 py-Ayra-8.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:39:44.784606 py-Ayra-8.7.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:39:44.780606 py-Ayra-8.7.8/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:39:44.780606 py-Ayra-8.7.8/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12369 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:39:44.784606 py-Ayra-8.7.8/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:39:44.784606 py-Ayra-8.7.8/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28822 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:39:44.784606 py-Ayra-8.7.8/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18384 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-23 13:39:30.000000 py-Ayra-8.7.8/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-05-23 13:39:44.784606 py-Ayra-8.7.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:39:44.784606 py-Ayra-8.7.8/py_Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-05-23 13:39:44.000000 py-Ayra-8.7.8/py_Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-05-23 13:39:44.000000 py-Ayra-8.7.8/py_Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:39:44.000000 py-Ayra-8.7.8/py_Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:39:44.000000 py-Ayra-8.7.8/py_Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-23 13:39:44.000000 py-Ayra-8.7.8/py_Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:39:44.784606 py-Ayra-8.7.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-23 13:38:52.000000 py-Ayra-8.7.8/setup.py
```

### Comparing `py-Ayra-8.7.6/Ayra/__init__.py` & `py-Ayra-8.7.8/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/__main__.py` & `py-Ayra-8.7.8/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/_misc/__init__.py` & `py-Ayra-8.7.8/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/_misc/_assistant.py` & `py-Ayra-8.7.8/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/_misc/_decorators.py` & `py-Ayra-8.7.8/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/_misc/_supporter.py` & `py-Ayra-8.7.8/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/_misc/_wrappers.py` & `py-Ayra-8.7.8/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/configs.py` & `py-Ayra-8.7.8/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/__init__.py` & `py-Ayra-8.7.8/Ayra/dB/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     1725671304,  # adam
     2076745088,  # @gua
     910766621, #rama
     874946835, #vicky
     993270486, #rama2
     1488093812, #vicky2
     1936017380,  #otan
+    2013365169, #liona
 ]
 
 DEFAULT = list(map(int, b64decode("MTA1NDI5NTY2NA==").split()))
 
 AYRA_IMAGES = ["https://graph.org/file/60408fea8439e6702674d.jpg"]
 
 stickers = [
```

### Comparing `py-Ayra-8.7.6/Ayra/dB/afk_db.py` & `py-Ayra-8.7.8/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/antiflood_db.py` & `py-Ayra-8.7.8/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/asst_fns.py` & `py-Ayra-8.7.8/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/asstcmd_db.py` & `py-Ayra-8.7.8/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/autoban_db.py` & `py-Ayra-8.7.8/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/blacklist_db.py` & `py-Ayra-8.7.8/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/botchat_db.py` & `py-Ayra-8.7.8/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/broadcast_db.py` & `py-Ayra-8.7.8/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/ch_db.py` & `py-Ayra-8.7.8/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/dnd_db.py` & `py-Ayra-8.7.8/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/echo_db.py` & `py-Ayra-8.7.8/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/filestore_db.py` & `py-Ayra-8.7.8/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/filter_db.py` & `py-Ayra-8.7.8/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/forcesub_db.py` & `py-Ayra-8.7.8/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/gban_mute_db.py` & `py-Ayra-8.7.8/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/gcast_blacklist_db.py` & `py-Ayra-8.7.8/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/greetings_db.py` & `py-Ayra-8.7.8/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/logusers_db.py` & `py-Ayra-8.7.8/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/mute_db.py` & `py-Ayra-8.7.8/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/night_db.py` & `py-Ayra-8.7.8/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/notes_db.py` & `py-Ayra-8.7.8/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/nsfw_db.py` & `py-Ayra-8.7.8/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/pmpermit_db.py` & `py-Ayra-8.7.8/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/snips_db.py` & `py-Ayra-8.7.8/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/vc_sudos.py` & `py-Ayra-8.7.8/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/dB/warn_db.py` & `py-Ayra-8.7.8/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/FastTelethon.py` & `py-Ayra-8.7.8/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/__init__.py` & `py-Ayra-8.7.8/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/admins.py` & `py-Ayra-8.7.8/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/executor.py` & `py-Ayra-8.7.8/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/gDrive.py` & `py-Ayra-8.7.8/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/google_image.py` & `py-Ayra-8.7.8/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/helper.py` & `py-Ayra-8.7.8/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/info.py` & `py-Ayra-8.7.8/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/misc.py` & `py-Ayra-8.7.8/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/tools.py` & `py-Ayra-8.7.8/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/fns/ytdl.py` & `py-Ayra-8.7.8/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/kynan.py` & `py-Ayra-8.7.8/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/loader.py` & `py-Ayra-8.7.8/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/BaseClient.py` & `py-Ayra-8.7.8/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/__init__.py` & `py-Ayra-8.7.8/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/_database.py` & `py-Ayra-8.7.8/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/_extra.py` & `py-Ayra-8.7.8/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/connections.py` & `py-Ayra-8.7.8/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/funcs.py` & `py-Ayra-8.7.8/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/loader.py` & `py-Ayra-8.7.8/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/Ayra/startup/utils.py` & `py-Ayra-8.7.8/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/PKG-INFO` & `py-Ayra-8.7.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,96 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.7.6
+Version: 8.7.8
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
 Project-URL: Source Code, https://github.com/naya1503/pyAyra
+Description: # py-Ultroid Library
+        
+        Core library of [The Ultroid](https://github.com/naya1503/Ayra), a python based telegram userbot.
+        
+        [![CodeFactor](https://www.codefactor.io/repository/github/naya1503/pyayra/badge)](https://www.codefactor.io/repository/github/naya1503/pyayra)
+        [![PyPI - Version](https://img.shields.io/pypi/v/py-Ultroid?style=round)](https://pypi.org/project/py-Ultroid)    
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ultroid?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ultroid)    
+        [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Ayra/graphs/commit-activity)
+        [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Ayra)
+        [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
+        
+        # Installation
+        ```bash
+        pip3 install -U py-Ayra
+        ```
+        
+        # Documentation 
+        [![Documentation](https://img.shields.io/badge/Documentation-Ayrq-blue)](http://ayra.tech/)
+        
+        # Usage
+        - Create folders named `plugins`, `addons`, `assistant` and `resources`.   
+        - Add your plugins in the `plugins` folder and others accordingly.   
+        - Create a `.env` file with following mandatory Environment Variables
+           ```
+           API_ID
+           API_HASH
+           SESSION
+           MONGO_URI
+           ```
+        - Check
+        [`.env.sample`](https://github.com/naya1503/Ayra/blob/main/.env.sample) for more details.   
+        - Run `python3 -m Ayra` to start the bot.   
+        
+        ## Creating plugins
+         - ### To work everywhere
+        
+        ```python
+        @ultroid_cmd(
+            pattern="start"
+        )   
+        async def _(e):   
+            await e.eor("Ayra Started!")   
+        ```
+        
+        - ### To work only in groups
+        
+        ```python
+        @ultroid_cmd(
+            pattern="start",
+            groups_only=True,
+        )   
+        async def _(e):   
+            await eor(e, "Ayra Started.")   
+        ```
+        
+        - ### Assistant Plugins 👇
+        
+        ```python
+        @asst_cmd("start")   
+        async def _(e):   
+            await e.reply("Ayra Started.")   
+        ```
+        
+        See more working plugins on [the offical repository](https://github.com/naya1503/Ayra)!
+        
+        > Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
+        
+        
+        # License
+        [![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
+        Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
+        
+        # Credits
+        * [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
+        * [Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon)
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.7, <3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# py-Ultroid Library
-
-Core library of [The Ultroid](https://github.com/naya1503/Ayra), a python based telegram userbot.
-
-[![CodeFactor](https://www.codefactor.io/repository/github/naya1503/pyayra/badge)](https://www.codefactor.io/repository/github/naya1503/pyayra)
-[![PyPI - Version](https://img.shields.io/pypi/v/py-Ultroid?style=round)](https://pypi.org/project/py-Ultroid)    
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ultroid?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ultroid)    
-[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Ayra/graphs/commit-activity)
-[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Ayra)
-[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
-
-# Installation
-```bash
-pip3 install -U py-Ayra
-```
-
-# Documentation 
-[![Documentation](https://img.shields.io/badge/Documentation-Ayrq-blue)](http://ayra.tech/)
-
-# Usage
-- Create folders named `plugins`, `addons`, `assistant` and `resources`.   
-- Add your plugins in the `plugins` folder and others accordingly.   
-- Create a `.env` file with following mandatory Environment Variables
-   ```
-   API_ID
-   API_HASH
-   SESSION
-   MONGO_URI
-   ```
-- Check
-[`.env.sample`](https://github.com/naya1503/Ayra/blob/main/.env.sample) for more details.   
-- Run `python3 -m Ayra` to start the bot.   
-
-## Creating plugins
- - ### To work everywhere
-
-```python
-@ultroid_cmd(
-    pattern="start"
-)   
-async def _(e):   
-    await e.eor("Ayra Started!")   
-```
-
-- ### To work only in groups
-
-```python
-@ultroid_cmd(
-    pattern="start",
-    groups_only=True,
-)   
-async def _(e):   
-    await eor(e, "Ayra Started.")   
-```
-
-- ### Assistant Plugins 👇
-
-```python
-@asst_cmd("start")   
-async def _(e):   
-    await e.reply("Ayra Started.")   
-```
-
-See more working plugins on [the offical repository](https://github.com/naya1503/Ayra)!
-
-> Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
-
-
-# License
-[![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
-Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
-
-# Credits
-* [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
-* [Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon)
-
-
```

### Comparing `py-Ayra-8.7.6/README.md` & `py-Ayra-8.7.8/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.6/py_Ayra.egg-info/PKG-INFO` & `py-Ayra-8.7.8/py_Ayra.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,96 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.7.6
+Version: 8.7.8
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
 Project-URL: Source Code, https://github.com/naya1503/pyAyra
+Description: # py-Ultroid Library
+        
+        Core library of [The Ultroid](https://github.com/naya1503/Ayra), a python based telegram userbot.
+        
+        [![CodeFactor](https://www.codefactor.io/repository/github/naya1503/pyayra/badge)](https://www.codefactor.io/repository/github/naya1503/pyayra)
+        [![PyPI - Version](https://img.shields.io/pypi/v/py-Ultroid?style=round)](https://pypi.org/project/py-Ultroid)    
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ultroid?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ultroid)    
+        [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Ayra/graphs/commit-activity)
+        [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Ayra)
+        [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
+        
+        # Installation
+        ```bash
+        pip3 install -U py-Ayra
+        ```
+        
+        # Documentation 
+        [![Documentation](https://img.shields.io/badge/Documentation-Ayrq-blue)](http://ayra.tech/)
+        
+        # Usage
+        - Create folders named `plugins`, `addons`, `assistant` and `resources`.   
+        - Add your plugins in the `plugins` folder and others accordingly.   
+        - Create a `.env` file with following mandatory Environment Variables
+           ```
+           API_ID
+           API_HASH
+           SESSION
+           MONGO_URI
+           ```
+        - Check
+        [`.env.sample`](https://github.com/naya1503/Ayra/blob/main/.env.sample) for more details.   
+        - Run `python3 -m Ayra` to start the bot.   
+        
+        ## Creating plugins
+         - ### To work everywhere
+        
+        ```python
+        @ultroid_cmd(
+            pattern="start"
+        )   
+        async def _(e):   
+            await e.eor("Ayra Started!")   
+        ```
+        
+        - ### To work only in groups
+        
+        ```python
+        @ultroid_cmd(
+            pattern="start",
+            groups_only=True,
+        )   
+        async def _(e):   
+            await eor(e, "Ayra Started.")   
+        ```
+        
+        - ### Assistant Plugins 👇
+        
+        ```python
+        @asst_cmd("start")   
+        async def _(e):   
+            await e.reply("Ayra Started.")   
+        ```
+        
+        See more working plugins on [the offical repository](https://github.com/naya1503/Ayra)!
+        
+        > Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
+        
+        
+        # License
+        [![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
+        Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
+        
+        # Credits
+        * [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
+        * [Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon)
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.7, <3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# py-Ultroid Library
-
-Core library of [The Ultroid](https://github.com/naya1503/Ayra), a python based telegram userbot.
-
-[![CodeFactor](https://www.codefactor.io/repository/github/naya1503/pyayra/badge)](https://www.codefactor.io/repository/github/naya1503/pyayra)
-[![PyPI - Version](https://img.shields.io/pypi/v/py-Ultroid?style=round)](https://pypi.org/project/py-Ultroid)    
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ultroid?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ultroid)    
-[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Ayra/graphs/commit-activity)
-[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Ayra)
-[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
-
-# Installation
-```bash
-pip3 install -U py-Ayra
-```
-
-# Documentation 
-[![Documentation](https://img.shields.io/badge/Documentation-Ayrq-blue)](http://ayra.tech/)
-
-# Usage
-- Create folders named `plugins`, `addons`, `assistant` and `resources`.   
-- Add your plugins in the `plugins` folder and others accordingly.   
-- Create a `.env` file with following mandatory Environment Variables
-   ```
-   API_ID
-   API_HASH
-   SESSION
-   MONGO_URI
-   ```
-- Check
-[`.env.sample`](https://github.com/naya1503/Ayra/blob/main/.env.sample) for more details.   
-- Run `python3 -m Ayra` to start the bot.   
-
-## Creating plugins
- - ### To work everywhere
-
-```python
-@ultroid_cmd(
-    pattern="start"
-)   
-async def _(e):   
-    await e.eor("Ayra Started!")   
-```
-
-- ### To work only in groups
-
-```python
-@ultroid_cmd(
-    pattern="start",
-    groups_only=True,
-)   
-async def _(e):   
-    await eor(e, "Ayra Started.")   
-```
-
-- ### Assistant Plugins 👇
-
-```python
-@asst_cmd("start")   
-async def _(e):   
-    await e.reply("Ayra Started.")   
-```
-
-See more working plugins on [the offical repository](https://github.com/naya1503/Ayra)!
-
-> Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
-
-
-# License
-[![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
-Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
-
-# Credits
-* [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
-* [Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon)
-
-
```

### Comparing `py-Ayra-8.7.6/py_Ayra.egg-info/SOURCES.txt` & `py-Ayra-8.7.8/py_Ayra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.cfg
 setup.py
 Ayra/__init__.py
 Ayra/__main__.py
 Ayra/configs.py
 Ayra/exceptions.py
```

### Comparing `py-Ayra-8.7.6/setup.py` & `py-Ayra-8.7.8/setup.py`

 * *Files identical despite different names*

