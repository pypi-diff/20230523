# Comparing `tmp/edman_cli-2023.5.12.tar.gz` & `tmp/edman_cli-2023.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_cli-2023.5.12.tar", last modified: Fri May 12 07:10:39 2023, max compression
+gzip compressed data, was "edman_cli-2023.5.23.tar", last modified: Tue May 23 00:42:37 2023, max compression
```

## Comparing `edman_cli-2023.5.12.tar` & `edman_cli-2023.5.23.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2023.5.12/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3345 2023-01-20 03:57:51.000000 edman_cli-2023.5.12/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/edman_cli.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1495 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/entry_points.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       71 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1468 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/pyproject.toml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/scripts/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16460 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/scripts/action.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2229 2022-03-23 07:12:34.000000 edman_cli-2023.5.12/scripts/assign_bson_type.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2022-11-21 07:40:05.000000 edman_cli-2023.5.12/scripts/db_create.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2022-11-21 07:40:05.000000 edman_cli-2023.5.12/scripts/db_destroy.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1573 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2557 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/entry.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2328 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/scripts/file_add.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2947 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/file_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2513 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/scripts/file_dl.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2022-04-13 08:48:24.000000 edman_cli-2023.5.12/scripts/find.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2628 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/item_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1907 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/pullout.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2403 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/structure_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2096 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/update.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2022-11-21 07:40:05.000000 edman_cli-2023.5.12/tests/test_action.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:41:13.000000 edman_cli-2023.5.12/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     2180 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rstpep2html.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/src/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/src/edman-cli/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/venv/src/edman-cli/scripts/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16618 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/action.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2287 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/assign_bson_type.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/db_create.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/db_destroy.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1618 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2624 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/entry.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_add.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3027 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3177 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_dl.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/find.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2702 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/item_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1960 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/pullout.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2462 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/structure_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2156 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/update.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      855 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/setup.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/venv/src/edman-cli/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/tests/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2023.5.23/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3345 2023-01-20 03:57:51.000000 edman_cli-2023.5.23/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/edman_cli.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1495 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       71 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1468 2023-05-23 00:41:39.000000 edman_cli-2023.5.23/pyproject.toml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16460 2023-05-12 07:08:01.000000 edman_cli-2023.5.23/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2229 2022-03-23 07:12:34.000000 edman_cli-2023.5.23/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2022-11-21 07:40:05.000000 edman_cli-2023.5.23/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2022-11-21 07:40:05.000000 edman_cli-2023.5.23/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1573 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2557 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2328 2023-05-12 07:08:01.000000 edman_cli-2023.5.23/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2947 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2513 2023-05-12 07:08:01.000000 edman_cli-2023.5.23/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2022-04-13 08:48:24.000000 edman_cli-2023.5.23/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2628 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1907 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2403 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2096 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2022-11-21 07:40:05.000000 edman_cli-2023.5.23/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:41:13.000000 edman_cli-2023.5.23/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/venv/src/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/src/edman-cli/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/src/edman-cli/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16618 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2287 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1618 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2624 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3027 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3177 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2702 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1960 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2462 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2156 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      855 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/src/edman-cli/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/tests/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/tests/test_action.py
```

### Comparing `edman_cli-2023.5.12/LICENSE.txt` & `edman_cli-2023.5.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/PKG-INFO` & `edman_cli-2023.5.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_cli
-Version: 2023.5.12
+Version: 2023.5.23
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `edman_cli-2023.5.12/README.rst` & `edman_cli-2023.5.23/README.rst`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/edman_cli.egg-info/PKG-INFO` & `edman_cli-2023.5.23/edman_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman-cli
-Version: 2023.5.12
+Version: 2023.5.23
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `edman_cli-2023.5.12/edman_cli.egg-info/SOURCES.txt` & `edman_cli-2023.5.23/edman_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/edman_cli.egg-info/entry_points.txt` & `edman_cli-2023.5.23/edman_cli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/pyproject.toml` & `edman_cli-2023.5.23/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
     "pymongo~=4.3.3",
     " python-dateutil~=2.8.2",
     "jmespath~=1.0.1",
-    "edman~=2023.5.12",
+    "edman~=2023.5.23",
 ]
-version = "2023.5.12"
+version = "2023.5.23"
 
 [project.urls]
 "repository" = "https://github.com/ryde/edman_cli"
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
```

### Comparing `edman_cli-2023.5.12/scripts/action.py` & `edman_cli-2023.5.23/scripts/action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/assign_bson_type.py` & `edman_cli-2023.5.23/scripts/assign_bson_type.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/db_create.py` & `edman_cli-2023.5.23/scripts/db_create.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/db_destroy.py` & `edman_cli-2023.5.23/scripts/db_destroy.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/delete.py` & `edman_cli-2023.5.23/scripts/delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/entry.py` & `edman_cli-2023.5.23/scripts/entry.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/file_add.py` & `edman_cli-2023.5.23/scripts/file_add.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/file_delete.py` & `edman_cli-2023.5.23/scripts/file_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/file_dl.py` & `edman_cli-2023.5.23/scripts/file_dl.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/find.py` & `edman_cli-2023.5.23/scripts/find.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/item_delete.py` & `edman_cli-2023.5.23/scripts/item_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/pullout.py` & `edman_cli-2023.5.23/scripts/pullout.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/structure_convert.py` & `edman_cli-2023.5.23/scripts/structure_convert.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/scripts/update.py` & `edman_cli-2023.5.23/scripts/update.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/tests/test_action.py` & `edman_cli-2023.5.23/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/jp.py` & `edman_cli-2023.5.23/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2html.py` & `edman_cli-2023.5.23/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2html4.py` & `edman_cli-2023.5.23/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2html5.py` & `edman_cli-2023.5.23/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2latex.py` & `edman_cli-2023.5.23/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2man.py` & `edman_cli-2023.5.23/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2odt.py` & `edman_cli-2023.5.23/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2pseudoxml.py` & `edman_cli-2023.5.23/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2s5.py` & `edman_cli-2023.5.23/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2xetex.py` & `edman_cli-2023.5.23/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rst2xml.py` & `edman_cli-2023.5.23/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/bin/rstpep2html.py` & `edman_cli-2023.5.23/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/action.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/assign_bson_type.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/assign_bson_type.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/db_create.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_create.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/db_destroy.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_destroy.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/delete.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/entry.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/entry.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_add.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_add.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_delete.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_dl.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_dl.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/find.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/find.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/item_delete.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/item_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/pullout.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/pullout.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/structure_convert.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/structure_convert.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/scripts/update.py` & `edman_cli-2023.5.23/venv/src/edman-cli/scripts/update.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/setup.py` & `edman_cli-2023.5.23/venv/src/edman-cli/setup.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.12/venv/src/edman-cli/tests/test_action.py` & `edman_cli-2023.5.23/venv/src/edman-cli/tests/test_action.py`

 * *Files identical despite different names*

