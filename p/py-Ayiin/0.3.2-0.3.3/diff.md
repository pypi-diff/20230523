# Comparing `tmp/py-Ayiin-0.3.2.tar.gz` & `tmp/py-Ayiin-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.3.2.tar", last modified: Fri May 19 07:04:15 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.3.tar", last modified: Tue May 23 10:54:34 2023, max compression
```

## Comparing `py-Ayiin-0.3.2.tar` & `py-Ayiin-0.3.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.257192 py-Ayiin-0.3.3/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.257192 py-Ayiin-0.3.3/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.261192 py-Ayiin-0.3.3/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.261192 py-Ayiin-0.3.3/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/setup.py
```

### Comparing `py-Ayiin-0.3.2/LICENSE` & `py-Ayiin-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/NOTICE` & `py-Ayiin-0.3.3/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/PKG-INFO` & `py-Ayiin-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.2/README.md` & `py-Ayiin-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.3/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.3/pyAyiin/Clients/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         session_string=Var.STRING_1,
         in_memory=True,
     )
     if Var.STRING_1
     else None
 )
 
-
 AYIIN2 = (
     Client(
         name="AYIIN2",
         api_id=Var.API_ID,
         api_hash=Var.API_HASH,
         session_string=Var.STRING_2,
         in_memory=True,
```

### Comparing `py-Ayiin-0.3.2/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.3.3/pyAyiin/Clients/pytgcalls.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 
 
 # ========================×========================
 #            Jangan Hapus Credit Ngentod
 # ========================×========================
 
 
+from typing import Optional
+
+from fipper.types import Message
 from fipper.raw.functions.channels import GetFullChannel
 from fipper.raw.functions.messages import GetFullChat
-from fipper.raw.functions.phone import CreateGroupCall, EditGroupCallTitle
-from fipper.raw.types import InputPeerChannel, InputPeerChat
+from fipper.raw.functions.phone import CreateGroupCall, DiscardGroupCall, EditGroupCallTitle
+from fipper.raw.types import InputGroupCall, InputPeerChannel, InputPeerChat
 
 from ..methods.queue import Queues
 
 from .client import *
 
 
 try:
@@ -40,41 +43,70 @@
     def __init__(self):
         self.chat_id = []
         self.clients = {}
         self.active_calls = []
         self.msgid_cache = {}
         self.play_on = {}
     
+    async def get_group_call(
+        self,
+        client: Client, 
+        message: Message, 
+        err_msg: str = "",
+    ) -> Optional[InputGroupCall]:
+        chat_peer = await client.resolve_peer(message.chat.id)
+        if isinstance(chat_peer, (InputPeerChannel, InputPeerChat)):
+            if isinstance(chat_peer, InputPeerChannel):
+                full_chat = (await client.invoke(GetFullChannel(channel=chat_peer))).full_chat
+            elif isinstance(chat_peer, InputPeerChat):
+                full_chat = (
+                    await client.invoke(GetFullChat(chat_id=chat_peer.chat_id))
+                ).full_chat
+            if full_chat is not None:
+                return full_chat.call
+        await message.edit(f"<b>No group call Found</b> {err_msg}")
+        return False
+    
     async def TitleVc(self, client, m, title: str):
         peer = await client.resolve_peer(m.chat.id)
         if isinstance(peer, InputPeerChannel):
-            chat = await client.send(GetFullChannel(channel=peer))
+            chat = await client.invoke(GetFullChannel(channel=peer))
         if isinstance(peer, InputPeerChat):
-            chat = await client.send(GetFullChat(chat_id=peer.chat_id))
-        return await client.send(
+            chat = await client.invoke(GetFullChat(chat_id=peer.chat_id))
+        return await client.invoke(
             EditGroupCallTitle(
                 call=chat.full_chat.call,
                 title=title,
             )
         )
 
     async def StartVc(self, client, m, title=None):
         peer = await client.resolve_peer(m.chat.id)
-        await client.send(
+        await client.invoke(
             CreateGroupCall(
                 peer=InputPeerChannel(
                     channel_id=peer.channel_id,
                     access_hash=peer.access_hash,
                 ),
                 random_id=client.rnd_id() // 9000000000,
             )
         )
         titt = title if title else "🎧 Ayiin Music 🎧"
         await self.TitleVc(client, m, title=titt)
 
+    async def StopVc(
+        self,
+        client,
+        message,
+    ):
+        group_call = await self.get_group_call(client, message, err_msg="group call already ended")
+        if not group_call:
+            return
+        await client.invoke(DiscardGroupCall(call=group_call))
+
     async def pause_stream(self, chat_id: int):
         await assistant.pause_stream(chat_id)
 
     async def resume_stream(self, chat_id: int):
         await assistant.resume_stream(chat_id)
 
     async def mute_stream(self, chat_id: int):
```

### Comparing `py-Ayiin-0.3.2/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.3/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/__init__.py` & `py-Ayiin-0.3.3/pyAyiin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,24 +42,26 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
 ]
 
+API_AI = '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'
+
 GCAST_BLACKLIST = [
     -1001675396283,  # AyiinXdSupport
     -1001473548283,  # SharingUserbot
     -1001433238829,  # TedeSupport
     -1001476936696,  # AnosSupport
     -1001327032795,  # UltroidSupport
     -1001294181499,  # UserBotIndo
```

### Comparing `py-Ayiin-0.3.2/pyAyiin/__main__.py` & `py-Ayiin-0.3.3/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/assistant.py` & `py-Ayiin-0.3.3/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/config.py` & `py-Ayiin-0.3.3/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.3/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.3/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.3/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.3/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.3/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.3.3/pyAyiin/dB/blacklistgcast.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,18 +34,15 @@
     return True
 
 
 async def add_blacklist_gcast(chat_id: int):
     is_served = await is_blacklist_gcast(chat_id)
     if is_served:
         return
-    await chatsdb.insert_one({"chat_id": chat_id})
-    await blacklisted()
-    return
+    return await chatsdb.insert_one({"chat_id": chat_id})
 
 
 async def remove_blacklist_gcast(chat_id: int):
     is_served = await is_blacklist_gcast(chat_id)
     if not is_served:
         return
-    BLACKLIST_GCAST.remove(chat_id)
     return await chatsdb.delete_one({"chat_id": chat_id})
```

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.3/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.3/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.3/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.3/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.3/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.3/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/start.py` & `py-Ayiin-0.3.3/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.3/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.3/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.3/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.3/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/decorator.py` & `py-Ayiin-0.3.3/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/exceptions.py` & `py-Ayiin-0.3.3/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.3/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.3/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.3/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.3/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/func.py` & `py-Ayiin-0.3.3/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/funcb.py` & `py-Ayiin-0.3.3/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.3/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.3/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.3/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.3/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.3/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.3/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/pyAyiin/xd.py` & `py-Ayiin-0.3.3/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.3/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.2/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.3/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.2/setup.py` & `py-Ayiin-0.3.3/setup.py`

 * *Files identical despite different names*

