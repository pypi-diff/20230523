# Comparing `tmp/talondoc-1.0.0rc4.tar.gz` & `tmp/talondoc-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talondoc-1.0.0rc4.tar", last modified: Tue May 23 12:57:30 2023, max compression
+gzip compressed data, was "talondoc-1.0.0rc5.tar", last modified: Tue May 23 13:36:35 2023, max compression
```

## Comparing `talondoc-1.0.0rc4.tar` & `talondoc-1.0.0rc5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/talondoc/
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/talondoc/_autogen/
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/conf.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/index.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/index.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/talon_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_autogen/resources/talon_file.rst.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    38478 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_cache_builtin/resources/talon.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_util/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/live/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/registry/
--rw-r--r--   0 runner    (1001) docker     (123)    24349 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/serialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/analysis/static/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22430 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/python/shims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/analysis/static/talon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/description/
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/description/describer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.968224 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/fragtable.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/_util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/capture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.972224 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/hlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/directives/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-23 12:57:17.000000 talondoc-1.0.0rc4/src/talondoc/sphinx/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:57:30.964224 talondoc-1.0.0rc4/src/talondoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 12:57:30.000000 talondoc-1.0.0rc4/src/talondoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.529234 talondoc-1.0.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 13:36:35.529234 talondoc-1.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:36:35.529234 talondoc-1.0.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.517234 talondoc-1.0.0rc5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/_autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/conf.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/index.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/index.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/python_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/python_file.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/talon_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_autogen/resources/talon_file.rst.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/_cache_builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_cache_builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/_cache_builtin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    38478 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_cache_builtin/resources/talon.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_util/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_util/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc/analysis/live/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/analysis/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)    24349 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/analysis/registry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/registry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/registry/data/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/registry/data/serialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/analysis/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/analysis/static/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/static/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22430 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/static/python/shims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/analysis/static/talon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/description/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/description/describer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/sphinx/_util/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/sphinx/_util/addnodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/_util/addnodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/_util/addnodes/fragtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/_util/addnodes/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/_util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.525234 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/capture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.529234 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/hlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/directives/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-23 13:36:23.000000 talondoc-1.0.0rc5/src/talondoc/sphinx/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:35.521234 talondoc-1.0.0rc5/src/talondoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 13:36:35.000000 talondoc-1.0.0rc5/src/talondoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-23 13:36:35.000000 talondoc-1.0.0rc5/src/talondoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:36:35.000000 talondoc-1.0.0rc5/src/talondoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 13:36:35.000000 talondoc-1.0.0rc5/src/talondoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 13:36:35.000000 talondoc-1.0.0rc5/src/talondoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 13:36:35.000000 talondoc-1.0.0rc5/src/talondoc.egg-info/top_level.txt
```

### Comparing `talondoc-1.0.0rc4/PKG-INFO` & `talondoc-1.0.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-1.0.0rc4/README.md` & `talondoc-1.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/pyproject.toml` & `talondoc-1.0.0rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talondoc"
-version = "1.0.0rc4"
+version = "1.0.0rc5"
 description = "A Sphinx extension for Talon user directories."
 license = { file = 'LICENSE' }
 authors = [{ name = "Wen Kokke", email = "wenkokke@users.noreply.github.com" }]
 readme = "README.md"
 keywords = ["talon", "sphinx"]
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `talondoc-1.0.0rc4/src/talondoc/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_autogen/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/_autogen/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_autogen/resources/conf.py.jinja2` & `talondoc-1.0.0rc5/src/talondoc/_autogen/resources/conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.md.jinja2` & `talondoc-1.0.0rc5/src/talondoc/_autogen/resources/python_file.md.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_autogen/resources/python_file.rst.jinja2` & `talondoc-1.0.0rc5/src/talondoc/_autogen/resources/python_file.rst.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_cache_builtin/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/_cache_builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_cache_builtin/resources/talon.json` & `talondoc-1.0.0rc5/src/talondoc/_cache_builtin/resources/talon.json`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_util/io.py` & `talondoc-1.0.0rc5/src/talondoc/_util/io.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_util/logging.py` & `talondoc-1.0.0rc5/src/talondoc/_util/logging.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/_util/progress_bar.py` & `talondoc-1.0.0rc5/src/talondoc/_util/progress_bar.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/live/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/live/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_actions.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_actions.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_captures.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_captures.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_commands.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_commands.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_lists.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_lists.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/live/resources/get_settings.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/live/resources/get_settings.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/registry/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/registry/data/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/abc.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/registry/data/abc.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/registry/data/serialise.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/registry/data/serialise.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/static/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/static/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/static/python/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/static/python/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/static/python/shims.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/static/python/shims.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/analysis/static/talon.py` & `talondoc-1.0.0rc5/src/talondoc/analysis/static/talon.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/description/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/description/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/description/describer.py` & `talondoc-1.0.0rc5/src/talondoc/description/describer.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/_util/addnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/_util/addnodes/fragtable.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/_util/addnodes/fragtable.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/_util/typing.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/_util/typing.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/action.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/action.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/capture.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/capture.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/__init__.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/__init__.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/abc.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/abc.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/hlist.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/hlist.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/command/table.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/command/table.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/errors.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/errors.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/list.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/list.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/mode.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/mode.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/setting.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/setting.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/directives/tag.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/directives/tag.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/domains.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/domains.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc/sphinx/typing.py` & `talondoc-1.0.0rc5/src/talondoc/sphinx/typing.py`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc.egg-info/PKG-INFO` & `talondoc-1.0.0rc5/src/talondoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-1.0.0rc4/src/talondoc.egg-info/SOURCES.txt` & `talondoc-1.0.0rc5/src/talondoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talondoc-1.0.0rc4/src/talondoc.egg-info/requires.txt` & `talondoc-1.0.0rc5/src/talondoc.egg-info/requires.txt`

 * *Files identical despite different names*

