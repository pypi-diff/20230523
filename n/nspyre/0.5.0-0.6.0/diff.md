# Comparing `tmp/nspyre-0.5.0.tar.gz` & `tmp/nspyre-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nspyre-0.5.0.tar", last modified: Tue Nov 15 20:47:55 2022, max compression
+gzip compressed data, was "nspyre-0.6.0.tar", max compression
```

## Comparing `nspyre-0.5.0.tar` & `nspyre-0.6.0.tar`

### file list

```diff
@@ -1,101 +1,54 @@
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.324414 nspyre-0.5.0/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      129 2022-11-15 20:47:39.000000 nspyre-0.5.0/AUTHORS
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1556 2022-11-15 20:47:39.000000 nspyre-0.5.0/LICENSE
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      398 2022-11-15 20:47:39.000000 nspyre-0.5.0/MANIFEST.in
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2905 2022-11-15 20:47:55.324152 nspyre-0.5.0/PKG-INFO
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1261 2022-11-15 20:47:39.000000 nspyre-0.5.0/README.md
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.291579 nspyre-0.5.0/docs/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      608 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/Makefile
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.295503 nspyre-0.5.0/docs/source/
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.295889 nspyre-0.5.0/docs/source/_static/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)       58 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/_static/custom.css
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      637 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/api.rst
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     3678 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/conf.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    28028 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/contributing.rst
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     3789 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/data_server.rst
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     4439 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/getting_started.rst
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.296444 nspyre-0.5.0/docs/source/guides/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    23431 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/guides/ni-daqmx.rst
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.298843 nspyre-0.5.0/docs/source/images/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    17989 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/images/Bootcamp-Fork.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    11064 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/images/compare-and-pr.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    56678 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/images/delete-button.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)   121313 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/images/merge-button.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2819 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/index.rst
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     3788 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/install.rst
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     4022 2022-11-15 20:47:39.000000 nspyre-0.5.0/docs/source/instrument_server.rst
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      524 2022-11-15 20:47:39.000000 nspyre-0.5.0/pyproject.toml
--rw-r--r--   0 michaelsolomon   (501) staff       (20)       38 2022-11-15 20:47:55.324520 nspyre-0.5.0/setup.cfg
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     3866 2022-11-15 20:47:39.000000 nspyre-0.5.0/setup.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.285275 nspyre-0.5.0/src/
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.299335 nspyre-0.5.0/src/nspyre/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1893 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/__init__.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.305543 nspyre-0.5.0/src/nspyre/cli/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)       74 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/cli/__init__.py
--rwxr-xr-x   0 michaelsolomon   (501) staff       (20)     4368 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/cli/dataserv_cli.py
--rwxr-xr-x   0 michaelsolomon   (501) staff       (20)     7399 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/cli/inserv_cli.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.306486 nspyre-0.5.0/src/nspyre/dataserv/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      195 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/dataserv/__init__.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    54251 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/dataserv/dataserv.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.307604 nspyre-0.5.0/src/nspyre/gui/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      663 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/__init__.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2731 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/app.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.310305 nspyre-0.5.0/src/nspyre/gui/images/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      207 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/images/down_arrow.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)   114910 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/images/favicon.ico
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      207 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/images/left_arrow.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      204 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/images/right_arrow.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    16666 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/images/spyre.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    31996 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/images/ssssspin.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      201 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/images/up_arrow.png
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      611 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/misc.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.312371 nspyre-0.5.0/src/nspyre/gui/style/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      178 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/style/__init__.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    38602 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/style/colormap.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1548 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/style/colors.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2179 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/style/style.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      758 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/style/style.qss
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.317166 nspyre-0.5.0/src/nspyre/gui/widgets/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      448 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/__init__.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     5424 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/colormap_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     4621 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/experiment_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    22074 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/flex_line_plot_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    10776 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/line_plot_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     9085 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/main_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     5381 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/params_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     3985 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/save_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      606 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/separator_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1065 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/snake_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     9992 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/splitter_widget.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1401 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/gui/widgets/widget_update_thread.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.318753 nspyre-0.5.0/src/nspyre/inserv/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      215 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/inserv/__init__.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     6078 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/inserv/gateway.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)    11997 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/inserv/inserv.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.320576 nspyre-0.5.0/src/nspyre/misc/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)       93 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/misc/__init__.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     4737 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/misc/logging.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     5494 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/misc/misc.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2401 2022-11-15 20:47:39.000000 nspyre-0.5.0/src/nspyre/misc/pint.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.304115 nspyre-0.5.0/src/nspyre.egg-info/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2905 2022-11-15 20:47:55.000000 nspyre-0.5.0/src/nspyre.egg-info/PKG-INFO
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2319 2022-11-15 20:47:55.000000 nspyre-0.5.0/src/nspyre.egg-info/SOURCES.txt
--rw-r--r--   0 michaelsolomon   (501) staff       (20)        1 2022-11-15 20:47:55.000000 nspyre-0.5.0/src/nspyre.egg-info/dependency_links.txt
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      108 2022-11-15 20:47:55.000000 nspyre-0.5.0/src/nspyre.egg-info/entry_points.txt
--rw-r--r--   0 michaelsolomon   (501) staff       (20)        1 2022-11-15 20:47:54.000000 nspyre-0.5.0/src/nspyre.egg-info/not-zip-safe
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      264 2022-11-15 20:47:55.000000 nspyre-0.5.0/src/nspyre.egg-info/requires.txt
--rw-r--r--   0 michaelsolomon   (501) staff       (20)        7 2022-11-15 20:47:55.000000 nspyre-0.5.0/src/nspyre.egg-info/top_level.txt
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.321232 nspyre-0.5.0/tests/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      208 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/__init__.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     2874 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/conftest.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.287869 nspyre-0.5.0/tests/fixtures/
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.322637 nspyre-0.5.0/tests/fixtures/drivers/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1295 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/fixtures/drivers/fake_daq.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)      361 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/fixtures/drivers/fake_pellicle.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1143 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/fixtures/drivers/fake_sg.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.322982 nspyre-0.5.0/tests/tests/
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.323281 nspyre-0.5.0/tests/tests/dataserv/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     6694 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/tests/dataserv/test_dataserv.py
-drwxr-xr-x   0 michaelsolomon   (501) staff       (20)        0 2022-11-15 20:47:55.323577 nspyre-0.5.0/tests/tests/inserv/
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     5039 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/tests/inserv/test_inserv.py
--rw-r--r--   0 michaelsolomon   (501) staff       (20)     1703 2022-11-15 20:47:39.000000 nspyre-0.5.0/tests/tests/test_errors.py
+-rw-r--r--   0        0        0     1556 2022-11-12 17:38:33.919530 nspyre-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1952 2023-04-04 02:41:48.465068 nspyre-0.6.0/README.md
+-rw-r--r--   0        0        0     2172 2023-05-23 03:45:42.918943 nspyre-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1294 2023-05-10 15:07:09.976140 nspyre-0.6.0/src/nspyre/__init__.py
+-rw-r--r--   0        0        0      136 2023-04-01 16:52:54.096452 nspyre-0.6.0/src/nspyre/cli/__init__.py
+-rwxr-xr-x   0        0        0     4514 2023-05-10 15:54:48.962860 nspyre-0.6.0/src/nspyre/cli/dataserv.py
+-rwxr-xr-x   0        0        0     8227 2023-05-10 17:14:26.766672 nspyre-0.6.0/src/nspyre/cli/inserv.py
+-rw-r--r--   0        0        0       95 2023-05-10 16:19:34.767631 nspyre-0.6.0/src/nspyre/data/__init__.py
+-rw-r--r--   0        0        0     4065 2023-05-10 15:51:46.230215 nspyre-0.6.0/src/nspyre/data/_asyncio_worker.py
+-rw-r--r--   0        0        0     1417 2023-05-04 03:03:36.211823 nspyre-0.6.0/src/nspyre/data/save.py
+-rw-r--r--   0        0        0    21970 2023-05-10 16:20:56.487893 nspyre-0.6.0/src/nspyre/data/server.py
+-rw-r--r--   0        0        0    14241 2023-05-10 16:27:37.221183 nspyre-0.6.0/src/nspyre/data/sink.py
+-rw-r--r--   0        0        0     9838 2023-05-10 17:02:35.099923 nspyre-0.6.0/src/nspyre/data/source.py
+-rw-r--r--   0        0        0       32 2023-05-10 16:19:31.503620 nspyre-0.6.0/src/nspyre/data/streaming/__init__.py
+-rw-r--r--   0        0        0     7423 2023-05-23 03:04:58.614271 nspyre-0.6.0/src/nspyre/data/streaming/_pickle.py
+-rw-r--r--   0        0        0     6501 2023-05-22 03:39:48.838183 nspyre-0.6.0/src/nspyre/data/streaming/list.py
+-rw-r--r--   0        0        0       33 2023-05-04 03:03:36.211823 nspyre-0.6.0/src/nspyre/extras/__init__.py
+-rw-r--r--   0        0        0     9076 2023-05-23 02:48:13.234532 nspyre-0.6.0/src/nspyre/extras/subsystem.py
+-rw-r--r--   0        0        0     1372 2023-05-10 16:08:16.521481 nspyre-0.6.0/src/nspyre/gui/__init__.py
+-rw-r--r--   0        0        0     2745 2023-03-31 18:26:29.419619 nspyre-0.6.0/src/nspyre/gui/app.py
+-rw-r--r--   0        0        0      620 2023-04-22 17:57:53.348455 nspyre-0.6.0/src/nspyre/gui/debug.py
+-rw-r--r--   0        0        0   114910 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/images/favicon.ico
+-rw-r--r--   0        0        0    31996 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/images/ssssspin.png
+-rw-r--r--   0        0        0       63 2023-03-29 21:58:45.183197 nspyre-0.6.0/src/nspyre/gui/style/__init__.py
+-rw-r--r--   0        0        0     1507 2023-05-10 15:15:39.049295 nspyre-0.6.0/src/nspyre/gui/style/_colors.py
+-rw-r--r--   0        0        0     2184 2023-03-29 22:00:09.367399 nspyre-0.6.0/src/nspyre/gui/style/_style.py
+-rw-r--r--   0        0        0      758 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/style/style.qss
+-rw-r--r--   0        0        0     6942 2023-05-22 04:32:20.928749 nspyre-0.6.0/src/nspyre/gui/threadsafe.py
+-rw-r--r--   0        0        0      457 2023-04-04 18:24:34.475281 nspyre-0.6.0/src/nspyre/gui/widgets/__init__.py
+-rw-r--r--   0        0        0     9992 2022-11-12 17:38:33.927531 nspyre-0.6.0/src/nspyre/gui/widgets/_splitter.py
+-rw-r--r--   0        0        0     6542 2023-05-22 03:40:04.058260 nspyre-0.6.0/src/nspyre/gui/widgets/colormap.py
+-rw-r--r--   0        0        0     7504 2023-05-23 03:00:11.489233 nspyre-0.6.0/src/nspyre/gui/widgets/experiment.py
+-rw-r--r--   0        0        0    31065 2023-05-23 03:15:43.116571 nspyre-0.6.0/src/nspyre/gui/widgets/flex_line_plot.py
+-rw-r--r--   0        0        0     4108 2023-05-10 15:52:37.130396 nspyre-0.6.0/src/nspyre/gui/widgets/layout.py
+-rw-r--r--   0        0        0    16128 2023-05-23 03:15:24.132503 nspyre-0.6.0/src/nspyre/gui/widgets/line_plot.py
+-rw-r--r--   0        0        0     7060 2023-05-23 02:53:28.371745 nspyre-0.6.0/src/nspyre/gui/widgets/load.py
+-rw-r--r--   0        0        0     9725 2023-05-23 03:02:47.121797 nspyre-0.6.0/src/nspyre/gui/widgets/main.py
+-rw-r--r--   0        0        0     7581 2023-05-23 03:05:58.638486 nspyre-0.6.0/src/nspyre/gui/widgets/params.py
+-rw-r--r--   0        0        0     7177 2023-05-23 02:52:37.151551 nspyre-0.6.0/src/nspyre/gui/widgets/save.py
+-rw-r--r--   0        0        0      714 2023-05-10 16:01:06.724155 nspyre-0.6.0/src/nspyre/gui/widgets/separator.py
+-rw-r--r--   0        0        0     1041 2023-04-01 17:12:58.468408 nspyre-0.6.0/src/nspyre/gui/widgets/snake.py
+-rw-r--r--   0        0        0     5731 2023-05-10 16:15:21.798822 nspyre-0.6.0/src/nspyre/gui/widgets/subsystem.py
+-rw-r--r--   0        0        0     2692 2023-05-10 15:44:12.280514 nspyre-0.6.0/src/nspyre/gui/widgets/update_loop.py
+-rw-r--r--   0        0        0      300 2023-04-12 23:30:05.012100 nspyre-0.6.0/src/nspyre/instrument/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-22 03:38:56.309872 nspyre-0.6.0/src/nspyre/instrument/gateway.py
+-rw-r--r--   0        0        0     4249 2023-05-23 02:59:03.800986 nspyre-0.6.0/src/nspyre/instrument/manager.py
+-rw-r--r--   0        0        0    12718 2023-05-23 03:00:48.633368 nspyre-0.6.0/src/nspyre/instrument/server.py
+-rw-r--r--   0        0        0       93 2023-05-07 22:07:03.250115 nspyre-0.6.0/src/nspyre/misc/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-10 15:44:31.736591 nspyre-0.6.0/src/nspyre/misc/_stacktracer.py
+-rw-r--r--   0        0        0     5290 2023-05-23 03:01:33.457531 nspyre-0.6.0/src/nspyre/misc/logging.py
+-rw-r--r--   0        0        0     7892 2023-05-22 04:32:20.964750 nspyre-0.6.0/src/nspyre/misc/misc.py
+-rw-r--r--   0        0        0     2612 2023-05-10 17:01:20.811758 nspyre-0.6.0/src/nspyre/misc/pint.py
+-rw-r--r--   0        0        0     3441 1970-01-01 00:00:00.000000 nspyre-0.6.0/setup.py
+-rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 nspyre-0.6.0/PKG-INFO
```

### Comparing `nspyre-0.5.0/LICENSE` & `nspyre-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nspyre-0.5.0/src/nspyre/cli/dataserv_cli.py` & `nspyre-0.6.0/src/nspyre/cli/dataserv.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import logging
 import pdb
 import signal
 from cmd import Cmd
 from pathlib import Path
 from threading import Thread
 
-from ..dataserv.dataserv import _DataServer
+from ..data.server import DataServer
 from ..misc.logging import LOG_FILE_MAX_SIZE
 from ..misc.logging import nspyre_init_logger
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
-class DataservCmdPrompt(Cmd):
+class _DataservCmdPrompt(Cmd):
     """Data Server shell prompt processor"""
 
     def __init__(self, dataserv):
         super().__init__()
         self.dataserv = dataserv
 
     def emptyline(self):
@@ -37,44 +37,45 @@
             print(d)
 
     def do_debug(self, arg_string):
         """Drop into the debugging console"""
         if arg_string:
             print('Expected 0 args')
             return
+        # use self.dataserv.datasets['my_dataset'] to access datasets directly
         pdb.set_trace()
 
     def do_quit(self, arg_string):
         """Quit the program"""
         if arg_string:
             print('Expected 0 args')
             return
-        logger.info('exiting...')
+        _logger.info('exiting...')
         # stop the server
         self.dataserv.stop()
         # notify the command loop to exit
         return True
 
 
-def dataserv_cli(dataserv):
+def serve_data_server_cli(dataserv):
     """Run a command-line interface to allow user interaction with the data server.
 
     Args:
-        dataserv: DataServer object.
+        dataserv: :py:class:`~nspyre.data.server.DataServer` object.
     """
     # start the shell prompt event loop
-    dataserv_cmd = DataservCmdPrompt(dataserv)
+    dataserv_cmd = _DataservCmdPrompt(dataserv)
     dataserv_cmd.prompt = 'dataserv > '
     try:
         dataserv_cmd.cmdloop('')
     except KeyboardInterrupt:
         pass
 
 
-def main():
+def _main():
     """Entry point for data server"""
 
     # parse command-line arguments
     arg_parser = argparse.ArgumentParser(
         prog='nspyre-dataserv', description='Run an nspyre data server'
     )
     arg_parser.add_argument(
@@ -126,31 +127,34 @@
             )
         else:
             # the user asked for no log file
             nspyre_init_logger(log_level)
 
     # init the data server
     if cmd_args.port:
-        dataserv = _DataServer(cmd_args.port)
+        dataserv = DataServer(cmd_args.port)
     else:
-        dataserv = _DataServer()
+        dataserv = DataServer()
 
     # properly stop the server when a kill signal is received
     def stop_server(signum, frame):
         dataserv.stop()
 
     signal.signal(signal.SIGINT, stop_server)
     signal.signal(signal.SIGTERM, stop_server)
 
     # start the shell prompt event loop in a new thread, since DataServer
     # must be run in the main thread
-    # daemon=True so that the program will exit when the data server is stopped with a signal - otherwise the cmd loop will hang forever
-    cmd_prompt_thread = Thread(target=dataserv_cli, args=(dataserv, ), daemon=True)
+    # daemon=True so that the program will exit when the data server is stopped with
+    # a signal - otherwise the cmd loop will hang forever
+    cmd_prompt_thread = Thread(
+        target=serve_data_server_cli, args=(dataserv,), daemon=True
+    )
     cmd_prompt_thread.start()
 
     # start the data server event loop
-    logger.info('starting data server...')
+    _logger.info('starting data server...')
     dataserv.serve_forever()
 
 
 if __name__ == '__main__':
-    main()
+    _main()
```

### Comparing `nspyre-0.5.0/src/nspyre/cli/inserv_cli.py` & `nspyre-0.6.0/src/nspyre/cli/inserv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #!/usr/bin/env python
 """
 Serves a shell prompt allowing the user runtime control of the instrument server.
 """
 import argparse
-from cmd import Cmd
 import logging
 import pdb
 import signal
+from cmd import Cmd
 from pathlib import Path
 from typing import Union
 
-from ..inserv.gateway import InstrumentGateway
-from ..inserv.gateway import InstrumentGatewayError
-from ..inserv.inserv import InstrumentServer
-from ..inserv.inserv import InstrumentServerError
+from ..instrument.gateway import InstrumentGateway
+from ..instrument.gateway import InstrumentGatewayError
+from ..instrument.server import InstrumentServer
+from ..instrument.server import InstrumentServerError
 from ..misc.logging import LOG_FILE_MAX_SIZE
 from ..misc.logging import nspyre_init_logger
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
-def inserv_cli(inserv):
-    """Run a command-line interface to allow user interaction with the instrument server.
+def serve_instrument_server_cli(inserv):
+    """Run a command-line interface to allow user interaction with the instrument \
+    server.
 
     Args:
-        inserv: InstrumentServer or InstrumentGateway object.
+        inserv: :py:class:`~nspyre.instrument.server.InstrumentServer` or
+            :py:class:`~nspyre.instrument.gateway.InstrumentGateway` object.
     """
     # start the shell prompt event loop
-    cmd_prompt = InservCmdPrompt(inserv)
+    cmd_prompt = _InservCmdPrompt(inserv)
     cmd_prompt.prompt = 'inserv > '
     try:
         cmd_prompt.cmdloop('')
     except KeyboardInterrupt:
         pass
 
 
-class InservCmdPrompt(Cmd):
+class _InservCmdPrompt(Cmd):
     """Instrument Server shell prompt processor"""
 
     def __init__(self, inserv: Union[InstrumentServer, InstrumentGateway]):
         super().__init__()
         self.inserv = inserv
 
     def emptyline(self):
@@ -60,69 +62,88 @@
         if not arg_string or len(args) > 1:
             print('Expected 1 arg: device name')
             return
         dev_name = args[0]
         try:
             self.inserv.remove(dev_name)
         except Exception as exc:
-            logger.exception(exc)
+            _logger.exception(exc)
             print(f'Failed to delete device [{dev_name}]')
             return
 
     def do_restart(self, arg_string: str):
         """Restart a device\narg 1: <string> the device name"""
         args = arg_string.split(' ')
         if not arg_string or len(args) > 1:
             print('Expected 1 arg: device name')
             return
         dev_name = args[0]
         try:
             self.inserv.restart(dev_name)
         except Exception as exc:
-            logger.exception(exc)
+            _logger.exception(exc)
             print(f'Failed to reload device [{dev_name}]')
             return
 
     def do_restart_all(self, arg_string: str):
         """Restart all devices"""
         if arg_string:
             print('Expected 0 args')
             return
         try:
             self.inserv.restart_all()
         except Exception as exc:
-            logger.exception(exc)
+            _logger.exception(exc)
             print('Failed to reload all devices')
             return
 
     def do_py(self, arg_string: str):
-        """Drop into the pdb (python debugger) console. From there, arbitrary Python commands can be executed and/or the instrument server can be debugged. Enter "c" or "continue" to return to the main inserv console. The instrument gateway/server object can be accessed via "self.inserv". If the instrument server was created in this session, self.inserv will be an InstrumentServer object. If a server was connected to, it will be an InstrumentGateway. See instrument gateway/server documentation for details on how to add/manipulate drivers."""
+        """Drop into the pdb (python debugger) console. From there, arbitrary
+        Python commands can be executed and/or the instrument server can be
+        debugged. Enter "c" or "continue" to return to the main inserv console.
+        The instrument gateway/server object can be accessed via
+        :code:`self.inserv`. If the instrument server was created in this
+        session, :code:`self.inserv` will be an
+        :py:class:`~nspyre.instrument.server.InstrumentServer` object. If a server
+        was connected to, it will be an
+        :py:class:`~nspyre.instrument.gateway.InstrumentGateway`. See
+        :py:class:`~nspyre.instrument.server.InstrumentServer`/
+        :py:class:`~nspyre.instrument.gateway.InstrumentGateway`
+        documentation for details on how to add/manipulate drivers."""
         if arg_string:
             print('Expected 0 args')
             return
         # use self.inserv.devs()['my_device'] to access drivers directly
         pdb.set_trace()
 
     def do_quit(self, arg_string: str):
         """Quit the program"""
         if arg_string:
             print('Expected 0 args')
             return
-        logger.info('exiting...')
+        _logger.info('exiting...')
 
         raise SystemExit
 
 
-def main():
-    """Entry point for instrument server CLI"""
+def start_instrument_server(drivers=None, inserv_kwargs=None):
+    """Start an instrument server and serve a CLI.
+
+    Args:
+        drivers: A list of dictionaries, where each dictionary contains keyword
+            arguments to the InstrumentServer
+            :py:meth:`~nspyre.instrument.server.InstrumentServer.add` method.
+        inserv_kwargs: Keyword args to pass to InstrumentServer, as in
+            :code:`InstrumentServer(**inserv_kwargs)`.
+    """
 
     # parse command-line arguments
     arg_parser = argparse.ArgumentParser(
-        prog='nspyre-inserv',
-        description='Start or connect to an nspyre instrument server. By default, an attempt will be made to connect to an existing server. To create a new server, use the -s option.',
+        description='Start or connect to an nspyre instrument server. By default, an '
+        'attempt will be made to connect to an existing server.'
     )
     arg_parser.add_argument(
         '-a',
         '--address',
         default=None,
         help='address of an existing instrument server to connect to',
     )
@@ -142,15 +163,15 @@
     arg_parser.add_argument(
         '-q', '--quiet', action='store_true', help='disable logging'
     )
     arg_parser.add_argument(
         '-s',
         '--start',
         action='store_true',
-        help='start a new instrument server',
+        help='don\'t attempt connecting - just start a new instrument server',
     )
     arg_parser.add_argument(
         '-v',
         '--verbosity',
         default='info',
         help='the verbosity of logging to stdout - options are: '
         'debug, info, warning, error',
@@ -165,15 +186,15 @@
             log_level = logging.INFO
         elif cmd_args.verbosity.lower() == 'warning':
             log_level = logging.WARNING
         elif cmd_args.verbosity.lower() == 'error':
             log_level = logging.ERROR
         else:
             raise InstrumentServerError(
-                'didn\'t recognize logging level [{}]'.format(cmd_args.verbosity)
+                f'Didn\'t recognize logging level [{cmd_args.verbosity}].'
             )
 
         if cmd_args.log:
             nspyre_init_logger(
                 log_level,
                 log_path=Path(cmd_args.log),
                 log_path_level=logging.DEBUG,
@@ -181,39 +202,32 @@
                 file_size=LOG_FILE_MAX_SIZE,
             )
         else:
             # the user asked for no log file
             nspyre_init_logger(log_level)
 
     # keyword args to pass to the inserv / gateway instantiation
-    inserv_kwargs = {}
+    if inserv_kwargs is None:
+        inserv_kwargs = {}
     if cmd_args.address:
         inserv_kwargs['addr'] = cmd_args.address
     if cmd_args.port:
         inserv_kwargs['port'] = cmd_args.port
 
     # whether a new instrument server should be started
     new_server = False
     if cmd_args.start:
         new_server = True
     else:
         # try connecting to a running instrument server
         try:
             inserv = InstrumentGateway(**inserv_kwargs)
             inserv.connect()
-        except InstrumentGatewayError as exc:
-            logger.exception(exc)
-            answer = input(
-                'Failed connecting to the Instrument Server. Create one? [Y/n] '
-            )
-            if answer in ['y', 'Y', '']:
-                new_server = True
-            else:
-                logger.info('exiting...')
-                return
+        except InstrumentGatewayError:
+            new_server = True
 
     if new_server:
         # start a new instrument server
         inserv = InstrumentServer(**inserv_kwargs)
 
         # properly stop the server when a kill signal is received
         def stop_server(signum, frame):
@@ -221,13 +235,28 @@
             raise SystemExit
 
         signal.signal(signal.SIGINT, stop_server)
         signal.signal(signal.SIGTERM, stop_server)
 
         inserv.start()
 
-    # start the shell prompt event loop
-    inserv_cli(inserv)
+    try:
+        # add the provided drivers
+        if drivers is not None:
+            for d in drivers:
+                inserv.add(**d)
+
+        # start the shell prompt event loop
+        serve_instrument_server_cli(inserv)
+    except Exception as err:
+        raise err
+    finally:
+        if new_server:
+            inserv.stop()
+
+
+def _main():
+    start_instrument_server()
 
 
 if __name__ == '__main__':
-    main()
+    _main()
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/app.py` & `nspyre-0.6.0/src/nspyre/gui/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,87 +8,87 @@
 
 from pyqtgraph import _connectCleanup
 from pyqtgraph import setConfigOptions
 from pyqtgraph.Qt import QtCore
 from pyqtgraph.Qt import QtGui
 from pyqtgraph.Qt import QtWidgets
 
-from .style.style import nspyre_font
-from .style.style import nspyre_palette
-from .style.style import nspyre_style_sheet
+from .style._style import nspyre_font
+from .style._style import nspyre_palette
+from .style._style import nspyre_style_sheet
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
-HERE = Path(__file__).parent
+_HERE = Path(__file__).parent
 
 
 class nspyreApp(QtWidgets.QApplication):
     """Create a Qt application object with the default nspyre settings.
 
     Typical usage example:
 
     .. code-block:: python
 
-        from nspyre import NspyreApp
+        from nspyre import nspyreApp
 
-        app = NspyreApp()
+        app = nspyreApp()
         some_widget = SomeWidget()
         some_widget.show()
-        # run the GUI event loop
         app.exec()
 
     """
 
     def __init__(
         self,
         app_name: str = 'nspyre',
         palette: QtGui.QPalette = nspyre_palette,
         font: QtGui.QFont = nspyre_font,
     ):
         """
         Args:
-            app_name: display name of the application.
-            palette: Qt palette
+            app_name: Display name of the application.
+            palette: Qt palette.
             font: QFont to use for the application.
         """
         # for high DPI displays in Qt5
         if hasattr(QtCore.Qt, 'AA_EnableHighDpiScaling'):
             QtCore.QCoreApplication.setAttribute(
                 QtCore.Qt.AA_EnableHighDpiScaling, True
             )
         if hasattr(QtCore.Qt, 'AA_UseHighDpiPixmaps'):
             QtCore.QCoreApplication.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps, True)
 
         super().__init__(sys.argv)
 
         self.setApplicationName(app_name)
         # dock icon
-        icon_path = HERE / 'images' / 'favicon.ico'
+        icon_path = _HERE / 'images' / 'favicon.ico'
         self.setWindowIcon(QtGui.QIcon(str(icon_path)))
 
         # make sure pyqtgraph gets cleaned up properly
         _connectCleanup()
         # enable plot antialiasing
         setConfigOptions(antialias=True)
 
         # appearance settings for nspyre
         self.setStyle(QtWidgets.QStyleFactory.create('Fusion'))
         self.setPalette(palette)
         self.setStyleSheet(nspyre_style_sheet)
         self.setFont(font)
 
     def exec(self, *args, **kwargs):
+        """Run the GUI event loop."""
         try:
             super().exec(*args, **kwargs)
         except AttributeError:
             super().exec_(*args, **kwargs)
         # invoke garbage collector to make sure we don't get any false leak reports
         gc.collect()
         # report Qt leaks
         leaked_widgets = self.allWidgets()
         if leaked_widgets:
             leaked_str = f'Leaked {len(leaked_widgets)} Qt widgets:\n'
             for w in leaked_widgets:
                 leaked_str += repr(w) + '\n'
-            logger.debug(leaked_str)
+            _logger.debug(leaked_str)
         else:
-            logger.debug('No Qt widgets leaked.')
+            _logger.debug('No Qt widgets leaked.')
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/images/favicon.ico` & `nspyre-0.6.0/src/nspyre/gui/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `nspyre-0.5.0/src/nspyre/gui/images/ssssspin.png` & `nspyre-0.6.0/src/nspyre/gui/images/ssssspin.png`

 * *Files identical despite different names*

### Comparing `nspyre-0.5.0/src/nspyre/gui/misc.py` & `nspyre-0.6.0/src/nspyre/gui/debug.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-A collection of miscellaneous functionality for GUIs.
+A collection of miscellaneous functionality for Qt GUIs.
 """
 import logging
 from pdb import set_trace
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 try:
     from pyqtgraph.Qt.QtCore import pyqtRemoveInputHook
 except ImportError:
-    qt_remove_hook = False
-    logger.debug(
+    _qt_remove_hook = False
+    _logger.debug(
         'Ignoring Qt remove hook because the PyQt implementation doesn\'t required it.'
     )
 else:
-    qt_remove_hook = True
-    logger.debug('Using PyQt remove input hook.')
+    _qt_remove_hook = True
+    _logger.debug('Using PyQt remove input hook.')
 
 
 def qt_set_trace():
     """Set a tracepoint in the Python debugger (pdb) that works with Qt."""
-    if qt_remove_hook:
+    if _qt_remove_hook:
         pyqtRemoveInputHook()
     set_trace()
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/style/style.py` & `nspyre-0.6.0/src/nspyre/gui/style/_style.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 nspyre application style settings.
 """
 from pathlib import Path
 
 from pyqtgraph.Qt import QtCore
 from pyqtgraph.Qt import QtGui
 
-from .colors import almost_white
-from .colors import avg_colors
-from .colors import blackish
-from .colors import dark_grey
-from .colors import grey
+from ._colors import almost_white
+from ._colors import avg_colors
+from ._colors import blackish
+from ._colors import dark_grey
+from ._colors import grey
 
 HERE = Path(__file__).parent
 
 # nspyre color scheme
 nspyre_palette = QtGui.QPalette()
 nspyre_palette.setColor(QtGui.QPalette.ColorRole.AlternateBase, QtGui.QColor(*grey))
 nspyre_palette.setColor(QtGui.QPalette.ColorRole.Base, QtGui.QColor(*blackish))
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/style/style.qss` & `nspyre-0.6.0/src/nspyre/gui/style/style.qss`

 * *Files identical despite different names*

### Comparing `nspyre-0.5.0/src/nspyre/gui/widgets/flex_line_plot_widget.py` & `nspyre-0.6.0/src/nspyre/gui/widgets/flex_line_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,389 @@
-"""
-A plotting widget that connects to an nspyre data server, collects and processes the data, and offers a variety of user-controlled plotting options.
-"""
 import logging
 import time
-from threading import Lock
+from collections import namedtuple
+from typing import Callable
+from typing import Optional
 
 import numpy as np
 from pyqtgraph.Qt import QtCore
 from pyqtgraph.Qt import QtGui
 from pyqtgraph.Qt import QtWidgets
 
-from ...dataserv.dataserv import DataSink
-from .line_plot_widget import LinePlotWidget
+from ...data.sink import DataSink
+from ..threadsafe import QThreadSafeObject
+from .layout import tree_layout
+from .line_plot import LinePlotWidget
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
-class FlexLinePlotWidget(QtWidgets.QWidget):
-    """QWidget that allows the user to connect to an arbitrary nspyre DataSource and plot its data.
+_FlexLinePlotSeriesSettings = namedtuple(
+    '_FlexLinePlotSeriesSettings',
+    ['series', 'scan_i', 'scan_j', 'processing', 'hidden'],
+)
+"""Contain the settings for a single plot."""
 
-    The DataSource may contain the following attributes:
 
-    - title: plot title string
-    - xlabel: x label string
-    - ylabel: y label string
-    - datasets: dictionary where keys are a data series name, and values are data as a list of 2D numpy array like::
+class _FlexLinePlotSettings(QThreadSafeObject):
+    """Container class to hold the plot settings for a _FlexLinePlotWidget."""
 
-        [np.array([[x0, x1, ...], [y0, y1, ...]]), np.array([[x10, x11, ...], [y10, y11, ...]]), ...]
+    def __init__(self):
+        self.series_settings = {}
+        # DataSink for pulling plot data from the data server
+        self.sink = None
+        # protect access to the sink
+        self.sink_mutex = QtCore.QMutex()
+        # flag indicating that the plots should be updated
+        self.force_update = False
+        super().__init__()
+
+    def get_settings(self, name: str, callback=None):
+        with QtCore.QMutexLocker(self.mutex):
+            settings = self.series_settings[name]
+            if callback is not None:
+                self.run_main(callback, name, settings, blocking=True)
+
+    def add_plot(
+        self,
+        name: str,
+        series: str,
+        scan_i: str,
+        scan_j: str,
+        processing: str,
+        hidden: bool,
+        callback: Optional[Callable] = None,
+    ):
+        with QtCore.QMutexLocker(self.mutex):
+            if name in self.series_settings:
+                _logger.info(
+                    f'A plot with the name [{name}] already exists. Ignoring add_plot '
+                    'request.'
+                )
+                return
+            self.series_settings[name] = _FlexLinePlotSeriesSettings(
+                series=series,
+                scan_i=scan_i,
+                scan_j=scan_j,
+                processing=processing,
+                hidden=hidden,
+            )
+            self.force_update = True
+            if callback is not None:
+                self.run_main(callback, name, blocking=True)
+
+    def remove_plot(self, name, callback=None):
+        with QtCore.QMutexLocker(self.mutex):
+            if name not in self.series_settings:
+                _logger.info(
+                    f'A plot with the name [{name}] does not exist. Ignoring '
+                    'remove_plot request.'
+                )
+                return
+
+            if callback is not None:
+                self.run_main(callback, name, blocking=True)
+
+            del self.series_settings[name]
+
+    def hide_plot(self, name, callback=None):
+        with QtCore.QMutexLocker(self.mutex):
+            if name not in self.series_settings:
+                _logger.info(
+                    f'A plot with the name [{name}] does not exist. Ignoring '
+                    'hide_plot request.'
+                )
+                return
+            if self.series_settings[name].hidden:
+                _logger.info(
+                    f'The plot [{name}] is already hidden. Ignoring hide_plot request.'
+                )
+                return
+            self.series_settings[name].hidden = True
+            if callback is not None:
+                self.run_main(callback, name, blocking=True)
+
+    def show_plot(self, name, callback=None):
+        with QtCore.QMutexLocker(self.mutex):
+            if name not in self.series_settings:
+                _logger.info(
+                    f'A plot with the name [{name}] does not exist. Ignoring show_plot '
+                    'request.'
+                )
+                return
+            if not self.series_settings[name].hidden:
+                _logger.info(
+                    f'The plot [{name}] is already shown. Ignoring show_plot request.'
+                )
+                return
+            self.series_settings[name].hidden = False
+            if callback is not None:
+                self.run_main(callback, name, blocking=True)
+
+    def update_settings(self, name, series, scan_i, scan_j, processing):
+        with QtCore.QMutexLocker(self.mutex):
+            if name not in self.series_settings:
+                _logger.info(
+                    f'A plot with the name [{name}] does not exist. Ignoring '
+                    'update_settings request.'
+                )
+                return
+            self.series_settings[name].series = series
+            self.series_settings[name].scan_i = scan_i
+            self.series_settings[name].scan_j = scan_j
+            self.series_settings[name].processing = processing
+            self.force_update = True
+
+
+class FlexLinePlotWidget(QtWidgets.QWidget):
+    """Qt widget for flexible plotting of user data.
+    It connects to an arbitrary data set stored in the
+    :py:class:`~nspyre.data.server.DataServer`, collects and processes the data, and
+    offers a variety of user-controlled plotting options.
+
+    The user should push a dictionary containing the following key/value pairs
+    to the corresponding :py:class:`~nspyre.data.source.DataSource`
+    object sourcing data to the :py:class:`~nspyre.data.server.DataServer`:
+
+    - key: :code:`title`, value: Plot title string
+    - key: :code:`xlabel`, value: X label string
+    - key: :code:`ylabel`, value: Y label string
+    - key: :code:`datasets`, value: Dictionary where keys are a data series \
+        name, and values are data as a list of 2D numpy arrays of shape (2, n). \
+        The two rows represent the x and y axes, respectively, of the plot, and \
+        the n columns each represent a data point.
+
+    You may use np.NaN values in the data arrays to represent invalid entries,
+    which won't contribute to the data averaging. An example is given below:
+
+    .. code-block:: python
+
+        from nspyre import DataSource, StreamingList
+
+        with DataSource('my_dataset') as ds:
+            channel_1_data = StreamingList([np.array([[1, 2, 3], [12, 12.5, 12.25]]), \
+np.array([[4, 5, 6], [12.6, 13, 11.2]])])
+            channel_2_data = StreamingList([np.array([[1, 2, 3], [3, 3.3, 3.1]]), \
+np.array([[4, 5, 6], [3.4, 3.6, 3.5]])])
+            my_plot_data = {
+                'title': 'MyVoltagePlot',
+                'xlabel': 'Time (s)',
+                'ylabel': 'Amplitude (V)',
+                'datasets': {
+                    'channel_1': channel_1_data
+                    'channel_2': channel_2_data
+                }
+            }
+            ds.push(my_plot_data)
 
     """
 
-    def __init__(self):
+    def __init__(
+        self, timeout: float = 1, data_processing_func: Optional[Callable] = None
+    ):
+        """
+        Args:
+            timeout: Timeout for :py:meth:`~nspyre.data.sink.DataSink.pop`.
+            data_processing_func: Function to do any post-processing of the data
+                popped by the :py:class:`~nspyre.data.sink.DataSink`. Takes one
+                argument, which is the :py:class:`~nspyre.data.sink.DataSink`.
+        """
         super().__init__()
 
-        layout = QtWidgets.QVBoxLayout()
-
-        # lineplot widget
-        self.flex_line_plot = _FlexLinePlotWidget()
+        self.line_plot = _FlexLinePlotWidget(
+            timeout=timeout, data_processing_func=data_processing_func
+        )
+        """Underlying LinePlotWidget."""
 
-        # lineedit and button for selecting the data source
-        datasource_layout = QtWidgets.QHBoxLayout()
+        # data source lineedit
         self.datasource_lineedit = QtWidgets.QLineEdit()
-        self.update_button = QtWidgets.QPushButton('Connect')
-        self.update_button.clicked.connect(self._update_source_clicked)
-        datasource_layout.addWidget(QtWidgets.QLabel('Data Set'))
-        datasource_layout.addWidget(self.datasource_lineedit)
-        datasource_layout.addWidget(self.update_button)
 
-        # contains plot settings
-        plot_settings_layout = QtWidgets.QHBoxLayout()
+        # data source connect button
+        connect_button = QtWidgets.QPushButton('Connect')
+        connect_button.clicked.connect(self._update_source_clicked)
 
-        # add new subplot layout
-        plot_add_layout = QtWidgets.QVBoxLayout()
+        # plot settings label
         plot_settings_label = QtWidgets.QLabel('Plot Settings')
         plot_settings_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter)
-        plot_add_layout.addWidget(plot_settings_label)
 
-        # plot name
-        plot_name_layout = QtWidgets.QHBoxLayout()
-        plot_name_layout.addWidget(QtWidgets.QLabel('Name'))
+        # plot name lineedit
         self.plot_name_lineedit = QtWidgets.QLineEdit('avg')
-        plot_name_layout.addWidget(self.plot_name_lineedit)
-        plot_add_layout.addLayout(plot_name_layout)
 
-        # plot series
-        plot_data_series_layout = QtWidgets.QHBoxLayout()
-        plot_data_series_layout.addWidget(QtWidgets.QLabel('Series'))
-        self.plot_series_lineedit = QtWidgets.QLineEdit('mydata')
-        plot_data_series_layout.addWidget(self.plot_series_lineedit)
-        plot_add_layout.addLayout(plot_data_series_layout)
-
-        # scan indices layout
-        scan_indices_layout = QtWidgets.QHBoxLayout()
-        scan_indices_layout.addWidget(QtWidgets.QLabel('Scan'))
+        # data series lineedit
+        self.plot_series_lineedit = QtWidgets.QLineEdit('series1')
+
+        # scan indices lineedits
         self.add_plot_scan_i_textbox = QtWidgets.QLineEdit()
-        scan_indices_layout.addWidget(self.add_plot_scan_i_textbox)
-        scan_indices_layout.addWidget(QtWidgets.QLabel(' to '))
         self.add_plot_scan_j_textbox = QtWidgets.QLineEdit()
-        scan_indices_layout.addWidget(self.add_plot_scan_j_textbox)
 
-        plot_add_layout.addLayout(scan_indices_layout)
-
-        # average / append
-        plot_processing_layout = QtWidgets.QHBoxLayout()
+        # avg/append label
         plot_processing_label = QtWidgets.QLabel('Processing')
         plot_processing_label.setSizePolicy(
             QtWidgets.QSizePolicy(
                 QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed
             )
         )
-        plot_processing_layout.addWidget(plot_processing_label)
+
+        # avg/append dropdown
         self.plot_processing_dropdown = QtWidgets.QComboBox()
         self.plot_processing_dropdown.addItem('Average')  # index 0
         self.plot_processing_dropdown.addItem('Append')  # index 1
         # default to average
         self.plot_processing_dropdown.setCurrentIndex(0)
-        plot_processing_layout.addWidget(self.plot_processing_dropdown)
-        plot_add_layout.addLayout(plot_processing_layout)
-
-        plot_add_layout.addStretch()
-        plot_settings_layout.addLayout(plot_add_layout)
-        # set to minimum size
-        plot_add_layout.setSizeConstraint(
-            QtWidgets.QLayout.SizeConstraint.SetMinimumSize
-        )
 
-        # subplot show/hide/add/del buttons
-        plot_actions_layout = QtWidgets.QVBoxLayout()
         # show button
-        self.show_button = QtWidgets.QPushButton('Show')
-        self.show_button.clicked.connect(self._show_plot_clicked)
-        plot_actions_layout.addWidget(self.show_button)
+        show_button = QtWidgets.QPushButton('Show')
+        show_button.clicked.connect(self._show_plot_clicked)
+
         # hide button
-        self.hide_button = QtWidgets.QPushButton('Hide')
-        self.hide_button.clicked.connect(self._hide_plot_clicked)
-        plot_actions_layout.addWidget(self.hide_button)
+        hide_button = QtWidgets.QPushButton('Hide')
+        hide_button.clicked.connect(self._hide_plot_clicked)
+
         # update button
-        self.add_plot_button = QtWidgets.QPushButton('Update')
-        self.add_plot_button.clicked.connect(self._update_plot_clicked)
-        plot_actions_layout.addWidget(self.add_plot_button)
+        update_plot_button = QtWidgets.QPushButton('Update')
+        update_plot_button.clicked.connect(self._update_plot_clicked)
+
         # add button
-        self.add_plot_button = QtWidgets.QPushButton('Add')
-        self.add_plot_button.clicked.connect(self._add_plot_clicked)
-        plot_actions_layout.addWidget(self.add_plot_button)
+        add_plot_button = QtWidgets.QPushButton('Add')
+        add_plot_button.clicked.connect(self._add_plot_clicked)
+
         # del button
-        self.remove_button = QtWidgets.QPushButton('Remove')
-        self.remove_button.clicked.connect(self._remove_plot_clicked)
-        plot_actions_layout.addWidget(self.remove_button)
-        plot_actions_layout.addStretch()
-        plot_settings_layout.addLayout(plot_actions_layout)
+        remove_button = QtWidgets.QPushButton('Remove')
+        remove_button.clicked.connect(self._remove_plot_clicked)
+
+        # plots label
+        plots_label = QtWidgets.QLabel('Plots')
+        plots_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter)
 
         # list of plots
         self.plots_list_widget = QtWidgets.QListWidget()
         self.plots_list_widget.currentItemChanged.connect(self._plot_selection_changed)
-        plot_settings_layout.addWidget(self.plots_list_widget)
 
-        # layout for containing the data source selection layout and the plot settings layout
-        settings_layout = QtWidgets.QVBoxLayout()
-        settings_layout.addLayout(datasource_layout)
-        settings_layout.addLayout(plot_settings_layout)
-        # widget for containing the settings layout
-        settings_widget = QtWidgets.QWidget()
-        settings_widget.setLayout(settings_layout)
+        # spacer
+        fixed_spacer = QtWidgets.QLabel('')
+        fixed_spacer.setSizePolicy(
+            QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed
+        )
+
+        # spacer
+        expanding_spacer = QtWidgets.QLabel('')
+        expanding_spacer.setSizePolicy(
+            QtWidgets.QSizePolicy.Policy.Expanding,
+            QtWidgets.QSizePolicy.Policy.Expanding,
+        )
+
+        # layout
+        settings_layout_config = {
+            'type': QtWidgets.QVBoxLayout,
+            'data_source': {
+                'type': QtWidgets.QHBoxLayout,
+                'label': QtWidgets.QLabel('Data Set'),
+                'edit': self.datasource_lineedit,
+                'button': connect_button,
+            },
+            'config': {
+                'type': QtWidgets.QHBoxLayout,
+                'plot': {
+                    'type': QtWidgets.QVBoxLayout,
+                    'label': plot_settings_label,
+                    'settings': {
+                        'type': QtWidgets.QVBoxLayout,
+                        'name': {
+                            'type': QtWidgets.QHBoxLayout,
+                            'label': QtWidgets.QLabel('Plot Name'),
+                            'edit': self.plot_name_lineedit,
+                        },
+                        'series': {
+                            'type': QtWidgets.QHBoxLayout,
+                            'label': QtWidgets.QLabel('Data Series'),
+                            'edit': self.plot_series_lineedit,
+                        },
+                        'index': {
+                            'type': QtWidgets.QHBoxLayout,
+                            'l1': QtWidgets.QLabel('Scan'),
+                            'i': self.add_plot_scan_i_textbox,
+                            'l2': QtWidgets.QLabel(' to '),
+                            'j': self.add_plot_scan_j_textbox,
+                        },
+                        'processing': {
+                            'type': QtWidgets.QHBoxLayout,
+                            'label': plot_processing_label,
+                            'dropdown': self.plot_processing_dropdown,
+                        },
+                        'spacer': expanding_spacer,
+                    },
+                },
+                'settings_buttons': {
+                    'type': QtWidgets.QVBoxLayout,
+                    'spacer_t': fixed_spacer,
+                    'update': update_plot_button,
+                    'add': add_plot_button,
+                    'remove': remove_button,
+                    'spacer_b': expanding_spacer,
+                },
+                'plots': {
+                    'type': QtWidgets.QVBoxLayout,
+                    'label': plots_label,
+                    'list': self.plots_list_widget,
+                },
+                'list_buttons': {
+                    'type': QtWidgets.QVBoxLayout,
+                    'spacer_t': fixed_spacer,
+                    'show': show_button,
+                    'hide': hide_button,
+                    'spacer_b': expanding_spacer,
+                },
+            },
+        }
+        self.layout_tree = tree_layout(settings_layout_config)
+        # make the plots list (index=2) take up all extra space (stretch=1)
+        self.layout_tree.config.layout.setStretch(2, 1)
 
         # splitter
         splitter = QtWidgets.QSplitter()
         splitter.setOrientation(QtCore.Qt.Orientation.Vertical)
-        splitter.addWidget(self.flex_line_plot)
-        splitter.addWidget(settings_widget)
+        splitter.addWidget(self.line_plot)
+        layout_container = QtWidgets.QWidget()
+        layout_container.setLayout(self.layout_tree.layout)
+        splitter.addWidget(layout_container)
 
         # main layout
+        layout = QtWidgets.QVBoxLayout()
         layout.addWidget(splitter)
 
         self.setLayout(layout)
 
     def _plot_selection_changed(self):
         """Called when the selected plot changes."""
         # selected QListWidgetItem
         selected_item = self.plots_list_widget.currentItem()
         if selected_item is None:
             return
         # get the selected plot name
         name = selected_item.text()
-        # retrieve all of the associated info for this plot
-        series = self.flex_line_plot.plot_settings[name]['series']
-        scan_i = self.flex_line_plot.plot_settings[name]['scan_i']
-        scan_j = self.flex_line_plot.plot_settings[name]['scan_j']
-        processing = self.flex_line_plot.plot_settings[name]['processing']
-        # update the plot settings GUI elements
+        self.line_plot.plot_settings.run_safe(
+            self.line_plot.plot_settings.get_settings,
+            name,
+            callback=self._plot_selection_changed_callback,
+        )
+
+    def _plot_selection_changed_callback(
+        self, name: str, settings: _FlexLinePlotSeriesSettings
+    ):
+        """Called after the selection is changed to update the plot settings GUI
+        elements."""
         self.plot_name_lineedit.setText(name)
-        self.add_plot_scan_i_textbox.setText(scan_i)
-        self.add_plot_scan_j_textbox.setText(scan_j)
-        self.plot_series_lineedit.setText(series)
-        self.plot_processing_dropdown.setCurrentText(processing)
+        self.plot_series_lineedit.setText(settings.series)
+        self.add_plot_scan_i_textbox.setText(settings.scan_i)
+        self.add_plot_scan_j_textbox.setText(settings.scan_j)
+        self.plot_processing_dropdown.setCurrentText(settings.processing)
 
     def _get_plot_settings(self):
-        """Retrieve the user-entered plot settings from the GUI and check them for errors."""
+        """Retrieve the user-entered plot settings from the GUI and check them for
+        errors."""
         scan_i = self.add_plot_scan_i_textbox.text()
         try:
             if scan_i != '':
                 int(scan_i)
         except ValueError as err:
             raise ValueError(
                 f'Scan start [{scan_i}] must be either an integer or empty.'
@@ -198,60 +402,68 @@
 
         return name, series, scan_i, scan_j, processing
 
     def _update_plot_clicked(self):
         """Called when the user clicks the update button."""
         name, series, scan_i, scan_j, processing = self._get_plot_settings()
         # set the plot settings
-        self.flex_line_plot.update_plot_settings(
-            name, series, scan_i, scan_j, processing
+        self.line_plot.plot_settings.run_safe(
+            self.line_plot.plot_settings.update_settings,
+            name,
+            series,
+            scan_i,
+            scan_j,
+            processing,
         )
 
     def _add_plot_clicked(self):
         """Called when the user clicks the add button."""
         name, series, scan_i, scan_j, processing = self._get_plot_settings()
         self.add_plot(name, series, scan_i, scan_j, processing)
 
     def add_plot(
         self, name: str, series: str, scan_i: str, scan_j: str, processing: str
     ):
         """Add a new subplot.
 
         Args:
-            name: name for the new plot
-            series: see FlexLinePlotWidget doc
-            scan_i: String value of the scan to start plotting from. Use Python
-            list indexing notation e.g. [scan_i, scan_j] = ['-1', ''] for
-            the last element; [scan_i, scan_j] = ['0', '1'] for the first
-            element; [scan_i, scan_j] = ['-3', ''] for the last 3 elements.
-            scan_j: String value of the scan to stop plotting at.
-            processing: 'Average' to average the x and y values of scans i through j, 'Append' to concatenate them
+            name: Name for the new plot.
+            series: The data series name pushed by the \
+                :py:class:`~nspyre.data.source.DataSource`, e.g. \
+                :code:`channel_1` for the example given in \
+                :py:class:`~nspyre.gui.widgets.flex_line_plot.FlexLinePlotWidget`
+            scan_i: String value of the scan to start plotting from.
+            scan_j: String value of the scan to stop plotting at. \
+                Use Python list indexing notation, e.g.:
+
+                - :code:`scan_i = '-1'`, :code:`scan_j = ''` for the last element
+                - :code:`scan_i = '0'`, :code:`scan_j = '1'` for the first element
+                - :code:`scan_i = '-3'`, :code:`scan_j = ''` for the last 3 elements.
+
+            processing: 'Average' to average the x and y values of scans i
+                through j, 'Append' to concatenate them.
         """
-        if name in self.flex_line_plot.plot_settings:
-            raise ValueError(f'Plot [{name}] already exists.')
-        with self.flex_line_plot.mutex:
-            # add the plot to the pyqtgraph plotwidget
-            self.flex_line_plot.add_plot(name)
-            # set the plot settings
-            self.flex_line_plot.plot_settings[name] = {
-                'series': series,
-                'scan_i': scan_i,
-                'scan_j': scan_j,
-                'processing': processing,
-                'hidden': False,
-            }
-            # add the plot name to the list of plots
-            self.plots_list_widget.addItem(name)
+        self.line_plot.plot_settings.run_safe(
+            self.line_plot.plot_settings.add_plot,
+            name,
+            series,
+            scan_i,
+            scan_j,
+            processing,
+            False,
+            callback=self._add_plot_callback,
+        )
+
+    def _add_plot_callback(self, name: str):
+        """Called in main thread after a plot is added."""
+        self.plots_list_widget.addItem(name)
+        self.line_plot.add_plot(name)
 
     def _find_plot_item(self, name):
         """Return the index of the list widget plot item with the given name."""
-        if name not in self.flex_line_plot.plot_settings:
-            raise ValueError(f'Plot [{name}] does not exist.')
-
-        # search for the list widget item whose text is the same as name
         list_widget_index = None
         for i in range(self.plots_list_widget.count()):
             if self.plots_list_widget.item(i).text() == name:
                 list_widget_index = i
                 break
         if list_widget_index is None:
             raise RuntimeError(
@@ -268,246 +480,316 @@
             name = i.text()
             self.remove_plot(name)
 
     def remove_plot(self, name: str):
         """Remove a subplot.
 
         Args:
-            name: name of the subplot
+            name: Name of the subplot.
         """
-        with self.flex_line_plot.mutex:
-            # remove the plot name from the list of plots
-            self.plots_list_widget.takeItem(self._find_plot_item(name))
-            # remove the plot settings
-            self.flex_line_plot.plot_settings.pop(name)
-            # remove the plot from the pyqtgraph plotwidget
-            self.flex_line_plot.remove_plot(name)
+        # remove the plot settings
+        self.line_plot.plot_settings.run_safe(
+            self.line_plot.plot_settings.remove_plot,
+            name,
+            callback=self._remove_plot_callback,
+        )
+
+    def _remove_plot_callback(self, name: str):
+        """Called in main thread after a plot is removed."""
+        # remove the plot name from the list of plots
+        self.plots_list_widget.takeItem(self._find_plot_item(name))
+        # remove the plot from the pyqtgraph plotwidget
+        self.line_plot.remove_plot(name)
 
     def _hide_plot_clicked(self):
         """Called when the user clicks the hide button."""
         # array of selected QListWidgetItems
         selected_items = self.plots_list_widget.selectedItems()
         for i in selected_items:
             name = i.text()
             self.hide_plot(name)
 
     def hide_plot(self, name: str):
         """Hide a subplot.
 
         Args:
-            name: name of the subplot
+            name: Name of the subplot.
         """
-        with self.flex_line_plot.mutex:
-            self.flex_line_plot.plot_settings[name]['hidden'] = True
-            self.flex_line_plot.hide(name)
-            # change the list widget item color scheme
-            idx = self._find_plot_item(name)
-            self.plots_list_widget.item(idx).setForeground(QtCore.Qt.GlobalColor.gray)
-            self.plots_list_widget.item(idx).setBackground(
-                self.palette().color(QtGui.QPalette.ColorRole.Mid)
-            )
+        # update the settings
+        self.line_plot.plot_settings.run_safe(
+            self.line_plot.plot_settings.hide_plot,
+            name,
+            callback=self._hide_plot_callback,
+        )
+
+    def _hide_plot_callback(self, name: str):
+        """Called in main thread after a plot is hidden."""
+        # hide the plot in the pyqtgraph plotting widget
+        self.line_plot.hide_plot(name)
+        # change the list widget item color scheme
+        idx = self._find_plot_item(name)
+        self.plots_list_widget.item(idx).setForeground(QtCore.Qt.GlobalColor.gray)
+        self.plots_list_widget.item(idx).setBackground(
+            self.palette().color(QtGui.QPalette.ColorRole.Mid)
+        )
 
     def _show_plot_clicked(self):
         """Called when the user clicks the show button."""
         # array of selected QListWidgetItems
         selected_items = self.plots_list_widget.selectedItems()
         for i in selected_items:
             name = i.text()
             self.show_plot(name)
 
     def show_plot(self, name: str):
         """Show a previously hidden subplot.
 
         Args:
-            name: name of the subplot
+            name: Name of the subplot.
         """
-        with self.flex_line_plot.mutex:
-            self.flex_line_plot.plot_settings[name]['hidden'] = False
-            self.flex_line_plot.show(name)
-            # return list widget item to normal color scheme
-            # text
-            idx = self._find_plot_item(name)
-            normal_text_color = self.palette().color(QtGui.QPalette.ColorRole.Text)
-            normal_bg_color = self.palette().color(QtGui.QPalette.ColorRole.Base)
-            self.plots_list_widget.item(idx).setForeground(normal_text_color)
-            self.plots_list_widget.item(idx).setBackground(normal_bg_color)
+        # update the settings
+        self.line_plot.plot_settings.run_safe(
+            self.line_plot.plot_settings.show_plot,
+            name,
+            callback=self._show_plot_callback,
+        )
+
+    def _show_plot_callback(self, name: str):
+        """Called after a plot is shown."""
+        # show the plot in the pyqtgraph plotting widget
+        self.line_plot.show_plot(name)
+        # return list widget item to normal color scheme
+        idx = self._find_plot_item(name)
+        normal_text_color = self.palette().color(QtGui.QPalette.ColorRole.Text)
+        normal_bg_color = self.palette().color(QtGui.QPalette.ColorRole.Base)
+        self.plots_list_widget.item(idx).setForeground(normal_text_color)
+        self.plots_list_widget.item(idx).setBackground(normal_bg_color)
 
     def _update_source_clicked(self):
         """Called when the user clicks the connect button."""
-        self.flex_line_plot.new_source(self.datasource_lineedit.text())
+        self.line_plot.new_source(self.datasource_lineedit.text())
 
 
 class _FlexLinePlotWidget(LinePlotWidget):
     """See FlexLinePlotWidget."""
 
-    def __init__(self):
+    def __init__(self, timeout: float, data_processing_func: Optional[Callable]):
+        """
+        Args:
+            timeout: see :py:class:`FlexLinePlotWidget`.
+            data_processing_func: see :py:class:`FlexLinePlotWidget`.
+        """
+        self.timeout = timeout
+        self.data_processing_func = data_processing_func
+        self.plot_settings = _FlexLinePlotSettings()
+        self.plot_settings.start()
         super().__init__()
-        self.sink = None
-        # mutex for protecting access to the data sink and plot settings
-        self.mutex = Lock()
-        self.plot_settings = {}
-        # flag indicating that this is the first pop from the sink
-        self.first = False
-
-    def update_plot_settings(self, name, series, scan_i, scan_j, processing):
-        with self.mutex:
-            if name not in self.plot_settings:
-                raise ValueError(f'Plot [{name}] does not exist.')
-            hidden = self.plot_settings[name]['hidden']
-            self.plot_settings[name] = {
-                'series': series,
-                'scan_i': scan_i,
-                'scan_j': scan_j,
-                'processing': processing,
-                'hidden': hidden,
-            }
 
-    def new_source(self, data_source_name, timeout=1):
-        # connect to a new data set
-        with self.mutex:
-            self.teardown()
-            self.data_source_name = data_source_name
-
-            # clear previous plots
-            self.plot_widget.getPlotItem().clear()
-            self.plots = {}
+    def _stop(self):
+        """Stop the updating and plot data management threads."""
+        self.plot_settings.stop()
+        super()._stop()
+
+    def new_source(self, data_set_name: str):
+        """Connect to a new data set on the data server.
+
+        Args:
+            data_set_name: Name of the new data set.
+        """
+        # run on the plot_settings thread since we'll need to acquire mutexes
+        self.plot_settings.run_safe(self._new_source, data_set_name)
 
-            # try to get the plot title and x/y labels
+    def _new_source(self, data_set_name: str):
+        # connect to a new data set
+        with QtCore.QMutexLocker(self.plot_settings.sink_mutex):
+            self.clear_plots()
             try:
-                self.sink = DataSink(self.data_source_name)
-                self.sink.__enter__()
-                if self.sink.pop(timeout=timeout):
-                    # set title
-                    try:
-                        title = self.sink.title
-                    except AttributeError:
-                        logger.info(
-                            f'Data source [{data_source_name}] has no "title" attribute - skipping...'
-                        )
-                    else:
-                        self.set_title(title)
-                    # set xlabel
-                    try:
-                        xlabel = self.sink.xlabel
-                    except AttributeError:
-                        logger.info(
-                            f'Data source [{data_source_name}] has no "xlabel" attribute - skipping...'
-                        )
-                    else:
-                        self.xaxis.setLabel(text=xlabel)
-                    # set ylabel
-                    try:
-                        ylabel = self.sink.ylabel
-                    except AttributeError:
-                        logger.info(
-                            f'Data source [{data_source_name}] has no "ylabel" attribute - skipping...'
-                        )
-                    else:
-                        self.yaxis.setLabel(text=ylabel)
-                    try:
-                        dsets = self.sink.datasets
-                    except AttributeError as err:
+                # connect to the new data source
+                self.plot_settings.sink = DataSink(data_set_name)
+                self.plot_settings.sink.start()
+
+                # try to get the plot title and x/y labels
+                self.plot_settings.sink.pop(timeout=self.timeout)
+
+                # set title
+                try:
+                    title = self.plot_settings.sink.title
+                except AttributeError:
+                    _logger.info(
+                        f'Data source [{data_set_name}] has no "title" attribute - '
+                        'skipping...'
+                    )
+                else:
+                    title = None
+
+                # set xlabel
+                try:
+                    xlabel = self.plot_settings.sink.xlabel
+                except AttributeError:
+                    _logger.info(
+                        f'Data source [{data_set_name}] has no "xlabel" attribute - '
+                        'skipping...'
+                    )
+                else:
+                    xlabel = None
+
+                # set ylabel
+                try:
+                    ylabel = self.plot_settings.sink.ylabel
+                except AttributeError:
+                    _logger.info(
+                        f'Data source [{data_set_name}] has no "ylabel" attribute - '
+                        'skipping...'
+                    )
+                else:
+                    ylabel = None
+
+                # try to access datasets
+                try:
+                    dsets = self.plot_settings.sink.datasets
+                except AttributeError as err:
+                    raise RuntimeError(
+                        f'Data source [{data_set_name}] has no "datasets" attribute - '
+                        'exiting...'
+                    ) from err
+                else:
+                    if not isinstance(dsets, dict):
                         raise RuntimeError(
-                            f'Data source [{data_source_name}] has no "datasets" attribute - exiting...'
-                        ) from err
-                    else:
-                        if not isinstance(dsets, dict):
-                            logger.error(
-                                f'Data source [{data_source_name}] "datasets" attribute is not a dictionary - exiting...'
-                            )
-                            raise RuntimeError
-                    # add the existing plots
-                    for plot_name in self.plot_settings:
+                            f'Data source [{data_set_name}] "datasets" attribute is '
+                            'not a dictionary - exiting...'
+                        )
+
+                # set the new title/labels in the main thread
+                self.plot_settings.run_main(
+                    self._new_source_callback, title, xlabel, ylabel, blocking=True
+                )
+
+                # add the existing plots
+                with QtCore.QMutexLocker(self.plot_settings.mutex):
+                    for plot_name in self.plot_settings.series_settings:
                         self.add_plot(plot_name)
-                        if self.plot_settings[plot_name]['hidden']:
-                            self.hide(plot_name)
-                    # flag indicating that this is the first pop from the sink
-                    self.first = True
-                else:
-                    # some other pop error occured
-                    raise RuntimeError
+                        if self.plot_settings.series_settings[plot_name].hidden:
+                            self.hide_plot(plot_name)
+
+                # force plot the data since we used the first pop() to extract the
+                # plot info
+                self.plot_settings.force_update = True
             except (TimeoutError, RuntimeError) as err:
                 self.teardown()
                 raise RuntimeError(
-                    f'Could not connect to new data source [{data_source_name}]'
+                    f'Could not connect to new data source [{data_set_name}]'
                 ) from err
 
+    def _new_source_callback(self, title, xlabel, ylabel):
+        """Callback for when a new data source connects."""
+        if title is not None:
+            self.set_title(title)
+        if xlabel is not None:
+            self.xaxis.setLabel(text=xlabel)
+        if ylabel is not None:
+            self.yaxis.setLabel(text=ylabel)
+
     def teardown(self):
-        if self.sink is not None:
-            self.sink.__exit__(None, None, None)
-            self.sink = None
+        """Clean up."""
+        # run on the plot_settings thread since we'll need to acquire mutexes
+        self.plot_settings.run_safe(self._close_source)
+
+    def _close_source(self):
+        """Disconnect from the data source."""
+        with QtCore.QMutexLocker(self.plot_settings.sink_mutex):
+            if self.plot_settings.sink is not None:
+                self.plot_settings.sink.stop()
+                self.plot_settings.sink = None
 
     def update(self):
-        # update the plot data
-        # plot immediately if this is the first time, otherwise wait for new
-        # data to be available from the sink with pop()
-        if self.sink is not None and (self.first or self.sink.pop()):
-            with self.mutex:
-                # check again to be sure
-                if self.sink is not None:
-                    for plot_name in self.plot_settings:
-                        series = self.plot_settings[plot_name]['series']
-                        scan_i = self.plot_settings[plot_name]['scan_i']
-                        scan_j = self.plot_settings[plot_name]['scan_j']
-                        processing = self.plot_settings[plot_name]['processing']
+        """Update the plot if there is new data available."""
+        with QtCore.QMutexLocker(self.plot_settings.sink_mutex):
+            if self.plot_settings.sink is None:
+                # rate limit how often update() runs if there is no sink connected
+                time.sleep(0.1)
+                return
+
+            if self.plot_settings.force_update:
+                self.plot_settings.force_update = False
+            else:
+                try:
+                    # wait for new data to be available from the sink
+                    self.plot_settings.sink.pop(timeout=self.timeout)
+                except TimeoutError:
+                    return
+
+            if self.data_processing_func is not None:
+                self.data_processing_func(self.plot_settings.sink)
+
+            with QtCore.QMutexLocker(self.plot_settings.mutex):
+                for plot_name in self.plot_settings.series_settings:
+                    settings = self.plot_settings.series_settings[plot_name]
+                    series = settings.series
+                    scan_i = settings.scan_i
+                    scan_j = settings.scan_j
+                    processing = settings.processing
+
+                    # pick out the particular data series
+                    try:
+                        data = self.plot_settings.sink.datasets[series]
+                    except KeyError:
+                        _logger.error(f'Data series [{series}] does not exist.')
+                        continue
+
+                    if not isinstance(data, list):
+                        raise ValueError(
+                            f'Data series [{series}] must be a list of numpy arrays, '
+                            f'but has type [{type(data)}].'
+                        )
+
+                    if len(data) == 0:
+                        continue
+                    else:
+                        # check for numpy array
+                        if not isinstance(data[0], np.ndarray):
+                            raise ValueError(
+                                f'Data series [{series}] must be a list of numpy '
+                                'arrays, but the first list element has type '
+                                f'[{type(data[0])}].'
+                            )
+                        # check numpy array shape
+                        if data[0].shape[0] != 2 or len(data[0].shape) != 2:
+                            raise ValueError(
+                                f'Data series [{series}] first list element has '
+                                f'shape {data.shape}, but should be (2, n).'
+                            )
 
-                        # pick out the particulary data series
                         try:
-                            data = self.sink.datasets[series]
-                        except KeyError:
-                            logger.error(
-                                f'Data series [{series}] does not exist in data set [{self.data_source_name}]'
+                            if scan_i == '' and scan_j == '':
+                                data_subset = data[:]
+                            elif scan_j == '':
+                                data_subset = data[int(scan_i) :]
+                            elif scan_i == '':
+                                data_subset = data[: int(scan_j)]
+                            else:
+                                data_subset = data[int(scan_i) : int(scan_j)]
+                        except IndexError:
+                            _logger.warning(
+                                f'Data series [{series}] invalid scan indices '
+                                f'[{scan_i}, {scan_j}].'
                             )
                             continue
 
-                        if isinstance(data, list):
-                            if len(data) == 0:
-                                continue
-                            else:
-                                # check for numpy array
-                                if not isinstance(data[0], np.ndarray):
-                                    raise ValueError(
-                                        f'Data series [{series}] must be a list of numpy arrays, but the first list element has type [{type(data[0])}].'
-                                    )
-                                # check numpy array shape
-                                if data[0].shape[0] != 2 or len(data[0].shape) != 2:
-                                    raise ValueError(
-                                        f'Data series [{series}] first list element has shape {data.shape}, but should be (2, n).'
-                                    )
-
-                                try:
-                                    if scan_i == '' and scan_j == '':
-                                        data_subset = data[:]
-                                    elif scan_j == '':
-                                        data_subset = data[int(scan_i) :]
-                                    elif scan_i == '':
-                                        data_subset = data[: int(scan_j)]
-                                    else:
-                                        data_subset = data[int(scan_i) : int(scan_j)]
-                                except IndexError:
-                                    logger.warning(
-                                        f'Data series [{series}] invalid scan indices [{scan_i}, {scan_j}]'
-                                    )
-                                    continue
-
-                                if processing == 'Append':
-                                    # concatenate the numpy arrays
-                                    processed_data = np.concatenate(data_subset, axis=1)
-                                elif processing == 'Average':
-                                    # average the numpy arrays
-                                    processed_data = np.average(
-                                        np.stack(data_subset), axis=0
-                                    )
-                                else:
-                                    raise ValueError(
-                                        f'processing has unsupported value [{processing}].'
-                                    )
+                        if processing == 'Append':
+                            # concatenate the numpy arrays
+                            processed_data = np.concatenate(data_subset, axis=1)
+                        elif processing == 'Average':
+                            # create a single numpy array
+                            stacked_data = np.stack(data_subset)
+                            # mask the NaN entries
+                            masked_data = np.ma.array(
+                                stacked_data, mask=np.isnan(stacked_data)
+                            )
+                            # average the numpy arrays
+                            processed_data = np.ma.average(masked_data, axis=0)
                         else:
                             raise ValueError(
-                                f'Data series [{series}] must be a list of numpy arrays, but has type [{type(data)}].'
+                                f'Processing has unsupported value [{processing}].'
                             )
 
-                        # update the plot
-                        self.set_data(plot_name, processed_data[0], processed_data[1])
-            self.first = False
-        else:
-            time.sleep(0.1)
+                    # update the plot
+                    self.set_data(plot_name, processed_data[0], processed_data[1])
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/widgets/main_widget.py` & `nspyre-0.6.0/src/nspyre/gui/widgets/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """
-This widget creates an interface that allows the user to easily launch Qt widgets. The widgets are placed in a pyqtgraph dock area.
+Creates an interface that allows the user to easily launch Qt widgets. The
+widgets are placed in a pyqtgraph :code:`DockArea`.
 """
 from importlib import reload
 from types import ModuleType
+from typing import Dict
+from typing import Optional
 
 from pyqtgraph.dockarea import Dock
 from pyqtgraph.dockarea import DockArea
 from pyqtgraph.Qt import QtCore
 from pyqtgraph.Qt import QtGui
 from pyqtgraph.Qt import QtWidgets
 
-from .snake_widget import sssss
+from .snake import sssss
 
 
 class MainWidgetItem:
-    """Represents a QWidget which can be loaded from the MainWidget."""
+    """Represents an arbitrary QWidget that can be loaded from the MainWidget."""
 
     def __init__(
         self,
         module: ModuleType,
         cls: str,
-        args: list = None,
-        kwargs: dict = None,
-        stretch: tuple = None,
+        args: Optional[list] = None,
+        kwargs: Optional[dict] = None,
+        stretch: Optional[tuple] = None,
     ):
         """
         Args:
-            name: display name for the widget
-            module: python module that contains cls
-            cls: python class name as a string (that descends from QWidget).
+            name: Display name for the widget.
+            module: Python module that contains cls.
+            cls: Python class name as a string (that descends from QWidget).
                 An instance of this class will be created when the user tries
-                to load the widget and it will be added to the DockArea.
-            args: list of arguments to pass to the __init__ function of cls
-            kwargs: dictionary of keyword arguments to pass to the __init__
-                function of cls
-            stretch: the dock stretch factor as a tuple (stretch_x, stretch_y) (see https://pyqtgraph.readthedocs.io/en/latest/api_reference/dockarea.html)
+                to load the widget and it will be added to the :code:`DockArea`.
+            args: Arguments to pass to the __init__ function of cls.
+            kwargs: Keyword arguments to pass to the __init__ function of cls.
+            stretch: The dock stretch factor as a tuple (stretch_x, stretch_y) \
+                (see `DockArea docs <https://pyqtgraph.readthedocs.io/en/latest/\
+                api_reference/dockarea.html>`__)
         """
         super().__init__()
         self.module = module
         self.cls = cls
         self.stretch = stretch
         if args is None:
             self.args = []
@@ -74,15 +78,18 @@
         super().__init__()
         self.name = name
         self.setEditable(False)
         self.setText(name)
 
 
 class MainWidget(QtWidgets.QWidget):
-    """Qt widget that contains a list of widgets to run, and a pyqtgraph DockArea where they are displayed.
+    """Qt widget for loading other QWidgets.
+    It displays a hierarchy of widgets for the user to select and launch, and a
+    pyqtgraph :code:`DockArea` where they are displayed. The widgets dictionary
+    passed to __init__ can contain sub-dictionaries in order to group widgets together.
 
     Typical usage example:
 
     .. code-block:: python
 
         import my_module
         import nspyre
@@ -90,27 +97,34 @@
         from nspyre import MainWidget
 
         # Create Qt application and apply nspyre visual settings.
         app = nspyreApp()
 
         # Create the GUI.
         main_widget = MainWidget({
-            'Save_File': MainWidgetItem(nspyre, 'SaveWidget'),
-            'ODMR': MainWidgetItem(my_module, 'ODMRWidget'),
+            'Experiments': {
+                'ODMR': MainWidgetItem(my_module, 'ODMRWidget'),
+            },
+            'Plot': MainWidgetItem(nspyre.gui.widgets.flex_line_plot, \
+'FlexLinePlotWidget'),
+            'Data': {
+                'Save': MainWidgetItem(nspyre.gui.widgets.save_widget, 'SaveWidget'),
+                'Load': MainWidgetItem(nspyre.gui.widgets.load_widget, 'LoadWidget'),
+            }
         })
         main_widget.show()
         # Run the GUI event loop.
         app.exec()
 
     """
 
-    def __init__(self, widgets, font_size='18px'):
+    def __init__(self, widgets: Dict, font_size: str = '18px'):
         """
         Args:
-            widgets: Dictionary - see example usage for the required form.
+            widgets: See example usage for the required form.
             font_size: Dock label font size as a string (e.g. '14px').
         """
         super().__init__()
 
         # delete any children Qt widgets when this widget is closed
         self.setAttribute(QtCore.Qt.WidgetAttribute.WA_DeleteOnClose, True)
 
@@ -141,64 +155,65 @@
                 elif isinstance(value, dict):
                     # non-leaf node
                     node = _MainWidgetItemContainer(name)
                     parent.appendRow(node)
                     parse_widgets(value, node)
                 else:
                     raise ValueError(
-                        'Value in widgets dictionary must be a MainWidgetItem or another dictionary containing MainWidgetItem.'
+                        'Value in widgets dictionary must be a MainWidgetItem or '
+                        'another dictionary containing MainWidgetItem.'
                     )
 
-        parse_widgets(widgets, tree_root_node)
+        parse_widgets(self.widgets, tree_root_node)
         self.tree_widget.setModel(tree_model)
         self.tree_widget.collapseAll()
-        self.tree_widget.doubleClicked.connect(self.tree_item_double_click)
+        self.tree_widget.doubleClicked.connect(self._tree_item_double_click)
 
         # Qt button that loads a widget from the widget list when clicked
         load_button = QtWidgets.QPushButton('Load')
         # run the load widget method on button press
-        load_button.clicked.connect(self.load_widget_clicked)
+        load_button.clicked.connect(self._load_widget_clicked)
 
         # Qt layout that arranges the widget list and load button vertically
         main_layout = QtWidgets.QVBoxLayout()
         main_layout.addWidget(self.tree_widget)
         main_layout.addWidget(load_button)
         # Dummy widget containing the layout
         widget_tree_container = QtWidgets.QWidget()
         widget_tree_container.setLayout(main_layout)
 
         # add the widget list to the dock area
-        widget_list_dock = self.dock_widget(widget_tree_container, name='Widgets')
+        widget_list_dock = self._dock_widget(widget_tree_container, name='Widgets')
         # set size relative to other docks
         widget_list_dock.setStretch(20, 1)
 
         # add the snake logo to the dock area
         logo_widget = sssss()
-        self.logo_dock = self.dock_widget(logo_widget, name='snake')
+        self.logo_dock = self._dock_widget(logo_widget, name='snake')
         self.logo_dock.hideTitleBar()
         self.logo_dock.setStretch(80, 1)
 
         layout = QtWidgets.QVBoxLayout()
         layout.addWidget(self.dock_area)
         self.setLayout(layout)
 
-    def tree_item_double_click(self, model_index):
+    def _tree_item_double_click(self, model_index):
         tree_widget_item = self.tree_widget.model().itemFromIndex(model_index)
-        self.load_widget(tree_widget_item)
+        self._load_widget(tree_widget_item)
 
-    def load_widget_clicked(self):
+    def _load_widget_clicked(self):
         # get the currently selected tree index
         selected_tree_index = self.tree_widget.selectedIndexes()[0]
         # retrieve the item
         tree_widget_item = self.tree_widget.model().itemFromIndex(selected_tree_index)
-        self.load_widget(tree_widget_item)
+        self._load_widget(tree_widget_item)
 
-    def load_widget(self, tree_widget_item):
+    def _load_widget(self, tree_widget_item):
         """Loads the QWidget corresponding to the given tree item and add it to
-        the dock area."""
+        the :code:`DockArea`."""
         if isinstance(tree_widget_item, _MainWidgetItemContainer):
             # do nothing if the user tried to load a container class item
             return
 
         widget_name = tree_widget_item.name
         widget_module = tree_widget_item.main_widget_item.module
         widget_class_name = tree_widget_item.main_widget_item.cls
@@ -207,23 +222,23 @@
 
         # reload the module at runtime in case any changes were made to the code
         widget_module = reload(widget_module)
         widget_class = getattr(widget_module, widget_class_name)
         # create an instance of the widget class
         widget = widget_class(*widget_args, **widget_kwargs)
         # add the widget to the GUI
-        dock = self.dock_widget(widget, name=widget_name, closable=True)
+        dock = self._dock_widget(widget, name=widget_name, closable=True)
         # set the dock stretch factor
         # see https://pyqtgraph.readthedocs.io/en/latest/api_reference/dockarea.html
         stretch = tree_widget_item.main_widget_item.stretch
         if stretch is not None:
             dock.setStretch(*stretch)
 
-    def dock_widget(self, widget, *args, **kwargs):
-        """Create a new dock for the given widget and add it to the dock area."""
+    def _dock_widget(self, widget, *args, **kwargs):
+        """Create a new dock for the given widget and add it to the :code:`DockArea`."""
         # if the logo dock is there, remove it
         try:
             if self.logo_dock is not None:
                 self.logo_dock.close()
                 self.logo_dock = None
         except AttributeError:
             # if logo_dock hasn't been defined yet
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/widgets/params_widget.py` & `nspyre-0.6.0/src/nspyre/gui/widgets/params.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,108 @@
-"""Widget that generates a simple GUI that allows the user to enter a set of parameters.
+"""Widget that generates a simple GUI that allows the user to enter a set of
+parameters.
 """
+from typing import Dict
+from typing import Optional
+
 from pyqtgraph import SpinBox
 from pyqtgraph.Qt import QtWidgets
 
 
 class ParamsWidget(QtWidgets.QWidget):
-    """Create a simple GUI widget containing a list of parameters.
+    """Qt widget containing a set of line edit boxes for the user to enter \
+    parameters into.
 
     Typical usage example:
 
     .. code-block:: python
 
-        self.params_widget = ParamsWidget({
-                            'pulse_power': {'suffix': 'V', 'siPrefix': True},
-                            'pulse_length': {'suffix': 's', 'siPrefix': True},
-                            })
+        from pyqtgraph import SpinBox
+        from pyqtgraph.Qt import QtWidgets
 
-        def doSomething(self):
-            print(f'Making a pulse with power = {self.params_widget.pulse_power} V, length = {self.params_widget.pulse_length} V'
+        class MyWidget(QtWidgets.QWidget)
+            def __init__(self):
+                super().__init__()
+                self.params_widget = ParamsWidget({
+                    'start_freq': {
+                        'display_text': 'Start Frequency',
+                        'widget': SpinBox(
+                            value=3e9,
+                            suffix='Hz',
+                            siPrefix=True,
+                            bounds=(100e3, 10e9),
+                            dec=True,
+                        ),
+                    },
+                    'stop_freq': {
+                        'display_text': 'Stop Frequency',
+                        'widget': SpinBox(
+                            value=4e9,
+                            suffix='Hz',
+                            siPrefix=True,
+                            bounds=(100e3, 10e9),
+                            dec=True,
+                        ),
+                    },
+                    'num_points': {
+                        'display_text': 'Number of Scan Points',
+                        'widget': \
+SpinBox(value=100, int=True, bounds=(1, None), dec=True),
+                    },
+                    'iterations': {
+                        'display_text': 'Number of Experiment Repeats',
+                        'widget': \
+SpinBox(value=20, int=True, bounds=(1, None), dec=True),
+                    },
+                    'dataset': {
+                        'display_text': 'Data Set',
+                        'widget': QtWidgets.QLineEdit('odmr'),
+                    },
+                })
+
+            ...
+
+            def doSomething(self):
+                print(f'Scanning from = {self.params_widget.start_freq} Hz to = \
+{self.params_widget.stop_freq} Hz.'
 
     """
 
-    def __init__(self, params_config: dict, get_param_value_funs: dict = None):
+    def __init__(
+        self, params_config: Dict, get_param_value_funs: Optional[Dict] = None
+    ):
         """
         Args:
             params_config: Dictionary mapping parameter names to a parameter
                 configuration dictionary, which should contain:
-                - widget: QWidget instance that represents the parameter
-                - display_text[optional]: parameter text label
-            get_param_value_funs: Dictionary mapping python classes to a
+
+                - :code:`widget`: QWidget instance that represents the parameter
+                - :code:`display_text` [optional]: parameter text label
+
+            get_param_value_funs: Dictionary mapping Python classes to a
                 function that takes an instance of that class and returns its
                 value. This can be used to show ParamsWidget how to handle new
                 QWidgets. There is built-in support for pyqtgraph SpinBox,
-                QLineEdit, QComboBox, QCheckBox.
+                QLineEdit, QComboBox, QCheckBox. E.g.:
+
+                .. code-block:: python
+
+                    def get_lineedit_val(lineedit):
+                        return lineedit.text()
+
+                    pw = ParamsWidget({
+                                'dataset': {
+                                    'display_text': 'Data Set',
+                                    'widget': QtWidgets.QLineEdit('odmr'),
+                                },
+                                ...
+                            },
+                            get_param_value_funs={QLineEdit: get_lineedit_val}
+                        )
+
         """
         super().__init__()
         self.params_config = params_config
         self.widgets = {}
 
         # getter functions of GUI parameter widgets
         if get_param_value_funs is None:
@@ -126,14 +192,16 @@
         """Allow easy access to the parameter values."""
         if attr in self.params_config:
             widget = self.params_config[attr]['widget']
             try:
                 fun = self.get_param_value_funs[type(widget)]
             except KeyError as err:
                 raise ValueError(
-                    f'Parameter [{attr}] has no function for retrieving its value from the GUI. This should be set using the "get_param_value_funs" in the ParamsWidget constructor.'
+                    f'Parameter [{attr}] has no function for retrieving its value '
+                    'from the GUI. This should be set using the "get_param_value_funs" '
+                    'in the ParamsWidget constructor.'
                 ) from err
             else:
                 return fun(widget)
         else:
             # raise the default python error when an attribute isn't found
             return self.__getattribute__(attr)
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/widgets/separator_widget.py` & `nspyre-0.6.0/src/nspyre/gui/widgets/separator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """
-Lines to separate GUI elements. From https://stackoverflow.com/questions/5671354/how-to-programmatically-make-a-horizontal-line-in-qt.
+Lines to separate GUI elements. From
+https://stackoverflow.com/questions/5671354/how-to-programmatically-make-a-horizontal\
+-line-in-qt.
 """
 from pyqtgraph.Qt import QtWidgets
 
 
 class QHLine(QtWidgets.QFrame):
+    """Qt widget that displays a horizontal line."""
+
     def __init__(self):
         super(QHLine, self).__init__()
         self.setFrameShape(QtWidgets.QFrame.Shape.HLine)
         self.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
 
 
 class QVLine(QtWidgets.QFrame):
+    """Qt widget that displays a vertical line."""
+
     def __init__(self):
         super(QVLine, self).__init__()
         self.setFrameShape(QtWidgets.QFrame.Shape.VLine)
         self.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/widgets/snake_widget.py` & `nspyre-0.6.0/src/nspyre/gui/widgets/snake.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-"""
-Ssssspin snake logo.
-"""
 from pathlib import Path
 
 from pyqtgraph.Qt import QtCore
 from pyqtgraph.Qt import QtGui
 from pyqtgraph.Qt import QtWidgets
 
-HERE = Path(__file__).parent
+_HERE = Path(__file__).parent
 
 
 class sssss(QtWidgets.QWidget):
-    """Image widget showing the nspyre logo."""
+    """Qt widget that displays the nspyre logo."""
 
     def __init__(self, size=300):
         """
         Args:
-            size: size of the logo in pixels.
+            size: Size of the logo in pixels.
         """
         super().__init__()
 
         # label to display the image
         spin_snake_img_widget = QtWidgets.QLabel(self)
         # logo image
-        pixmap = QtGui.QPixmap(str(HERE / '../images/ssssspin.png'))
+        pixmap = QtGui.QPixmap(str(_HERE / '../images/ssssspin.png'))
         # rescale the image
         scaled_pixmap = pixmap.scaledToHeight(
             size, QtCore.Qt.TransformationMode.SmoothTransformation
         )
         spin_snake_img_widget.setPixmap(scaled_pixmap)
 
         # put the widget centered in a vertical layout
```

### Comparing `nspyre-0.5.0/src/nspyre/gui/widgets/splitter_widget.py` & `nspyre-0.6.0/src/nspyre/gui/widgets/_splitter.py`

 * *Files identical despite different names*

### Comparing `nspyre-0.5.0/src/nspyre/inserv/inserv.py` & `nspyre-0.6.0/src/nspyre/instrument/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
-This module starts a process running an RPyC server. Clients may connect and access devices, or command the server to add, remove, or restart devices.
+This module provides a wrapper around an
+`RPyC <https://rpyc.readthedocs.io/en/latest/>`__ server. Clients may connect and
+access devices, or command the server to add, remove, or restart devices.
 """
 import logging
 import threading
 import time
 from pathlib import Path
 from typing import Any
 from typing import Dict
+from typing import Optional
 
 from rpyc import ClassicService
 from rpyc.core.protocol import Connection
 from rpyc.utils.classic import obtain
 from rpyc.utils.server import ThreadedServer
 
 from ..misc.misc import _load_class_from_file
@@ -21,88 +24,73 @@
     from ..misc.pint import register_quantity_brining
 except ImportError:
     pass
 else:
     # monkey-patch fix for pint module
     register_quantity_brining(Q_)
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
-# default instrument server port
-INSERV_DEFAULT_PORT = 42068
+INSTRUMENT_SERVER_DEFAULT_PORT = 42068
+"""Default instrument server port."""
 
-# rpyc send/receive timeout in s (don't set to None)
 RPYC_SYNC_TIMEOUT = 30
+"""RPyC send/receive timeout in seconds (don't set to None)."""
 
 # event used for waiting until the rpyc server thread has finished
-RPYC_SERVER_STOP_EVENT = threading.Event()
+_RPYC_SERVER_STOP_EVENT = threading.Event()
 
 
 class InstrumentServerError(Exception):
-    """Raised for failures related to the InstrumentServer."""
+    """Raised for failures related to the
+    :py:class:`~nspyre.instrument.server.InstrumentServer`."""
+
+    def __init__(self, *args, **kwargs):
+        """
+        Args:
+            args: Arguments to pass to super class Exception().
+            kwargs: Keyword arguments to pass to super class Exception().
+        """
+        # override this so that the docs don't the print superclass docstring
+        super().__init__(*args, **kwargs)
 
 
 class InstrumentServerDeviceExistsError(InstrumentServerError):
-    """Raised if attempting to add a device that already exists to the InstrumentServer."""
+    """Raised if attempting to add a device that already exists to the
+    :py:class:`~nspyre.instrument.server.InstrumentServer`."""
+
+    def __init__(self, *args, **kwargs):
+        """
+        Args:
+            args: Arguments to pass to super class Exception().
+            kwargs: Keyword arguments to pass to super class Exception().
+        """
+        # override this so that the docs don't the print superclass docstring
+        super().__init__(*args, **kwargs)
 
 
 class InstrumentServer(ClassicService):
     """RPyC service that loads devices and exposes them to the client.
 
-    The RPyC service (https://rpyc.readthedocs.io/en/latest/) starts a new thread running an RPyC server. Clients may connect and access devices or command the server to add, remove, or restart devices (through the InstrumentGateway).
-
-    Typical usage example:
-
-    .. code-block:: python
-
-        from nspyre import InstrumentServer, InstrumentServerDeviceExistsError, InstrumentGateway, InstrumentGatewayError
-
-        port = 4000
-
-        # first try connecting to an existing instrument server, if one is already running
-        try:
-            inserv = InstrumentGateway(port=port)
-            inserv.connect()
-        except InstrumentGatewayError:
-            # if no server was running, start one
-            inserv = InstrumentServer(port=port)
-            inserv.start()
-
-        # add some devices to the server (if they aren't already added)
-
-        # sig gen
-        try:
-            inserv.add('sg', '~/my_project/drivers/siggen.py', 'SigGen')
-        except InstrumentServerDeviceExistsError:
-            pass
-
-        # NI DAQ
-        try:
-            inserv.add('daq', '~/my_project/drivers/daq.py', 'NIDAQ')
-        except InstrumentServerDeviceExistsError:
-            pass
-
-        # flip pellicle
-        try:
-            inserv.add('pel', '~/my_project/drivers/flip_pel.py', 'FlipPellicle')
-        except InstrumentServerDeviceExistsError:
-            pass
-
-        while True:
-            time.sleep(1)
+    The `RPyC <https://rpyc.readthedocs.io/en/latest/>`__ service starts a new
+    thread running an RPyC server. Clients may connect and access devices or
+    command the server to add, remove, or restart devices (through the
+    :py:class:`~nspyre.instrument.gateway.InstrumentGateway`).
 
     """
 
     def __init__(
-        self, port: int = INSERV_DEFAULT_PORT, sync_timeout: float = RPYC_SYNC_TIMEOUT
+        self,
+        port: int = INSTRUMENT_SERVER_DEFAULT_PORT,
+        sync_timeout: float = RPYC_SYNC_TIMEOUT,
     ):
         """
         Args:
-            port: port number to use for the RPyC server
-            sync_timeout: Time to wait for requests / function calls to finish
+            port: Port number to use for the RPyC server.
+            sync_timeout: Time to wait for requests / function calls to finish.
         """
 
         super().__init__()
         # dictionary where keys are the device names, values are tuples:
         # (device object, device configuration settings dictionary)
         self._devs: Dict[str, Any] = {}
         # rpyc server port
@@ -112,80 +100,103 @@
         self._rpyc_server = None
 
     def add(
         self,
         name: str,
         class_path: str,
         class_name: str,
-        *args,
+        args: Optional[list] = None,
+        kwargs: Optional[Dict] = None,
         import_or_file: str = 'file',
-        **kwargs,
+        local_args: bool = False,
     ):
-        r"""Create an instance of the specified class and add it to the instrument server.
+        """Create an instance of the specified class and add it to the instrument
+        server.
 
         Args:
             name: Alias for the device.
-            class_path: If import_or_file is 'file', path to the file containing the class, e.g. '~/drivers/oscilloscopes/rtb2004.py'. If import_or_file is 'import', python module containing the class, e.g. 'driver_module.oscilloscopes.rtb2004'
-            class_name: Name of the class to create an instance of, e.g. 'RTB2004'.
-            import_or_file: 'file' for creating the device object from a file on disk, 'import' for creating the device object from a python module.
-            args: arguments to pass to the class during initialization, as in RTB2004(\*args, \*\*kwargs).
-            kwargs: keyword args to pass to the class during initialization, as in RTB2004(\*args, \*\*kwargs).
+            class_path: If import_or_file is :code:`'file'`, path to the file on
+                the filesystem containing the class, e.g.
+                :code:`'~/drivers/rohde_schwarz/hmp4040.py'`. If import_or_file
+                is :code:`'import'`, python module containing the class, e.g.
+                :code:`'nspyre_drivers.rohde_schwarz.hmp4040.hmp4040'`.
+            class_name: Name of the class to create an instance of, e.g.
+                :code:`'HMP4040'`.
+            args: Arguments to pass to the class during initialization, as in
+                :code:`HMP4040(*args, **kwargs)`.
+            kwargs: Keyword args to pass to the class during initialization,
+                as in :code:`HMP4040(*args, **kwargs)`.
+            import_or_file: :code:`'file'` for creating the device object from
+                a file on the filesystem, :code:`'import'` for creating the
+                device object from a python module.
+            local_args: If True, all arguments to this method are assumed to be
+                local variables not passed through an
+                :py:class:`~nspyre.instrument.gateway.InstrumentGateway`. In
+                this case, the arguments will be taken as-is. If False, all
+                arguments will be retrieved using rpyc.utils.classic.obtain
+                in order to ensure they are not netrefs.
 
         Raises:
             ValueError: An argument was invalid.
-            InstrumentServerDeviceExistsError: Tried to add a device that already exists.
+            InstrumentServerDeviceExistsError: Tried to add a device that already
+                exists.
             InstrumentServerError: Anything else.
         """
-
-        # make sure that the arguments actually exist on the local machine
-        # and are not netrefs - otherwise there could be dangling references left over
-        # in the self._devs dictionary after the client disconnects
-        name = obtain(name)
-        class_path = obtain(class_path)
-        class_name = obtain(class_name)
-        import_or_file = obtain(import_or_file)
-        args = obtain(args)
-        kwargs = obtain(kwargs)
+        if not local_args:
+            # make sure that the arguments actually exist on the local machine
+            # and are not netrefs - otherwise there could be dangling references
+            # left over in the self._devs dictionary after the client disconnects
+            name = obtain(name)
+            class_path = obtain(class_path)
+            class_name = obtain(class_name)
+            import_or_file = obtain(import_or_file)
+            args = obtain(args)
+            kwargs = obtain(kwargs)
+
+        if args is None:
+            args = []
+        if kwargs is None:
+            kwargs = {}
 
         if name in self._devs:
-            raise InstrumentServerDeviceExistsError(f'device "{name}" already exists')
+            raise ValueError(f'Device [{name}] already exists on the InstrumentServer.')
 
         if import_or_file == 'file':
             # load the class from a file on disk
             try:
                 dev_class_path = Path(class_path).resolve()
                 dev_class = _load_class_from_file(dev_class_path, class_name)
             except Exception as exc:
                 raise InstrumentServerError(
-                    f'The specified class "{class_name}" from file "{class_path}" for'
-                    f' device "{name}" couldn\'t be loaded'
+                    f'The specified class [{class_name}] from file [{class_path}] for'
+                    f' device [{name}] couldn\'t be loaded.'
                 ) from exc
         elif import_or_file == 'import':
             # load the class from a python module
             try:
                 dev_class_mod = f'{class_path}.{class_name}'
                 dev_class = _load_class_from_str(dev_class_mod)
             except Exception as exc:
                 raise InstrumentServerError(
-                    f'The specified class "{dev_class_mod}" for device "{name}"'
-                    ' couldn\'t be loaded',
+                    f'The specified class [{dev_class_mod}] for device [{name}]'
+                    ' couldn\'t be loaded.',
                 ) from exc
         else:
             raise ValueError(
-                'argument import_or_file must be "file" or "import"; got'
-                f' "{import_or_file}"'
+                'Argument import_or_file must be "file" or "import"; got'
+                f' [{import_or_file}].'
             )
 
         # create an instance of the device
         try:
             instance = dev_class(*args, **kwargs)
         except Exception as exc:
             raise InstrumentServerError(
-                f'Failed to create an instance of device "{name}" of class'
-                f' "{dev_class}"',
+                f'Failed to create an instance of device [{name}] of class'
+                f' [{dev_class}].',
             ) from exc
 
         # initialize the driver if it implements an __enter__ function
         try:
             instance.__enter__()
         except AttributeError:
             pass
@@ -196,37 +207,37 @@
             'class_name': class_name,
             'import_or_file': import_or_file,
             'args': args,
             'kwargs': kwargs,
         }
         self._devs[name] = (instance, config)
 
-        logger.info(f'added device "{name}" with args: {args} kwargs: {kwargs}')
+        _logger.info(f'Added device [{name}] with args: {args} kwargs: {kwargs}.')
 
     def remove(self, name: str):
         """Remove a device from the instrument server.
 
         Args:
             name: Alias for the device.
 
         Raises:
             InstrumentServerError: Deleting the device failed.
         """
         try:
             dev, _ = self._devs.pop(name)
         except Exception as exc:
-            raise InstrumentServerError(f'Failed deleting device "{name}"') from exc
+            raise InstrumentServerError(f'Failed deleting device [{name}].') from exc
 
         # teardown the driver if it implements an __exit__ function
         try:
             dev.__exit__(None, None, None)
         except AttributeError:
             pass
 
-        logger.info(f'deleted device "{name}"')
+        _logger.info(f'Deleted device [{name}].')
 
     def restart(self, name: str):
         """Restart the specified device by deleting it and creating a new instance.
 
         Args:
             name: Alias for the device.
 
@@ -240,17 +251,17 @@
         import_or_file = config_dict['import_or_file']
         kwargs = config_dict['kwargs']
         self.remove(name)
         self.add(
             name,
             class_path,
             class_name,
-            *args,
+            args=args,
             import_or_file=import_or_file,
-            **kwargs,
+            kwargs=kwargs,
         )
 
     def restart_all(self):
         """Restart all devices on the server.
 
         Raises:
             InstrumentServerError: Deleting a device failed.
@@ -262,67 +273,67 @@
         """Start the RPyC server.
 
         Raises:
             InstrumentServerError: The server was already running.
         """
         if self._rpyc_server:
             raise InstrumentServerError(
-                'Can\'t start the rpyc server because one is already running.'
+                'Can\'t start the RPyC server because one is already running.'
             )
         thread = threading.Thread(target=self._rpyc_server_thread)
         thread.start()
         # wait for the server to start
         while not (self._rpyc_server and self._rpyc_server.active):
             time.sleep(0.1)
 
     def _rpyc_server_thread(self):
         """Thread for running the RPyC server asynchronously"""
-        logger.info('starting InstrumentServer RPyC server...')
+        _logger.info('Starting InstrumentServer RPyC server...')
         self._rpyc_server = ThreadedServer(
             self,
             hostname='127.0.0.1',
             port=self._port,
             protocol_config={
                 'allow_pickle': True,
                 'allow_all_attrs': True,
                 'allow_setattr': True,
                 'allow_delattr': True,
                 'sync_request_timeout': self._sync_timeout,
             },
         )
         self._rpyc_server.start()
-        logger.info('RPyC server stopped')
-        RPYC_SERVER_STOP_EVENT.set()
+        _logger.info('RPyC server stopped.')
+        _RPYC_SERVER_STOP_EVENT.set()
 
     def stop(self):
         """Stop the RPyC server.
 
         Raises:
             InstrumentServerError: The server wasn't running.
         """
         if not self._rpyc_server:
             raise InstrumentServerError(
-                'Can\'t stop the rpyc server because there isn\'t one running.'
+                'Can\'t stop the RPyC server because there isn\'t one running.'
             )
 
-        logger.info('removing devices...')
+        _logger.info('Removing devices...')
         for d in list(self._devs):
             self.remove(d)
 
-        logger.info('stopping RPyC server...')
+        _logger.info('Stopping RPyC server...')
         self._rpyc_server.close()
-        RPYC_SERVER_STOP_EVENT.wait()
-        RPYC_SERVER_STOP_EVENT.clear()
+        _RPYC_SERVER_STOP_EVENT.wait()
+        _RPYC_SERVER_STOP_EVENT.clear()
         self._rpyc_server = None
 
     def devs(self):
-        """Get all of the devices on the InstrumentSever.
+        """Return all of the devices on the InstrumentSever.
 
         Returns:
-            dict: the device name as keys and device object as values
+            dict: The device names as keys and device objects as values.
         """
         devs = {}
         for d in self._devs:
             devs[d] = getattr(self, d)
         return devs
 
     def __getattr__(self, attr: str):
@@ -335,20 +346,20 @@
         if attr in self._devs:
             return self._devs[attr][0]
         else:
             # raise the default python error when an attribute isn't found
             return self.__getattribute__(attr)
 
     def on_connect(self, conn: Connection):
-        """Called when a client connects to the RPyC server"""
-        logger.info(f'client {conn} connected')
+        """Called when a client connects to the RPyC server."""
+        _logger.info(f'Client {conn} connected.')
 
     def on_disconnect(self, conn: Connection):
-        """Called when a client disconnects from the RPyC server"""
-        logger.info(f'client {conn} disconnected')
+        """Called when a client disconnects from the RPyC server."""
+        _logger.info(f'Client {conn} disconnected.')
 
     def __enter__(self):
         """Python context manager setup"""
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `nspyre-0.5.0/src/nspyre/misc/logging.py` & `nspyre-0.6.0/src/nspyre/misc/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
 import logging
 import sys
 from io import TextIOBase
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from typing import Any
+from typing import Optional
 
-# max size of a log file (in bytes) before creating a new one
-LOG_FILE_MAX_SIZE = 100e6
+LOG_FILE_MAX_SIZE = 10e6
+"""Max size of a log file (in bytes) before creating a new one."""
 
 
 class _StreamToLog(TextIOBase):
     """Fake stream object that redirects writes to a logger"""
 
     def __init__(self, logger: logging.Logger, log_level: int, terminator: str):
         super().__init__()
@@ -41,30 +42,43 @@
         """Write out the contents of the current buffer"""
         if self.write_buffer:
             self.write(self.terminator)
 
 
 def nspyre_init_logger(
     log_level: int,
-    log_path: Path = None,
+    log_path: Optional[Path] = None,
     log_path_level: int = 0,
     prefix: str = '',
-    file_size: int = None,
+    file_size: Optional[int] = None,
+    remove_handlers: bool = True,
 ):
     """Initialize system-wide logging to stdout/err and, optionally, a file.
 
     Args:
-        log_level: Log messages of lower severity than this will not be sent to stdout/err (e.g. logging.INFO).
-        log_path: If a file, log to that file. If a directory, generate a log file name and create a new log file in that directory. If None, only log to stdout/err.
-        log_path_level: Logging level for the log file. Leave as None for same as log_level.
-        prefix: If a directory was specified for log_path, prepend this string to the log file name.
-        file_size: Maximum log file size (bytes). If this size is exceeded, the log file is rotated according to RotatingFileHandler (https://docs.python.org/3/library/logging.handlers.html).
+        log_level: Log messages of lower severity than this will not be sent
+            to stdout/err (e.g. :code:`logging.INFO`).
+        log_path: If a file, log to that file. If a directory, generate a log
+            file name containing the prefix and date/time, and create a new
+            log file in that directory. If :code:`None`, only log to stdout/err.
+        log_path_level: Logging level for the log file. Leave as :code:`None`
+            for same as log_level.
+        prefix: If a directory was specified for log_path, prepend this string
+            to the log file name.
+        file_size: Maximum log file size (bytes). If this size is exceeded,
+            the log file is rotated according to :code:`RotatingFileHandler`
+            (https://docs.python.org/3/library/logging.handlers.html).
+        remove_handlers: If true, remove any existing log handlers.
     """
-
     root_logger = logging.getLogger()
+
+    if remove_handlers:
+        # remove any previous root_logger handlers
+        root_logger.handlers.clear()
+
     # the root logger will accept all messages
     root_logger.setLevel(logging.DEBUG)
 
     # log format for stdout messages
     stdout_formatter = logging.Formatter(
         '%(asctime)s.%(msecs)03d [%(levelname)s] (%(filename)s:%(lineno)s) %(message)s',
         '%Y-%m-%d %H:%M:%S',
@@ -73,14 +87,19 @@
     stdout_handler = logging.StreamHandler(stream=sys.stdout)
     stdout_handler.setLevel(log_level)
     stdout_handler.setFormatter(stdout_formatter)
     root_logger.addHandler(stdout_handler)
 
     # all stderr messages will now be redirected to a special logger
     stderr_logger = logging.getLogger('stderr')
+
+    if remove_handlers:
+        # remove any previous stderr_logger handlers
+        stderr_logger.handlers.clear()
+
     stderr_logger.propagate = False
     sys.stderr = _StreamToLog(stderr_logger, logging.CRITICAL, '\n')  # type: ignore
 
     # log format for stderr messages
     stderr_formatter = logging.Formatter('[stderr] %(message)s')
     # create stderr log handler
     stderr_handler = logging.StreamHandler(stream=sys.stdout)
@@ -107,15 +126,16 @@
         if file_size:
             file_handler: Any = RotatingFileHandler(
                 log_path, maxBytes=file_size, backupCount=1000
             )
         else:
             file_handler = logging.FileHandler(log_path)
         file_formatter = logging.Formatter(
-            '%(asctime)s.%(msecs)03d [%(levelname)8s] (%(filename)20s:%(lineno)4s) %(message)s',
+            '%(asctime)s.%(msecs)03d [%(levelname)8s] (%(filename)20s:%(lineno)4s) '
+            '%(message)s',
             '%Y-%m-%d %H:%M:%S',
         )
         file_handler.setFormatter(file_formatter)
         if log_path_level:
             file_handler.setLevel(log_path_level)
         else:
             file_handler.setLevel(log_level)
```

### Comparing `nspyre-0.5.0/src/nspyre/misc/pint.py` & `nspyre-0.6.0/src/nspyre/misc/pint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
-Monkey patch to get pint to work with rpyc.
+Monkey patch to get `Pint <https://pint.readthedocs.io/en/stable/>`__ to work
+with `RPyC <https://rpyc.readthedocs.io/en/latest/>`__.
 """
 
 try:
     from pint import get_application_registry
 except ImportError:
     Q_ = None
+    """Pint Quantity class. This is provided for backwards compatibility but is not \
+    recommended for future use."""
 else:
     import rpyc
 
     # create a pint registry universal to nspyre
     ureg = get_application_registry()
     Q_ = ureg.Quantity
```

