# Comparing `tmp/chat-downloader-0.2.6.tar.gz` & `tmp/chat-downloader-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-downloader-0.2.6.tar", last modified: Fri May 19 11:06:22 2023, max compression
+gzip compressed data, was "chat-downloader-0.2.7.tar", last modified: Tue May 23 21:42:27 2023, max compression
```

## Comparing `chat-downloader-0.2.6.tar` & `chat-downloader-0.2.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.501308 chat-downloader-0.2.6/chat_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/chat_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.501308 chat-downloader-0.2.6/chat_downloader/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/formatting/custom_formats.json
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/formatting/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/chat_downloader/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/output/continuous_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/chat_downloader/sites/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    57794 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    81549 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/zoom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/chat_downloader/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/utils/timed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.501308 chat-downloader-0.2.6/chat_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/items.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/options.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/source/chat_downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/source/sites.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   136131 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/other youtube actions
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_chat_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_init_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    67588 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/youtube_actions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.506852 chat-downloader-0.2.7/chat_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/chat_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.506852 chat-downloader-0.2.7/chat_downloader/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/formatting/custom_formats.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/formatting/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.506852 chat-downloader-0.2.7/chat_downloader/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/output/continuous_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/chat_downloader/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/sites/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/sites/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57258 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/sites/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81549 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/sites/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/sites/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/chat_downloader/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/chat_downloader/utils/timed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.506852 chat-downloader-0.2.7/chat_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-23 21:42:27.000000 chat-downloader-0.2.7/chat_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-23 21:42:27.000000 chat-downloader-0.2.7/chat_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:42:27.000000 chat-downloader-0.2.7/chat_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 21:42:27.000000 chat-downloader-0.2.7/chat_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:42:27.000000 chat-downloader-0.2.7/chat_downloader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-23 21:42:27.000000 chat-downloader-0.2.7/chat_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 21:42:27.000000 chat-downloader-0.2.7/chat_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/items.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/options.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/source/chat_downloader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/docs/source/sites.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:42:27.510852 chat-downloader-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136131 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/other youtube actions
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_chat_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_init_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67588 2023-05-23 21:42:15.000000 chat-downloader-0.2.7/tests/youtube_actions.json
```

### Comparing `chat-downloader-0.2.6/LICENSE` & `chat-downloader-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/PKG-INFO` & `chat-downloader-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-downloader
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple tool used to retrieve chat messages from livestreams, videos, clips and past broadcasts. No authentication needed!
 Home-page: https://github.com/xenova/chat-downloader
 Author: xenova
 Author-email: admin@xenova.com
 License: MIT license
 Keywords: python chat downloader youtube twitch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chat-downloader-0.2.6/README.rst` & `chat-downloader-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/chat_downloader.py` & `chat-downloader-0.2.7/chat_downloader/chat_downloader.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/cli.py` & `chat-downloader-0.2.7/chat_downloader/cli.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/debugging.py` & `chat-downloader-0.2.7/chat_downloader/debugging.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/errors.py` & `chat-downloader-0.2.7/chat_downloader/errors.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/formatting/custom_formats.json` & `chat-downloader-0.2.7/chat_downloader/formatting/custom_formats.json`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/formatting/format.py` & `chat-downloader-0.2.7/chat_downloader/formatting/format.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/output/continuous_write.py` & `chat-downloader-0.2.7/chat_downloader/output/continuous_write.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/sites/__init__.py` & `chat-downloader-0.2.7/chat_downloader/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/sites/common.py` & `chat-downloader-0.2.7/chat_downloader/sites/common.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/sites/facebook.py` & `chat-downloader-0.2.7/chat_downloader/sites/facebook.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/sites/twitch.py` & `chat-downloader-0.2.7/chat_downloader/sites/twitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,28 +86,18 @@
 
     def close_connection(self):
         self.socket.close()
 
 
 class TwitchChatDownloader(BaseChatDownloader):
     _BADGE_INFO = {}
-    _BADGE_INFO_URL = 'https://badges.twitch.tv/v1/badges/global/display'
-    # TODO add local version of badge list?
+    _SUBSCRIBER_BADGE_INFO = {}  # local cache for subscriber badge info
 
     _NAME = 'twitch.tv'
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-        # Only get badge info if not already retrieved
-        # TODO add argument (no_badges)
-        if not TwitchChatDownloader._BADGE_INFO:
-            TwitchChatDownloader._BADGE_INFO = self._session_get_json(
-                self._BADGE_INFO_URL).get('badge_sets') or {}
-
     _TESTS = [
         # Live
         {
             'name': 'Livestream',
             'params': {
                 'url': 'https://www.twitch.tv/xenova',
                 'timeout': 5
@@ -457,15 +447,14 @@
         # created elsewhere
         'message', 'time_in_seconds', 'message_id', 'time_text', 'author', 'timestamp', 'message_type', 'emotes'
     }
 
     _KNOWN_COMMENT_KEYS.update(BaseChatDownloader.get_mapped_keys({
         **_COMMENT_REMAPPING, **_MESSAGE_PARAM_REMAPPING
     }))
-    # print('_KNOWN_COMMENT_KEYS',_KNOWN_COMMENT_KEYS)
 
     _IRC_REMAPPING = {
         # CLEARCHAT
         # Purges all chat messages in a channel, or purges chat messages from a specific user, typically after a timeout or ban.
         # (Optional) Duration of the timeout, in seconds. If omitted, the ban is permanent.
         'ban-duration': r('ban_duration', int_or_none),
 
@@ -788,26 +777,37 @@
         _value = _MESSAGE_GROUP_REMAPPINGS[_message_group]
         _MESSAGE_TYPE_REMAPPING.update(_value)
 
         if _message_group not in _MESSAGE_GROUPS:
             _MESSAGE_GROUPS[_message_group] = []
         _MESSAGE_GROUPS[_message_group] += list(_value.values())
 
-    _SUBSCRIBER_BADGE_INFO = {}  # local cache for subscriber badge info
-    _SUBSCRIBER_BADGE_URL = 'https://badges.twitch.tv/v1/badges/channels/{}/display'
+    def _update_badge_info(self, channel):
+        query = [{
+            'operationName': 'ChatList_Badges',
+            'variables': {
+                'channelLogin': channel
+            }
+        }]
+        data = multi_get(self._download_gql(query), 0, 'data') or {}
 
-    def _update_subscriber_badge_info(self, channel_id):
-        # print('updated sub badges')
-        url = self._SUBSCRIBER_BADGE_URL.format(channel_id)
-
-        # only get if not in dict
-        channel_id = int(channel_id)  # ensure integer
-        if channel_id not in self._SUBSCRIBER_BADGE_INFO:
-            self._SUBSCRIBER_BADGE_INFO[channel_id] = self._session_get_json(
-                url).get('badge_sets') or {}
+        badges = data.get('badges') or []
+        user = multi_get(data, 'user', 'broadcastBadges') or []
+        for badge in badges + user:
+            setID, version, channelID = base64.b64decode(
+                badge['id']).decode().strip().split(';')
+
+            if channelID:
+                if channelID not in self._SUBSCRIBER_BADGE_INFO:
+                    self._SUBSCRIBER_BADGE_INFO[channelID] = {}
+
+                self._SUBSCRIBER_BADGE_INFO[channelID][(
+                    setID, version)] = badge
+            else:
+                self._BADGE_INFO[(setID, version)] = badge
 
     @staticmethod
     def _parse_item(item, offset, channel_id=None):
         info = {}
 
         for key in item:
             r.remap(info, TwitchChatDownloader._COMMENT_REMAPPING,
@@ -816,31 +816,35 @@
         if 'time_in_seconds' in info:
             info['time_in_seconds'] -= offset
             info['time_text'] = seconds_to_time(int(info['time_in_seconds']))
 
         badges = info.pop('author_badges', None)
         if badges:
             info['author']['badges'] = [
-                TwitchChatDownloader._parse_badge_info(x.get('setID'), x.get('version'), channel_id)
+                TwitchChatDownloader._parse_badge_info(
+                    x.get('setID'), x.get('version'), channel_id)
                 for x in badges
                 if x.get('setID') and x.get('version')
             ]
+            if not info['author']['badges']:
+                del info['author']['badges']
 
         BaseChatDownloader._move_to_dict(info, 'author')
 
         original_message_type = info.get('message_type')
         if original_message_type:
             TwitchChatDownloader._set_message_type(
                 info, original_message_type)
         else:
             info['message_type'] = 'text_message'
 
         return info
 
     _OPERATION_HASHES = {
+        'ChatList_Badges': '86f43113c04606e6476e39dcd432dee47c994d77a83e54b732e11d4935f0cd08',
         'StreamMetadata': '1c719a40e481453e5c48d9bb585d971b8b372f8ebb105b17076722264dfa5b3e',
         'BrowsePage_Popular': 'c3322a9df3121f437182beb5a75c2a8db9a1e27fa57701ffcae70e681f502557',
         'ChannelVideoShelvesQuery': 'fb663273aa958ebe2f58d5fcb3aacc112d67ebfd7f414b095c5d1498d21aad92',
         'ClipsCards__User': 'b73ad2bfaecfd30a9e6c28fada15bd97032c83ec77a0440766a56fe0bd632777',
         'VideoMetadata': '226edb3e692509f727fd56821f5653c05740242c82b0388883e0c0e75dcbf687',
         'FilterableVideoTower_Videos': 'a937f1d22e269e39a03b509f65a7490f9fc247d7f83d6ac1421523e3b68042cb',
 
@@ -1031,15 +1035,14 @@
             'variables': {
                 'channelLogin': username,
                 'first': 5
             }
         }]
         edges = self._download_gql(
             query)[0]['data']['user']['videoShelves']['edges']
-        # print(len(edges))
         return edges
 
     _LIVESTREAM_REMAPPING = {
 
         'id': r('id', str_or_none),
         'title': 'title',
         'viewersCount': 'viewers',
@@ -1059,15 +1062,14 @@
 
         cursor = ''
 
         while True:
             num_to_get = max(min(remaining_count, 30), 0)
             if num_to_get <= 0:
                 break
-            # print('num_to_get', num_to_get)
 
             query = [{
                 'operationName': 'BrowsePage_Popular',
                 'variables': {
                     'limit': num_to_get,
                     'cursor': cursor,
                     'platformType': 'all',
@@ -1247,18 +1249,16 @@
 
         if not video:
             raise VideoUnavailable(
                 "Sorry. Unless you've got a time machine, that content is unavailable.")
         title = video.get('title')
         duration = video.get('lengthSeconds')
 
-        # print('duration', duration)
-
-        channel_id = multi_get(video, 'owner', 'id')
-        self._update_subscriber_badge_info(channel_id)
+        channel_name = multi_get(video, 'owner', 'login')
+        self._update_badge_info(channel_name)
 
         return Chat(
             self._get_chat_messages_by_vod_id(
                 vod_id, params, duration),
             title=title,
             duration=duration,
             status='past',
@@ -1270,15 +1270,15 @@
         return self.get_chat_by_clip_id(match.group('id'), params)
 
     def get_chat_by_clip_id(self, clip_id, params):
 
         max_attempts = params.get('max_attempts')
 
         query = {
-            'query': '{ clip(slug: "%s") { broadcaster { id } video { id createdAt } createdAt durationSeconds videoOffsetSeconds title url slug } }' % clip_id,
+            'query': '{ clip(slug: "%s") { broadcaster { id login } video { id createdAt } createdAt durationSeconds videoOffsetSeconds title url slug } }' % clip_id,
         }
 
         for attempt_number in attempts(max_attempts):
             try:
                 clip = self._download_base_gql(query)['data']['clip']
                 break
             except (JSONDecodeError, RequestException) as e:
@@ -1291,16 +1291,16 @@
                 "This clip's past broadcast has expired and chat replay is no longer available.")
 
         offset = clip.get('videoOffsetSeconds')
 
         duration = clip.get('durationSeconds')
         title = f"{clip.get('title')} ({clip_id})"
 
-        channel_id = multi_get(clip, 'broadcaster', 'id')
-        self._update_subscriber_badge_info(channel_id)
+        channel_name = multi_get(clip, 'broadcaster', 'login')
+        self._update_badge_info(channel_name)
 
         return Chat(
             self._get_chat_messages_by_vod_id(
                 vod_id, params, duration, offset),
             title=title,
             duration=duration,
             status='past',
@@ -1311,56 +1311,45 @@
     _MESSAGE_REGEX = re.compile(
         r'^@(.+?(?=\s+:)).*tmi\.twitch\.tv\s+(\S+)(?:[^#\r\n]+#)?\s(?:\S+)?(?:\s:([^\r\n]*))?', re.MULTILINE)
     # Groups:
     # 1. Tag info
     # 2. Action type
     # 3. Message
 
-    # A full list can be found here: https://badges.twitch.tv/v1/badges/global/display
-
-    _BADGE_KEYS = ('title', 'description', 'image_url_1x',
-                   'image_url_2x', 'image_url_4x', 'click_action', 'click_url')
-    _BADGE_ID_REGEX = r'v1/([^/]+)/'
+    _BADGE_KEYS = ('title', 'image1x', 'image2x',
+                   'image4x', 'clickAction', 'clickURL')
 
     @staticmethod
     def _parse_badge_info(name, version, channel_id=None):
         new_badge = {
             'name': replace_with_underscores(name),
             'version': int_or_none(version, version)
         }
 
         # prioritise custom emotes (e.g. subscriber and bits)
-
         new_badge_info = None
         if channel_id is not None:
-            new_badge_info = multi_get(TwitchChatDownloader._SUBSCRIBER_BADGE_INFO, int(
-                channel_id), name, 'versions', version)
+            new_badge_info = multi_get(
+                TwitchChatDownloader._SUBSCRIBER_BADGE_INFO, str(channel_id), (name, version))
 
         if not new_badge_info:
             new_badge_info = multi_get(
-                TwitchChatDownloader._BADGE_INFO, name, 'versions', version)
+                TwitchChatDownloader._BADGE_INFO, (name, version))
 
         if new_badge_info:
             for key in TwitchChatDownloader._BADGE_KEYS:
                 new_badge[key] = new_badge_info.get(key)
 
             image_urls = [
-                (new_badge.pop(f'image_url_{i}x', ''), i * 18) for i in (1, 2, 4)]
-            if image_urls:
-                new_badge['icons'] = []
+                (new_badge.pop(f'image{i}x', ''), i * 18) for i in (1, 2, 4)]
 
+            new_badge['icons'] = []
             for image_url, size in image_urls:
                 new_badge['icons'].append(Image(image_url, size, size).json())
 
-            if image_urls:
-                badge_id = re.search(
-                    TwitchChatDownloader._BADGE_ID_REGEX, image_urls[0][0] or '')
-                if badge_id:
-                    new_badge['id'] = badge_id.group(1)
-
         return new_badge
 
     @staticmethod
     def _parse_irc_badges(badges, channel_id):
         info = []
         if not badges:
             return info
@@ -1676,15 +1665,15 @@
             raise UserNotFound(f'Unable to find user: "{stream_id}"')
 
         is_live = multi_get(stream_info, 'stream', 'type') == 'live'
         channel_id = multi_get(stream_info, 'channel', 'id')
         title = multi_get(stream_info, 'lastBroadcast',
                           'title') if is_live else stream_id
 
-        self._update_subscriber_badge_info(channel_id)
+        self._update_badge_info(stream_id)
 
         return Chat(
             self._get_chat_messages_by_stream_id(
                 stream_id, params),
             title=title,
             duration=None,
             status='live' if is_live else 'upcoming',  # Always live or upcoming
```

### Comparing `chat-downloader-0.2.6/chat_downloader/sites/youtube.py` & `chat-downloader-0.2.7/chat_downloader/sites/youtube.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/sites/zoom.py` & `chat-downloader-0.2.7/chat_downloader/sites/zoom.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/utils/core.py` & `chat-downloader-0.2.7/chat_downloader/utils/core.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader/utils/timed_utils.py` & `chat-downloader-0.2.7/chat_downloader/utils/timed_utils.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/chat_downloader.egg-info/PKG-INFO` & `chat-downloader-0.2.7/chat_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-downloader
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple tool used to retrieve chat messages from livestreams, videos, clips and past broadcasts. No authentication needed!
 Home-page: https://github.com/xenova/chat-downloader
 Author: xenova
 Author-email: admin@xenova.com
 License: MIT license
 Keywords: python chat downloader youtube twitch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chat-downloader-0.2.6/chat_downloader.egg-info/SOURCES.txt` & `chat-downloader-0.2.7/chat_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/Makefile` & `chat-downloader-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/README.rst` & `chat-downloader-0.2.7/docs/README.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/changelog.rst` & `chat-downloader-0.2.7/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/cli.rst` & `chat-downloader-0.2.7/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/conf.py` & `chat-downloader-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/contributing.rst` & `chat-downloader-0.2.7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/items.rst` & `chat-downloader-0.2.7/docs/items.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/options.rst` & `chat-downloader-0.2.7/docs/options.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/source/chat_downloader.rst` & `chat-downloader-0.2.7/docs/source/chat_downloader.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/docs/source/sites.rst` & `chat-downloader-0.2.7/docs/source/sites.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/setup.py` & `chat-downloader-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/other youtube actions` & `chat-downloader-0.2.7/tests/other youtube actions`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/test_chat_downloader.py` & `chat-downloader-0.2.7/tests/test_chat_downloader.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/test_formatting.py` & `chat-downloader-0.2.7/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/test_generators.py` & `chat-downloader-0.2.7/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/test_init_params.py` & `chat-downloader-0.2.7/tests/test_init_params.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/test_sites.py` & `chat-downloader-0.2.7/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/test_utils.py` & `chat-downloader-0.2.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/test_writers.py` & `chat-downloader-0.2.7/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.6/tests/youtube_actions.json` & `chat-downloader-0.2.7/tests/youtube_actions.json`

 * *Files identical despite different names*

