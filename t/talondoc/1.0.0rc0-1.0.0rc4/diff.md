# Comparing `tmp/talondoc-1.0.0rc0.tar.gz` & `tmp/talondoc-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talondoc-1.0.0rc0.tar", last modified: Mon May 22 22:42:11 2023, max compression
+gzip compressed data, was "talondoc-1.0.0rc4.tar", last modified: Tue May 23 12:57:30 2023, max compression
```

## Comparing `talondoc-1.0.0rc0.tar` & `talondoc-1.0.0rc4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.612201 talondoc-1.0.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.616201 talondoc-1.0.0rc0/src/talondoc/
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.616201 talondoc-1.0.0rc0/src/talondoc/_autogen/
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/conf.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/index.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/index.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/python_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/python_file.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/talon_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_autogen/resources/talon_file.rst.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    38478 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_cache_builtin/resources/talon.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_util/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/live/
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.620201 talondoc-1.0.0rc0/src/talondoc/analysis/registry/
--rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/serialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/analysis/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/analysis/static/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22422 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/python/shims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/analysis/static/talon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/description/
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/description/describer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/fragtable.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/_util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.624201 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/capture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.628201 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/hlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/directives/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-22 22:41:55.000000 talondoc-1.0.0rc0/src/talondoc/sphinx/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:42:11.616201 talondoc-1.0.0rc0/src/talondoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 22:42:11.000000 talondoc-1.0.0rc0/src/talondoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/talondoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/talondoc/_autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/conf.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/index.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/index.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/talon_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/talon_file.rst.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    38478 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/resources/talon.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/live/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)    24349 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/serialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/static/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22430 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/python/shims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/talon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/description/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/description/describer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/fragtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/capture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/hlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/talondoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/top_level.txt
```

### Comparing `talondoc-1.0.0rc0/PKG-INFO` & `talondoc-1.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 1.0.0rc0
+Version: 1.0.0rc4
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-1.0.0rc0/README.md` & `talondoc-1.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/pyproject.toml` & `talondoc-1.0.0rc4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talondoc"
-version = "1.0.0rc0"
+version = "1.0.0rc4"
 description = "A Sphinx extension for Talon user directories."
 license = { file = 'LICENSE' }
 authors = [{ name = "Wen Kokke", email = "wenkokke@users.noreply.github.com" }]
 readme = "README.md"
 keywords = ["talon", "sphinx"]
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -96,32 +96,30 @@
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py39, py39-md, py310, py310-md, py311, py311-md
 isolated_build = true
 
 [testenv]
-allowlist_externals = cp, mkdir, sh, rm
+allowlist_externals = cp, mkdir, rm
 extras =
   test
 setenv =
   TALONDOC_STRICT = 1
 commands_pre =
-  cp '{tox_root}/example/autogen.sh' '{env_tmp_dir}/autogen.sh'
   cp -R '{tox_root}/example/knausj_talon' '{env_tmp_dir}/knausj_talon'
   mkdir -p '{env_tmp_dir}/docs'
   cp '{tox_root}/example/docs/conf.py' '{env_tmp_dir}/docs/conf.py'
   cp '{tox_root}/example/docs/index.md' '{env_tmp_dir}/docs/index.md'
   cp -R '{tox_root}/example/docs/_static' '{env_tmp_dir}/docs/_static'
 commands =
   {envpython} -m bumpver update --patch --no-fetch --dry
-  sh '{env_tmp_dir}/autogen.sh'
-  {envpython} -m talondoc build '{env_tmp_dir}/docs' '{env_tmp_dir}/docs/_build'
+  {envpython} -X utf8 -m talondoc autogen '{env_tmp_dir}/docs' -o 'knausj_talon' --generate-index
+  {envpython} -X utf8 -m talondoc build '{env_tmp_dir}/docs' '{env_tmp_dir}/docs/_build'
 commands_post =
-  rm -f '{env_tmp_dir}/autogen.sh'
   rm -rf '{env_tmp_dir}/knausj_talon'
   rm -f '{env_tmp_dir}/docs/conf.py'
   rm -f '{env_tmp_dir}/docs/index.md'
   rm -rf '{env_tmp_dir}/docs/_static'
 
 [testenv:py39-md]
 setenv =
```

### Comparing `talondoc-1.0.0rc0/src/talondoc/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 import os
 import socket
 import threading
 import webbrowser
 from http.server import HTTPServer, SimpleHTTPRequestHandler, ThreadingHTTPServer
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Optional, Sequence
 
 import click
 from typing_extensions import Literal
 
 from ._autogen import autogen
 from ._cache_builtin import cache_builtin
 from ._util import logging
@@ -51,56 +51,49 @@
 
 ################################################################################
 # TalonDoc CLI - Autogen
 ################################################################################
 
 
 @talondoc.command(name="autogen")
+@click.argument("config_dir", type=click.Path(), default=os.path.curdir)
+@click.option("-o", "--output-dir", type=click.Path())
 @click.option(
     "--package-name",
     type=str,
     default=None,
 )
 @click.option(
     "--package-dir",
     type=click.Path(),
-    required=True,
-)
-@click.option(
-    "-o",
-    "--output-dir",
-    type=click.Path(),
-)
-@click.option(
-    "--sphinx-root",
-    type=click.Path(),
+    default=None,
 )
 @click.option(
     "-t",
     "--template-dir",
     type=click.Path(),
     default=None,
 )
 @click.option(
     "--include",
     type=click.Path(),
     multiple=True,
-    default=[],
+    default=None,
 )
 @click.option(
     "--exclude",
     type=click.Path(),
     multiple=True,
-    default=[],
+    default=None,
 )
 @click.option(
     "--trigger",
     type=str,
     multiple=True,
-    default=["ready"],
+    default=None,
 )
 @click.option(
     "--project",
     type=str,
     default=None,
 )
 @click.option(
@@ -111,56 +104,56 @@
 @click.option(
     "--release",
     type=str,
     default=None,
 )
 @click.option(
     "--generate-conf/--no-generate-conf",
-    default=True,
+    default=False,
 )
 @click.option(
     "--generate-index/--no-generate-index",
-    default=True,
+    default=False,
 )
 @click.option(
     "--continue-on-error/--no-continue-on-error",
     default=bool(os.environ.get("TALONDOC_STRICT", False)),
 )
 @click.option(
     "--format",
     type=click.Choice(["rst", "md"]),
-    default="rst",
+    default=None,
 )
 def _autogen(
+    config_dir: str,
     *,
-    output_dir: str,
-    sphinx_root: str,
-    template_dir: Optional[str],
-    package_dir: str,
+    output_dir: Optional[str],
+    package_dir: Optional[str],
     package_name: Optional[str],
-    include: list[str],
-    exclude: list[str],
-    trigger: list[str],
+    template_dir: Optional[str],
+    include: Optional[Sequence[str]],
+    exclude: Optional[Sequence[str]],
+    trigger: Optional[Sequence[str]],
     project: Optional[str],
     author: Optional[str],
     release: Optional[str],
     generate_conf: bool,
     generate_index: bool,
     continue_on_error: bool,
-    format: Literal["rst", "md"],
+    format: Optional[Literal["rst", "md"]],
 ) -> None:
     autogen(
-        package_dir,
+        config_dir=config_dir,
         output_dir=output_dir,
-        sphinx_root=sphinx_root,
         template_dir=template_dir,
         package_name=package_name,
-        include=tuple(include),
-        exclude=tuple(exclude),
-        trigger=tuple(trigger),
+        package_dir=package_dir,
+        include=include,
+        exclude=exclude,
+        trigger=trigger,
         project=project,
         author=author,
         release=release,
         generate_conf=generate_conf,
         generate_index=generate_index,
         continue_on_error=continue_on_error,
         format=format,
@@ -179,14 +172,15 @@
     type=click.Path(),
 )
 @click.argument(
     "output_dir",
     type=click.Path(),
 )
 @click.option(
+    "-c",
     "--config-dir",
     type=click.Path(),
     default=None,
 )
 @click.option(
     "--server/--no-server",
     default=False,
```

### Comparing `talondoc-1.0.0rc0/src/talondoc/_autogen/resources/conf.py.jinja2` & `talondoc-1.0.0rc4/src/talondoc/_autogen/resources/conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/_autogen/resources/python_file.md.jinja2` & `talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.md.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/_autogen/resources/python_file.rst.jinja2` & `talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.rst.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/_cache_builtin/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/_cache_builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/_cache_builtin/resources/talon.json` & `talondoc-1.0.0rc4/src/talondoc/_cache_builtin/resources/talon.json`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/_util/io.py` & `talondoc-1.0.0rc4/src/talondoc/_util/io.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/_util/logging.py` & `talondoc-1.0.0rc4/src/talondoc/_util/logging.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/_util/progress_bar.py` & `talondoc-1.0.0rc4/src/talondoc/_util/progress_bar.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/live/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/live/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,95 +117,95 @@
 
     @property
     def actions(self) -> Sequence[data.Action]:
         actions_json = self.eval_resource("get_actions.py")
         try:
             actions_fields = json.loads(actions_json)
         except json.JSONDecodeError as e:
-            _LOGGER.error(e)
+            _LOGGER.warning(e)
             return ()
         return tuple(map(data.Action.from_dict, actions_fields))
 
     @property
     def builtin_actions(self) -> Sequence[data.Action]:
         return tuple(filter(lambda action: action.builtin, self.actions))
 
     @property
     def captures(self) -> Sequence[data.Capture]:
         captures_json = self.eval_resource("get_captures.py")
         try:
             captures_fields = json.loads(captures_json)
         except json.JSONDecodeError as e:
-            _LOGGER.error(e)
+            _LOGGER.warning(e)
             return ()
         return tuple(map(data.Capture.from_dict, captures_fields))
 
     @property
     def builtin_captures(self) -> Sequence[data.Capture]:
         return tuple(filter(lambda capture: capture.builtin, self.captures))
 
     @property
     def commands(self) -> Sequence[data.Command]:
         commands_json = self.eval_resource("get_commands.py")
         try:
             commands_fields = json.loads(commands_json)
         except json.JSONDecodeError as e:
-            _LOGGER.error(e)
+            _LOGGER.warning(e)
             return ()
         return tuple(map(data.Command.from_dict, commands_fields))
 
     @property
     def lists(self) -> Sequence[data.List]:
         lists_json = self.eval_resource("get_lists.py")
         try:
             lists_fields = json.loads(lists_json)
         except json.JSONDecodeError as e:
-            _LOGGER.error(e)
+            _LOGGER.warning(e)
             return ()
         return tuple(map(data.List.from_dict, lists_fields))
 
     @property
     def builtin_lists(self) -> Sequence[data.List]:
         return tuple(filter(lambda list: list.builtin, self.lists))
 
     @property
     def settings(self) -> Sequence[data.Setting]:
         settings_json = self.eval_resource("get_settings.py")
         try:
             settings_fields = json.loads(settings_json)
         except json.JSONDecodeError as e:
-            _LOGGER.error(e)
+            _LOGGER.warning(e)
             return ()
         return tuple(map(data.Setting.from_dict, settings_fields))
 
     @property
     def builtin_settings(self) -> Sequence[data.Setting]:
         return tuple(filter(lambda setting: setting.builtin, self.settings))
 
     @property
     def modes(self) -> Sequence[data.Mode]:
         modes_json = self.eval_resource("get_modes.py")
         try:
             modes_fields = json.loads(modes_json)
         except json.JSONDecodeError as e:
-            _LOGGER.error(e)
+            _LOGGER.warning(e)
             return ()
         return tuple(map(data.Mode.from_dict, modes_fields))
 
     @property
     def builtin_modes(self) -> Sequence[data.Mode]:
         return tuple(filter(lambda mode: mode.builtin, self.modes))
 
     @property
     def tags(self) -> Sequence[data.Tag]:
         tags_json = self.eval_resource("get_tags.py")
         try:
             tags_fields = json.loads(tags_json)
         except json.JSONDecodeError as e:
-            _LOGGER.error(e)
+            _LOGGER.warning(e)
             return ()
         return tuple(map(data.Tag.from_dict, tags_fields))
 
     @property
     def builtin_tags(self) -> Sequence[data.Tag]:
         return tuple(filter(lambda tag: tag.builtin, self.tags))
```

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_actions.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_actions.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_captures.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_captures.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_commands.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_commands.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_lists.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_lists.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/live/resources/get_settings.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_settings.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/registry/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,42 +138,42 @@
         for package in packages:
             if isinstance(package, data.Package):
                 yield package
             else:
                 try:
                     yield self.get(data.Package, package)
                 except UnknownReference as e:
-                    _LOGGER.error(f"resolve_packages: {e}")
+                    _LOGGER.warning(f"resolve_packages: {e}")
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
-                    _LOGGER.error(f"resolve_files: {e}")
+                    _LOGGER.warning(f"resolve_files: {e}")
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
-                        _LOGGER.error(f"resolve_contexts: {e}")
+                        _LOGGER.warning(f"resolve_contexts: {e}")
                         continue
                 assert isinstance(value, data.File)
                 for context_name in value.contexts:
                     yield self.get(data.Context, context_name, referenced_by=value)
 
     def get_commands(
         self,
```

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/abc.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/abc.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/registry/data/serialise.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/serialise.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/static/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/static/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/static/python/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/static/python/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/static/python/shims.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/static/python/shims.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,15 +497,15 @@
             return "\n".join(match.text for match in self._context.matches)
 
         @matches.setter
         def matches(self, matches: str) -> None:
             try:
                 self._context.matches.extend(data.parse_matches(matches))
             except tree_sitter_talon.ParseError as e:
-                _LOGGER.error(f"Could not parse matches:\n{matches}\n: {e}")
+                _LOGGER.warning(f"Could not parse matches:\n{matches}\n: {e}")
 
         @property
         def lists(self) -> Mapping[str, data.ListValue]:
             return self._lists
 
         @lists.setter
         def lists(self, lists: Mapping[str, data.ListValue]) -> None:
@@ -593,22 +593,22 @@
 
         def capture(
             self, name: Optional[str] = None, rule: Optional[str] = None
         ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
             def __decorator(func: Callable[..., Any]) -> Callable[..., Any]:
                 # LINT: check if decorated function is a function
                 if not inspect.isfunction(func):
-                    _LOGGER.error(f"Decorated object is not a function.")
+                    _LOGGER.warning(f"Decorated object is not a function.")
                     return func
 
                 location = Location.from_function(func)
 
                 # LINT: check if rule is set
                 if rule is None:
-                    _LOGGER.error(f"Missing capture rule at {location}.")
+                    _LOGGER.warning(f"Missing capture rule at {location}.")
                     # insert placeholder rule
                     parsed_rule = data.Rule(
                         text="",
                         type_name="rule",
                         start_position=Point(-1, -1),
                         end_position=Point(-1, -1),
                         children=[],
@@ -626,15 +626,15 @@
                             f"function for capture {name} "
                             f"at {location} "
                             f"is named {act_funcname} "
                             f"instead of {exp_funcname}"
                         )
                     resolved_name = self._registry.resolve_name(name)
                 else:
-                    _LOGGER.error(
+                    _LOGGER.warning(
                         f"Missing name for capture decorator "
                         f"applied to {func.__name__} "
                         f"at {location}."
                     )
                     resolved_name = f"{self._package.name}.{func.__name__}"
 
                 function = data.Function(
```

### Comparing `talondoc-1.0.0rc0/src/talondoc/analysis/static/talon.py` & `talondoc-1.0.0rc4/src/talondoc/analysis/static/talon.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/description/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/description/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/description/describer.py` & `talondoc-1.0.0rc4/src/talondoc/description/describer.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/_util/addnodes/fragtable.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/fragtable.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/_util/typing.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/_util/typing.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/action.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/action.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/capture.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/capture.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/__init__.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/abc.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/abc.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/hlist.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/hlist.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/command/table.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/table.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/errors.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/errors.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/list.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/list.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/mode.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/mode.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/setting.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/setting.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/directives/tag.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/tag.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/domains.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/domains.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc/sphinx/typing.py` & `talondoc-1.0.0rc4/src/talondoc/sphinx/typing.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc.egg-info/PKG-INFO` & `talondoc-1.0.0rc4/src/talondoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 1.0.0rc0
+Version: 1.0.0rc4
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-1.0.0rc0/src/talondoc.egg-info/SOURCES.txt` & `talondoc-1.0.0rc4/src/talondoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc0/src/talondoc.egg-info/requires.txt` & `talondoc-1.0.0rc4/src/talondoc.egg-info/requires.txt`

 * *Files identical despite different names*

