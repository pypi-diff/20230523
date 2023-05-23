# Comparing `tmp/QPUIQ-0.2.0.tar.gz` & `tmp/QPUIQ-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.2.0.tar", last modified: Mon May 15 21:55:43 2023, max compression
+gzip compressed data, was "QPUIQ-0.2.1.tar", last modified: Tue May 23 17:06:28 2023, max compression
```

## Comparing `QPUIQ-0.2.0.tar` & `QPUIQ-0.2.1.tar`

### file list

```diff
@@ -1,72 +1,78 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.715850 QPUIQ-0.2.0/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.2.0/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     5972 2023-05-15 21:55:43.715700 QPUIQ-0.2.0/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.702451 QPUIQ-0.2.0/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.706205 QPUIQ-0.2.0/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)     1177 2023-05-15 20:37:16.000000 QPUIQ-0.2.0/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.2.0/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     3734 2023-05-15 20:35:11.000000 QPUIQ-0.2.0/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      575 2023-05-14 18:07:46.000000 QPUIQ-0.2.0/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2708 2023-05-12 01:01:59.000000 QPUIQ-0.2.0/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      764 2023-05-14 14:59:50.000000 QPUIQ-0.2.0/PUI/PySide6/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     2343 2023-05-14 16:38:10.000000 QPUIQ-0.2.0/PUI/PySide6/combobox.py
--rw-r--r--   0 Bug        (504) staff       (20)      722 2023-05-14 18:07:33.000000 QPUIQ-0.2.0/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      941 2023-05-10 09:26:37.000000 QPUIQ-0.2.0/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      493 2023-05-04 13:36:49.000000 QPUIQ-0.2.0/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      784 2023-05-14 14:54:11.000000 QPUIQ-0.2.0/PUI/PySide6/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     3895 2023-05-14 15:12:52.000000 QPUIQ-0.2.0/PUI/PySide6/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1544 2023-05-14 18:06:04.000000 QPUIQ-0.2.0/PUI/PySide6/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      820 2023-05-04 13:36:56.000000 QPUIQ-0.2.0/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1996 2023-05-12 05:40:38.000000 QPUIQ-0.2.0/PUI/PySide6/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      488 2023-05-15 21:54:54.000000 QPUIQ-0.2.0/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      432 2023-05-15 20:31:59.000000 QPUIQ-0.2.0/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     2790 2023-05-13 06:35:30.000000 QPUIQ-0.2.0/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.708682 QPUIQ-0.2.0/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      388 2023-05-12 01:01:47.000000 QPUIQ-0.2.0/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      516 2023-05-06 22:58:40.000000 QPUIQ-0.2.0/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.2.0/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      482 2023-05-14 18:08:03.000000 QPUIQ-0.2.0/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.2.0/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      955 2023-05-15 17:33:27.000000 QPUIQ-0.2.0/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.2.0/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.2.0/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      447 2023-05-06 22:58:40.000000 QPUIQ-0.2.0/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     4214 2023-05-15 21:05:53.000000 QPUIQ-0.2.0/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)    12370 2023-05-15 16:57:03.000000 QPUIQ-0.2.0/PUI/state.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.711782 QPUIQ-0.2.0/PUI/textual/
--rw-r--r--   0 Bug        (504) staff       (20)      942 2023-05-15 21:44:28.000000 QPUIQ-0.2.0/PUI/textual/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1776 2023-05-15 21:49:20.000000 QPUIQ-0.2.0/PUI/textual/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      223 2023-05-15 17:15:48.000000 QPUIQ-0.2.0/PUI/textual/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      421 2023-05-15 19:40:06.000000 QPUIQ-0.2.0/PUI/textual/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      531 2023-05-15 21:53:10.000000 QPUIQ-0.2.0/PUI/textual/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     1288 2023-05-15 21:02:44.000000 QPUIQ-0.2.0/PUI/textual/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1014 2023-05-15 19:41:34.000000 QPUIQ-0.2.0/PUI/textual/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      484 2023-05-15 19:42:35.000000 QPUIQ-0.2.0/PUI/textual/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      634 2023-05-15 21:50:12.000000 QPUIQ-0.2.0/PUI/textual/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)      367 2023-05-15 20:40:47.000000 QPUIQ-0.2.0/PUI/textual/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      371 2023-05-15 21:11:27.000000 QPUIQ-0.2.0/PUI/textual/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      700 2023-05-15 21:46:56.000000 QPUIQ-0.2.0/PUI/textual/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      591 2023-05-15 18:04:39.000000 QPUIQ-0.2.0/PUI/textual/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1253 2023-05-15 20:38:31.000000 QPUIQ-0.2.0/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.714820 QPUIQ-0.2.0/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      436 2023-05-12 08:12:36.000000 QPUIQ-0.2.0/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      554 2023-05-10 11:03:55.000000 QPUIQ-0.2.0/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      564 2023-05-10 11:04:22.000000 QPUIQ-0.2.0/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-05-14 18:07:17.000000 QPUIQ-0.2.0/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1283 2023-05-12 18:42:45.000000 QPUIQ-0.2.0/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      522 2023-05-14 18:06:49.000000 QPUIQ-0.2.0/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     2197 2023-05-12 09:01:37.000000 QPUIQ-0.2.0/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.2.0/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      565 2023-05-12 15:00:48.000000 QPUIQ-0.2.0/PUI/tkinter/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.2.0/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1524 2023-05-12 08:31:21.000000 QPUIQ-0.2.0/PUI/tkinter/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      505 2023-05-07 08:48:56.000000 QPUIQ-0.2.0/PUI/utils.py
--rw-r--r--   0 Bug        (504) staff       (20)     3082 2023-05-15 20:36:28.000000 QPUIQ-0.2.0/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-15 21:55:43.715502 QPUIQ-0.2.0/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     5972 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1345 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-05-15 21:55:43.000000 QPUIQ-0.2.0/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     5712 2023-05-15 21:26:34.000000 QPUIQ-0.2.0/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-05-15 21:55:43.715894 QPUIQ-0.2.0/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.2.0/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.244078 QPUIQ-0.2.1/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.2.1/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     6125 2023-05-23 17:06:28.243929 QPUIQ-0.2.1/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.227040 QPUIQ-0.2.1/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.232369 QPUIQ-0.2.1/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)     1245 2023-05-22 07:48:34.000000 QPUIQ-0.2.1/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.2.1/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5095 2023-05-21 20:51:56.000000 QPUIQ-0.2.1/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      575 2023-05-14 18:07:46.000000 QPUIQ-0.2.1/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2708 2023-05-12 01:01:59.000000 QPUIQ-0.2.1/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      764 2023-05-14 14:59:50.000000 QPUIQ-0.2.1/PUI/PySide6/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2343 2023-05-14 16:38:10.000000 QPUIQ-0.2.1/PUI/PySide6/combobox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      722 2023-05-14 18:07:33.000000 QPUIQ-0.2.1/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      941 2023-05-10 09:26:37.000000 QPUIQ-0.2.1/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      667 2023-05-20 18:18:18.000000 QPUIQ-0.2.1/PUI/PySide6/mdi.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2818 2023-05-22 05:29:49.000000 QPUIQ-0.2.1/PUI/PySide6/menu.py
+-rw-r--r--   0 Bug        (504) staff       (20)      493 2023-05-04 13:36:49.000000 QPUIQ-0.2.1/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      784 2023-05-14 14:54:11.000000 QPUIQ-0.2.1/PUI/PySide6/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3453 2023-05-22 11:07:05.000000 QPUIQ-0.2.1/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1363 2023-05-22 10:28:02.000000 QPUIQ-0.2.1/PUI/PySide6/splitter.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1544 2023-05-14 18:06:04.000000 QPUIQ-0.2.1/PUI/PySide6/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-05-20 03:18:54.000000 QPUIQ-0.2.1/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2251 2023-05-22 07:59:01.000000 QPUIQ-0.2.1/PUI/PySide6/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-05-23 17:05:44.000000 QPUIQ-0.2.1/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      432 2023-05-15 20:31:59.000000 QPUIQ-0.2.1/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3541 2023-05-23 12:21:44.000000 QPUIQ-0.2.1/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.235509 QPUIQ-0.2.1/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      658 2023-05-23 17:06:02.000000 QPUIQ-0.2.1/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      236 2023-05-22 11:27:04.000000 QPUIQ-0.2.1/PUI/flet/appbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      610 2023-05-20 06:55:30.000000 QPUIQ-0.2.1/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      612 2023-05-22 11:17:29.000000 QPUIQ-0.2.1/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      482 2023-05-14 18:08:03.000000 QPUIQ-0.2.1/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      645 2023-05-18 18:20:23.000000 QPUIQ-0.2.1/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1203 2023-05-23 15:24:05.000000 QPUIQ-0.2.1/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      499 2023-05-23 15:26:28.000000 QPUIQ-0.2.1/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1559 2023-05-23 15:23:00.000000 QPUIQ-0.2.1/PUI/flet/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      799 2023-05-18 17:43:47.000000 QPUIQ-0.2.1/PUI/flet/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.2.1/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      729 2023-05-23 15:25:40.000000 QPUIQ-0.2.1/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     4613 2023-05-20 17:17:52.000000 QPUIQ-0.2.1/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)    13532 2023-05-20 07:10:33.000000 QPUIQ-0.2.1/PUI/state.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.239605 QPUIQ-0.2.1/PUI/textual/
+-rw-r--r--   0 Bug        (504) staff       (20)      967 2023-05-20 08:22:45.000000 QPUIQ-0.2.1/PUI/textual/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1963 2023-05-20 06:54:39.000000 QPUIQ-0.2.1/PUI/textual/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1177 2023-05-17 14:39:47.000000 QPUIQ-0.2.1/PUI/textual/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      421 2023-05-15 19:40:06.000000 QPUIQ-0.2.1/PUI/textual/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      531 2023-05-15 21:53:10.000000 QPUIQ-0.2.1/PUI/textual/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1288 2023-05-16 07:25:36.000000 QPUIQ-0.2.1/PUI/textual/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2681 2023-05-23 07:47:17.000000 QPUIQ-0.2.1/PUI/textual/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      484 2023-05-15 19:42:35.000000 QPUIQ-0.2.1/PUI/textual/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      634 2023-05-15 21:50:12.000000 QPUIQ-0.2.1/PUI/textual/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1349 2023-05-23 07:46:17.000000 QPUIQ-0.2.1/PUI/textual/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      371 2023-05-16 08:39:00.000000 QPUIQ-0.2.1/PUI/textual/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      725 2023-05-17 14:33:03.000000 QPUIQ-0.2.1/PUI/textual/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      381 2023-05-20 17:16:55.000000 QPUIQ-0.2.1/PUI/textual/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-05-20 17:15:22.000000 QPUIQ-0.2.1/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.243078 QPUIQ-0.2.1/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      461 2023-05-20 08:22:54.000000 QPUIQ-0.2.1/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      614 2023-05-20 06:55:48.000000 QPUIQ-0.2.1/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      564 2023-05-10 11:04:22.000000 QPUIQ-0.2.1/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-05-14 18:07:17.000000 QPUIQ-0.2.1/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1283 2023-05-12 18:42:45.000000 QPUIQ-0.2.1/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      522 2023-05-14 18:06:49.000000 QPUIQ-0.2.1/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2197 2023-05-12 09:01:37.000000 QPUIQ-0.2.1/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.2.1/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      565 2023-05-12 15:00:48.000000 QPUIQ-0.2.1/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.2.1/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1524 2023-05-12 08:31:21.000000 QPUIQ-0.2.1/PUI/tkinter/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      505 2023-05-07 08:48:56.000000 QPUIQ-0.2.1/PUI/utils.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2860 2023-05-20 17:17:35.000000 QPUIQ-0.2.1/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-23 17:06:28.243728 QPUIQ-0.2.1/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     6125 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1463 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-05-23 17:06:28.000000 QPUIQ-0.2.1/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     5865 2023-05-18 06:35:30.000000 QPUIQ-0.2.1/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-05-23 17:06:28.244119 QPUIQ-0.2.1/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.2.1/setup.py
```

### Comparing `QPUIQ-0.2.0/LICENSE.txt` & `QPUIQ-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PKG-INFO` & `QPUIQ-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: QPUIQ
-Version: 0.2.0
-Summary: "PUI" Python Declarative UI Framework
-Home-page: https://github.com/buganini/PUI
-Author: Buganini Chiu
-Author-email: buganini@b612.tw
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # What is PUI
 PUI is a declarative UI framework with two-way data binding
 
 # Installation
 ```
 pip install QPUIQ
 ```
@@ -155,14 +145,18 @@
 
 ![Cookbook 1](https://github.com/buganini/PUI/raw/main/screenshots/cookbook1.png)
 ![Cookbook 2](https://github.com/buganini/PUI/raw/main/screenshots/cookbook2.png)
 
 `python -m cookbook textual`
 ![Cookbook textual](https://github.com/buganini/PUI/raw/main/screenshots/cookbook_textual.png)
 
+## Hot-Reload with Reloadium
+[![Hot-Reload with Reloadium](https://img.youtube.com/vi/X716rwchPBM/0.jpg)](https://www.youtube.com/watch?v=X716rwchPBM)
+
+
 # Backends
 ## Tier-1
 * PySide6
 ## Lower Priority
 * tkinter
     * or https://github.com/rdbende/Sun-Valley-ttk-theme
 * flet
@@ -236,8 +230,8 @@
         * ...
     * Table
     * Tree
     * ~~Scrollbar (or as a layout setting)~~
 * Better DOM syncer
     * Prevent unnecessary nested update
     * Trace Event Source (TextField) and prevent update it DOM Sync
-* Pydantic State
+* Pydantic State
```

### Comparing `QPUIQ-0.2.0/PUI/PySide6/__init__.py` & `QPUIQ-0.2.1/PUI/PySide6/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from .checkbox import *
 from .combobox import *
 from .label import *
 from .layout import *
 from .progressbar import *
 from .radiobutton import *
 from .scroll import *
+from .splitter import *
 from .text import *
 from .textfield import *
 from .window import *
+from .mdi import *
 
 Application = QtApplication
 Window = QtWindow
 HBox = QtHBox
 VBox = QtVBox
 Label = QtLabel
 Button = QtButton
@@ -49,7 +51,9 @@
 
         ret = PUIViewWrapper(func.__name__)
         return ret
 
     return func_wrapper
 
 PUI = QtPUI
+
+PUI_BACKEND = "PySide6"
```

### Comparing `QPUIQ-0.2.0/PUI/PySide6/base.py` & `QPUIQ-0.2.1/PUI/PySide6/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .. import *
 
-from PySide6 import QtCore, QtWidgets
+from PySide6 import QtCore, QtWidgets, QtGui
 
 class QtViewSignal(QtCore.QObject):
     redraw = QtCore.Signal()
 
 def _apply_params(ui, params):
     HorizontalPolicy = params.get("HorizontalPolicy")
     if not HorizontalPolicy is None:
@@ -122,8 +122,55 @@
             child.ui.setParent(None)
         elif child.children:
             self.removeChild(idx, child.children[0])
 
     def qt(self, **kwargs):
         for k,v in kwargs.items():
             self.qt_params[k] = v
-        return self
+        return self
+
+class QtBaseFrame(QtBaseWidget):
+    terminal = False
+
+    def __init__(self):
+        self.widget = None
+        super().__init__()
+
+    def destroy(self, direct):
+        if direct:
+            if self.ui:
+                self.ui.deleteLater()
+                self.ui = None
+            if self.widget:
+                self.widget.deleteLater()
+                self.widget = None
+
+    def addChild(self, idx, child):
+        if idx != 0:
+            return
+        if isinstance(child, QtBaseLayout):
+            self.widget = QtWidgets.QWidget()
+            self.ui.setWidget(self.widget)
+            self.widget.setLayout(child.outer)
+        elif isinstance(child, QtBaseWidget):
+            self.ui.setWidget(child.outer)
+        elif child.children:
+            self.addChild(idx, child.children[0])
+
+    def removeChild(self, idx, child):
+        if idx != 0:
+            return
+        if isinstance(child, QtBaseLayout):
+            child.outer.setParent(None)
+            self.widget.setParent(None)
+        elif isinstance(child, QtBaseWidget):
+            child.outer.setParent(None)
+        elif child.children:
+            self.removeChild(idx, child.children[0])
+
+class QtWrapper(QtBaseWidget):
+    def __init__(self, widget, *args):
+        super().__init__(*args)
+        self.ui = widget
+
+    def destroy(self, direct):
+        pass
```

### Comparing `QPUIQ-0.2.0/PUI/PySide6/button.py` & `QPUIQ-0.2.1/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/canvas.py` & `QPUIQ-0.2.1/PUI/PySide6/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/checkbox.py` & `QPUIQ-0.2.1/PUI/PySide6/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/combobox.py` & `QPUIQ-0.2.1/PUI/PySide6/combobox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/label.py` & `QPUIQ-0.2.1/PUI/PySide6/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/layout.py` & `QPUIQ-0.2.1/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/radiobutton.py` & `QPUIQ-0.2.1/PUI/PySide6/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/scroll.py` & `QPUIQ-0.2.1/PUI/PySide6/scroll.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 class QtScrollArea(QtBaseWidget):
     terminal = False
 
     def __init__(self, vertical=None, horizontal=False):
         self.vertical = vertical
         self.horizontal = horizontal
-        self.widget = None
         super().__init__()
 
     def destroy(self, direct):
         if direct:
-            if self.ui:
-                self.ui.deleteLater()
             if self.widget:
                 self.widget.deleteLater()
+                self.widget = None
+        super().destroy(direct)
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.widget = prev.widget
         else:
             self.ui = QtWidgets.QScrollArea()
             self.ui.setWidgetResizable(True)
+            self.widget = None
             if self.vertical is None:
                 self.ui.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAsNeeded)
             elif self.vertical:
                 self.ui.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOn)
             else:
                 self.ui.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
             if self.horizontal is None:
@@ -42,51 +42,42 @@
     def addChild(self, idx, child):
         if idx != 0:
             return
         if isinstance(child, QtBaseLayout):
             self.widget = QtWidgets.QWidget()
             self.ui.setWidget(self.widget)
             self.widget.setLayout(child.outer)
-            if not hasattr(self.widget, "origResizeEvent"):
-                self.widget.origResizeEvent = self.widget.resizeEvent
             self.widget.resizeEvent = self.onUiResized
         elif isinstance(child, QtBaseWidget):
             self.ui.setWidget(child.outer)
-            if not hasattr(child.outer, "origResizeEvent"):
-                child.outer.origResizeEvent = child.outer.resizeEvent
             child.outer.resizeEvent = self.onUiResized
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if idx != 0:
             return
         if isinstance(child, QtBaseLayout):
             child.outer.setParent(None)
             self.widget.setParent(None)
+            self.widget.deleteLater()
+            self.widget = None
         elif isinstance(child, QtBaseWidget):
             child.outer.setParent(None)
         elif child.children:
             self.removeChild(idx, child.children[0])
 
     def onUiResized(self, event):
-        node = self
-        while node.retired_by:
-            node = node.retired_by
+        node = self.get_node()
+        if node.destroyed:
+            return
         if node.widget:
             node.widget.resizeEvent = self.onUiResized
         else:
             node.children[0].outer.resizeEvent = self.onUiResized
-        if node.widget:
-            node.widget.origResizeEvent(event)
-        elif node.children[0].outer:
-            node.children[0].outer.origResizeEvent(event)
-        else:
-            node.children[0].children[0].outer.origResizeEvent(event)
-
         if node.horizontal is False:
             if isinstance(node.children[0], QtBaseLayout):
                 node.outer.setMinimumWidth(node.children[0].outer.sizeHint().width())
             elif isinstance(node.children[0], QtBaseWidget):
                 node.outer.setMinimumWidth(node.children[0].outer.sizeHint().width())
 
         if node.vertical is False:
```

### Comparing `QPUIQ-0.2.0/PUI/PySide6/text.py` & `QPUIQ-0.2.1/PUI/PySide6/text.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/PySide6/textfield.py` & `QPUIQ-0.2.1/PUI/textual/radiobutton.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from .. import *
 from .base import *
 
-class QtLineEdit(QtBaseWidget):
-    def __init__(self, model):
+class TRadioButton(TBase):
+    def __init__(self, text, value, model):
         super().__init__()
+        self.text = text
+        self.value = value
         self.model = model
 
     def update(self, prev):
-        value = self.model.value
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
-            if prev.last_value != value:
-                self.ui.textChanged.disconnect()
-                self.ui.setText(str(value))
-                self.ui.textChanged.connect(self.on_textchanged)
-            self.last_value = value
         else:
-            self.last_value = value
-            self.ui = QtWidgets.QLineEdit()
-            self.ui.setText(str(value))
-            self.ui.textChanged.connect(self.on_textchanged)
+            self.ui = widgets.RadioButton(self.text)
+        self.ui.puinode = self
+        self.ui.value = self.value  == self.model.value
         super().update(prev)
 
-    def on_textchanged(self):
-        self.model.value = self.ui.text()
+    def _changed(self, value):
+        if value:
+            self.model.value = self.value
+        else:
+            self.root.redraw()
```

### Comparing `QPUIQ-0.2.0/PUI/PySide6/window.py` & `QPUIQ-0.2.1/PUI/PySide6/window.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .. import *
 from .base import *
+from .menu import *
 
 class QtWindow(QtBaseWidget):
     terminal = False
 
     def __init__(self, title=None, size=None, maximize=None, fullscreen=None):
         super().__init__()
         self.title = title
@@ -13,23 +14,22 @@
         self.curr_maximize = None
         self.fullscreen = fullscreen
         self.curr_fullscreen = None
 
     def update(self, prev=None):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
+            self.frame = prev.frame
             self.curr_size = prev.curr_size
             self.curr_maximize = prev.curr_maximize
             self.curr_fullscreen = prev.curr_fullscreen
         else:
             from PySide6 import QtWidgets
-            self.ui = QtWidgets.QWidget()
-            self.ui.setObjectName("Window")
-            self.box = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.Direction.LeftToRight)
-            self.ui.setLayout(self.box)
+            self.ui = QtWidgets.QMainWindow()
+            self.frame = None
 
         if self.curr_size != self.size:
             self.curr_size = self.size
             self.ui.resize(*self.size)
         if self.curr_maximize !=  self.maximize:
             self.curr_maximize = self.maximize
             self.ui.showMaximized()
@@ -37,21 +37,29 @@
             self.curr_fullscreen = self.fullscreen
             self.ui.showFullScreen()
         if not self.title is None:
             self.ui.setWindowTitle(self.title)
         super().update(prev)
 
     def addChild(self, idx, child):
-        if isinstance(child, QtBaseLayout):
-            self.box.addLayout(child.ui)
+        if isinstance(child, QtMenuBar):
+            self.ui.setMenuBar(child.outer)
+        elif isinstance(child, QtBaseLayout):
+            self.frame = QtWidgets.QWidget()
+            self.ui.setCentralWidget(self.frame)
+            self.frame.setLayout(child.outer)
         elif isinstance(child, QtBaseWidget):
-            self.box.addWidget(child.ui)
+            self.ui.setCentralWidget(child.outer)
         else:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
-        if isinstance(child, QtBaseLayout):
-            self.box.removeItem(child.ui)
+        if isinstance(child, QtMenuBar):
+            child.outer.close()
+        elif isinstance(child, QtBaseLayout):
+            self.frame.setParent(None)
+            self.frame.deleteLater()
+            self.frame = None
         elif isinstance(child, QtBaseWidget):
-            child.ui.setParent(None)
+            child.outer.setParent(None)
         else:
             self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.2.0/PUI/dom.py` & `QPUIQ-0.2.1/PUI/dom.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,114 @@
 # dprint = print
 dprint = lambda *x: x
 
-def recur_delete(node, idx, child, direct):
+def recur_delete(node, child, direct):
     child.destroyed = True
-    for sidx,sc in enumerate(child.children):
-        recur_delete(child, sidx, sc, False)
+    for sc in child.children:
+        recur_delete(child, sc, False)
     child.destroy(direct)
 
 def sync(node, oldDOM, newDOM):
     dprint("syncing", node.key, len(oldDOM), len(newDOM))
+
     dprint("  ===OLD===")
     for c in oldDOM:
         dprint("   ", c.key)
+
     dprint("  ===NEW===")
     for c in newDOM:
         dprint("   ", c.key)
     oldMap = [x.key for x in oldDOM]
+    newMap = [x.key for x in newDOM]
+
+    tbd = []
+    for i,new in enumerate(newDOM):
+        while True:
+            if i < len(oldDOM) and oldMap[i] == new.key: # matched
+                dprint(f"MATCHED {i} {new.key}")
+                old = oldDOM[i]
+
+                try:
+                    new.update(old)
+                except:
+                    import traceback
+                    print("## <ERROR OF update() >")
+                    print(node.key)
+                    traceback.print_exc()
+                    print("## </ERROR OF update()>")
+
+                if not new.terminal:
+                    sync(new, old.children, new.children)
+
+                break # finish
+
+            trimmed = False
+            while i < len(oldDOM) and not oldDOM[i].key in newMap: # trim old nodes
+                dprint(f"TRIM {i} {oldDOM[i].key}")
+                old = oldDOM.pop(i)
+                oldMap.pop(i)
+                node.removeChild(i, old)
+                tbd.append(old)
+                trimmed = True
+
+            if trimmed:
+                continue # restart
+
+            try: # node exists
+                idx = oldMap[i+1:].index(new.key)+i+1
+                if idx==i+1: # move wrong node
+                    oldMap.pop(i)
+                    old = oldDOM.pop(i)
+                    node.removeChild(i, old)
+
+                    node.addChild(len(oldDOM), old)
+                    oldMap.append(old.key)
+                    oldDOM.append(old)
+
+                    continue # restart
+                else: # move target node
+                    oldMap.pop(idx)
+                    old = oldDOM.pop(idx)
+                    node.removeChild(idx, old)
+
+                    try:
+                        new.update(old)
+                    except:
+                        import traceback
+                        print("## <ERROR OF update() >")
+                        print(node.key)
+                        traceback.print_exc()
+                        print("## </ERROR OF update()>")
+
+                    if not new.terminal:
+                        sync(new, old.children, new.children)
+
+                    node.addChild(i, new)
+                    oldDOM.insert(i, None) # placeholder
+                    oldMap.insert(i, new.key)
+
+            except: # new node
+                try:
+                    new.update(None)
+                except:
+                    import traceback
+                    print("## <ERROR OF update() >")
+                    print(new.key)
+                    traceback.print_exc()
+                    print("## </ERROR OF update()>")
+                if not new.terminal:
+                    sync(new, [], new.children)
+                node.addChild(i, new)
+                oldDOM.insert(i, None) # placeholder
+                oldMap.insert(i, new.key)
+
+            break # finish
+
+    nl = len(newDOM)
+    while len(oldDOM) > nl:
+        old = oldDOM.pop(nl)
+        oldMap.pop(nl)
+        node.removeChild(nl, old)
+        tbd.append(old)
 
-    skipHead = 0
-    for i in range(0, min(len(oldDOM), len(newDOM))):
-        if oldDOM[i].key == newDOM[i].key:
-            oldMap[i] = None
-            old = oldDOM[i]
-            new = newDOM[i]
-            try:
-                new.update(old)
-            except:
-                import traceback
-                print("## <ERROR OF update() >")
-                print(node.key)
-                traceback.print_exc()
-                print("## </ERROR OF update()>")
-
-            if not new.terminal:
-                sync(new, old.children, new.children)
-            skipHead += 1
-        else:
-            break
-
-    skipTail = 0
-    # for i in range(0, min(len(oldDOM)-skipHead, len(newDOM)-skipHead)):
-    #     if oldDOM[-1-i].key == newDOM[-1-i].key:
-    #         oldMap[-1-i] = None
-    #         old = oldDOM[-1-i]
-    #         new = newDOM[-1-i]
-    #         new.update(old)
-    #         sync(new, old.children, new.children)
-    #         skipTail += 1
-    #     else:
-    #         break
-
-    for i, new in enumerate(newDOM[skipHead:len(newDOM)-skipTail]):
-        new_idx = skipHead + i
-        try:
-            old_idx = oldMap.index(new.key)
-        except:
-            old_idx = -1
-        if old_idx >= 0:
-            oldMap[old_idx] = None
-            old = oldDOM[old_idx]
-            node.removeChild(old_idx, old)
-            try:
-                new.update(old)
-            except:
-                import traceback
-                print("## <ERROR OF update() >")
-                print(new.key)
-                traceback.print_exc()
-                print("## </ERROR OF update()>")
-            if not new.terminal:
-                sync(new, old.children, new.children)
-            node.addChild(new_idx, old)
-        else:
-            try:
-                new.update(None)
-            except:
-                import traceback
-                print("## <ERROR OF update() >")
-                print(new.key)
-                traceback.print_exc()
-                print("## </ERROR OF update()>")
-            if not new.terminal:
-                sync(new, [], new.children)
-            node.addChild(new_idx, new)
-
-    for old_idx, key in enumerate(oldMap):
-        if key:
-            old = oldDOM[old_idx]
-            recur_delete(node, old_idx, old, True)
+    for old in tbd:
+        recur_delete(node, old, True)
```

### Comparing `QPUIQ-0.2.0/PUI/flet/application.py` & `QPUIQ-0.2.1/PUI/tkinter/label.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 from .. import *
 from .base import *
-
-class FApplication(PUIView):
-    def __init__(self):
-        super().__init__()
-        self.ready = False
-
-    def update(self, prev=None):
-        if not self.ready:
-            return
-        super().update()
-
-    def flet_app(self, page: ft.Page):
-        self.ui = page
-        self.ready = True
-        self.update()
-
-    def addChild(self, idx, child):
-        pass
-
-    def removeChild(self, idx, child):
-        pass
-
-    def start(self):
-        ft.app(self.flet_app)
+class TkLabel(TkBaseWidget):
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
+        self.text = text
+
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+            self.ui.config(text = self.text)
+        else:
+            self.ui = tk.Label(self.parent.ui, text=self.text, **self.kwargs)
+            self.ui.bind("<Button-1>", self._clicked)
+        if self.onClicked:
+            self.ui.config(cursor="")
```

### Comparing `QPUIQ-0.2.0/PUI/flet/layout.py` & `QPUIQ-0.2.1/PUI/flet/layout.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,36 +3,46 @@
 
 class FRow(FBase):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = ft.Row(expand=self.layout_weight)
+        super().update(prev)
 
     def addChild(self, idx, child):
-        self.ui.controls.append(child.outer)
+        self.ui.controls.insert(idx, child.outer)
         try:
             self.ui.update()
         except:
             pass
 
     def removeChild(self, idx, child):
-        self.ui.controls.remove(child.outer)
+        self.ui.controls.pop(idx)
         self.ui.update()
 
 class FColumn(FBase):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = ft.Column(expand=self.layout_weight)
+        super().update(prev)
 
     def addChild(self, idx, child):
-        self.ui.controls.append(child.outer)
+        self.ui.controls.insert(idx, child.outer)
         try:
             self.ui.update()
         except:
             pass
 
     def removeChild(self, idx, child):
-        self.ui.controls.remove(child.outer)
+        self.ui.controls.pop(idx)
         self.ui.update()
+
+class FSpacer(FBase):
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = ft.Container()
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.0/PUI/flet/textfield.py` & `QPUIQ-0.2.1/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/node.py` & `QPUIQ-0.2.1/PUI/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,19 +65,25 @@
         # print("exit", type(self).__name__, id(self))
         self.root.frames.pop()
         if ex_type is None: # don't consume exception
             return self
 
     @property
     def inner(self):
-        return self.ui
+        if self.ui:
+            return self.ui
+        return self.parent.inner
 
     @property
     def outer(self):
-        return self.ui
+        if self.ui:
+            return self.ui
+        if self.children:
+            return self.children[0].outer
+        return None
 
     def comment(self):
         return None
 
     def update(self, prev):
         if prev:
             prev.retired_by = self
@@ -92,14 +98,20 @@
     def removeChild(self, idx, child):
         pass
 
     def debug(self, level=1):
         self._debug = level
         return self
 
+    def get_node(self):
+        node = self
+        while node.retired_by:
+            node = node.retired_by
+        return node
+
     def __repr__(self):
         segs = []
         headline = [
             "  "*len(self.path),
             self.name or type(self).__name__,
             # f"@{str(id(self))}", # print view id
             " {",
@@ -144,15 +156,22 @@
     def click(self, callback, *cb_args, **cb_kwargs):
         self.onClicked = callback
         self.click_args = cb_args
         self.click_kwargs = cb_kwargs
         return self
 
     def _clicked(self, *args, **kwargs):
-        node = self
-        while node.retired_by:
-            node = node.retired_by
+        node = self.get_node()
         if node.onClicked:
             node.onClicked(*self.click_args, **self.click_kwargs)
 
+    def flet(self, **kwargs):
+        return self
+
+    def textual(self, **kwargs):
+        return self
+
+    def tk(self, **kwargs):
+        return self
+
     def qt(self, **kwargs):
         return self
```

### Comparing `QPUIQ-0.2.0/PUI/state.py` & `QPUIQ-0.2.1/PUI/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,23 +26,28 @@
 
     @property
     def value(self):
         return getattr(self.state, self.key)
 
     @value.setter
     def value(self, value):
-        try:
+        try: # skip validation error
             setattr(self.state, self.key, self.func(value))
         except:
             pass
 
     def change(self, callback):
         getattr(self.state, "_StateObject__callbacks")[self.key].add(callback)
 
-class IndexBinding():
+    def bind(self, getter, setter):
+        getattr(self.state, "_StateObject__binders")[self.key] = None
+        setattr(getattr(self.state, "_StateObject__values"), self.key, getter())
+        getattr(self.state, "_StateObject__binders")[self.key] = (getter, setter)
+
+class ListBinding():
     def __init__(self, state, key):
         try:
             self.viewroot = find_puiview()
             self.viewparent = self.viewroot.frames[-1]
         except PuiViewNotFoundError:
             pass
         self.state = state
@@ -55,27 +60,32 @@
         elif dt is float:
             self.func = float
         else:
             self.func = lambda x:x
 
     @property
     def value(self):
-        return self.state[self.key]
+        try: # skip validation error
+            return self.state[self.key]
+        except:
+            pass
 
     @value.setter
     def value(self, value):
-        try:
-            self.state[self.key] = self.func(value)
-        except:
-            pass
+        self.state[self.key] = self.func(value)
 
     def change(self, callback):
         getattr(self.state, "_StateList__callbacks")[self.key].add(callback)
 
-class KeyBinding():
+    def bind(self, getter, setter):
+        getattr(self.state, "_StateList__binders")[self.key] = None
+        self.state[self.key] = getter()
+        getattr(self.state, "_StateList__binders")[self.key] = (getter, setter)
+
+class DictBinding():
     def __init__(self, state, key):
         try:
             self.viewroot = find_puiview()
             self.viewparent = self.viewroot.frames[-1]
         except PuiViewNotFoundError:
             pass
         self.state = state
@@ -92,22 +102,27 @@
 
     @property
     def value(self):
         return self.state[self.key]
 
     @value.setter
     def value(self, value):
-        try:
+        try: # skip validation error
             self.state[self.key] = self.func(value)
         except:
             pass
 
     def change(self, callback):
         getattr(self.state, "_StateDict__callbacks")[self.key].add(callback)
 
+    def bind(self, getter, setter):
+        getattr(self.state, "_StateDict__binders")[self.key] = None
+        self.state[self.key] = getter()
+        getattr(self.state, "_StateDict__binders")[self.key] = (getter, setter)
+
 def _notify(listeners):
     tbd = []
     for l in listeners:
         if l.retired_by:
             tbd.append(l)
     for l in tbd:
         listeners.remove(l)
@@ -126,20 +141,21 @@
         return StateDict(data)
     return StateObject(data)
 
 class StateObject(BaseState):
     def __init__(self, values=None):
         self.__listeners = set()
         self.__callbacks = defaultdict(set)
+        self.__binders = {}
         if values is None:
             self.__values = BaseState()
         else:
             self.__values = values
 
-    def __call__(self, key):
+    def __call__(self, key=None):
         return AttrBinding(self, key)
 
     def __getattr__(self, key):
         if not key.startswith("_"):
             try:
                 view = find_puiview()
                 self.__listeners.add(view)
@@ -147,14 +163,17 @@
                 pass
         return getattr(self.__values, key)
 
     def __setattr__(self, key, value):
         if key.startswith("_"):
             object.__setattr__(self, key, value)
         else:
+            if self.__binders.get(key):
+                self.__binders[key][1](value)
+
             if type(value) is list:
                 value = StateList(value)
             elif type(value) is dict:
                 value = StateDict(value)
             if not hasattr(self.__values, key) or getattr(self.__values, key) != value:
                 setattr(self.__values, key, value)
                 _notify(self.__listeners)
@@ -164,31 +183,35 @@
     def __repr__(self):
         return f"StateObject({self.__values.__repr__()})"
 
 class StateList(BaseState):
     def __init__(self, values=None):
         self.__listeners = set()
         self.__callbacks = defaultdict(set)
+        self.__binders = {}
         if values is None:
             self.__values = []
         else:
             self.__values = values
 
-    def __call__(self, key):
-        return IndexBinding(self, key)
+    def __call__(self, key=None):
+        return ListBinding(self, key)
 
     def __getitem__(self, key):
         try:
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
+
         return self.__values[key]
 
     def __setitem__(self, key, value):
+        if self.__binders.get(key):
+            self.__binders[key][1](value)
         new = key >= len(self.__values)
         if new or self.__values[key] != value:
             self.__values[key] = value
             _notify(self.__listeners)
             for cb in self.__callbacks[key]:
                 cb(value)
             if new:
@@ -316,21 +339,22 @@
     def range(self):
         return range(len(self.__values))
 
 class StateDict(BaseState):
     def __init__(self, values=None):
         self.__listeners = set()
         self.__callbacks = defaultdict(set)
+        self.__binders = {}
         if values is None:
             self.__values = {}
         else:
             self.__values = values
 
-    def __call__(self, key, callback=None):
-        return KeyBinding(self, key)
+    def __call__(self, key=None):
+        return DictBinding(self, key)
 
     def __delitem__(self, key):
         self.__values.__delitem__(key)
         _notify(self.__listeners)
         for cb in self.__callbacks[None]:
             cb(self.__values)
 
@@ -352,16 +376,17 @@
         return getattr(self.__values, key)
 
 
     def __setattr__(self, key, value):
         if key.startswith("_"):
             object.__setattr__(self, key, value)
         else:
-            if not key.startswith("_"):
-                _notify(self.__listeners)
+            if self.__binders.get(key):
+                self.__binders[key][1](value)
+            _notify(self.__listeners)
             return setattr(self.__values, key, value)
 
     def __bool__(self):
         try:
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
@@ -381,14 +406,16 @@
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
         return self.__values.__repr__()
 
     def __setitem__(self, key, value):
+        if self.__binders.get(key):
+            self.__binders[key][1](value)
         if not key in self.__values or self.__values[key] != value:
             self.__values[key] = value
             _notify(self.__listeners)
         for cb in self.__callbacks[key]:
             cb(value)
         for cb in self.__callbacks[None]:
             cb(self.__values)
```

### Comparing `QPUIQ-0.2.0/PUI/textual/__init__.py` & `QPUIQ-0.2.1/PUI/textual/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,7 +37,9 @@
 Scroll = TScroll
 Spacer = TSpacer
 Text = TText
 Html = DummyWidget
 MarkDown = TLabel
 Combobox = DummyWidget
 ComboboxItem = DummyWidget
+
+PUI_BACKEND = "textual"
```

### Comparing `QPUIQ-0.2.0/PUI/textual/application.py` & `QPUIQ-0.2.1/PUI/textual/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,28 @@
 class TApplication(PUIView):
     def __init__(self):
         super().__init__()
         self.ui = PUIApp(self)
 
     def addChild(self, idx, child):
         if idx>0:
-            raise RuntimeError("Textual port only support single window")
+            raise RuntimeError("Textual backend only support single window")
         self.ui.query_one("#frame").mount(child.outer)
 
     def redraw(self):
+        self.dirty = True
+        if self.updating:
+            return
+        self.updating = True
+        self.ui.call_next(self._redraw)
+
+    def _redraw(self):
         with self.ui.batch_update():
-            self.update()
+            self.update(redraw=True)
+        self.updating = False
 
     def run(self):
-        self.setup()
         # self.redraw() # need to be after on_mount
         self.start()
 
     def start(self):
         self.ui.run()
```

### Comparing `QPUIQ-0.2.0/PUI/textual/checkbox.py` & `QPUIQ-0.2.1/PUI/textual/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/textual/label.py` & `QPUIQ-0.2.1/PUI/textual/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/textual/layout.py` & `QPUIQ-0.2.1/PUI/PySide6/mdi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 from .. import *
 from .base import *
 
-class TVertical(TBase):
+class QtMdiArea(QtBaseWidget):
+    terminal = False
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            self.ui = containers.Vertical()
-            self.ui.set_styles("height: auto;")
+            self.ui = QtWidgets.QMdiArea()
 
-    def addChild(self, idx, child):
-        self.inner.mount(child.outer)
-
-    def removeChild(self, idx, child):
-        child.tremove()
-
-class THorizontal(TBase):
-    def update(self, prev):
-        if prev and hasattr(prev, "ui"):
-            self.ui = prev.ui
-        else:
-            self.ui = containers.Horizontal()
-            self.ui.set_styles("width: auto;")
+        super().update(prev)
 
     def addChild(self, idx, child):
-        self.inner.mount(child.outer)
+        self.ui.addSubWindow(child.outer)
 
     def removeChild(self, idx, child):
-        child.tremove()
+        self.ui.removeSubWindow(child.outer)
 
-class TSpacer(TBase):
+class QtMdiSubWindow(QtBaseFrame):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            self.ui = widgets.Static("")
-            self.ui.set_styles("width: 1fr; height: 1fr;")
+            self.ui = QtWidgets.QMdiSubWindow()
+
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.0/PUI/textual/textfield.py` & `QPUIQ-0.2.1/PUI/textual/textfield.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .. import *
 from .base import *
 
 class TInput(TBase):
+    content_width = None
     def __init__(self, model):
         super().__init__()
         self.model = model
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
```

### Comparing `QPUIQ-0.2.0/PUI/textual/window.py` & `QPUIQ-0.2.1/PUI/tkinter/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from .. import *
-import sys
-
-class TWindow(PUINode):
-    def __init__(self, title=None, size=None, maximize=None, fullscreen=None):
+import tkinter as tk
+from tkinter import ttk
+class TkBaseWidget(PUINode):
+    def __init__(self, layout=None, side=None, **kwargs):
         super().__init__()
-        self.title = title
-        self.size = size
-        self.curr_size = None
-        self.maximize = maximize
-        self.curr_maximize = None
-        self.fullscreen = fullscreen
-        self.curr_fullscreen = None
+        self.layout_type = layout
+        self.side = side
+        self.kwargs = kwargs
 
     @property
-    def inner(self):
-        return self.parent.inner
+    def tkparent(self):
+        parent = self.parent
+        while not isinstance(parent, TkBaseWidget):
+            parent = parent.parent
+        return parent
 
-    @property
-    def outer(self):
-        if self.children:
-            return self.children[0].outer
-        else:
-            return None
+    def destroy(self, direct):
+        if self.ui:
+            self.ui.destroy() # tk's destroy
+            self.ui = None
```

### Comparing `QPUIQ-0.2.0/PUI/timeline.py` & `QPUIQ-0.2.1/PUI/timeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,34 +13,22 @@
         else:
             self.timer = Timer(self.ttl_sec, self.timer_cb)
             self.timer.start()
 
     def timer_cb(self):
         if not self.timer:
             return
-        node = self
-        while node.retired_by:
-            node = node.retired_by
+        node = self.get_node()
         root = node.root
         if not root:
             return
         root.redraw()
         node.timer = Timer(self.ttl_sec, self.timer_cb)
         node.timer.start()
 
-    @property
-    def inner(self):
-        return self.parent.inner
-
-    @property
-    def outer(self):
-        if self.children:
-            return self.children[0].outer
-        return None
-
     def destroy(self, direct):
         timer = self.timer
         self.timer = None
         if timer:
             timer.cancel()
         super().destroy(direct)
```

### Comparing `QPUIQ-0.2.0/PUI/tkinter/application.py` & `QPUIQ-0.2.1/PUI/tkinter/application.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .. import *
 from .base import *
+import functools
 
 class TkApplication(PUIView):
     def redraw(self):
         if self.ui:
-            self.ui.after(0, self.update)
+            self.ui.after(0, functools.partial(self.update, redraw=True))
         else:
-            self.update()
+            self.update(redraw=True)
 
     def update(self, prev=None):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = tk.Tk()
             self.ui.withdraw()
```

### Comparing `QPUIQ-0.2.0/PUI/tkinter/canvas.py` & `QPUIQ-0.2.1/PUI/tkinter/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/tkinter/label.py` & `QPUIQ-0.2.1/PUI/flet/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from .. import *
-from .base import *
-class TkLabel(TkBaseWidget):
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
-        self.text = text
+import flet as ft
+
+def _apply_params(ui, params):
+    for k,v in params.items():
+        setattr(ui, k, v)
+class FBase(PUINode):
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.flet_params = {}
+
+    def flet(self, **kwargs):
+        for k,v in kwargs.items():
+            self.flet_params[k] = v
+        return self
 
     def update(self, prev):
-        if prev and hasattr(prev, "ui"):
-            self.ui = prev.ui
-            self.ui.config(text = self.text)
-        else:
-            self.ui = tk.Label(self.parent.ui, text=self.text, **self.kwargs)
-            self.ui.bind("<Button-1>", self._clicked)
-        if self.onClicked:
-            self.ui.config(cursor="")
+        _apply_params(self.ui, self.flet_params)
+        super().update(prev)
+
+def find_flet_outer(node):
+    if isinstance(node, FBase):
+        return node.outer
+    else:
+        return find_flet_outer(node.children[0])
```

### Comparing `QPUIQ-0.2.0/PUI/tkinter/layout.py` & `QPUIQ-0.2.1/PUI/tkinter/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/tkinter/scroll.py` & `QPUIQ-0.2.1/PUI/tkinter/scroll.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/tkinter/textfield.py` & `QPUIQ-0.2.1/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/tkinter/window.py` & `QPUIQ-0.2.1/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.0/PUI/view.py` & `QPUIQ-0.2.1/PUI/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,21 +48,23 @@
         return scope
 
     def destroy(self, direct):
         PUIView.__ALLVIEWS__.remove(self)
         return super().destroy(direct)
 
     def redraw(self):
-        self.update()
+        self.update(redraw=True)
 
-    def update(self, prev=None):
+    def update(self, prev=None, redraw=False):
         if self.retired_by:
             return
         if self.destroyed:
             return
+        if not prev and not redraw:
+            self.setup()
         update_start = time.time()
         dprint("update()", self.key)
         if prev:
             self.children = prev.children
             prev.retired_by = self
             PUIView.__ALLVIEWS__.remove(prev)
 
@@ -92,24 +94,9 @@
 
         dprint(f"update() time: {time.time()-update_start:.5f}", self.key)
 
     def setup(self):
         pass
 
     def run(self):
-        self.setup()
         self.redraw()
         self.start()
-
-    @property
-    def inner(self):
-        if self.ui:
-            return self.ui
-        return self.parent.inner
-
-    @property
-    def outer(self):
-        if self.ui:
-            return self.ui
-        if self.children:
-            return self.children[0].outer
-        return None
```

### Comparing `QPUIQ-0.2.0/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.0
+Version: 0.2.1
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -155,14 +155,18 @@
 
 ![Cookbook 1](https://github.com/buganini/PUI/raw/main/screenshots/cookbook1.png)
 ![Cookbook 2](https://github.com/buganini/PUI/raw/main/screenshots/cookbook2.png)
 
 `python -m cookbook textual`
 ![Cookbook textual](https://github.com/buganini/PUI/raw/main/screenshots/cookbook_textual.png)
 
+## Hot-Reload with Reloadium
+[![Hot-Reload with Reloadium](https://img.youtube.com/vi/X716rwchPBM/0.jpg)](https://www.youtube.com/watch?v=X716rwchPBM)
+
+
 # Backends
 ## Tier-1
 * PySide6
 ## Lower Priority
 * tkinter
     * or https://github.com/rdbende/Sun-Valley-ttk-theme
 * flet
```

### Comparing `QPUIQ-0.2.0/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.2.1/QPUIQ.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,27 +14,33 @@
 PUI/PySide6/base.py
 PUI/PySide6/button.py
 PUI/PySide6/canvas.py
 PUI/PySide6/checkbox.py
 PUI/PySide6/combobox.py
 PUI/PySide6/label.py
 PUI/PySide6/layout.py
+PUI/PySide6/mdi.py
+PUI/PySide6/menu.py
 PUI/PySide6/progressbar.py
 PUI/PySide6/radiobutton.py
 PUI/PySide6/scroll.py
+PUI/PySide6/splitter.py
 PUI/PySide6/text.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
 PUI/flet/__init__.py
+PUI/flet/appbar.py
 PUI/flet/application.py
 PUI/flet/base.py
 PUI/flet/button.py
 PUI/flet/label.py
 PUI/flet/layout.py
 PUI/flet/progressbar.py
+PUI/flet/scroll.py
+PUI/flet/text.py
 PUI/flet/textfield.py
 PUI/flet/window.py
 PUI/textual/__init__.py
 PUI/textual/application.py
 PUI/textual/base.py
 PUI/textual/button.py
 PUI/textual/checkbox.py
```

### Comparing `QPUIQ-0.2.0/README.md` & `QPUIQ-0.2.1/QPUIQ.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: QPUIQ
+Version: 0.2.1
+Summary: "PUI" Python Declarative UI Framework
+Home-page: https://github.com/buganini/PUI
+Author: Buganini Chiu
+Author-email: buganini@b612.tw
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # What is PUI
 PUI is a declarative UI framework with two-way data binding
 
 # Installation
 ```
 pip install QPUIQ
 ```
@@ -145,14 +155,18 @@
 
 ![Cookbook 1](https://github.com/buganini/PUI/raw/main/screenshots/cookbook1.png)
 ![Cookbook 2](https://github.com/buganini/PUI/raw/main/screenshots/cookbook2.png)
 
 `python -m cookbook textual`
 ![Cookbook textual](https://github.com/buganini/PUI/raw/main/screenshots/cookbook_textual.png)
 
+## Hot-Reload with Reloadium
+[![Hot-Reload with Reloadium](https://img.youtube.com/vi/X716rwchPBM/0.jpg)](https://www.youtube.com/watch?v=X716rwchPBM)
+
+
 # Backends
 ## Tier-1
 * PySide6
 ## Lower Priority
 * tkinter
     * or https://github.com/rdbende/Sun-Valley-ttk-theme
 * flet
@@ -226,8 +240,8 @@
         * ...
     * Table
     * Tree
     * ~~Scrollbar (or as a layout setting)~~
 * Better DOM syncer
     * Prevent unnecessary nested update
     * Trace Event Source (TextField) and prevent update it DOM Sync
-* Pydantic State
+* Pydantic State
```

### Comparing `QPUIQ-0.2.0/setup.py` & `QPUIQ-0.2.1/setup.py`

 * *Files identical despite different names*

