# Comparing `tmp/oarepo-vocabularies-1.0.9.tar.gz` & `tmp/oarepo-vocabularies-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-vocabularies-1.0.9.tar", last modified: Sun Mar 26 07:43:56 2023, max compression
+gzip compressed data, was "oarepo-vocabularies-2.0.0.tar", last modified: Tue May 23 07:50:29 2023, max compression
```

## Comparing `oarepo-vocabularies-1.0.9.tar` & `oarepo-vocabularies-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/ui_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/oarepo_ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/oarepo_ui/components/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/models/ui.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/ui_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/templates/oarepo_ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/templates/oarepo_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/resources/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.851674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/grid.overrides
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.overrides
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.variables
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.843674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.855674 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileLanguages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/ui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:50:29.847674 oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-23 07:50:29.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-23 07:50:29.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:50:29.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-23 07:50:29.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 07:50:29.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 07:50:29.000000 oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-23 07:50:29.859674 oarepo-vocabularies-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 07:45:58.000000 oarepo-vocabularies-2.0.0/setup.py
```

### Comparing `oarepo-vocabularies-1.0.9/LICENSE` & `oarepo-vocabularies-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.9/PKG-INFO` & `oarepo-vocabularies-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: oarepo-vocabularies
-Version: 1.0.9
-Summary: Support for custom fields and hierarchy on Invenio vocabularies
-Description-Content-Type: text/markdown
-Provides-Extra: devs
-Provides-Extra: tests
-License-File: LICENSE
-
 # OARepo vocabularies
 
 This is an extension of invenio vocabularies that allows:
 
 * Use the vocabularies with custom fields
 * Treat vocabulary items as hierarchy
```

### Comparing `oarepo-vocabularies-1.0.9/README.md` & `oarepo-vocabularies-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: oarepo-vocabularies
+Version: 2.0.0
+Summary: Support for custom fields and hierarchy on Invenio vocabularies
+Description-Content-Type: text/markdown
+Provides-Extra: devs
+Provides-Extra: tests
+License-File: LICENSE
+
 # OARepo vocabularies
 
 This is an extension of invenio vocabularies that allows:
 
 * Use the vocabularies with custom fields
 * Treat vocabulary items as hierarchy
```

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/config.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 )
 from oarepo_vocabularies.services.custom_fields import hierarchy
 
 OAREPO_VOCABULARIES_HIERARCHY_CF = [
     hierarchy.HierarchyLevelCF("level"),
     hierarchy.HierarchyTitleCF("title"),
     hierarchy.HierarchyAncestorsCF("ancestors", multiple=True),
+    hierarchy.HierarchyAncestorsOrSelfCF("ancestors_or_self", multiple=True),
     KeywordCF("parent"),
 ]
 
 
 OAREPO_VOCABULARIES_CUSTOM_CF = []
 
 DATASTREAMS_CONFIG_GENERATOR_VOCABULARIES = vocabularies_generator
```

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/ext.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/fixtures.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/api.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/resources/config.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/config.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from invenio_records_resources.services import Link
 from invenio_vocabularies.services import VocabulariesServiceConfig
 
 from oarepo_vocabularies.records.api import Vocabulary
 from oarepo_vocabularies.services.components.hierarchy import HierarchyComponent
-from oarepo_vocabularies.services.schemas import VocabularySchema
+from oarepo_vocabularies.services.schema import VocabularySchema
 from oarepo_vocabularies.services.search import VocabularySearchOptions
 
 
 class VocabulariesConfig(VocabulariesServiceConfig):
     record_cls = Vocabulary
     schema = VocabularySchema
     search = VocabularySearchOptions
     components = [*VocabulariesServiceConfig.components, HierarchyComponent]
+    url_prefix = "/vocabularies/"
     links_item = {
         **VocabulariesServiceConfig.links_item,
+        "vocabulary": Link(
+            "{+api}/vocabularies/{type}",
+            vars=lambda record, vars: vars.update(
+                {
+                    "type": record.type.id,
+                }
+            ),
+        ),
         "parent": Link(
             "{+api}/vocabularies/{type}/{parent}",
             vars=lambda record, vars: vars.update(
                 {
                     "type": record.type.id,
                     "parent": record.get("hierarchy", {}).get("parent"),
                 }
```

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,7 +36,18 @@
         if parent:
             record.hierarchy["ancestors"] = [
                 parent["id"],
                 *parent["hierarchy"]["ancestors"],
             ]
         else:
             record.hierarchy["ancestors"] = []
+
+
+class HierarchyAncestorsOrSelfCF(HierarchyCF, KeywordCF):
+    def update(self, record, parent):
+        if parent:
+            record.hierarchy["ancestors_or_self"] = [
+                record["id"],
+                *parent["hierarchy"]["ancestors_or_self"],
+            ]
+        else:
+            record.hierarchy["ancestors_or_self"] = [record["id"]]
```

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/schemas.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,7 +24,8 @@
 class HierarchySchema(ma.Schema):
     """HierarchySchema schema."""
 
     parent = ma_fields.String()
     level = ma_fields.Integer()
     title = ma_fields.List(i18n_strings)
     ancestors = ma_fields.List(ma_fields.String())
+    ancestors_or_self = ma_fields.List(ma_fields.String())
```

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/search.py` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies/services/search.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,8 +5,11 @@
 
 
 class VocabularySearchOptions(InvenioVocabularySearchOptions):
     params_interpreters_cls = [
         FilterParam.factory(param="h-level", field="hierarchy.level"),
         FilterParam.factory(param="h-parent", field="hierarchy.parent"),
         FilterParam.factory(param="h-ancestor", field="hierarchy.ancestors"),
+        FilterParam.factory(
+            param="h-ancestor-or-self", field="hierarchy.ancestors_or_self"
+        ),
     ] + InvenioVocabularySearchOptions.params_interpreters_cls
```

### Comparing `oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo-vocabularies-2.0.0/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 1.0.9
+Version: 2.0.0
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo vocabularies
```

