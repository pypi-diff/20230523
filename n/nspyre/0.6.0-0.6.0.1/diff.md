# Comparing `tmp/nspyre-0.6.0.tar.gz` & `tmp/nspyre-0.6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nspyre-0.6.0.tar", max compression
+gzip compressed data, was "nspyre-0.6.0.1.tar", max compression
```

## Comparing `nspyre-0.6.0.tar` & `nspyre-0.6.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1556 2022-11-12 17:38:33.919530 nspyre-0.6.0/LICENSE
--rw-r--r--   0        0        0     1952 2023-04-04 02:41:48.465068 nspyre-0.6.0/README.md
--rw-r--r--   0        0        0     2172 2023-05-23 03:45:42.918943 nspyre-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1294 2023-05-10 15:07:09.976140 nspyre-0.6.0/src/nspyre/__init__.py
--rw-r--r--   0        0        0      136 2023-04-01 16:52:54.096452 nspyre-0.6.0/src/nspyre/cli/__init__.py
--rwxr-xr-x   0        0        0     4514 2023-05-10 15:54:48.962860 nspyre-0.6.0/src/nspyre/cli/dataserv.py
--rwxr-xr-x   0        0        0     8227 2023-05-10 17:14:26.766672 nspyre-0.6.0/src/nspyre/cli/inserv.py
--rw-r--r--   0        0        0       95 2023-05-10 16:19:34.767631 nspyre-0.6.0/src/nspyre/data/__init__.py
--rw-r--r--   0        0        0     4065 2023-05-10 15:51:46.230215 nspyre-0.6.0/src/nspyre/data/_asyncio_worker.py
--rw-r--r--   0        0        0     1417 2023-05-04 03:03:36.211823 nspyre-0.6.0/src/nspyre/data/save.py
--rw-r--r--   0        0        0    21970 2023-05-10 16:20:56.487893 nspyre-0.6.0/src/nspyre/data/server.py
--rw-r--r--   0        0        0    14241 2023-05-10 16:27:37.221183 nspyre-0.6.0/src/nspyre/data/sink.py
--rw-r--r--   0        0        0     9838 2023-05-10 17:02:35.099923 nspyre-0.6.0/src/nspyre/data/source.py
--rw-r--r--   0        0        0       32 2023-05-10 16:19:31.503620 nspyre-0.6.0/src/nspyre/data/streaming/__init__.py
--rw-r--r--   0        0        0     7423 2023-05-23 03:04:58.614271 nspyre-0.6.0/src/nspyre/data/streaming/_pickle.py
--rw-r--r--   0        0        0     6501 2023-05-22 03:39:48.838183 nspyre-0.6.0/src/nspyre/data/streaming/list.py
--rw-r--r--   0        0        0       33 2023-05-04 03:03:36.211823 nspyre-0.6.0/src/nspyre/extras/__init__.py
--rw-r--r--   0        0        0     9076 2023-05-23 02:48:13.234532 nspyre-0.6.0/src/nspyre/extras/subsystem.py
--rw-r--r--   0        0        0     1372 2023-05-10 16:08:16.521481 nspyre-0.6.0/src/nspyre/gui/__init__.py
--rw-r--r--   0        0        0     2745 2023-03-31 18:26:29.419619 nspyre-0.6.0/src/nspyre/gui/app.py
--rw-r--r--   0        0        0      620 2023-04-22 17:57:53.348455 nspyre-0.6.0/src/nspyre/gui/debug.py
--rw-r--r--   0        0        0   114910 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/images/favicon.ico
--rw-r--r--   0        0        0    31996 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/images/ssssspin.png
--rw-r--r--   0        0        0       63 2023-03-29 21:58:45.183197 nspyre-0.6.0/src/nspyre/gui/style/__init__.py
--rw-r--r--   0        0        0     1507 2023-05-10 15:15:39.049295 nspyre-0.6.0/src/nspyre/gui/style/_colors.py
--rw-r--r--   0        0        0     2184 2023-03-29 22:00:09.367399 nspyre-0.6.0/src/nspyre/gui/style/_style.py
--rw-r--r--   0        0        0      758 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/style/style.qss
--rw-r--r--   0        0        0     6942 2023-05-22 04:32:20.928749 nspyre-0.6.0/src/nspyre/gui/threadsafe.py
--rw-r--r--   0        0        0      457 2023-04-04 18:24:34.475281 nspyre-0.6.0/src/nspyre/gui/widgets/__init__.py
--rw-r--r--   0        0        0     9992 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/widgets/_splitter.py
--rw-r--r--   0        0        0     6542 2023-05-22 03:40:04.058260 nspyre-0.6.0/src/nspyre/gui/widgets/colormap.py
--rw-r--r--   0        0        0     7504 2023-05-23 03:00:11.489233 nspyre-0.6.0/src/nspyre/gui/widgets/experiment.py
--rw-r--r--   0        0        0    31065 2023-05-23 03:15:43.116571 nspyre-0.6.0/src/nspyre/gui/widgets/flex_line_plot.py
--rw-r--r--   0        0        0     4108 2023-05-10 15:52:37.130396 nspyre-0.6.0/src/nspyre/gui/widgets/layout.py
--rw-r--r--   0        0        0    16128 2023-05-23 03:15:24.132503 nspyre-0.6.0/src/nspyre/gui/widgets/line_plot.py
--rw-r--r--   0        0        0     7060 2023-05-23 02:53:28.371745 nspyre-0.6.0/src/nspyre/gui/widgets/load.py
--rw-r--r--   0        0        0     9725 2023-05-23 03:02:47.121797 nspyre-0.6.0/src/nspyre/gui/widgets/main.py
--rw-r--r--   0        0        0     7581 2023-05-23 03:05:58.638486 nspyre-0.6.0/src/nspyre/gui/widgets/params.py
--rw-r--r--   0        0        0     7177 2023-05-23 02:52:37.151551 nspyre-0.6.0/src/nspyre/gui/widgets/save.py
--rw-r--r--   0        0        0      714 2023-05-10 16:01:06.724155 nspyre-0.6.0/src/nspyre/gui/widgets/separator.py
--rw-r--r--   0        0        0     1041 2023-04-01 17:12:58.468408 nspyre-0.6.0/src/nspyre/gui/widgets/snake.py
--rw-r--r--   0        0        0     5731 2023-05-10 16:15:21.798822 nspyre-0.6.0/src/nspyre/gui/widgets/subsystem.py
--rw-r--r--   0        0        0     2692 2023-05-10 15:44:12.280514 nspyre-0.6.0/src/nspyre/gui/widgets/update_loop.py
--rw-r--r--   0        0        0      300 2023-04-12 23:30:05.012100 nspyre-0.6.0/src/nspyre/instrument/__init__.py
--rw-r--r--   0        0        0    10334 2023-05-22 03:38:56.309872 nspyre-0.6.0/src/nspyre/instrument/gateway.py
--rw-r--r--   0        0        0     4249 2023-05-23 02:59:03.800986 nspyre-0.6.0/src/nspyre/instrument/manager.py
--rw-r--r--   0        0        0    12718 2023-05-23 03:00:48.633368 nspyre-0.6.0/src/nspyre/instrument/server.py
--rw-r--r--   0        0        0       93 2023-05-07 22:07:03.250115 nspyre-0.6.0/src/nspyre/misc/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-10 15:44:31.736591 nspyre-0.6.0/src/nspyre/misc/_stacktracer.py
--rw-r--r--   0        0        0     5290 2023-05-23 03:01:33.457531 nspyre-0.6.0/src/nspyre/misc/logging.py
--rw-r--r--   0        0        0     7892 2023-05-22 04:32:20.964750 nspyre-0.6.0/src/nspyre/misc/misc.py
--rw-r--r--   0        0        0     2612 2023-05-10 17:01:20.811758 nspyre-0.6.0/src/nspyre/misc/pint.py
--rw-r--r--   0        0        0     3441 1970-01-01 00:00:00.000000 nspyre-0.6.0/setup.py
--rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 nspyre-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1556 2023-05-23 04:45:28.213560 nspyre-0.6.0.1/LICENSE
+-rw-r--r--   0        0        0     1952 2023-04-04 02:41:48.465068 nspyre-0.6.0.1/README.md
+-rw-r--r--   0        0        0     2240 2023-05-23 04:47:47.926033 nspyre-0.6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1294 2023-05-10 15:07:09.976140 nspyre-0.6.0.1/src/nspyre/__init__.py
+-rw-r--r--   0        0        0      136 2023-04-01 16:52:54.096452 nspyre-0.6.0.1/src/nspyre/cli/__init__.py
+-rwxr-xr-x   0        0        0     4514 2023-05-10 15:54:48.962860 nspyre-0.6.0.1/src/nspyre/cli/dataserv.py
+-rwxr-xr-x   0        0        0     8227 2023-05-10 17:14:26.766672 nspyre-0.6.0.1/src/nspyre/cli/inserv.py
+-rw-r--r--   0        0        0       95 2023-05-10 16:19:34.767631 nspyre-0.6.0.1/src/nspyre/data/__init__.py
+-rw-r--r--   0        0        0     4065 2023-05-10 15:51:46.230215 nspyre-0.6.0.1/src/nspyre/data/_asyncio_worker.py
+-rw-r--r--   0        0        0     1417 2023-05-04 03:03:36.211823 nspyre-0.6.0.1/src/nspyre/data/save.py
+-rw-r--r--   0        0        0    21970 2023-05-10 16:20:56.487893 nspyre-0.6.0.1/src/nspyre/data/server.py
+-rw-r--r--   0        0        0    14241 2023-05-10 16:27:37.221183 nspyre-0.6.0.1/src/nspyre/data/sink.py
+-rw-r--r--   0        0        0     9838 2023-05-10 17:02:35.099923 nspyre-0.6.0.1/src/nspyre/data/source.py
+-rw-r--r--   0        0        0       32 2023-05-10 16:19:31.503620 nspyre-0.6.0.1/src/nspyre/data/streaming/__init__.py
+-rw-r--r--   0        0        0     7423 2023-05-23 03:04:58.614271 nspyre-0.6.0.1/src/nspyre/data/streaming/_pickle.py
+-rw-r--r--   0        0        0     6501 2023-05-22 03:39:48.838183 nspyre-0.6.0.1/src/nspyre/data/streaming/list.py
+-rw-r--r--   0        0        0       33 2023-05-04 03:03:36.211823 nspyre-0.6.0.1/src/nspyre/extras/__init__.py
+-rw-r--r--   0        0        0     9076 2023-05-23 02:48:13.234532 nspyre-0.6.0.1/src/nspyre/extras/subsystem.py
+-rw-r--r--   0        0        0     1372 2023-05-10 16:08:16.521481 nspyre-0.6.0.1/src/nspyre/gui/__init__.py
+-rw-r--r--   0        0        0     2745 2023-03-31 18:26:29.419619 nspyre-0.6.0.1/src/nspyre/gui/app.py
+-rw-r--r--   0        0        0      620 2023-04-22 17:57:53.348455 nspyre-0.6.0.1/src/nspyre/gui/debug.py
+-rw-r--r--   0        0        0   114910 2022-11-12 17:38:33.927531 nspyre-0.6.0.1/src/nspyre/gui/images/favicon.ico
+-rw-r--r--   0        0        0    31996 2022-11-12 17:38:33.927531 nspyre-0.6.0.1/src/nspyre/gui/images/ssssspin.png
+-rw-r--r--   0        0        0       63 2023-03-29 21:58:45.183197 nspyre-0.6.0.1/src/nspyre/gui/style/__init__.py
+-rw-r--r--   0        0        0     1507 2023-05-10 15:15:39.049295 nspyre-0.6.0.1/src/nspyre/gui/style/_colors.py
+-rw-r--r--   0        0        0     2184 2023-03-29 22:00:09.367399 nspyre-0.6.0.1/src/nspyre/gui/style/_style.py
+-rw-r--r--   0        0        0      758 2022-11-12 17:38:33.927531 nspyre-0.6.0.1/src/nspyre/gui/style/style.qss
+-rw-r--r--   0        0        0     6942 2023-05-22 04:32:20.928749 nspyre-0.6.0.1/src/nspyre/gui/threadsafe.py
+-rw-r--r--   0        0        0      457 2023-04-04 18:24:34.475281 nspyre-0.6.0.1/src/nspyre/gui/widgets/__init__.py
+-rw-r--r--   0        0        0     9992 2022-11-12 17:38:33.927531 nspyre-0.6.0.1/src/nspyre/gui/widgets/_splitter.py
+-rw-r--r--   0        0        0     6542 2023-05-22 03:40:04.058260 nspyre-0.6.0.1/src/nspyre/gui/widgets/colormap.py
+-rw-r--r--   0        0        0     7504 2023-05-23 03:00:11.489233 nspyre-0.6.0.1/src/nspyre/gui/widgets/experiment.py
+-rw-r--r--   0        0        0    31212 2023-05-23 04:23:35.696725 nspyre-0.6.0.1/src/nspyre/gui/widgets/flex_line_plot.py
+-rw-r--r--   0        0        0     4108 2023-05-10 15:52:37.130396 nspyre-0.6.0.1/src/nspyre/gui/widgets/layout.py
+-rw-r--r--   0        0        0    16128 2023-05-23 03:15:24.132503 nspyre-0.6.0.1/src/nspyre/gui/widgets/line_plot.py
+-rw-r--r--   0        0        0     7060 2023-05-23 02:53:28.371745 nspyre-0.6.0.1/src/nspyre/gui/widgets/load.py
+-rw-r--r--   0        0        0     9725 2023-05-23 03:02:47.121797 nspyre-0.6.0.1/src/nspyre/gui/widgets/main.py
+-rw-r--r--   0        0        0     7581 2023-05-23 03:05:58.638486 nspyre-0.6.0.1/src/nspyre/gui/widgets/params.py
+-rw-r--r--   0        0        0     7177 2023-05-23 02:52:37.151551 nspyre-0.6.0.1/src/nspyre/gui/widgets/save.py
+-rw-r--r--   0        0        0      714 2023-05-10 16:01:06.724155 nspyre-0.6.0.1/src/nspyre/gui/widgets/separator.py
+-rw-r--r--   0        0        0     1041 2023-04-01 17:12:58.468408 nspyre-0.6.0.1/src/nspyre/gui/widgets/snake.py
+-rw-r--r--   0        0        0     5731 2023-05-10 16:15:21.798822 nspyre-0.6.0.1/src/nspyre/gui/widgets/subsystem.py
+-rw-r--r--   0        0        0     2692 2023-05-10 15:44:12.280514 nspyre-0.6.0.1/src/nspyre/gui/widgets/update_loop.py
+-rw-r--r--   0        0        0      300 2023-04-12 23:30:05.012100 nspyre-0.6.0.1/src/nspyre/instrument/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-22 03:38:56.309872 nspyre-0.6.0.1/src/nspyre/instrument/gateway.py
+-rw-r--r--   0        0        0     4249 2023-05-23 02:59:03.800986 nspyre-0.6.0.1/src/nspyre/instrument/manager.py
+-rw-r--r--   0        0        0    12718 2023-05-23 03:00:48.633368 nspyre-0.6.0.1/src/nspyre/instrument/server.py
+-rw-r--r--   0        0        0       93 2023-05-07 22:07:03.250115 nspyre-0.6.0.1/src/nspyre/misc/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-10 15:44:31.736591 nspyre-0.6.0.1/src/nspyre/misc/_stacktracer.py
+-rw-r--r--   0        0        0     5290 2023-05-23 03:01:33.457531 nspyre-0.6.0.1/src/nspyre/misc/logging.py
+-rw-r--r--   0        0        0     7892 2023-05-22 04:32:20.964750 nspyre-0.6.0.1/src/nspyre/misc/misc.py
+-rw-r--r--   0        0        0     2612 2023-05-10 17:01:20.811758 nspyre-0.6.0.1/src/nspyre/misc/pint.py
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 nspyre-0.6.0.1/setup.py
+-rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 nspyre-0.6.0.1/PKG-INFO
```

### Comparing `nspyre-0.6.0/LICENSE` & `nspyre-0.6.0.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Alexandre Bourassa, Michael Solomon, Jacob Feder
+Copyright (c) 2023, Jacob Feder, Michael Solomon, Alexandre Bourassa
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `nspyre-0.6.0/README.md` & `nspyre-0.6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/pyproject.toml` & `nspyre-0.6.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "nspyre"
-version = "0.6.0"
+version = "0.6.0.1"
 license = "BSD-3-Clause"
 description = "Networked Scientific Python Research Environment."
 authors = [
     "Jacob Feder <jacobsfeder@gmail.com>",
     "Michael Solomon <msolo@uchicago.edu>",
     "Jose A. Mendez <mendez99@uchicago.edu >",
     "Alexandre Bourassa"
@@ -38,31 +42,28 @@
 sphinx = { version = "*", optional = true }
 sphinx-copybutton = { version = "*", optional = true }
 sphinx_rtd_theme = { version = "*", optional = true }
 sphinx-autoapi = { version = "*", optional = true }
 pytest = { version = "*", optional = true }
 pytest-cov = { version = "*", optional = true }
 pint = { version = "*", optional = true }
+poetry2setup = { version = "*", optional = true }
 
 [tool.poetry.extras]
-dev = ["pre-commit", "sphinx", "sphinx-copybutton", "sphinx_rtd_theme", 
+dev = ["poetry2setup", "pre-commit", "sphinx", "sphinx-copybutton", "sphinx_rtd_theme", 
     "sphinx-autoapi", "pytest", "pytest-cov", "pint"
 ]
 
 [tool.poetry.scripts]
 nspyre-inserv = 'nspyre.cli.inserv:_main'
 nspyre-dataserv = 'nspyre.cli.dataserv:_main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/nspyre-org/nspyre/issues"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.black]
 line-length = 88
 target-version = ['py310']
 include = '\.pyi?$'
 skip-string-normalization = true
 exclude = '''
 /(
```

### Comparing `nspyre-0.6.0/src/nspyre/__init__.py` & `nspyre-0.6.0.1/src/nspyre/__init__.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/cli/dataserv.py` & `nspyre-0.6.0.1/src/nspyre/cli/dataserv.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/cli/inserv.py` & `nspyre-0.6.0.1/src/nspyre/cli/inserv.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/data/_asyncio_worker.py` & `nspyre-0.6.0.1/src/nspyre/data/_asyncio_worker.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/data/save.py` & `nspyre-0.6.0.1/src/nspyre/data/save.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/data/server.py` & `nspyre-0.6.0.1/src/nspyre/data/server.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/data/sink.py` & `nspyre-0.6.0.1/src/nspyre/data/sink.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/data/source.py` & `nspyre-0.6.0.1/src/nspyre/data/source.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/data/streaming/_pickle.py` & `nspyre-0.6.0.1/src/nspyre/data/streaming/_pickle.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/data/streaming/list.py` & `nspyre-0.6.0.1/src/nspyre/data/streaming/list.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/extras/subsystem.py` & `nspyre-0.6.0.1/src/nspyre/extras/subsystem.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/__init__.py` & `nspyre-0.6.0.1/src/nspyre/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/app.py` & `nspyre-0.6.0.1/src/nspyre/gui/app.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/debug.py` & `nspyre-0.6.0.1/src/nspyre/gui/debug.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/images/favicon.ico` & `nspyre-0.6.0.1/src/nspyre/gui/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/images/ssssspin.png` & `nspyre-0.6.0.1/src/nspyre/gui/images/ssssspin.png`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/style/_colors.py` & `nspyre-0.6.0.1/src/nspyre/gui/style/_colors.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/style/_style.py` & `nspyre-0.6.0.1/src/nspyre/gui/style/_style.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/style/style.qss` & `nspyre-0.6.0.1/src/nspyre/gui/style/style.qss`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/threadsafe.py` & `nspyre-0.6.0.1/src/nspyre/gui/threadsafe.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/_splitter.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/_splitter.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/colormap.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/colormap.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/experiment.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/experiment.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/flex_line_plot.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/flex_line_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import time
-from collections import namedtuple
 from typing import Callable
 from typing import Optional
 
 import numpy as np
 from pyqtgraph.Qt import QtCore
 from pyqtgraph.Qt import QtGui
 from pyqtgraph.Qt import QtWidgets
@@ -13,19 +12,25 @@
 from ..threadsafe import QThreadSafeObject
 from .layout import tree_layout
 from .line_plot import LinePlotWidget
 
 _logger = logging.getLogger(__name__)
 
 
-_FlexLinePlotSeriesSettings = namedtuple(
-    '_FlexLinePlotSeriesSettings',
-    ['series', 'scan_i', 'scan_j', 'processing', 'hidden'],
-)
-"""Contain the settings for a single plot."""
+class _FlexLinePlotSeriesSettings:
+    """Contain the settings for a single plot."""
+
+    def __init__(
+        self, series: str, scan_i: str, scan_j: str, processing: str, hidden: bool
+    ):
+        self.series: str = series
+        self.scan_i: str = scan_i
+        self.scan_j: str = scan_j
+        self.processing: str = processing
+        self.hidden = hidden
 
 
 class _FlexLinePlotSettings(QThreadSafeObject):
     """Container class to hold the plot settings for a _FlexLinePlotWidget."""
 
     def __init__(self):
         self.series_settings = {}
```

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/layout.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/line_plot.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/line_plot.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/load.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/load.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/main.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/main.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/params.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/params.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/save.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/save.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/separator.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/snake.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/snake.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/subsystem.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/subsystem.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/gui/widgets/update_loop.py` & `nspyre-0.6.0.1/src/nspyre/gui/widgets/update_loop.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/instrument/gateway.py` & `nspyre-0.6.0.1/src/nspyre/instrument/gateway.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/instrument/manager.py` & `nspyre-0.6.0.1/src/nspyre/instrument/manager.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/instrument/server.py` & `nspyre-0.6.0.1/src/nspyre/instrument/server.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/misc/_stacktracer.py` & `nspyre-0.6.0.1/src/nspyre/misc/_stacktracer.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/misc/logging.py` & `nspyre-0.6.0.1/src/nspyre/misc/logging.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/misc/misc.py` & `nspyre-0.6.0.1/src/nspyre/misc/misc.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/src/nspyre/misc/pint.py` & `nspyre-0.6.0.1/src/nspyre/misc/pint.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.6.0/setup.py` & `nspyre-0.6.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,24 @@
 {'dev': ['pre-commit',
          'sphinx',
          'sphinx-copybutton',
          'sphinx_rtd_theme',
          'sphinx-autoapi',
          'pytest',
          'pytest-cov',
-         'pint']}
+         'pint',
+         'poetry2setup']}
 
 entry_points = \
 {'console_scripts': ['nspyre-dataserv = nspyre.cli.dataserv:_main',
                      'nspyre-inserv = nspyre.cli.inserv:_main']}
 
 setup_kwargs = {
     'name': 'nspyre',
-    'version': '0.6.0',
+    'version': '0.6.0.1',
     'description': 'Networked Scientific Python Research Environment.',
     'long_description': '# nspyre\n\n[![GitHub](https://img.shields.io/github/v/release/nspyre-org/nspyre?label=GitHub)](https://github.com/nspyre-org/nspyre/)\n[![PyPi version](https://img.shields.io/pypi/v/nspyre)](https://pypi.org/project/nspyre/)\n[![conda-forge version](https://img.shields.io/conda/v/conda-forge/nspyre)](https://github.com/conda-forge/nspyre-feedstock)\n[![License](https://img.shields.io/github/license/nspyre-org/nspyre)](https://github.com/nspyre-org/nspyre/blob/master/LICENSE)\n[![Docs build](https://readthedocs.org/projects/nspyre/badge/?version=latest)](https://nspyre.readthedocs.io/en/latest/?badge=latest)\n[![conda-forge platform](https://img.shields.io/conda/pn/conda-forge/nspyre)](https://github.com/conda-forge/nspyre-feedstock)\n[![DOI](https://zenodo.org/badge/220515183.svg)](https://zenodo.org/badge/latestdoi/220515183)\n\n(N)etworked (S)cientific (Py)thon (R)esearch (E)nvironment.\n\nSee https://nspyre.readthedocs.io/.\n\n# What is nspyre?\n\nnspyre is a Python package for conducting scientific experiments. It provides \na set of tools to allow for control of instrumentation, data collection, \nreal-time plotting, as well as GUI generation. Anyone in the research or \nindustrial spaces using computer-controlled equipment and collecting data can \npotentially benefit from using nspyre to run their experiments.\n\nThe hardware being controlled can be connected either locally on the machine \nrunning the experimental logic, or on a remote machine, which can be accessed \nin a simple, pythonic fashion. This allows for the easy integration of shared \ninstrumentation in a research environment. Data collection is also \nnetworked, and allows for real-time viewing locally, or from a remote machine. \nnspyre provides a set of tools for quickly generating a Qt-based GUI for \ncontrol and data viewing.\n\nIf you use nspyre for an experiment, we would really appreciate it if you \n[cite](https://doi.org/10.5281/zenodo.7315077) it in your publication!\n',
     'author': 'Jacob Feder',
     'author_email': 'jacobsfeder@gmail.com',
     'maintainer': 'Jacob Feder',
     'maintainer_email': 'jacobsfeder@gmail.com',
     'url': 'https://github.com/nspyre-org/nspyre',
```

### Comparing `nspyre-0.6.0/PKG-INFO` & `nspyre-0.6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nspyre
-Version: 0.6.0
+Version: 0.6.0.1
 Summary: Networked Scientific Python Research Environment.
 Home-page: https://github.com/nspyre-org/nspyre
 License: BSD-3-Clause
 Author: Jacob Feder
 Author-email: jacobsfeder@gmail.com
 Maintainer: Jacob Feder
 Maintainer-email: jacobsfeder@gmail.com
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Provides-Extra: dev
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pint; extra == "dev"
+Requires-Dist: poetry2setup; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyqt6 (>=6.2.3,<7.0.0)
 Requires-Dist: pyqtgraph (>=0.13.1,<0.14.0)
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: rpyc (>=5.2.3,<6.0.0)
 Requires-Dist: sphinx-autoapi; extra == "dev"
```

