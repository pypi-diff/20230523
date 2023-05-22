# Comparing `tmp/talondoc-0.6.0.tar.gz` & `tmp/talondoc-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talondoc-0.6.0.tar", last modified: Sun May 21 20:48:56 2023, max compression
+gzip compressed data, was "talondoc-1.0.0rc0.tar", last modified: Mon May 22 22:42:11 2023, max compression
```

## Comparing `talondoc-0.6.0.tar` & `talondoc-1.0.0rc0.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.210946 talondoc-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-21 20:48:42.000000 talondoc-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-21 20:48:56.210946 talondoc-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-21 20:48:42.000000 talondoc-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-21 20:48:42.000000 talondoc-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 20:48:56.210946 talondoc-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 20:48:42.000000 talondoc-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.198946 talondoc-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_autogen/
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_autogen/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/conf.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/index.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/index.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/python_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/python_file.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/talon_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/talon_file.rst.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_cache_builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_cache_builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_cache_builtin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    38478 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_cache_builtin/resources/talon.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/analysis/live/
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/live/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/registry/
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/registry/data/
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/data/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/data/serialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/static/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/python/shims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/talon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/description/
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/description/describer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/sphinx/_util/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/_util/addnodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/_util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/sphinx/directives/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/capture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.210946 talondoc-0.6.0/src/talondoc/sphinx/directives/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/hlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.612201 talondoc-1.0.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.616201 talondoc-1.0.0rc0/src/talondoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.616201 talondoc-1.0.0rc0/src/talondoc/_autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/conf.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/index.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/index.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/python_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/python_file.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/talon_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/talon_file.rst.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    38478 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/resources/talon.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/live/
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/serialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/analysis/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/analysis/static/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22422 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/python/shims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/talon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/description/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/description/describer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/fragtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/capture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/hlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.616201 talondoc-1.0.0rc0/src/talondoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/top_level.txt
```

### Comparing `talondoc-0.6.0/PKG-INFO` & `talondoc-1.0.0rc0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 0.6.0
+Version: 1.0.0rc0
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-0.6.0/README.md` & `talondoc-1.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/pyproject.toml` & `talondoc-1.0.0rc0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talondoc"
-version = "0.6.0"
+version = "1.0.0rc0"
 description = "A Sphinx extension for Talon user directories."
 license = { file = 'LICENSE' }
 authors = [{ name = "Wen Kokke", email = "wenkokke@users.noreply.github.com" }]
 readme = "README.md"
 keywords = ["talon", "sphinx"]
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -54,28 +54,28 @@
   "sphinx_tabs >=3.4,<5"
 ]
 
 [project.scripts]
 talondoc = "talondoc:talondoc"
 
 [tool.bumpver]
-current_version = "0.6.0"
-version_pattern = "MAJOR.MINOR.PATCH"
+current_version = "1.0.0-rc"
+version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
   '^current_version = "{version}"$',
-  '^version = "{version}"$',
+  '^version = "{pep440_version}"$',
 ]
-"example/docs/conf.py" = ['^release = "{version}"$']
-"src/talondoc/_version.py" = ['^__version__: str = "{version}"$']
+"example/docs/conf.py" = ['^release = "{pep440_version}"$']
+"src/talondoc/_version.py" = ['^__version__: str = "{pep440_version}"$']
 
 [tool.isort]
 profile = "black"
 line_length = 88
 
 [tool.mypy]
 python_version = 3.9
@@ -102,25 +102,26 @@
 [testenv]
 allowlist_externals = cp, mkdir, sh, rm
 extras =
   test
 setenv =
   TALONDOC_STRICT = 1
 commands_pre =
-  cp '{tox_root}/example/build.sh' '{env_tmp_dir}/build.sh'
+  cp '{tox_root}/example/autogen.sh' '{env_tmp_dir}/autogen.sh'
   cp -R '{tox_root}/example/knausj_talon' '{env_tmp_dir}/knausj_talon'
   mkdir -p '{env_tmp_dir}/docs'
   cp '{tox_root}/example/docs/conf.py' '{env_tmp_dir}/docs/conf.py'
   cp '{tox_root}/example/docs/index.md' '{env_tmp_dir}/docs/index.md'
   cp -R '{tox_root}/example/docs/_static' '{env_tmp_dir}/docs/_static'
 commands =
-  sh '{env_tmp_dir}/build.sh'
-  {envpython} -m bumpver update --patch --dry --no-fetch
+  {envpython} -m bumpver update --patch --no-fetch --dry
+  sh '{env_tmp_dir}/autogen.sh'
+  {envpython} -m talondoc build '{env_tmp_dir}/docs' '{env_tmp_dir}/docs/_build'
 commands_post =
-  rm -f '{env_tmp_dir}/build.sh'
+  rm -f '{env_tmp_dir}/autogen.sh'
   rm -rf '{env_tmp_dir}/knausj_talon'
   rm -f '{env_tmp_dir}/docs/conf.py'
   rm -f '{env_tmp_dir}/docs/index.md'
   rm -rf '{env_tmp_dir}/docs/_static'
 
 [testenv:py39-md]
 setenv =
```

### Comparing `talondoc-0.6.0/src/talondoc/_autogen/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/_autogen/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import os
 import subprocess
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Optional, Union
+from typing import Iterator, Optional, Union
 
 import jinja2
 import jinja2.sandbox
 from typing_extensions import Literal
 
 from .._util.progress_bar import ProgressBar
 from ..analysis.registry import Registry, data
@@ -18,14 +18,26 @@
 # https://github.com/sphinx-doc/sphinx/blob/5.x/sphinx/ext/autosummary/generate.py
 def _underline(title: str, line: str = "=") -> str:
     if "\n" in title:
         raise ValueError("Can only underline single lines")
     return title + "\n" + line * len(title)
 
 
+def _section(title: str) -> str:
+    return _underline(title, line="=")
+
+
+def _subsection(title: str) -> str:
+    return _underline(title, line="-")
+
+
+def _subsubsection(title: str) -> str:
+    return _underline(title, line="^")
+
+
 def _default_package_name(package_name: Optional[str], package_dir: Path) -> str:
     return package_name or package_dir.parts[-1]
 
 
 def _default_author(author: Optional[str]) -> str:
     if author:
         return author
@@ -80,14 +92,17 @@
     # Create jinja2 environment
     env = jinja2.sandbox.SandboxedEnvironment(
         loader=jinja2.ChoiceLoader(loaders),
         autoescape=False,
         keep_trailing_newline=False,
     )
     env.filters["underline"] = _underline
+    env.filters["section"] = _section
+    env.filters["subsection"] = _subsection
+    env.filters["subsubsection"] = _subsubsection
 
     # Analyse the package
     registry = Registry()
     analyse_package(
         registry=registry,
         package_dir=package_dir,
         package_name=package_name,
@@ -123,48 +138,87 @@
     toc: list[Path] = []
     total: int = len(package.files)
     if generate_conf:
         total += 1
     if generate_index:
         total += 1
     bar = ProgressBar(total=total)
-    for file_name in package.files:
-        file: data.File = registry.get(data.File, file_name, referenced_by=package)
+    files: list[data.File] = [
+        registry.get(data.File, file_name, referenced_by=package)
+        for file_name in package.files
+    ]
+    talon_files: list[data.File] = [
+        file for file in files if file.location.path.parts[-1].endswith(".talon")
+    ]
+    python_files: list[data.File] = [
+        file for file in files if file.location.path.parts[-1].endswith(".py")
+    ]
+
+    def _modules(file: data.File) -> list[data.Module]:
+        return [registry.get(data.Module, name) for name in file.modules]
+
+    def _contexts(file: data.File) -> list[data.Context]:
+        return [registry.get(data.Context, name) for name in file.contexts]
+
+    for file in talon_files:
         # Create path/to/talon/file.{md,rst}:
-        if file.location.path.suffix == ".talon":
-            bar.step(f" {str(file.location.path)}")
-            output_relpath = file.location.path.with_suffix(f".{format}")
+        bar.step(f" {str(file.location.path)}")
+        output_relpath = file.location.path.with_suffix(f".{format}")
+        output_path = output_dir / output_relpath
+        output_path.parent.mkdir(parents=True, exist_ok=True)
+
+        modules = _modules(file)
+        contexts = _contexts(file)
+
+        # Check whether the file has any content
+        has_content = any(module.has_content() for module in modules) or any(
+            context.has_content() for context in contexts
+        )
+
+        # Check whether the file defines any commands
+        has_commands = any(bool(context.commands) for context in contexts)
+
+        if has_content:
             toc.append(output_relpath)
-            output_path = output_dir / output_relpath
-            output_path.parent.mkdir(parents=True, exist_ok=True)
-            command_names: set[str] = set()
-            for context_name in file.contexts:
-                context = registry.get(data.Context, context_name)
-                command_names.update(context.commands)
             output_path.write_text(
                 template_talon_file.render(
-                    file_name=file_name, command_names=command_names, **ctx
+                    file=file,
+                    modules=modules,
+                    contexts=contexts,
+                    has_commands=has_commands,
+                    **ctx,
                 )
             )
 
+    for file in python_files:
         # Create path/to/python/file/api.{md,rst}:
-        elif file.location.path.suffix == ".py":
-            bar.step(f" {str(file.location.path)}")
-            output_relpath = file.location.path.with_suffix("") / f"api.{format}"
+        bar.step(f" {str(file.location.path)}")
+        output_relpath = file.location.path.with_suffix("") / f"api.{format}"
+        output_path = output_dir / output_relpath
+        output_path.parent.mkdir(parents=True, exist_ok=True)
+
+        modules = _modules(file)
+        contexts = _contexts(file)
+
+        # Check whether the file has any content
+        has_content = any(module.has_content() for module in modules) or any(
+            context.has_content() for context in contexts
+        )
+
+        if has_content:
             toc.append(output_relpath)
-            output_path = output_dir / output_relpath
-            output_path.parent.mkdir(parents=True, exist_ok=True)
             output_path.write_text(
-                template_python_file.render(file_name=file_name, **ctx)
+                template_python_file.render(
+                    file=file,
+                    modules=modules,
+                    contexts=contexts,
+                    **ctx,
+                )
             )
 
-        # Skip file entry:
-        else:
-            bar.step()
-
     # Create index.{md,rst}
     if generate_index:
         template_index = env.get_template(f"index.{format}.jinja2")
         output_path = output_dir / f"index.{format}"
         bar.step(f" index.{format}")
         output_path.parent.mkdir(parents=True, exist_ok=True)
         output_path.write_text(template_index.render(toc=toc, **ctx))
```

### Comparing `talondoc-0.6.0/src/talondoc/_autogen/resources/conf.py.jinja2` & `talondoc-1.0.0rc0/src/talondoc/_autogen/resources/conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/_cache_builtin/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/_cache_builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/_cache_builtin/resources/talon.json` & `talondoc-1.0.0rc0/src/talondoc/_cache_builtin/resources/talon.json`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/_util/io.py` & `talondoc-1.0.0rc0/src/talondoc/_util/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,28 +20,27 @@
         for line in self._stream:
             self._queue.put(line)
         self._stream.close()
 
     def readline(
         self, block: bool = False, timeout: Optional[float] = None
     ) -> Optional[str]:
-        if self._queue.empty() and self._stream.closed:
+        if self._stream.closed and self._queue.qsize() == 0:
             return None
         else:
             try:
                 return self._queue.get(block=block, timeout=timeout)
             except queue.Empty:
                 return None
 
     def readlines(
-        self, minlines: int = 0, timeout: Optional[float] = None
+        self, block: bool = False, timeout: Optional[float] = None
     ) -> Iterator[str]:
         while True:
-            line = self.readline(block=minlines > 0, timeout=timeout)
-            minlines -= 1
+            line = self.readline(block=block, timeout=timeout)
             if line is None:
                 return
             else:
                 yield line
 
     def readuntil(
         self, predicate: Callable[[str], bool], timeout: Optional[float] = None
@@ -59,8 +58,8 @@
             if line is not None:
                 line = line.rstrip()
                 if predicate(line):
                     yield line
                 else:
                     break
             else:
-                break
+                return
```

### Comparing `talondoc-0.6.0/src/talondoc/_util/logging.py` & `talondoc-1.0.0rc0/src/talondoc/_util/logging.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/_util/progress_bar.py` & `talondoc-1.0.0rc0/src/talondoc/_util/progress_bar.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/live/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/live/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,23 @@
         )
         # Create stderr wrapper:
         assert self._session.stderr is not None
         self._session_stderr = NonBlockingTextIOWrapper(
             io.TextIOWrapper(self._session.stderr, encoding="utf-8")
         )
         # Read at least one line from stdout:
-        for line in self._session_stdout.readlines(minlines=1):
+        line = self._session_stdout.readline(block=True, timeout=5)
+        if line:
             _LOGGER.debug(f"> {line}")
+        else:
+            buffer: list[str] = []
+            buffer.extend(self._session_stderr.readlines(timeout=3))
+            _LOGGER.debug("".join(buffer))
+            _LOGGER.error("Could not open repl. Is Talon running?")
+            exit(1)
 
     def eval(self, *line: str, encoding: str = "utf-8") -> str:
         assert self._session and self._session.stdin and self._session_stdout
         __EOR__ = "END_OF_RESPONSE"
         is_EOR = lambda line: line == __EOR__
         print_EOR = f"print('{__EOR__}')"
         self._session.stdin.write(bytes("\n".join([*line, print_EOR]) + "\n", encoding))
```

### Comparing `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_actions.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_actions.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_captures.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_captures.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_commands.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_commands.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_lists.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_lists.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_settings.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_settings.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/registry/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/registry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     @singledispatchmethod
     def register(self, value: DataVar) -> DataVar:
         raise TypeError(type(value))
 
     def _register_simple_data(self, value: SimpleDataVar) -> SimpleDataVar:
         # Print the value name to the log.
-        _LOGGER.debug(f"register {value.__class__.__name__} {value.name}")
+        _LOGGER.debug(f"Found declaration for {value.__class__.__name__} {value.name}")
         # Register the data in the store.
         store = self._typed_store(value.__class__)
         old_value = store.get(value.name, None)
         if old_value is not None:
             exc = DuplicateData([value, old_value])
             if self._continue_on_error:
                 _LOGGER.warning(exc)
@@ -78,23 +78,33 @@
             self._active_package = value
         if isinstance(value, data.File):
             self._active_file = value
         return value
 
     def _register_grouped_data(self, value: GroupDataVar) -> GroupDataVar:
         # Print the value name to the log.
-        _LOGGER.debug(f"register {value.__class__.__name__} {value.name}")
+        _LOGGER.debug(
+            " ".join(
+                [
+                    f"Found",
+                    "declaration"
+                    if issubclass(value.parent_type, data.Module)
+                    else "override",
+                    "for {value.__class__.__name__} {value.name}",
+                ]
+            )
+        )
         # Register the data in the store.
         store = self._typed_store(value.__class__)
         store.setdefault(value.name, []).append(value)
         return value
 
     def _register_callback(self, value: CallbackVar) -> CallbackVar:
         # Print the value name to the log.
-        _LOGGER.debug(f"register {value.__class__.__name__} {value.name}")
+        _LOGGER.debug(f"Found declaration for {value.__class__.__name__} {value.name}")
         # Register the data in the store.
         self._typed_store(data.Callback).setdefault(value.event_code, []).append(value)
         return value
 
     # Simple entries
     register.register(data.Package, _register_simple_data)
     register.register(data.File, _register_simple_data)
@@ -128,42 +138,42 @@
         for package in packages:
             if isinstance(package, data.Package):
                 yield package
             else:
                 try:
                     yield self.get(data.Package, package)
                 except UnknownReference as e:
-                    _LOGGER.error(e)
+                    _LOGGER.error(f"resolve_packages: {e}")
                     pass
 
     def resolve_files(
         self, files: Iterator[Union[data.FileName, data.File]]
     ) -> Iterator[data.File]:
         for file in files:
             if isinstance(file, data.File):
                 yield file
             else:
                 try:
                     yield self.get(data.File, file)
                 except UnknownReference as e:
-                    _LOGGER.error(e)
+                    _LOGGER.error(f"resolve_files: {e}")
                     pass
 
     def resolve_contexts(
         self, contexts: Iterator[Union[data.FileName, data.File, data.Context]]
     ) -> Iterator[data.Context]:
         for value in contexts:
             if isinstance(value, data.Context):
                 yield value
             else:
                 if isinstance(value, str):
                     try:
                         value = self.get(data.File, value)
                     except UnknownReference as e:
-                        _LOGGER.error(e)
+                        _LOGGER.error(f"resolve_contexts: {e}")
                         continue
                 assert isinstance(value, data.File)
                 for context_name in value.contexts:
                     yield self.get(data.Context, context_name, referenced_by=value)
 
     def get_commands(
         self,
@@ -212,32 +222,20 @@
             _LOGGER.warning(
                 f"Caught {e.__class__.__name__} "
                 f"when deciding if '{talonfmt(rule)}' "
                 f"matches '{' '.join(text)}'"
             )
         return False
 
-    # TODO: remove once builtins are properly supported
-    _BUILTIN_CAPTURE_NAMES: ClassVar[Sequence[data.CaptureName]] = (
-        "digit_string",
-        "digits",
-        "number",
-        "number_signed",
-        "number_small",
-        "phrase",
-        "word",
-    )
-
     def _get_capture_rule(self, name: data.CaptureName) -> Optional[data.Rule]:
         """Get the rule for a capture. Hook for 'match'."""
         try:
             return self.get(data.Capture, name).rule
         except UnknownReference as e:
-            # If the capture is not a builtin capture, log a warning:
-            if name not in self.__class__._BUILTIN_CAPTURE_NAMES:
+            if name not in ["phrase", "word"]:
                 _LOGGER.warning(e)
             return None
 
     def _get_list_value(self, name: data.ListName) -> Optional[data.ListValue]:
         """Get the values for a list. Hook for 'match'."""
         try:
             return self.get(data.List, name).value
@@ -274,15 +272,15 @@
         elif issubclass(cls, GroupData):
             declaration, defaults, others = self.lookup_partition(cls, name)
             for obj in itertools.chain((declaration,), defaults, others):
                 if obj:
                     value = cast(DataVar, obj)
                     break
         elif issubclass(cls, data.Callback):
-            raise ValueError(f"Registry.get does not support callbacks")
+            raise NotImplementedError(f"Registry.get does not support callbacks")
         if value is not None:
             return value
         else:
             raise UnknownReference(
                 cls,
                 name,
                 referenced_by=referenced_by,
@@ -326,15 +324,15 @@
         self, cls: type[GroupDataVar], data: Iterator[Optional[GroupDataVar]]
     ) -> Optional[GroupDataVar]:
         init_keys: set[str] = {field.name for field in fields(cls) if field.init}
         init_args: dict[str, Any] = {}
         for datum in data:
             if isinstance(datum, cls):
                 for name in init_keys:
-                    init_args[name] = init_args.get(name, getattr(datum, name))
+                    init_args[name] = init_args.get(name, None) or getattr(datum, name)
         if init_args:
             return cls(**init_args)
         else:
             return None
 
     def lookup_description(self, cls: type[Data], name: Any) -> Optional[str]:
         if issubclass(cls, SimpleData):
@@ -378,15 +376,15 @@
             declarations = tuple(declarations_iter)
             if len(declarations) >= 2:
                 _LOGGER.warning(DuplicateData([tup[1] for tup in declarations]))
             declaration = declarations[0][1] if len(declarations) >= 1 else None
 
             # Extract all overrides that are always on:
             default_overrides_iter, other_overrides_iter = partition(
-                lambda tup: tup[0] == _IS_ALWAYS_ON, overrides_iter
+                lambda tup: tup[0] != _IS_ALWAYS_ON, overrides_iter
             )
 
             default_overrides = tuple((tup[1] for tup in default_overrides_iter))
             other_overrides = tuple((tup[1] for tup in other_overrides_iter))
             if len(default_overrides) >= 2:
                 # NOTE: We warn the user if there are multiple overrides which
                 #       are always on, but suppress this warning for commands.
@@ -551,28 +549,24 @@
             data.Mode,
             data.Tag,
         ):
             _LOGGER.debug(f"Loading builtin {cls.__name__} objects...")
             store = parse_dict(registry.get(cls.__name__, {}))
             if issubclass(cls, GroupData):
                 for name, group in store.items():
-                    _LOGGER.debug(
-                        f"Found {len(group)} {cls.__name__} objects with {name}"
-                    )
                     for value in parse_list(group):
                         parsed_group_value = cls.from_dict(value)
                         if name != parsed_group_value.name:
                             _LOGGER.warning(
                                 f"Found {cls.__name__} {parsed_group_value.name} in group for {name}"
                             )
                         self.register(parsed_group_value)
 
             elif issubclass(cls, (data.Mode, data.Tag)):
                 for name, value in store.items():
-                    _LOGGER.debug(f"Found {cls.__name__} object with {name}")
                     parsed_simple_value = cls.from_dict(value)
                     if name != parsed_simple_value.name:
                         _LOGGER.warning(
                             f"Found {cls.__name__} {parsed_simple_value.name} in group for {name}"
                         )
                     self.register(parsed_simple_value)
             else:
```

### Comparing `talondoc-0.6.0/src/talondoc/analysis/registry/data/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import textwrap
-from collections.abc import Callable, Mapping, Sequence
+from collections.abc import Callable, Iterable, Mapping, Sequence
 from dataclasses import dataclass, field
 from functools import partial
 from inspect import Signature
 from typing import Any, Optional, Union
 
 import tree_sitter_talon
 from tree_sitter_talon import Node as Node
@@ -80,14 +80,16 @@
 
 ##############################################################################
 # Decoders - Matches
 ##############################################################################
 
 
 def parse_matches(value: Any) -> Sequence[Match]:
+    if isinstance(value, str):
+        value = "\n".join([line.strip() for line in value.splitlines()])
     src = f"{parse_str(value)}\n-\n"
     ast = tree_sitter_talon.parse(src, raise_parse_error=True)
     assert isinstance(ast, tree_sitter_talon.TalonSourceFile)
     for child in ast.children:
         if isinstance(child, tree_sitter_talon.TalonMatches):
             return [
                 match
@@ -196,91 +198,137 @@
 
 ##############################################################################
 # Packages
 ##############################################################################
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Package(SimpleData):
-    files: list["FileName"] = field(default_factory=list, init=False)
+    files: list["FileName"] = field(default_factory=list, init=False, hash=False)
 
     name: PackageName
-    description: None = field(default=None, init=False)
+    description: None = field(default=None, init=False, hash=False)
     location: Location
-    parent_name: None = field(default=None, init=False)
-    parent_type: None = field(default=None, init=False)
-    serialisable: bool = field(default=True, init=False)
+    parent_name: None = field(default=None, init=False, hash=False)
+    parent_type: None = field(default=None, init=False, hash=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
 
 ##############################################################################
 # Files
 ##############################################################################
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class File(SimpleData):
-    modules: list["ModuleName"] = field(default_factory=list, init=False)
-    contexts: list["ContextName"] = field(default_factory=list, init=False)
+    modules: list["ModuleName"] = field(default_factory=list, init=False, hash=False)
+    contexts: list["ContextName"] = field(default_factory=list, init=False, hash=False)
 
-    name: FileName = field(init=False)
-    description: None = field(default=None, init=False)
+    name: FileName = field(init=False, hash=False)
+    description: None = field(default=None, init=False, hash=False)
     location: Location
     parent_name: PackageName
-    parent_type: type[Package] = field(default=Package, init=False)
-    serialisable: bool = field(default=True, init=False)
+    parent_type: type[Package] = field(default=Package, init=False, hash=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = ".".join((self.parent_name, *self.location.path.parts))
+        super().__post_init__(*_args, **_kwargs)
 
 
 ##############################################################################
 # Modules and Contexts
 ##############################################################################
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Module(SimpleData):
     index: int
 
-    name: ModuleName = field(init=False)
+    name: ModuleName = field(init=False, hash=False)
     description: Optional[str]
     location: Location
     parent_name: FileName
-    parent_type: type[File] = field(default=File, init=False)
-    serialisable: bool = field(default=True, init=False)
+    parent_type: type[File] = field(default=File, init=False, hash=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
+
+    actions: list["ActionName"] = field(default_factory=list, init=False, hash=False)
+    captures: list["CaptureName"] = field(default_factory=list, init=False, hash=False)
+    lists: list["ListName"] = field(default_factory=list, init=False, hash=False)
+    modes: list["ModeName"] = field(default_factory=list, init=False, hash=False)
+    settings: list["CaptureName"] = field(default_factory=list, init=False, hash=False)
+    tags: list["TagName"] = field(default_factory=list, init=False, hash=False)
 
     def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         if self.index == 0:
             self.name = f"{self.parent_name}"
         else:
             self.name = f"{self.parent_name}.{self.index}"
+        super().__post_init__(*_args, **_kwargs)
+
+    def has_content(self) -> bool:
+        return any(
+            map(
+                bool,
+                [
+                    self.actions,
+                    self.captures,
+                    self.lists,
+                    self.modes,
+                    self.tags,
+                ],
+            )
+        )
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Context(SimpleData):
     index: int
     matches: list[Match]
-    commands: list["CommandName"] = field(default_factory=list, init=False)
 
-    name: ContextName = field(init=False)
+    name: ContextName = field(init=False, hash=False)
     description: Optional[str]
     location: Location
     parent_name: FileName
-    parent_type: type[File] = field(default=File, init=False)
-    serialisable: bool = field(default=True, init=False)
+    parent_type: type[File] = field(default=File, init=False, hash=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
+
+    commands: list["CommandName"] = field(default_factory=list, init=False, hash=False)
+    actions: list["ActionName"] = field(default_factory=list, init=False, hash=False)
+    captures: list["CaptureName"] = field(default_factory=list, init=False, hash=False)
+    lists: list["ListName"] = field(default_factory=list, init=False, hash=False)
+    modes: list["ModeName"] = field(default_factory=list, init=False, hash=False)
+    settings: list["CaptureName"] = field(default_factory=list, init=False, hash=False)
+    tags: list["TagName"] = field(default_factory=list, init=False, hash=False)
 
     def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         if self.index == 0:
             self.name = f"{self.parent_name}"
         else:
             self.name = f"{self.parent_name}.{self.index}"
+        super().__post_init__(*_args, **_kwargs)
+
+    def has_content(self) -> bool:
+        return any(
+            map(
+                bool,
+                [
+                    self.commands,
+                    self.actions,
+                    self.captures,
+                    self.lists,
+                    self.modes,
+                    self.tags,
+                ],
+            )
+        )
 
     @property
     def always_on(self) -> bool:
         return not self.matches
 
 
 ##############################################################################
@@ -294,76 +342,79 @@
 
 ##############################################################################
 # Functions
 ##############################################################################
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Function(SimpleData):
     namespace: str
-    name: str = field(init=False)
-    description: Optional[str] = field(init=False)
+    name: str = field(init=False, hash=False)
+    description: Optional[str] = field(init=False, hash=False)
     location: Location
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
-    serialisable: bool = field(default=False, init=False)
+    serialisable: bool = field(default=False, init=False, hash=False)
 
     function: Callable[..., Any] = field(repr=False)
 
     def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = f"{self.parent_name}:{self.namespace}.{self.function.__name__}"
         self.description = self.function.__doc__
+        super().__post_init__(*_args, **_kwargs)
 
 
 ##############################################################################
 # Callbacks
 ##############################################################################
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Callback(Data):
-    name: str = field(init=False)
-    description: Optional[str] = field(init=False)
+    name: str = field(init=False, hash=False)
+    description: Optional[str] = field(init=False, hash=False)
     location: Location
     parent_name: FileName
-    parent_type: type[File] = field(default=File, init=False)
-    serialisable: bool = field(default=False, init=False)
+    parent_type: type[File] = field(default=File, init=False, hash=False)
+    serialisable: bool = field(default=False, init=False, hash=False)
 
     event_code: EventCode
     function: Callable[..., Any] = field(repr=False)
 
     def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = f"{self.parent_name}:{self.function.__name__}"
         self.description = self.function.__doc__
+        super().__post_init__(*_args, **_kwargs)
 
 
 CallbackVar = TypeVar("CallbackVar", bound=Callback)
 
 ##############################################################################
 # Commands
 ##############################################################################
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Command(GroupData):
     rule: Rule
     script: Script
 
-    name: str = field(init=False)
+    name: str = field(init=False, hash=False)
     description: Optional[str]
     location: Location
     parent_name: ContextName
-    parent_type: type[Context] = field(default=Context, init=False)
-    serialisable: bool = field(default=True, init=False)
+    parent_type: type[Context] = field(default=Context, init=False, hash=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = rule_name(self.rule)
+        super().__post_init__(*_args, **_kwargs)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "Command":
         return Command(
             rule=field_rule(value),
             script=field_script(value),
             description=field_description(value),
@@ -395,25 +446,25 @@
         context["object_name"] = str(value.get("name", None))
     return parse_optfield(
         "function_signature", partial(parse_signature, context=context)
     )(value)
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Action(GroupDataHasFunction):
     function_name: Optional[FunctionName]
     function_signature: Optional[Signature]
 
     name: ActionName
     description: Optional[str]
     location: Union[Literal["builtin"], Location]
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
-    serialisable: bool = field(default=True, init=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "Action":
         return Action(
             function_name=None,
             function_signature=field_action_function_signature(value),
             name=field_name(value),
@@ -445,26 +496,26 @@
         context["object_name"] = str(value.get("name", None))
     return parse_optfield(
         "function_signature", partial(parse_signature, context=context)
     )(value)
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Capture(GroupDataHasFunction):
     rule: Rule
     function_name: Optional[FunctionName]
     function_signature: Optional[Signature]
 
     name: CaptureName
     description: Optional[str]
     location: Union[Literal["builtin"], Location]
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
-    serialisable: bool = field(default=True, init=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "Capture":
         return Capture(
             rule=field_rule(value),
             function_name=None,
             function_signature=field_capture_function_signature(value),
@@ -485,37 +536,38 @@
             "location": asdict_location(self.location),
             "parent_name": self.parent_name,
             "parent_type": self.parent_type.__name__,
         }
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class List(GroupData):
     value: Optional[ListValue]
     value_type_hint: Optional[type[Any]]
 
     name: ListName
     description: Optional[str]
     location: Union[None, Literal["builtin"], Location]
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
-    serialisable: bool = field(default=True, init=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         if isinstance(self.value, Mapping):
             self.value = dict(self.value)
-        elif isinstance(self.value, Sequence):
+        elif isinstance(self.value, Iterable):
             self.value = list(self.value)
         else:
             if type(self.value).__name__ != "ObjectShim" and self.value is not None:
                 _LOGGER.warning(  # type: ignore[unreachable]
                     f"List value for {self.name} should be list or dict, found {type(self.value)}"
                 )
             self.value = None
+        super().__post_init__(*_args, **_kwargs)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "List":
         return List(
             value=field_list_value(value),
             value_type_hint=field_value_type_hint(value),
             name=field_name(value),
@@ -534,25 +586,25 @@
             "location": asdict_opt(asdict_location)(self.location),
             "parent_name": self.parent_name,
             "parent_type": self.parent_type.__name__,
         }
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Setting(GroupData):
     value: Optional[SettingValue]
     value_type_hint: Optional[type[Any]]
 
     name: SettingName
     description: Optional[str]
     location: Union[None, Literal["builtin"], Location]
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
-    serialisable: bool = field(default=True, init=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "Setting":
         return Setting(
             value=field_setting_value(value),
             value_type_hint=field_value_type_hint(value),
             name=field_name(value),
@@ -571,22 +623,22 @@
             "location": asdict_opt(asdict_location)(self.location),
             "parent_name": self.parent_name,
             "parent_type": self.parent_type.__name__,
         }
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Mode(SimpleData):
     name: ModeName
     description: Optional[str]
     location: Union[None, Literal["builtin"], Location]
     parent_name: ModuleName
-    parent_type: type[Module] = field(default=Module, init=False)
-    serialisable: bool = field(default=True, init=False)
+    parent_type: type[Module] = field(default=Module, init=False, hash=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "Mode":
         return Mode(
             name=field_name(value),
             description=field_description(value),
             location=field_optlocation(value),
@@ -599,22 +651,22 @@
             "description": self.description,
             "location": asdict_opt(asdict_location)(self.location),
             "parent_name": self.parent_name,
         }
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Tag(SimpleData):
     name: TagName
     description: Optional[str]
     location: Union[None, Literal["builtin"], Location]
     parent_name: ModuleName
-    parent_type: type[Module] = field(default=Module, init=False)
-    serialisable: bool = field(default=True, init=False)
+    parent_type: type[Module] = field(default=Module, init=False, hash=False)
+    serialisable: bool = field(default=True, init=False, hash=False)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "Tag":
         return Tag(
             name=field_name(value),
             description=field_description(value),
             location=field_optlocation(value),
```

### Comparing `talondoc-0.6.0/src/talondoc/analysis/registry/data/abc.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from abc import abstractmethod
 from collections.abc import Callable, Mapping, Sequence
 from dataclasses import asdict, dataclass
 from functools import singledispatch
 from inspect import Signature
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Optional, Union
@@ -50,15 +51,15 @@
 
 ##############################################################################
 # Source Locations
 ##############################################################################
 
 
 @final
-@dataclass
+@dataclass(unsafe_hash=True)
 class Location:
     path: Path
     start_line: Optional[int] = None
     start_column: Optional[int] = None
     end_line: Optional[int] = None
     end_column: Optional[int] = None
 
@@ -69,15 +70,20 @@
                 return f"{line}:{column}"
             else:
                 return f"{line}"
         else:
             return None
 
     def __str__(self) -> str:
-        resolved_path = self.path.resolve().relative_to(Path.cwd())
+        resolved_path = self.path.resolve()
+        try:
+            if resolved_path.is_absolute():
+                resolved_path = resolved_path.relative_to(Path.cwd())
+        except ValueError as e:
+            _LOGGER.warning(e)
         start_position = Location._str_from_point(self.start_line, self.start_column)
         if start_position is not None:
             end_position = Location._str_from_point(self.end_line, self.end_column)
             if end_position is not None:
                 return f"{resolved_path}:{start_position}-{end_position}"
             else:
                 return f"{resolved_path}:{start_position}"
@@ -135,29 +141,42 @@
 
 
 ##############################################################################
 # Abstact Data
 ##############################################################################
 
 
-@dataclass
+@dataclass(unsafe_hash=True)
 class Data:
     name: str
     description: Optional[str]
     location: Union[None, Literal["builtin"], "Location"]
     parent_name: Optional[str]
     parent_type: Optional[Union[type[Package], type[File], type[Module], type[Context]]]
     serialisable: bool
 
     @property
     def builtin(self) -> bool:
         return self.name.split(".", maxsplit=2)[0] != "user" and (
             not self.parent_name or self.parent_name.split(".", maxsplit=2)[0] != "user"
         )
 
+    def validate(self) -> None:
+        if re.match(r"^\s+.*", self.name) or re.match(r".*\s+$", self.name):
+            _LOGGER.warning(
+                f"{self.location}: "
+                f"Leading or trailing whitespace "
+                f"in {self.__class__.__name__.lower()} "
+                f"name '{self.name}'"
+            )
+            self.name = self.name.strip()
+
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
+        self.validate()
+
 
 DataVar = TypeVar("DataVar", bound=Data)
 
 
 ##############################################################################
 # Simple Data
 ##############################################################################
@@ -174,15 +193,15 @@
 
 
 ##############################################################################
 # Grouped Data
 ##############################################################################
 
 
-@dataclass
+@dataclass(unsafe_hash=True)
 class GroupData(Data):
     parent_name: str
     parent_type: Union[type[Module], type[Context]]
 
     @classmethod
     @abstractmethod
     def from_dict(cls, value: JsonValue) -> Self:
@@ -215,15 +234,15 @@
 )
 
 ##############################################################################
 # Exceptions
 ##############################################################################
 
 
-@dataclass
+@dataclass(unsafe_hash=True)
 class DuplicateData(Exception):
     """Raised when an entry is defined in multiple modules."""
 
     data: Sequence[Data]
 
     def __str__(self) -> str:
         cls_names = set([data.__class__.__name__ for data in self.data])
@@ -240,15 +259,15 @@
             [
                 f"{cls_names.pop()} '{data_names.pop()}' is declared multiple times:",
                 *[f"- {data.location}" for data in self.data],
             ]
         )
 
 
-@dataclass
+@dataclass(unsafe_hash=True)
 class UnknownReference(Exception):
     """Raised when an entry is defined in multiple modules."""
 
     ref_type: type[Data]
     ref_name: str
 
     location: Optional[str] = None
```

### Comparing `talondoc-0.6.0/src/talondoc/analysis/registry/data/serialise.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/serialise.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/static/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/static/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/static/python/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/static/python/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/analysis/static/python/shims.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/static/python/shims.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import platform
 from collections.abc import Callable, Iterator, Mapping, Sequence
 from io import TextIOWrapper
 from types import ModuleType
 from typing import Any, Optional, Union, cast, overload
 
+import tree_sitter_talon
 from tree_sitter_talon import Point
 
 from ...._util.logging import getLogger
 from ...registry import Registry, data
 from ...registry.data.abc import Location, UnknownReference
 
 _LOGGER = getLogger(__name__)
@@ -200,28 +201,28 @@
 
 
 class TalonContextListsShim(Mapping[str, data.ListValue]):
     def __init__(self, context: "TalonShim.Context"):
         self._context = context
 
     def _add_list_value(self, name: str, value: data.ListValue) -> None:
-        self._context._registry.register(
-            data.List(
-                value=value,
-                value_type_hint=None,
-                # NOTE: list names on contexts are fully qualified
-                name=self._context._registry.resolve_name(
-                    name, package=self._context._package
-                ),
-                description=None,
-                location=self._context._context.location,
-                parent_name=self._context._context.name,
-                parent_type=data.Context,
-            )
+        datum = data.List(
+            value=value,
+            value_type_hint=None,
+            # NOTE: list names on contexts are fully qualified
+            name=self._context._registry.resolve_name(
+                name, package=self._context._package
+            ),
+            description=None,
+            location=self._context._context.location,
+            parent_name=self._context._context.name,
+            parent_type=data.Context,
         )
+        self._context._context.lists.append(datum.name)
+        self._context._registry.register(datum)
 
     def __setitem__(self, name: str, value: data.ListValue) -> None:
         self._add_list_value(name, value)
 
     def update(self, values: Mapping[str, data.ListValue]) -> None:
         for name, value in values.items():
             self._add_list_value(name, value)
@@ -237,28 +238,28 @@
 
 
 class TalonContextSettingsShim(Mapping[str, data.SettingValue]):
     def __init__(self, context: "TalonShim.Context"):
         self._context = context
 
     def _add_setting_value(self, name: str, value: data.SettingValue) -> None:
-        self._context._registry.register(
-            data.Setting(
-                value=value,
-                value_type_hint=None,
-                # NOTE: setting names on contexts are fully qualified
-                name=self._context._registry.resolve_name(
-                    name, package=self._context._package
-                ),
-                description=None,
-                location=self._context._context.location,
-                parent_name=self._context._context.name,
-                parent_type=data.Context,
-            )
+        datum = data.Setting(
+            value=value,
+            value_type_hint=None,
+            # NOTE: setting names on contexts are fully qualified
+            name=self._context._registry.resolve_name(
+                name, package=self._context._package
+            ),
+            description=None,
+            location=self._context._context.location,
+            parent_name=self._context._context.name,
+            parent_type=data.Context,
         )
+        self._context._context.settings.append(datum.name)
+        self._context._registry.register(datum)
 
     def __setitem__(self, name: str, value: data.SettingValue) -> None:
         self._add_setting_value(name, value)
 
     def update(self, values: Mapping[str, data.SettingValue]) -> None:
         for name, value in values.items():
             self._add_setting_value(name, value)
@@ -332,15 +333,15 @@
 
     class Module(ObjectShim):
         def __init__(self, desc: Optional[str] = None) -> None:
             self._registry = Registry.get_active_global_registry()
             self._package = self._registry.get_active_package()
             self._file = self._registry.get_active_file()
             self._module = data.Module(
-                index=len(self._file.modules),
+                index=len(self._file.modules) + 1,
                 description=desc,
                 location=self._file.location,
                 parent_name=self._file.name,
             )
             self._file.modules.append(self._module.name)
             self._registry.register(self._module)
 
@@ -352,24 +353,25 @@
                     namespace=package.name,
                     function=func,
                     location=Location.from_function(func),
                     parent_name=self._module.name,
                     parent_type=data.Module,
                 )
                 self._registry.register(function)
-                action = data.Action(
+                datum = data.Action(
                     function_name=function.name,
                     function_signature=inspect.signature(func),
                     name=f"{package.name}.{name}",
                     description=func.__doc__,
                     location=function.location,
                     parent_name=self._module.name,
                     parent_type=data.Module,
                 )
-                self._registry.register(action)
+                self._module.actions.append(datum.name)
+                self._registry.register(datum)
             return cls
 
         def action(self, name: str) -> Optional[Callable[..., Any]]:
             function = self._registry.lookup_default_function(data.Action, name)
             return function or ObjectShim()
 
         def capture(
@@ -382,119 +384,130 @@
                     namespace=package.name,
                     function=func,
                     location=Location.from_function(func),
                     parent_name=self._module.name,
                     parent_type=data.Module,
                 )
                 self._registry.register(function)
-                capture = data.Capture(
+                datum = data.Capture(
                     rule=data.parse_rule(rule),
                     function_name=function.name,
                     function_signature=inspect.signature(func),
                     name=f"{package.name}.{func.__name__}",
                     description=func.__doc__,
                     location=function.location,
                     parent_name=self._module.name,
                     parent_type=data.Module,
                 )
-                self._registry.register(capture)
+                self._module.captures.append(datum.name)
+                self._registry.register(datum)
                 return func
 
             return __decorator
 
         def setting(
             self,
             name: str,
             type: type,
             default: data.SettingValue = None,
             desc: Optional[str] = None,
         ) -> None:
-            self._registry.register(
-                data.Setting(
-                    value=default,
-                    value_type_hint=type,
-                    # NOTE: list names passed to modules are unqualified
-                    name=f"{self._package.name}.{name}",
-                    description=desc,
-                    location=self._module.location,
-                    parent_name=self._module.name,
-                    parent_type=data.Module,
-                )
+            datum = data.Setting(
+                value=default,
+                value_type_hint=type,
+                # NOTE: list names passed to modules are unqualified
+                name=f"{self._package.name}.{name}",
+                description=desc,
+                location=self._module.location,
+                parent_name=self._module.name,
+                parent_type=data.Module,
             )
+            self._module.settings.append(datum.name)
+            self._registry.register(datum)
 
         def list(
             self,
             name: str,
             desc: Optional[str] = None,
         ) -> None:
-            self._registry.register(
-                data.List(
-                    value=None,
-                    value_type_hint=None,
-                    # NOTE: list names passed to modules are unqualified
-                    name=f"{self._package.name}.{name}",
-                    description=desc,
-                    location=self._module.location,
-                    parent_name=self._module.name,
-                    parent_type=data.Module,
-                )
+            datum = data.List(
+                value=None,
+                value_type_hint=None,
+                # NOTE: list names passed to modules are unqualified
+                name=f"{self._package.name}.{name}",
+                description=desc,
+                location=self._module.location,
+                parent_name=self._module.name,
+                parent_type=data.Module,
             )
+            self._module.lists.append(datum.name)
+            self._registry.register(datum)
 
         def mode(
             self,
             name: str,
             desc: Optional[str] = None,
         ) -> None:
-            self._registry.register(
-                data.Mode(
-                    name=f"{self._package.name}.{name}",
-                    description=desc,
-                    location=self._module.location,
-                    parent_name=self._module.name,
-                )
+            datum = data.Mode(
+                name=f"{self._package.name}.{name}",
+                description=desc,
+                location=self._module.location,
+                parent_name=self._module.name,
             )
+            self._module.modes.append(datum.name)
+            self._registry.register(datum)
 
         def tag(
             self,
             name: str,
             desc: Optional[str] = None,
         ) -> None:
-            self._registry.register(
-                data.Tag(
-                    name=f"{self._package.name}.{name}",
-                    description=desc,
-                    location=self._module.location,
-                    parent_name=self._module.name,
-                )
+            datum = data.Tag(
+                name=f"{self._package.name}.{name}",
+                description=desc,
+                location=self._module.location,
+                parent_name=self._module.name,
             )
+            self._module.tags.append(datum.name)
+            self._registry.register(datum)
 
         # TODO: apps
         # TODO: scope
 
     class Context(ObjectShim):
         def __init__(self, desc: Optional[str] = None) -> None:
             self._registry = Registry.get_active_global_registry()
             self._package = self._registry.get_active_package()
             self._file = self._registry.get_active_file()
             self._context = data.Context(
                 matches=[],
-                index=len(self._file.contexts),
+                index=len(self._file.contexts) + 1,
                 description=desc,
                 location=self._file.location,
                 parent_name=self._file.name,
             )
             self._file.contexts.append(self._context.name)
             self._registry.register(self._context)
             self._lists = TalonContextListsShim(self)
             self._settings = TalonContextSettingsShim(self)
             self._tags = TalonContextTagsShim(self)
-            # TODO: matches
             # TODO: apps
 
         @property
+        def matches(self) -> str:
+            return "\n".join(match.text for match in self._context.matches)
+
+        @matches.setter
+        def matches(self, matches: str) -> None:
+            try:
+                self._context.matches.extend(data.parse_matches(matches))
+            except tree_sitter_talon.ParseError as e:
+                _LOGGER.error(f"Could not parse matches:\n{matches}\n: {e}")
+
+        @property
         def lists(self) -> Mapping[str, data.ListValue]:
             return self._lists
 
         @lists.setter
         def lists(self, lists: Mapping[str, data.ListValue]) -> None:
             self._lists.update(lists)
 
@@ -525,25 +538,26 @@
                         namespace=namespace,
                         function=func,
                         location=location,
                         parent_name=self._context.name,
                         parent_type=data.Context,
                     )
                     self._registry.register(function)
-                    action = data.Action(
+                    datum = data.Action(
                         function_name=function.name,
                         function_signature=inspect.signature(func),
                         # NOTE: function names on action classes are unqualified
                         name=f"{namespace}.{name}",
                         description=func.__doc__,
                         location=location,
                         parent_name=self._context.name,
                         parent_type=data.Context,
                     )
-                    self._registry.register(action)
+                    self._context.actions.append(datum.name)
+                    self._registry.register(datum)
                 return cls
 
             return __decorator
 
         def action(
             self, name: str
         ) -> Optional[Callable[[Callable[..., Any]], Callable[..., Any]]]:
@@ -557,43 +571,44 @@
                     namespace=namespace,
                     function=func,
                     location=location,
                     parent_name=self._context.name,
                     parent_type=data.Context,
                 )
                 self._registry.register(function)
-                action = data.Action(
+                datum = data.Action(
                     function_name=function.name,
                     function_signature=inspect.signature(func),
                     # NOTE: function names on actions are fully qualified
                     name=name,
                     description=func.__doc__,
                     location=location,
                     parent_name=self._context.name,
                     parent_type=data.Context,
                 )
-                self._registry.register(action)
+                self._context.actions.append(datum.name)
+                self._registry.register(datum)
                 return func
 
             return __decorator
 
         def capture(
             self, name: Optional[str] = None, rule: Optional[str] = None
         ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
             def __decorator(func: Callable[..., Any]) -> Callable[..., Any]:
                 # LINT: check if decorated function is a function
                 if not inspect.isfunction(func):
-                    _LOGGER.error(f"decorated object is not a function")
+                    _LOGGER.error(f"Decorated object is not a function.")
                     return func
 
                 location = Location.from_function(func)
 
                 # LINT: check if rule is set
                 if rule is None:
-                    _LOGGER.error(f"missing capture rule at {location}")
+                    _LOGGER.error(f"Missing capture rule at {location}.")
                     # insert placeholder rule
                     parsed_rule = data.Rule(
                         text="",
                         type_name="rule",
                         start_position=Point(-1, -1),
                         end_position=Point(-1, -1),
                         children=[],
@@ -612,36 +627,37 @@
                             f"at {location} "
                             f"is named {act_funcname} "
                             f"instead of {exp_funcname}"
                         )
                     resolved_name = self._registry.resolve_name(name)
                 else:
                     _LOGGER.error(
-                        f"missing name for capture decorator "
+                        f"Missing name for capture decorator "
                         f"applied to {func.__name__} "
-                        f"at {location}"
+                        f"at {location}."
                     )
                     resolved_name = f"{self._package.name}.{func.__name__}"
 
                 function = data.Function(
                     namespace=resolved_name,
                     function=func,
                     location=location,
                     parent_name=self._context.name,
                     parent_type=data.Context,
                 )
                 self._registry.register(function)
-                capture = data.Capture(
+                datum = data.Capture(
                     rule=parsed_rule,
                     # NOTE: capture names passed to contexts are fully qualified
                     name=resolved_name,
                     function_name=function.name,
                     function_signature=None,
                     description=func.__doc__,
                     location=location,
                     parent_name=self._context.name,
                     parent_type=data.Context,
                 )
-                self._registry.register(capture)
+                self._context.captures.append(datum.name)
+                self._registry.register(datum)
                 return func
 
             return __decorator
```

### Comparing `talondoc-0.6.0/src/talondoc/analysis/static/talon.py` & `talondoc-1.0.0rc0/src/talondoc/analysis/static/talon.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,30 +76,27 @@
             )
             context.commands.append(command.name)
             registry.register(command)
         elif isinstance(declaration, TalonSettingsDeclaration):
             # Register settings:
             for statement in declaration.right.children:
                 if isinstance(statement, TalonAssignmentStatement):
-                    registry.register(
-                        data.Setting(
-                            value=statement.right,
-                            value_type_hint=None,
-                            name=statement.left.text,
-                            description=None,
-                            location=Location.from_ast(
-                                context.location.path, statement
-                            ),
-                            parent_name=context.name,
-                            parent_type=data.Context,
-                        )
+                    datum = data.Setting(
+                        value=statement.right,
+                        value_type_hint=None,
+                        name=statement.left.text,
+                        description=None,
+                        location=Location.from_ast(context.location.path, statement),
+                        parent_name=context.name,
+                        parent_type=data.Context,
                     )
+                    context.settings.append(datum.name)
+                    registry.register(datum)
         elif isinstance(declaration, TalonTagImportDeclaration):
-            # Register tag import:
-            # TODO: add use entries
+            # TODO: Register tag import:
             pass
 
 
 def analyse_files(
     registry: Registry,
     paths: Sequence[Path],
     package: data.Package,
```

### Comparing `talondoc-0.6.0/src/talondoc/description/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/description/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/description/describer.py` & `talondoc-1.0.0rc0/src/talondoc/description/describer.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 from sphinx.application import BuildEnvironment, Sphinx
 from typing_extensions import TypeGuard
 
 from .._util.logging import getLogger
 from .._version import __version__
 from ..analysis.registry import NoActiveFile, NoActivePackage, NoActiveRegistry
 from ..analysis.static import analyse_package
+from ._util.addnodes.fragtable import (
+    depart_fragtable,
+    depart_fragtable_html,
+    fragtable,
+    visit_fragtable,
+    visit_fragtable_html,
+)
 from .domains import TalonDomain
 from .typing import TalonPackage
 
 _LOGGER = getLogger(__name__)
 
 
 def _is_talon_package(talon_package: Any) -> TypeGuard[TalonPackage]:
@@ -136,16 +143,26 @@
             except NoActiveFile as e:
                 _LOGGER.exception(e)
     except Exception as e:
         _LOGGER.exception(e)
 
 
 def setup(app: Sphinx) -> dict[str, Any]:
+    # Add fragmenting table nodes
+    app.add_node(
+        fragtable,
+        html=(visit_fragtable_html, depart_fragtable_html),
+        latex=(visit_fragtable, depart_fragtable),
+        text=(visit_fragtable, depart_fragtable),
+    )
+
+    # Add the Talon domain
     app.add_domain(TalonDomain)
 
+    # Add the TalonDoc configuration options
     app.add_config_value(
         name="talon_docstring_hook",
         default=None,
         rebuild="env",
         types=[
             Callable,  # _TalonDocstringHook_Callable
             dict,  # _TalonDocstringHook_Dict
@@ -168,14 +185,15 @@
         rebuild="env",
         types=[
             list,  # list[TalonPackage]
             tuple,  # Tuple[TalonPackage]
         ],
     )
 
+    # Add the hook to load any Talon packages
     app.connect("env-before-read-docs", _talondoc_load_package)
 
     return {
         "version": __version__,
         "parallel_read_safe": False,
         "parallel_write_safe": False,
     }
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, Optional, cast
 
 import sphinx.directives
-from docutils import nodes
-from sphinx import addnodes
-from talonfmt import talonfmt
-from typing_extensions import final
-
-from ...analysis.registry import data
 
 if TYPE_CHECKING:
     from ..domains import TalonDomain
 else:
     TalonDomain = Any
 
 
@@ -47,11 +41,7 @@
             return __docstring_hook
 
 
 class TalonDocObjectDescription(
     sphinx.directives.ObjectDescription[str], TalonDocDirective  # type: ignore[misc]
 ):
     pass
-
-    @final
-    def describe_rule(self, rule: data.Rule) -> nodes.Text:
-        return nodes.Text(talonfmt(rule, safe=False))
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/action.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/action.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from docutils import nodes
 from sphinx import addnodes
 from typing_extensions import override
 
 from ..._util.logging import getLogger
 from ...analysis.registry import data
 from ...analysis.registry.data.abc import UnknownReference
-from .._util.addnodes import desc_content, desc_name, paragraph
+from .._util.addnodes import desc_content, desc_qualname, desc_signature, paragraph
 from . import TalonDocObjectDescription
 
 _LOGGER = getLogger(__name__)
 
 
 class TalonActionDirective(TalonDocObjectDescription):
     has_content = True
@@ -24,21 +24,25 @@
         assert len(self.arguments) == 1
         return [str(self.arguments[0]).strip()]
 
     @override
     def handle_signature(self, sig: str, signode: addnodes.desc_signature) -> str:
         default = self.talon.registry.lookup_default(data.Action, sig)
         if default:
-            signature = default.function_signature or inspect.Signature()
-            signode += desc_name(nodes.Text(default.name + str(signature)))
+            # Add the action name:
+            desc_qualname(signode, default.name)
+
+            # Add the action type signature:
+            desc_signature(signode, default.function_signature or inspect.Signature())
+
             if default.description:
                 signode += desc_content(paragraph(nodes.Text(default.description)))
             return default.name
         else:
             e = UnknownReference(
                 ref_type=data.Action,
                 ref_name=sig,
                 location=self.get_location(),
                 known_references=tuple(self.talon.registry.actions.keys()),
             )
-            _LOGGER.error(e)
+            _LOGGER.error(f"talon:action: {e}")
             raise ValueError(e)
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/command/__init__.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,9 +36,9 @@
                 command,
                 signode,
                 always_include_script=self.always_include_script,
                 docstring_hook=self.docstring_hook,
             )
             return command.name
         except (UnknownReference, AmbiguousSignature) as e:
-            _LOGGER.error(e)
+            _LOGGER.error(f"talon:command: {e}")
             raise ValueError(e)
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/command/abc.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/abc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import re
-from typing import ClassVar, Iterator, Optional, Sequence, cast
+from typing import ClassVar, Iterator, Optional, Sequence, Union, cast
 
 from docutils import nodes
 from sphinx import addnodes
 from talonfmt import talonfmt
 from tree_sitter_talon import TalonComment
-from typing_extensions import final
+from typing_extensions import Literal, final
 
 from ...._util.logging import getLogger
 from ....analysis.registry import data
 from ....analysis.registry.data.abc import UnknownReference
 from ....description import InvalidInterpolation
 from ....description.describer import TalonScriptDescriber
 from ....sphinx.directives import TalonDocObjectDescription
 from ....sphinx.typing import TalonDocstringHook_Callable
 from ..._util.addnodes import desc_content, desc_name, paragraph
+from ..._util.addnodes.rule import desc_rule
 from ..errors import AmbiguousSignature
 
 _LOGGER = getLogger(__name__)
 
 
 class TalonDocCommandDescription(TalonDocObjectDescription):
     @property
@@ -92,15 +93,15 @@
         self,
         command: data.Command,
         signode: addnodes.desc_signature,
         *,
         always_include_script: bool,
         docstring_hook: Optional[TalonDocstringHook_Callable],
     ) -> addnodes.desc_signature:
-        signode += desc_name(self.describe_rule(command.rule))
+        signode += desc_name(desc_rule(command.rule))
         signode += desc_content(
             *self.describe_script(
                 command,
                 always_include_script=always_include_script,
                 docstring_hook=docstring_hook,
             )
         )
@@ -195,30 +196,42 @@
 class TalonDocCommandListDescription(TalonDocCommandDescription):
     @property
     def caption(self) -> str:
         # Get caption from options or from file name
         return cast(str, self.options.get("caption", None) or ".".join(self.arguments))
 
     @property
-    def include(self) -> Sequence[Sequence[str]]:
-        return tuple(
-            self._split_phrase(phrase) for phrase in self.options.get("include", ())
+    def include(self) -> Union[Literal["*"], Sequence[Sequence[str]]]:
+        phrases = cast(
+            Union[Literal["*"], Sequence[str]], self.options.get("include", "*")
         )
+        if (
+            phrases == "*"
+            or len(phrases) == 0
+            or (len(phrases) == 1 and phrases[0] == "*")
+        ):
+            return "*"
+        else:
+            return tuple(map(self._split_phrase, phrases))
 
     @property
     def exclude(self) -> Sequence[Sequence[str]]:
         return tuple(
             self._split_phrase(phrase) for phrase in self.options.get("exclude", ())
         )
 
     @property
     def columns(self) -> int:
         return cast(int, self.options.get("columns", 2))
 
     @property
+    def width(self) -> Optional[int]:
+        return cast(Optional[int], self.options.get("width", None))
+
+    @property
     def commands(self) -> Iterator[data.Command]:
         for command in self.get_commands(restrict_to=self.contexts):
             if self._should_include(command.rule):
                 yield command
 
     def _should_include(
         self,
@@ -239,15 +252,20 @@
     @final
     def _matches_include(
         self,
         rule: data.Rule,
         *,
         fullmatch: bool = False,
     ) -> bool:
-        return self._match_any_of(rule, self.include, default=True, fullmatch=fullmatch)
+        if self.include == "*":
+            return True
+        else:
+            return self._match_any_of(
+                rule, self.include, default=True, fullmatch=fullmatch
+            )
 
     @final
     def _matches_exclude(
         self,
         rule: data.Rule,
         *,
         fullmatch: bool = False,
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/command/hlist.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/hlist.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/command/table.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import sys
 
 from docutils import nodes
 from sphinx.util.typing import OptionSpec
 
 from ...._util.logging import getLogger
-from ..._util.addnodes import colspec, entry, row, table, tbody, tgroup, title
-from ..._util.typing import flag, optional_str, optional_strlist
+from ..._util.addnodes import (
+    colspec,
+    entry,
+    fragtable,
+    row,
+    table,
+    tbody,
+    tgroup,
+    title,
+)
+from ..._util.addnodes.rule import desc_rule
+from ..._util.typing import flag, optional_int, optional_str, optional_strlist
 from .abc import TalonDocCommandListDescription
 
 _LOGGER = getLogger(__name__)
 
 
 class TalonCommandTableDirective(TalonDocCommandListDescription):
     has_content = False
@@ -18,35 +28,37 @@
     option_spec: OptionSpec = {
         "context": optional_strlist,
         "contexts": optional_strlist,
         "always_include_script": flag,
         "caption": optional_str,
         "include": optional_strlist,
         "exclude": optional_strlist,
+        "width": optional_int,
     }
     final_argument_whitespace = False
 
     def run(self) -> list[nodes.Node]:
         return [
-            table(
+            fragtable(
                 title(nodes.Text(self.caption)),
                 tgroup(
                     colspec(colwidth=1),
                     colspec(colwidth=1),
                     tbody(
                         row(
-                            entry(self.describe_rule(command.rule)),
+                            entry(desc_rule(command.rule)),
                             entry(
                                 *self.describe_script(
                                     command,
                                     always_include_script=self.always_include_script,
                                     docstring_hook=self.docstring_hook,
                                 )
                             ),
                         )
                         for command in self.commands
                     ),
                     cols=2,
                 ),
                 classes="compact",
+                width=self.width,
             )
         ]
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/errors.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/errors.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/list.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/tag.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from docutils import nodes
 from sphinx import addnodes
 from typing_extensions import override
 
+from talondoc.analysis.registry.data.abc import UnknownReference
+
 from ..._util.logging import getLogger
 from ...analysis.registry import data
-from ...analysis.registry.data.abc import UnknownReference
-from .._util.addnodes import desc_content, desc_name, paragraph
+from .._util.addnodes import desc_content, desc_name, desc_qualname, paragraph
 from . import TalonDocObjectDescription
 
 _LOGGER = getLogger(__name__)
 
 
-class TalonListDirective(TalonDocObjectDescription):
+class TalonTagDirective(TalonDocObjectDescription):
     has_content = True
     required_arguments = 1
     optional_arguments = 0
     final_argument_whitespace = False
 
     @override
     def get_signatures(self) -> list[str]:
         assert len(self.arguments) == 1
         return [str(self.arguments[0]).strip()]
 
     @override
     def handle_signature(self, sig: str, signode: addnodes.desc_signature) -> str:
-        default = self.talon.registry.lookup_default(data.List, sig)
-        if default:
-            signode += desc_name(nodes.Text(default.name))
-            if default.description:
-                signode += desc_content(paragraph(nodes.Text(default.description)))
-            return default.name
+        tag = self.talon.registry.lookup(data.Tag, sig)
+        if tag:
+            desc_qualname(signode, tag.name)
+            if tag.description:
+                signode += desc_content(paragraph(nodes.Text(tag.description)))
+            return tag.name
         else:
             e = UnknownReference(
-                ref_type=data.List,
+                ref_type=data.Tag,
                 ref_name=sig,
                 location=self.get_location(),
-                known_references=tuple(self.talon.registry.lists.keys()),
+                known_references=tuple(self.talon.registry.tags.keys()),
             )
-            _LOGGER.error(e)
+            _LOGGER.error(f"talon:tag: {e}")
             raise ValueError(e)
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/mode.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/mode.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from docutils import nodes
 from sphinx import addnodes
 from typing_extensions import override
 
 from ..._util.logging import getLogger
 from ...analysis.registry import data
 from ...analysis.registry.data.abc import UnknownReference
-from .._util.addnodes import desc_content, desc_name, paragraph
+from .._util.addnodes import desc_content, desc_name, desc_qualname, paragraph
 from . import TalonDocObjectDescription
 
 _LOGGER = getLogger(__name__)
 
 
 class TalonModeDirective(TalonDocObjectDescription):
     has_content = True
@@ -22,20 +22,20 @@
         assert len(self.arguments) == 1
         return [str(self.arguments[0]).strip()]
 
     @override
     def handle_signature(self, sig: str, signode: addnodes.desc_signature) -> str:
         mode = self.talon.registry.lookup(data.Mode, sig)
         if mode:
-            signode += desc_name(nodes.Text(mode.name))
+            desc_qualname(signode, mode.name)
             if mode.description:
                 signode += desc_content(paragraph(nodes.Text(mode.description)))
             return mode.name
         else:
             e = UnknownReference(
                 ref_type=data.Mode,
                 ref_name=sig,
                 location=self.get_location(),
                 known_references=tuple(self.talon.registry.modes.keys()),
             )
-            _LOGGER.error(e)
+            _LOGGER.error(f"talon:mode: {e}")
             raise ValueError(e)
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/directives/setting.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/capture.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,66 @@
+from inspect import Signature
+
 from docutils import nodes
 from sphinx import addnodes
 from typing_extensions import override
 
 from ..._util.logging import getLogger
 from ...analysis.registry import data
 from ...analysis.registry.data.abc import UnknownReference
-from .._util.addnodes import desc_content, desc_name, paragraph
+from .._util.addnodes import (
+    desc_content,
+    desc_qualname,
+    desc_sig_operator,
+    desc_sig_space,
+    desc_type,
+    paragraph,
+)
+from .._util.addnodes.rule import desc_rule
 from . import TalonDocObjectDescription
 
 _LOGGER = getLogger(__name__)
 
 
-class TalonSettingDirective(TalonDocObjectDescription):
+class TalonCaptureDirective(TalonDocObjectDescription):
     has_content = True
     required_arguments = 1
     optional_arguments = 0
     final_argument_whitespace = False
 
     @override
     def get_signatures(self) -> list[str]:
         assert len(self.arguments) == 1
         return [str(self.arguments[0]).strip()]
 
     @override
     def handle_signature(self, sig: str, signode: addnodes.desc_signature) -> str:
-        default = self.talon.registry.lookup_default(data.Setting, sig)
+        default = self.talon.registry.lookup_default(data.Capture, sig)
         if default:
-            signode += desc_name(nodes.Text(default.name))
+            desc_qualname(signode, default.name)
+
+            # Add the return type
+            if (
+                default.function_signature
+                and default.function_signature.return_annotation is not Signature.empty
+            ):
+                signode += desc_sig_operator(nodes.Text(":"))
+                signode += desc_sig_space()
+                signode += desc_type(default.function_signature.return_annotation)
+
+            # Add the rule
+            signode += desc_content(desc_rule(default.rule))
+
+            # Add the description
             if default.description:
                 signode += desc_content(paragraph(nodes.Text(default.description)))
+
             return default.name
         else:
             e = UnknownReference(
-                ref_type=data.Setting,
+                ref_type=data.Capture,
                 ref_name=sig,
                 location=self.get_location(),
-                known_references=tuple(self.talon.registry.settings.keys()),
+                known_references=tuple(self.talon.registry.captures.keys()),
             )
-            _LOGGER.error(e)
+            _LOGGER.error(f"talon:capture: {e}")
             raise ValueError(e)
```

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/domains.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/domains.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc/sphinx/typing.py` & `talondoc-1.0.0rc0/src/talondoc/sphinx/typing.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.6.0/src/talondoc.egg-info/PKG-INFO` & `talondoc-1.0.0rc0/src/talondoc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 0.6.0
+Version: 1.0.0rc0
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-0.6.0/src/talondoc.egg-info/SOURCES.txt` & `talondoc-1.0.0rc0/src/talondoc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/talondoc/_autogen/resources/python_file.md.jinja2
 src/talondoc/_autogen/resources/python_file.rst.jinja2
 src/talondoc/_autogen/resources/talon_file.md.jinja2
 src/talondoc/_autogen/resources/talon_file.rst.jinja2
 src/talondoc/_cache_builtin/__init__.py
 src/talondoc/_cache_builtin/resources/talon.json
 src/talondoc/_util/__init__.py
+src/talondoc/_util/builtin.py
 src/talondoc/_util/io.py
 src/talondoc/_util/logging.py
 src/talondoc/_util/progress_bar.py
 src/talondoc/analysis/__init__.py
 src/talondoc/analysis/live/__init__.py
 src/talondoc/analysis/live/resources/get_actions.py
 src/talondoc/analysis/live/resources/get_captures.py
@@ -44,16 +45,18 @@
 src/talondoc/analysis/static/python/__init__.py
 src/talondoc/analysis/static/python/shims.py
 src/talondoc/description/__init__.py
 src/talondoc/description/describer.py
 src/talondoc/sphinx/__init__.py
 src/talondoc/sphinx/domains.py
 src/talondoc/sphinx/typing.py
-src/talondoc/sphinx/_util/addnodes.py
 src/talondoc/sphinx/_util/typing.py
+src/talondoc/sphinx/_util/addnodes/__init__.py
+src/talondoc/sphinx/_util/addnodes/fragtable.py
+src/talondoc/sphinx/_util/addnodes/rule.py
 src/talondoc/sphinx/directives/__init__.py
 src/talondoc/sphinx/directives/action.py
 src/talondoc/sphinx/directives/capture.py
 src/talondoc/sphinx/directives/errors.py
 src/talondoc/sphinx/directives/list.py
 src/talondoc/sphinx/directives/mode.py
 src/talondoc/sphinx/directives/setting.py
```

### Comparing `talondoc-0.6.0/src/talondoc.egg-info/requires.txt` & `talondoc-1.0.0rc0/src/talondoc.egg-info/requires.txt`

 * *Files identical despite different names*

