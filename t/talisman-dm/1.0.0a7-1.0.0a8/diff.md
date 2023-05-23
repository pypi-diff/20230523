# Comparing `tmp/talisman-dm-1.0.0a7.tar.gz` & `tmp/talisman-dm-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/talisman-dm-1.0.0a7.tar", last modified: Wed May 10 12:47:08 2023, max compression
+gzip compressed data, was "dist/talisman-dm-1.0.0a8.tar", last modified: Tue May 23 20:53:41 2023, max compression
```

## Comparing `talisman-dm-1.0.0a7.tar` & `talisman-dm-1.0.0a8.tar`

### file list

```diff
@@ -1,123 +1,140 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/README.md
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/talisman_dm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/talisman_dm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3197 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/talisman_dm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/talisman_dm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/talisman_dm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/talisman_dm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/base.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     5072 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/document.py
--rw-rw-rw-   0 root         (0) root         (0)     3071 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/fact.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/fact_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/frozen.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/model.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/node.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/datamodel/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     1184 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     4547 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/identifiable.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/markup.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/mention.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/directives/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/directives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/directives/account.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/directives/concept.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/directives/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7372 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_container.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    13671 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_state.py
--rw-rw-rw-   0 root         (0) root         (0)     7193 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_structure.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5206 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/document/_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/facts/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/facts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2424 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/facts/concept.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/facts/links.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/facts/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/facts/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/links/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/links/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/mentions/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/mentions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/mentions/image.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/mentions/node.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/mentions/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/nodes/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/nodes/base64.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/nodes/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/nodes/structure.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/nodes/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/datamodel/values/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/values/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/values/date.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/values/geo.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/values/link.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/datamodel/values/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/json_schema/directives.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/json_schema/facts.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/json_schema/links.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/json_schema/mentions.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/json_schema/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/json_schema/values.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/v0/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4731 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/_facts.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     3689 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/fact.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/v0/json_schema/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/wrapper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:47:08.000000 talisman-dm-1.0.0a7/tdm/wrapper/node/
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/wrapper/node/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5509 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/wrapper/node/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/wrapper/node/_delegate.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/wrapper/node/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-10 12:46:47.000000 talisman-dm-1.0.0a7/tdm/wrapper/node/_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-13 06:48:56.000000 talisman-dm-1.0.0a8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/abstract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     6818 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     5838 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/identifiable.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/frozen.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      630 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/identifiable.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      982 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/type_.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/datamodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_container.py
+-rw-rw-rw-   0 root         (0) root         (0)    10036 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5206 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14014 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7193 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/_structure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_composite.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_property.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_slot.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3436 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     4384 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/links/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/links/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/geo.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/link.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/directives.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/facts.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/links.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/mentions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/values.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3262 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4733 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_facts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4071 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/wrapper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5509 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_delegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_interface.py
```

### Comparing `talisman-dm-1.0.0a7/PKG-INFO` & `talisman-dm-1.0.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a7/setup.py` & `talisman-dm-1.0.0a8/setup.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/talisman_dm.egg-info/PKG-INFO` & `talisman-dm-1.0.0a8/talisman_dm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a7/talisman_dm.egg-info/SOURCES.txt` & `talisman-dm-1.0.0a8/talisman_dm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 talisman_dm.egg-info/top_level.txt
 tdm/__init__.py
 tdm/helper.py
 tdm/legacy.py
 tdm/model.py
 tdm/abstract/__init__.py
 tdm/abstract/datamodel/__init__.py
-tdm/abstract/datamodel/base.py
 tdm/abstract/datamodel/directive.py
 tdm/abstract/datamodel/document.py
+tdm/abstract/datamodel/domain.py
 tdm/abstract/datamodel/fact.py
-tdm/abstract/datamodel/fact_filter.py
+tdm/abstract/datamodel/filter.py
+tdm/abstract/datamodel/identifiable.py
 tdm/abstract/datamodel/link.py
 tdm/abstract/datamodel/mention.py
 tdm/abstract/datamodel/node.py
 tdm/abstract/datamodel/value.py
 tdm/abstract/datamodel/markup/__init__.py
 tdm/abstract/datamodel/markup/_helper.py
 tdm/abstract/datamodel/markup/abstract.py
@@ -28,34 +29,47 @@
 tdm/abstract/datamodel/markup/model.py
 tdm/abstract/json_schema/__init__.py
 tdm/abstract/json_schema/composite.py
 tdm/abstract/json_schema/decorator.py
 tdm/abstract/json_schema/model.py
 tdm/abstract/json_schema/serializers/__init__.py
 tdm/abstract/json_schema/serializers/abstract.py
+tdm/abstract/json_schema/serializers/domain.py
 tdm/abstract/json_schema/serializers/identifiable.py
 tdm/abstract/json_schema/serializers/markup.py
 tdm/abstract/json_schema/serializers/mention.py
 tdm/abstract/json_schema/serializers/metadata.py
 tdm/abstract/json_schema/serializers/serializers.py
+tdm/abstract/json_schema/serializers/type_.py
 tdm/abstract/json_schema/serializers/value.py
 tdm/datamodel/__init__.py
+tdm/datamodel/common/__init__.py
+tdm/datamodel/common/_container.py
+tdm/datamodel/common/_impl.py
+tdm/datamodel/common/_state.py
+tdm/datamodel/common/_types.py
+tdm/datamodel/common/_view.py
 tdm/datamodel/directives/__init__.py
 tdm/datamodel/directives/account.py
 tdm/datamodel/directives/concept.py
 tdm/datamodel/directives/platform.py
 tdm/datamodel/document/__init__.py
-tdm/datamodel/document/_base.py
-tdm/datamodel/document/_container.py
 tdm/datamodel/document/_factory.py
 tdm/datamodel/document/_impl.py
-tdm/datamodel/document/_state.py
 tdm/datamodel/document/_structure.py
-tdm/datamodel/document/_types.py
-tdm/datamodel/document/_view.py
+tdm/datamodel/domain/__init__.py
+tdm/datamodel/domain/_impl.py
+tdm/datamodel/domain/_manager.py
+tdm/datamodel/domain/types/__init__.py
+tdm/datamodel/domain/types/_composite.py
+tdm/datamodel/domain/types/_concept.py
+tdm/datamodel/domain/types/_property.py
+tdm/datamodel/domain/types/_relation.py
+tdm/datamodel/domain/types/_slot.py
+tdm/datamodel/domain/types/_value.py
 tdm/datamodel/facts/__init__.py
 tdm/datamodel/facts/concept.py
 tdm/datamodel/facts/links.py
 tdm/datamodel/facts/mention.py
 tdm/datamodel/facts/value.py
 tdm/datamodel/links/__init__.py
 tdm/datamodel/links/reference.py
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/__init__.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 __all__ = [
-    'EnsureIdentifiable', 'Identifiable',
     'AbstractDirective',
     'AbstractDocumentFactory', 'TalismanDocument',
+    'AbstractDomainType', 'AbstractLinkDomainType', 'AbstractDomain',
     'AbstractFact', 'AbstractLinkFact', 'FactStatus',
     'and_filter', 'not_filter', 'or_filter',
+    'EnsureIdentifiable', 'Identifiable',
     'AbstractNodeLink',
     'AbstractMarkup', 'FrozenMarkup',
     'AbstractNodeMention',
     'AbstractContentNode', 'AbstractNode', 'BaseNodeMetadata',
     'AbstractValue'
 ]
 
-from .base import EnsureIdentifiable, Identifiable
 from .directive import AbstractDirective
 from .document import AbstractDocumentFactory, TalismanDocument
+from .domain import AbstractDomain, AbstractDomainType, AbstractLinkDomainType
 from .fact import AbstractFact, AbstractLinkFact, FactStatus
-from .fact_filter import and_filter, not_filter, or_filter
+from .filter import and_filter, not_filter, or_filter
+from .identifiable import EnsureIdentifiable, Identifiable
 from .link import AbstractNodeLink
 from .markup import AbstractMarkup, FrozenMarkup
 from .mention import AbstractNodeMention
 from .node import AbstractContentNode, AbstractNode, BaseNodeMetadata
 from .value import AbstractValue
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/base.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/identifiable.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/document.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/document.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union
 
-from .base import Identifiable
 from .directive import AbstractDirective
 from .fact import AbstractFact
+from .identifiable import Identifiable
 from .link import AbstractNodeLink
 from .node import AbstractNode
 
 _TD = TypeVar('_TD', bound='TalismanDocument')
 _Fact = TypeVar('_Fact', bound=AbstractFact)
 _NodeLink = TypeVar('_NodeLink', bound=AbstractNodeLink)
 _Node = TypeVar('_Node', bound=AbstractNode)
+_Directive = TypeVar('_Directive', bound=AbstractDirective)
 
 NodeOrId = Union[str, AbstractNode]
 
 
 class TalismanDocument(metaclass=ABCMeta):
     __slots__ = ()
 
     @property
     @abstractmethod
     def id(self) -> str:
         pass
 
+    # nodes methods
+
+    @property
+    @abstractmethod
+    def id2node(self) -> Dict[str, AbstractNode]:
+        pass
+
     @property
     @abstractmethod
-    def nodes(self) -> Dict[str, AbstractNode]:
+    def nodes(self) -> Dict[Type[AbstractNode], Iterable[AbstractNode]]:
         pass
 
     @abstractmethod
     def get_node(self, id_: str) -> AbstractNode:
         pass
 
     @abstractmethod
     def get_nodes(
             self, type_: Type[_Node] = AbstractNode, *,
             filter_: Union[Callable[[_Node], bool], Iterable[Callable[[_Node], bool]]] = tuple()
     ) -> Iterator[_Node]:
         pass
 
     @abstractmethod
+    def related_nodes(
+            self, obj: Union[Identifiable, str], type_: Type[_Node] = AbstractNode, *,
+            filter_: Union[Callable[[_Node], bool], Iterable[Callable[[_Node], bool]]] = tuple()
+    ) -> Iterator[_Node]:
+        pass
+
+    @abstractmethod
     def with_nodes(self: _TD, nodes: Iterable[AbstractNode]) -> _TD:
         pass
 
     @abstractmethod
     def without_nodes(self: _TD, nodes: Iterable[NodeOrId], *, cascade: bool = True) -> _TD:
         pass
 
+    # structure methods
+
     @property
     @abstractmethod
     def roots(self) -> Set[AbstractNode]:
         pass
 
     @property
     @abstractmethod
@@ -81,20 +98,31 @@
     def with_roots(self: _TD, nodes: Iterable[NodeOrId]) -> _TD:
         pass
 
     @abstractmethod
     def without_structure(self: _TD, structure: Dict[NodeOrId, Iterable[NodeOrId]]) -> _TD:
         pass
 
+    # semantic link methods
+
+    @property
+    @abstractmethod
+    def id2node_link(self) -> Dict[str, AbstractNodeLink]:
+        pass
+
     @property
     @abstractmethod
     def node_links(self) -> Dict[Type[AbstractNodeLink], Iterable[AbstractNodeLink]]:
         pass
 
     @abstractmethod
+    def get_node_link(self, id_: str) -> AbstractNodeLink:
+        pass
+
+    @abstractmethod
     def get_node_links(
             self, type_: Type[_NodeLink] = AbstractNodeLink, *,
             filter_: Union[Callable[[_NodeLink], bool], Iterable[Callable[[_NodeLink], bool]]] = tuple()
     ) -> Iterator[_NodeLink]:
         pass
 
     @abstractmethod
@@ -108,20 +136,31 @@
     def with_node_links(self: _TD, links: Iterable[AbstractNodeLink], *, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
     def without_node_links(self: _TD, links: Iterable[Union[str, AbstractNodeLink]], *, cascade: bool = False) -> _TD:
         pass
 
+    # facts methods
+
+    @property
+    @abstractmethod
+    def id2fact(self) -> Dict[str, AbstractFact]:
+        pass
+
     @property
     @abstractmethod
     def facts(self) -> Dict[Type[AbstractFact], Iterable[AbstractFact]]:
         pass
 
     @abstractmethod
+    def get_fact(self, id_: str) -> AbstractFact:
+        pass
+
+    @abstractmethod
     def get_facts(
             self, type_: Type[_Fact] = AbstractFact, *,
             filter_: Union[Callable[[_Fact], bool], Iterable[Callable[[_Fact], bool]]] = tuple()
     ) -> Iterator[_Fact]:
         pass
 
     @abstractmethod
@@ -135,27 +174,54 @@
     def with_facts(self: _TD, facts: Iterable[AbstractFact], *, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
     def without_facts(self: _TD, facts: Iterable[Union[str, AbstractFact]], *, cascade: bool = False) -> _TD:
         pass
 
+    # directive methods
+
+    @property
+    @abstractmethod
+    def id2directive(self) -> Dict[str, AbstractDirective]:
+        pass
+
     @property
     @abstractmethod
     def directives(self) -> Dict[Type[AbstractDirective], Iterable[AbstractDirective]]:
         pass
 
     @abstractmethod
+    def get_directive(self, id_: str) -> AbstractDirective:
+        pass
+
+    @abstractmethod
+    def get_directives(
+            self, type_: Type[_Directive] = AbstractDirective, *,
+            filter_: Union[Callable[[_Directive], bool], Iterable[Callable[[_Directive], bool]]] = tuple()
+    ) -> Iterator[_Directive]:
+        pass
+
+    @abstractmethod
+    def related_directives(
+            self, obj: Union[Identifiable, str], type_: Type[_Directive] = AbstractDirective, *,
+            filter_: Union[Callable[[_Directive], bool], Iterable[Callable[[_Directive], bool]]] = tuple()
+    ) -> Iterator[_Directive]:
+        pass
+
+    @abstractmethod
     def with_directives(self: _TD, directives: Iterable[AbstractDirective], *, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
     def without_directives(self: _TD, directives: Iterable[Union[str, AbstractDirective]], *, cascade: bool = False) -> _TD:
         pass
 
+    # metadata methods
+
     @property
     @abstractmethod
     def metadata(self) -> Dict[str, Any]:
         pass
 
     @abstractmethod
     def with_metadata(self: _TD, metadata: Dict[str, Any]) -> _TD:
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/fact_filter.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/filter.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/link.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/link.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import Callable, Generic, Set, TypeVar
 
-from .base import EnsureIdentifiable
+from .identifiable import EnsureIdentifiable
 from .mention import AbstractNodeMention
 
 _ST = TypeVar('_ST', bound=AbstractNodeMention)
 _TT = TypeVar('_TT', bound=AbstractNodeMention)
 
 
 @dataclass(frozen=True)
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/_helper.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/_helper.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/abstract.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/markup/frozen.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/frozen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 
 from immutabledict import immutabledict
 
-from tdm.abstract.datamodel.markup.abstract import AbstractMarkup
 from ._helper import freeze_dict
+from .abstract import AbstractMarkup
 
 
 @dataclass(frozen=True)
 class FrozenMarkup(AbstractMarkup):
     _markup: immutabledict = immutabledict()
 
     @property
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/node.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Generic, Set, TypeVar
 
 from tdm.helper import generics_mapping
-from .base import Identifiable
+from .identifiable import Identifiable
 from .markup import AbstractMarkup, FrozenMarkup
 
 
 @dataclass(frozen=True)
 class BaseNodeMetadata:
     hidden: bool = False
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/datamodel/value.py` & `talisman-dm-1.0.0a8/tdm/abstract/datamodel/value.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/composite.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/composite.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/decorator.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/decorator.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/model.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,16 +70,22 @@
     for field in fields(type_):
         name = field.name
         default_value = field.default if field.default is not dataclasses.MISSING else ...
         field_type = type_vars.get(field.type, field.type)
         union_types = unfold_union(field_type)
         model_field = False
         f_t = []
-        for t in union_types:
+        for t in map(lambda ut: type_vars.get(ut, ut), union_types):
             typing_type, real_type, arg = uniform_collection(t)
+            if real_type is type:
+                serializer = BaseSerializers[type]
+                f_t.append(serializer.field_type(arg))
+                special_fields[name].append(serializer.deserialize)
+                model_field = True
+                continue
             for _type, serializer in BaseSerializers.items():
                 if issubclass(arg, _type):
                     if typing_type is None:
                         f_t.append(serializer.field_type(arg))
                         special_fields[name].append(serializer.deserialize)
                     else:
                         f_t.append(typing_type[serializer.field_type(arg)])
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/__init__.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
     'AbstractElementModel', 'AbstractElementSerializer', 'AbstractModelSerializer',
     'IdSerializer',
     'NodeMentionSerializer',
     'NodeMetadataSerializer',
     'BaseSerializers'
 ]
 
-from typing import Dict
+from typing import Mapping
 
 from immutabledict import immutabledict
 
 from .abstract import AbstractElementModel, AbstractElementSerializer, AbstractModelSerializer
 from .identifiable import IdSerializer
 from .mention import NodeMentionSerializer
 from .metadata import NodeMetadataSerializer
 from .serializers import build_serializers
 
-BaseSerializers: Dict[type, AbstractElementSerializer] = immutabledict(build_serializers())
+BaseSerializers: Mapping[type, AbstractElementSerializer] = immutabledict(build_serializers())
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/abstract.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/identifiable.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/identifiable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Any, Dict, Type, TypeVar
+from typing import Any, Dict, Generic, Type, TypeVar
 
 from tdm.abstract.datamodel import EnsureIdentifiable
 from .abstract import AbstractElementSerializer
 
 _Identifiable = TypeVar('_Identifiable', bound=EnsureIdentifiable)
 
 
-class IdSerializer(AbstractElementSerializer[_Identifiable, str]):
+class IdSerializer(AbstractElementSerializer[_Identifiable, str], Generic[_Identifiable]):
     def __init__(self, type_: Type[_Identifiable]):
         self._type = type_
 
     def serialize(self, element: _Identifiable) -> str:
         return element.id
 
     def deserialize(self, serialized: str, typed_id2element: Dict[type, Dict[str, Any]]) -> _Identifiable:
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/markup.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/markup.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/mention.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/mention.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/metadata.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/metadata.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/serializers.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-from tdm.abstract.datamodel import AbstractFact, AbstractMarkup, AbstractNode, AbstractNodeMention, AbstractValue, BaseNodeMetadata
+from tdm.abstract.datamodel import AbstractDomainType, AbstractFact, AbstractMarkup, AbstractNode, AbstractNodeMention, AbstractValue, \
+    BaseNodeMetadata
+from .domain import DomainTypeSerializer
 from .identifiable import IdSerializer
 from .markup import MarkupSerializer
 from .mention import NodeMentionSerializer
 from .metadata import NodeMetadataSerializer
+from .type_ import TypeSerializer
 from .value import ValueSerializer
 
 
 def build_serializers():
     result = {
         AbstractNode: IdSerializer(AbstractNode),
         AbstractFact: IdSerializer(AbstractFact),
         AbstractNodeMention: NodeMentionSerializer(),
         BaseNodeMetadata: NodeMetadataSerializer(),
         AbstractValue: ValueSerializer(),
-        AbstractMarkup: MarkupSerializer()
+        AbstractMarkup: MarkupSerializer(),
+        AbstractDomainType: DomainTypeSerializer(),
+        type: TypeSerializer()
     }
     # other serializers could be added here
     return result
```

### Comparing `talisman-dm-1.0.0a7/tdm/abstract/json_schema/serializers/value.py` & `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/value.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/directives/concept.py` & `talisman-dm-1.0.0a8/tdm/datamodel/directives/concept.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/document/_container.py` & `talisman-dm-1.0.0a8/tdm/datamodel/common/_container.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/document/_factory.py` & `talisman-dm-1.0.0a8/tdm/datamodel/document/_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import uuid
 from typing import Any, Dict, Iterable, Optional, Tuple
 
-from tdm.abstract.datamodel import AbstractDirective, AbstractDocumentFactory, AbstractFact, AbstractNode, AbstractNodeLink, \
-    TalismanDocument
-from ._container import TypedIdsContainer
+from tdm.abstract.datamodel import AbstractDirective, AbstractDocumentFactory, AbstractDomain, AbstractFact, AbstractNode, \
+    AbstractNodeLink, TalismanDocument
+from tdm.datamodel.common import TypedIdsContainer
+from tdm.datamodel.domain import get_default_domain
 from ._impl import TalismanDocumentImpl
 from ._structure import NodesStructure
 
 
 class TalismanDocumentFactory(AbstractDocumentFactory):
 
+    def __init__(self, domain: Optional[AbstractDomain] = None):
+        self._domain = domain if domain is not None else get_default_domain()
+
     def create_document(self, *, id_: Optional[str] = None) -> TalismanDocument:
         return TalismanDocumentImpl(
             id2view={},
             dependencies={},
             structure=NodesStructure(),
             containers={
                 AbstractNode: TypedIdsContainer(AbstractNode, ()),
                 AbstractNodeLink: TypedIdsContainer(AbstractNodeLink, ()),
                 AbstractFact: TypedIdsContainer(AbstractFact, ()),
                 AbstractDirective: TypedIdsContainer(AbstractDirective, ())
             },
             metadata=None,
-            id_=id_ or self.generate_id())
+            id_=id_ or self.generate_id(),
+            domain=self._domain
+        )
 
     def construct(
             self,
             content: Iterable[AbstractNode] = (),
             structure: Dict[str, Tuple[str, ...]] = None,
             root: Optional[str] = None,
             node_links: Iterable[AbstractNodeLink] = (),
```

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/document/_state.py` & `talisman-dm-1.0.0a8/tdm/datamodel/common/_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from tdm.datamodel.document._view import AbstractView, generate_dataclass_view
+from ._view import AbstractView, generate_dataclass_view
 
 
 def pack_view_state(id2view: Dict[str, AbstractView]) -> dict:
     result = {
         id_: (_orig_type(view), view.__dict__)
         for id_, view in id2view.items()
     }
```

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/document/_structure.py` & `talisman-dm-1.0.0a8/tdm/datamodel/document/_structure.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/document/_types.py` & `talisman-dm-1.0.0a8/tdm/datamodel/common/_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Type, Union
 
-from tdm.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, EnsureIdentifiable
+from tdm.abstract.datamodel import AbstractDirective, AbstractDomainType, AbstractFact, AbstractNode, AbstractNodeLink, EnsureIdentifiable
 
-_BASE_TYPES = {AbstractNode, AbstractNodeLink, AbstractFact, AbstractDirective}
+_BASE_TYPES = {AbstractNode, AbstractNodeLink, AbstractFact, AbstractDirective, AbstractDomainType}
 
 _CACHE: Dict[Type[EnsureIdentifiable], Type[EnsureIdentifiable]] = {}
 
 
 def get_base_type(element: Union[EnsureIdentifiable, Type[EnsureIdentifiable]]) -> Type[EnsureIdentifiable]:
     if isinstance(element, EnsureIdentifiable):
         element = type(element)
```

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/document/_view.py` & `talisman-dm-1.0.0a8/tdm/datamodel/common/_view.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/facts/concept.py` & `talisman-dm-1.0.0a8/tdm/datamodel/facts/concept.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from dataclasses import dataclass
+from abc import ABCMeta
+from dataclasses import dataclass, replace
 from typing import Callable, Optional, Sequence, Set, Tuple, Union
 
-from tdm.abstract.datamodel import AbstractFact, FactStatus, Identifiable
+from tdm.abstract.datamodel import AbstractDomain, AbstractFact, FactStatus, Identifiable
 from tdm.abstract.json_schema import generate_model
+from tdm.datamodel.domain import ConceptType
 
 
 @dataclass(frozen=True)
 class ConceptValue(object):
     concept: str
     confidence: Optional[float] = None
 
@@ -20,19 +22,22 @@
             return value
         if isinstance(value, str):
             return cls(concept=value)
         raise ValueError
 
 
 @dataclass(frozen=True)
-class _ConceptFact(AbstractFact):  # not an error as id argument is kw only
-    type_id: str
+class _ConceptFact(AbstractFact, metaclass=ABCMeta):  # not an error as id argument is kw only
+    type_id: Union[str, ConceptType]
     value: Union[ConceptValue, Tuple[ConceptValue, ...]] = tuple()
 
     def __post_init__(self):
+        if not isinstance(self.type_id, str) and not isinstance(self.type_id, ConceptType):
+            raise ValueError(f"concept fact type id conflict: {self.type_id}")
+
         if isinstance(self.value, str):
             object.__setattr__(self, 'value', ConceptValue.build(self.value))
         elif isinstance(self.value, Sequence):
             object.__setattr__(self, 'value', tuple(map(ConceptValue.build, self.value)))
         else:
             object.__setattr__(self, 'value', ConceptValue.build(self.value))
 
@@ -47,14 +52,34 @@
     def constant_fields(cls) -> Set[str]:
         return {'type_id'}
 
 
 @generate_model(label='concept')
 @dataclass(frozen=True)
 class ConceptFact(Identifiable, _ConceptFact):
+
+    def replace_with_domain(self, domain: AbstractDomain) -> 'ConceptFact':
+        if isinstance(self.type_id, str):
+            domain_type = domain.get_type(self.type_id)
+            if not isinstance(domain_type, ConceptType):
+                raise ValueError
+            return replace(self, type_id=domain_type)
+        return self
+
+    def _as_tuple(self) -> tuple:
+        return self.id, (self.type_id if isinstance(self.type_id, str) else self.type_id.id), self.value
+
+    def __eq__(self, other):
+        if not isinstance(other, ConceptFact):
+            return NotImplemented
+        return self._as_tuple() == other._as_tuple()
+
+    def __hash__(self):
+        return hash(self._as_tuple())
+
     @staticmethod
     def empty_value_filter() -> Callable[['ConceptFact'], bool]:
         return lambda f: isinstance(f.value, tuple) and not f.value
 
     @staticmethod
     def tuple_value_filter() -> Callable[['ConceptFact'], bool]:
         return lambda f: isinstance(f.value, tuple)
```

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/facts/mention.py` & `talisman-dm-1.0.0a8/tdm/datamodel/facts/mention.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from dataclasses import dataclass
+from abc import ABCMeta
+from dataclasses import dataclass, replace
 from typing import Callable, Set, Union
 
-from tdm.abstract.datamodel import AbstractFact, AbstractNode, AbstractNodeMention, Identifiable
+from tdm.abstract.datamodel import AbstractDomain, AbstractFact, AbstractNode, AbstractNodeMention, Identifiable
 from tdm.abstract.json_schema import generate_model
 from .value import AtomValueFact
 
 
 @dataclass(frozen=True)
-class _MentionFact(AbstractFact):
+class _MentionFact(AbstractFact, metaclass=ABCMeta):
     mention: AbstractNodeMention
     value: AtomValueFact
 
     @classmethod
     def constant_fields(cls) -> Set[str]:
         return {'mention', 'value'}
 
 
 @generate_model(label='mention')
 @dataclass(frozen=True)
 class MentionFact(Identifiable, _MentionFact):
+
+    def replace_with_domain(self, domain: AbstractDomain) -> 'MentionFact':
+        value = self.value.replace_with_domain(domain)
+        if value is self.value:
+            return self
+        return replace(self, value=value)
+
     @staticmethod
     def node_filter(node: Union[AbstractNode, str]) -> Callable[['MentionFact'], bool]:
         node_id = node.id if isinstance(node, AbstractNode) else node
 
         def _filter(fact: MentionFact) -> bool:
             return fact.mention.node_id == node_id
```

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/links/reference.py` & `talisman-dm-1.0.0a8/tdm/datamodel/links/reference.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/mentions/image.py` & `talisman-dm-1.0.0a8/tdm/datamodel/mentions/image.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/mentions/text.py` & `talisman-dm-1.0.0a8/tdm/datamodel/mentions/text.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/nodes/__init__.py` & `talisman-dm-1.0.0a8/tdm/datamodel/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/nodes/file.py` & `talisman-dm-1.0.0a8/tdm/datamodel/nodes/file.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/nodes/structure.py` & `talisman-dm-1.0.0a8/tdm/datamodel/nodes/structure.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/nodes/text.py` & `talisman-dm-1.0.0a8/tdm/datamodel/nodes/text.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/values/date.py` & `talisman-dm-1.0.0a8/tdm/datamodel/values/date.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/values/geo.py` & `talisman-dm-1.0.0a8/tdm/datamodel/values/geo.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/datamodel/values/scalar.py` & `talisman-dm-1.0.0a8/tdm/datamodel/values/scalar.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/helper.py` & `talisman-dm-1.0.0a8/tdm/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     # check if it is union
     if hasattr(type_, '__origin__') and type_.__origin__ is Union:
         return type_.__args__
     return type_,
 
 
 _COLLECTIONS = {
-    tuple: Tuple,
+    tuple: List,  # in other case Tuple[A, ...] is converted to Tuple[A]. Deserializes to tuple
     set: Set,
     list: List,
     dict: Dict
 }
 
 
 def map_type(type_: type) -> type:
@@ -25,14 +25,17 @@
     if not hasattr(type_, '__origin__'):
         return None, None, type_
     if issubclass(type_.__origin__, Collection):
         args = tuple(filter(lambda t: t is not ..., type_.__args__))
         if len(args) != 1:
             raise NotImplementedError
         return map_type(type_.__origin__), type_.__origin__, args[0]
+    if type_.__origin__ is type:
+        return None, type, type_.__args__[0]
+    raise TypeError
 
 
 def check_base_type(type_: type, base_type: type) -> bool:
     if issubclass(type_, base_type):  # check simple subclass
         return True
     if not hasattr(type_, '__origin__'):  # check if it is some generic (Union, Tuple, etc)
         return False
```

### Comparing `talisman-dm-1.0.0a7/tdm/json_schema/directives.py` & `talisman-dm-1.0.0a8/tdm/json_schema/directives.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/json_schema/facts.py` & `talisman-dm-1.0.0a8/tdm/json_schema/facts.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/json_schema/mentions.py` & `talisman-dm-1.0.0a8/tdm/json_schema/mentions.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/json_schema/nodes.py` & `talisman-dm-1.0.0a8/tdm/json_schema/nodes.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/json_schema/values.py` & `talisman-dm-1.0.0a8/tdm/json_schema/values.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/legacy.py` & `talisman-dm-1.0.0a8/tdm/legacy.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/model.py` & `talisman-dm-1.0.0a8/tdm/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from typing import Dict, Optional, Tuple
+from typing import ClassVar, Dict, Optional, Tuple
 
 from immutabledict import immutabledict
-from pydantic import BaseModel, root_validator
+from pydantic import BaseModel, PrivateAttr, root_validator
 from typing_extensions import Literal
 
-from .abstract.datamodel import AbstractNode, TalismanDocument
+from .abstract.datamodel import AbstractDomain, AbstractNode, TalismanDocument
 from .datamodel.document import TalismanDocumentFactory
 from .json_schema.directives import DirectivesModel
 from .json_schema.facts import FactsModel
 from .json_schema.links import NodeLinksModel
 from .json_schema.nodes import NodeModel, fill_children, serialize_node
 from .legacy import DocumentMetadataModel
 
 
 class TalismanDocumentModel(BaseModel):
     class Config:
         json_encoders = {
             immutabledict: lambda x: dict(x)
         }
 
+    _DEFAULT_DOMAIN: ClassVar[AbstractDomain] = None
+    _domain: AbstractDomain = PrivateAttr(None)
+
     VERSION: Literal['1.0'] = ...
     id: str
     main_node: str
     content: Tuple[NodeModel, ...]
     links: NodeLinksModel
     facts: FactsModel
     directives: DirectivesModel
@@ -31,18 +34,26 @@
 
     @root_validator(pre=True)
     def _set_version(cls, values):  # noqa N805: pydantic requires cls to be first argument in validators
         if 'VERSION' not in values:
             values['VERSION'] = '1.0'
         return values
 
+    @classmethod
+    def set_default_domain(cls, domain: Optional[AbstractDomain]) -> None:
+        cls._DEFAULT_DOMAIN = domain
+
+    def set_domain(self, domain: Optional[AbstractDomain]) -> None:
+        self._domain = domain
+
     def deserialize(self) -> TalismanDocument:
+        document_factory = TalismanDocumentFactory(self._domain or self._DEFAULT_DOMAIN)
         id2node, structure = self._collect_nodes()
 
-        return TalismanDocumentFactory.construct(
+        return document_factory.construct(
             content=id2node.values(),
             structure=structure,
             root=self.main_node,
             node_links=self.links.deserialize(id2node),
             facts=self.facts.deserialize(id2node),
             directives=self.directives.deserialize(id2node),
             metadata=self.metadata.to_metadata() if self.metadata is not None else None,
@@ -58,15 +69,15 @@
             id2node[node_model.id] = node_model.deserialize({})
             if node_model.children:
                 links[node_model.id] = node_model.children
         return id2node, links
 
     @classmethod
     def serialize(cls, document: TalismanDocument) -> 'TalismanDocumentModel':
-        node_models = tuple(serialize_node(node) for node in document.nodes.values())
+        node_models = tuple(serialize_node(node) for node in document.id2node.values())
         fill_children(node_models, document)
         return cls(
             id=document.id,
             main_node=document.main_root.id,
             content=node_models,
             links=NodeLinksModel.serialize(document.node_links),
             facts=FactsModel.serialize(document.facts),
```

### Comparing `talisman-dm-1.0.0a7/tdm/v0/json_schema/content.py` & `talisman-dm-1.0.0a8/tdm/v0/json_schema/content.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/_facts.py` & `talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_facts.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         value=value,
         id=fact.id
     )
     yield value
 
     if fact.mention:
         # get only first span of multi-span mention
-        node = doc.nodes[fact.mention[0].node_id]
+        node = doc.id2node[fact.mention[0].node_id]
         if not isinstance(node, TextNode):
             return
         mention = TextNodeMention(node, fact.mention[0].start, fact.mention[0].end)
     elif fact.metadata and hasattr(fact.metadata, 'text'):
         # create node
         text = ' '.join(fact.metadata.text)
         mention = TextNodeMention(TextNode(text), 0, len(text))
```

### Comparing `talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/_metadata.py` & `talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_metadata.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/v0/json_schema/convert/_nodes.py` & `talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_nodes.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/v0/json_schema/directive.py` & `talisman-dm-1.0.0a8/tdm/v0/json_schema/directive.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/v0/json_schema/document.py` & `talisman-dm-1.0.0a8/tdm/v0/json_schema/document.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 from collections import defaultdict
-from typing import Dict, Optional, Tuple, Type
+from typing import ClassVar, Dict, Optional, Tuple, Type
 
 from pydantic import BaseModel
 
-from tdm.abstract.datamodel import AbstractFact, AbstractValue, TalismanDocument
+from tdm.abstract.datamodel import AbstractDomain, AbstractFact, AbstractValue, TalismanDocument
 from tdm.datamodel.document import TalismanDocumentFactory
 from tdm.legacy import DocumentMetadataModel
 from .content import TreeDocumentContentModel
 from .convert import build_structure, convert_concept_fact, convert_property_fact, convert_relation_fact, convert_value_fact, \
     get_metadata_facts
 from .directive import DirectiveModel
 from .fact import ConceptFactModel, FactModel, FactType, PropertyFactModel, RelationFactModel, ValueFactModel
 
 
 class TalismanDocumentModel(BaseModel):
+    _DEFAULT_DOMAIN: ClassVar[AbstractDomain] = None
+    _domain: AbstractDomain = None
+
     id: str
     content: TreeDocumentContentModel
     metadata: Optional[DocumentMetadataModel]
     facts: Optional[Tuple[FactModel, ...]]  # pydantic fails to serialize FrozenSet[FactModel]
     directives: Optional[Tuple[DirectiveModel, ...]]
 
+    @classmethod
+    def set_default_domain(cls, domain: Optional[AbstractDomain]) -> None:
+        cls._DEFAULT_DOMAIN = domain
+
+    def set_domain(self, domain: Optional[AbstractDomain]) -> None:
+        self._domain = domain
+
     def to_doc(self, titles: Dict[str, Tuple[str, str]], value_types: Dict[str, Type[AbstractValue]]) -> TalismanDocument:
-        result = TalismanDocumentFactory.create_document(id_=self.id)
+        result = TalismanDocumentFactory(self._domain or self._DEFAULT_DOMAIN).create_document(id_=self.id)
 
         nodes, structure, node_links = build_structure(self.content)
         result = result.with_nodes(nodes).with_structure(structure).with_node_links(node_links, update=True).with_main_root(self.content.id)
 
         # convert document metadata to facts
         metadata = self.metadata.to_metadata() if self.metadata else {}
         result = result.with_metadata(metadata).with_facts(get_metadata_facts(self.id, metadata), update=True)
```

### Comparing `talisman-dm-1.0.0a7/tdm/v0/json_schema/fact.py` & `talisman-dm-1.0.0a8/tdm/v0/json_schema/fact.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/wrapper/node/__init__.py` & `talisman-dm-1.0.0a8/tdm/wrapper/node/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/wrapper/node/_decorator.py` & `talisman-dm-1.0.0a8/tdm/wrapper/node/_decorator.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/wrapper/node/_delegate.py` & `talisman-dm-1.0.0a8/tdm/wrapper/node/_delegate.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a7/tdm/wrapper/node/_impl.py` & `talisman-dm-1.0.0a8/tdm/wrapper/node/_impl.py`

 * *Files identical despite different names*

