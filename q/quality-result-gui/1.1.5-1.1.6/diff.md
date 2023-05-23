# Comparing `tmp/quality-result-gui-1.1.5.tar.gz` & `tmp/quality-result-gui-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quality-result-gui-1.1.5.tar", last modified: Wed Mar 29 10:05:17 2023, max compression
+gzip compressed data, was "quality-result-gui-1.1.6.tar", last modified: Tue May 23 07:22:42 2023, max compression
```

## Comparing `quality-result-gui-1.1.5.tar` & `quality-result-gui-1.1.6.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.332890 quality-result-gui-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-03-29 10:05:17.332890 quality-result-gui-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-29 10:05:17.332890 quality-result-gui-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.312890 quality-result-gui-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.316890 quality-result-gui-1.1.5/src/quality_result_gui/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.320890 quality-result-gui-1.1.5/src/quality_result_gui/api/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/api/quality_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.320890 quality-result-gui-1.1.5/src/quality_result_gui/api/types/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/api/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/api/types/quality_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.320890 quality-result-gui-1.1.5/src/quality_result_gui/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/quality_data_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/quality_error_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/quality_error_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/quality_errors_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    28931 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/quality_errors_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/quality_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.320890 quality-result-gui-1.1.5/src/quality_result_gui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.324890 quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_error_fatal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_error_info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_error_warning.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_result_gui.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.324890 quality-result-gui-1.1.5/src/quality_result_gui/style/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/style/default_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/style/quality_layer_error_symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.324890 quality-result-gui-1.1.5/src/quality_result_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_error_tree_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_errors_dock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_errors_dock.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.328890 quality-result-gui-1.1.5/src/quality_result_gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/utils/layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui/utils/styling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.320890 quality-result-gui-1.1.5/src/quality_result_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-03-29 10:05:17.000000 quality-result-gui-1.1.5/src/quality_result_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-29 10:05:17.000000 quality-result-gui-1.1.5/src/quality_result_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 10:05:17.000000 quality-result-gui-1.1.5/src/quality_result_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-29 10:05:17.000000 quality-result-gui-1.1.5/src/quality_result_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-29 10:05:17.000000 quality-result-gui-1.1.5/src/quality_result_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-29 10:05:17.000000 quality-result-gui-1.1.5/src/quality_result_gui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.328890 quality-result-gui-1.1.5/src/quality_result_gui_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.328890 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.328890 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/example_quality_errors/
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/mock_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/metadata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.328890 quality-result-gui-1.1.5/src/quality_result_gui_plugin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.332890 quality-result-gui-1.1.5/src/quality_result_gui_plugin/resources/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/resources/i18n/fi.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 10:05:17.332890 quality-result-gui-1.1.5/src/quality_result_gui_plugin/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-03-29 10:05:07.000000 quality-result-gui-1.1.5/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.049575 quality-result-gui-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-23 07:22:42.049575 quality-result-gui-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-23 07:22:42.049575 quality-result-gui-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.037576 quality-result-gui-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/quality_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/api/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/api/types/quality_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/layer_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_data_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_error_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_error_manager_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_error_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29049 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/quality_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_fatal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_warning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_result_gui.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/style/default_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/style/quality_layer_error_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_error_tree_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/utils/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui/utils/styling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.041576 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 07:22:42.000000 quality-result-gui-1.1.6/src/quality_result_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/example_quality_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/mock_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/metadata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/i18n/fi.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:22:42.045575 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-23 07:22:29.000000 quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg
```

### Comparing `quality-result-gui-1.1.5/CHANGELOG.md` & `quality-result-gui-1.1.6/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## [1.1.6] - 2023-05-23
+
+- Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
+
 ## [1.1.5] - 2023-03-29
 
 - Fix: Do not zoom to error when geometry is null geometry
 
 ## [1.1.4] - 2023-03-08
 
 - Fix: Show correct error count when errors are filtered
@@ -63,7 +67,8 @@
 [1.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.0.0
 [1.1.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.0
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
+[1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
```

### Comparing `quality-result-gui-1.1.5/LICENSE` & `quality-result-gui-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/PKG-INFO` & `quality-result-gui-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quality-result-gui
-Version: 1.1.5
+Version: 1.1.6
 Summary: QGIS plugin for visualizing quality check results.
 Home-page: https://github.com/nlsfi/quality-result-gui
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/quality-result-gui/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -95,14 +95,18 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [1.1.6] - 2023-05-23
+
+- Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
+
 ## [1.1.5] - 2023-03-29
 
 - Fix: Do not zoom to error when geometry is null geometry
 
 ## [1.1.4] - 2023-03-08
 
 - Fix: Show correct error count when errors are filtered
@@ -162,7 +166,8 @@
 [1.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.0.0
 [1.1.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.0
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
+[1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
```

### Comparing `quality-result-gui-1.1.5/README.md` & `quality-result-gui-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/setup.cfg` & `quality-result-gui-1.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui/api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,7 @@
 #  quality-result-gui is distributed in the hope that it will be
 #  useful, but WITHOUT ANY WARRANTY; without even the implied warranty
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with quality-result-gui. If not, see <https://www.gnu.org/licenses/>.
-
-
-__version__ = "1.1.5"
-
-
-from enum import Enum, auto
-
-
-class SelectionType(Enum):
-    LeftClick = auto()
-    RightClick = auto()
-    Keyboard = auto()
-    Other = auto()
```

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/api/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/api/quality_api_client.py` & `quality-result-gui-1.1.6/src/quality_result_gui/api/quality_api_client.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/api/types/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/api/types/quality_error.py` & `quality-result-gui-1.1.6/src/quality_result_gui/api/types/quality_error.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/configuration/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/quality_data_fetcher.py` & `quality-result-gui-1.1.6/src/quality_result_gui/quality_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/quality_error_manager.py` & `quality-result-gui-1.1.6/src/quality_result_gui/quality_error_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,32 @@
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with quality-result-gui. If not, see <https://www.gnu.org/licenses/>.
 
 
-from typing import TYPE_CHECKING, Optional, cast
+from typing import TYPE_CHECKING, Dict, Optional, cast
 
 from qgis.gui import QgisInterface
 from qgis.PyQt.QtCore import QObject, pyqtSignal
 from qgis.utils import iface as utils_iface
 from qgis_plugin_tools.tools.i18n import tr
 
 from quality_result_gui import SelectionType
 from quality_result_gui.api.types.quality_error import QualityError
+from quality_result_gui.layer_mapping import LayerMapping
 from quality_result_gui.quality_data_fetcher import (
     CHECK_STATUS_LABELS,
     BackgroundQualityResultsFetcher,
     CheckStatus,
 )
+from quality_result_gui.quality_error_manager_settings import (
+    QualityResultManagerSettings,
+)
 from quality_result_gui.quality_error_visualizer import QualityErrorVisualizer
 from quality_result_gui.quality_errors_filters import (
     AbstractQualityErrorFilter,
     AttributeFilter,
     ErrorTypeFilter,
     FeatureTypeFilter,
 )
@@ -173,7 +177,12 @@
         self.dock_widget.hide()
         self.visualizer.remove_quality_error_layer()
 
     def add_filter(self, filter: AbstractQualityErrorFilter) -> None:
         filter.filters_changed.connect(self.dock_widget._update_filter_menu_icon_state)
         self.dock_widget.filter_menu.add_filter_menu(filter.menu)
         self._filter_model.add_filter(filter)
+
+    def set_layer_mapping(self, layer_mapping: Dict[str, str]) -> None:
+        QualityResultManagerSettings.get().set_layer_mapping(
+            LayerMapping(layer_map=layer_mapping)
+        )
```

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/quality_error_visualizer.py` & `quality-result-gui-1.1.6/src/quality_result_gui/quality_error_visualizer.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/quality_errors_filters.py` & `quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 from qgis.PyQt.QtCore import QObject, QSignalBlocker, pyqtSignal
 from qgis.PyQt.QtGui import QMouseEvent
 from qgis.PyQt.QtWidgets import QAction, QMenu
 from qgis_plugin_tools.tools.i18n import tr
 
 from quality_result_gui.api.types.quality_error import ERROR_TYPE_LABEL, QualityError
+from quality_result_gui.quality_error_manager_settings import (
+    QualityResultManagerSettings,
+)
 from quality_result_gui.quality_errors_tree_model import QualityErrorTreeItemType
 
 if TYPE_CHECKING:
     from qgis.PyQt.QtWidgets import QWidget
 
     from quality_result_gui.api.types.quality_error import QualityErrorsByPriority
 
@@ -379,21 +382,26 @@
     ) -> None:
         """
 
         Args:
             quality_errors (List[&quot;QualityErrorsByPriority&quot;]): _description_
         """
         feature_types_in_errors = {  # Dict[filter_value, filter_label]
-            errors.feature_type: errors.feature_type
+            errors.feature_type: self._get_label_value(errors.feature_type)
             for errors_by_feature_type in quality_errors
             for errors in errors_by_feature_type.errors
         }
 
         self._refresh_filters(feature_types_in_errors)
 
+    def _get_label_value(self, feature_type: str) -> str:
+        return QualityResultManagerSettings.get().layer_mapping.get_layer_alias(
+            feature_type
+        )
+
 
 class AttributeFilter(AbstractQualityErrorFilter):
     """Filter for the Attribute Errors of the Quality errors.
 
     Adds filterable Attribute names dynamically based on the current errors received.
     update_filter_from_errors slot should be connected to the signal that transmits
     received errors.
@@ -414,16 +422,23 @@
 
         return True
 
     def update_filter_from_errors(
         self, quality_errors: List["QualityErrorsByPriority"]
     ) -> None:
         attribute_names_in_errors = {  # Dict[filter_value, filter_label]
-            error.attribute_name: error.attribute_name
+            error.attribute_name: self._get_label_value(
+                error.feature_type, error.attribute_name
+            )
             for errors_by_priority in quality_errors
             for errors_by_feature_type in errors_by_priority.errors
             for errors_by_feature in errors_by_feature_type.errors
             for error in errors_by_feature.errors
             if error.attribute_name
         }
 
         self._refresh_filters(attribute_names_in_errors)
+
+    def _get_label_value(self, feature_type: str, attribute_name: str) -> str:
+        return QualityResultManagerSettings.get().layer_mapping.get_field_alias(
+            feature_type, attribute_name
+        )
```

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/quality_errors_tree_model.py` & `quality-result-gui-1.1.6/src/quality_result_gui/quality_errors_tree_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 from quality_result_gui.api.types.quality_error import (
     ERROR_PRIORITY_LABEL,
     ERROR_TYPE_LABEL,
     QualityError,
     QualityErrorPriority,
     QualityErrorsByPriority,
 )
+from quality_result_gui.quality_error_manager_settings import (
+    QualityResultManagerSettings,
+)
 
 if TYPE_CHECKING:
     from qgis.core import QgsRectangle
 
     from quality_result_gui.quality_errors_filters import AbstractQualityErrorFilter
 
 LOGGER = logging.getLogger(__name__)
@@ -229,17 +232,19 @@
             return (self.item_type, self._item_data[index])
 
         if role == Qt.DisplayRole and column == ModelColumn.TYPE_OR_ID:
             if self.item_type == QualityErrorTreeItemType.PRIORITY:
                 column_data = ERROR_PRIORITY_LABEL[QualityErrorPriority(item_data)]
 
             elif self.item_type == QualityErrorTreeItemType.FEATURE_TYPE:
-                column_data = item_data
-                # TODO: how to configurate custom data mapping
-                # column_data = common.FEATURE_TYPE_NAMES[item_data]
+                column_data = (
+                    QualityResultManagerSettings.get().layer_mapping.get_layer_alias(
+                        item_data
+                    )
+                )
 
             elif self.item_type == QualityErrorTreeItemType.FEATURE:
                 column_data = item_data[1][:8]
 
             elif self.item_type == QualityErrorTreeItemType.ERROR:
                 quality_error = cast(QualityError, item_data)
                 column_data = ERROR_TYPE_LABEL[quality_error.error_type]
@@ -442,15 +447,14 @@
             and item.item_type == QualityErrorTreeItemType.ERROR
         ):
             return super().flags(index) | Qt.ItemIsUserCheckable
 
         return super().flags(index)
 
     def refresh_model(self, quality_errors: List[QualityErrorsByPriority]) -> None:
-
         updated_quality_error_ids = {
             error.unique_identifier
             for errors_by_priority in quality_errors
             for error in errors_by_priority.get_all_errors()
         }
 
         current_quality_error_ids = set()
@@ -567,15 +571,14 @@
 
             self._add_item_to_model(
                 quality_error_item,
                 feature_item,
             )
 
     def _get_index_for_item(self, item: QualityErrorTreeItem) -> QModelIndex:
-
         if item.item_type == QualityErrorTreeItemType.HEADER:
             return QModelIndex()
         else:
             item_parent = item.parent()
             if item_parent is None:
                 raise ValueError
             return self.index(item.row(), 0, self._get_index_for_item(item_parent))
```

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/quality_layer.py` & `quality-result-gui-1.1.6/src/quality_result_gui/quality_layer.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/resources/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_error_fatal.svg` & `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_fatal.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_error_info.svg` & `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_info.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_error_warning.svg` & `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_error_warning.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/resources/icons/quality_result_gui.svg` & `quality-result-gui-1.1.6/src/quality_result_gui/resources/icons/quality_result_gui.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/style/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui/style/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/style/default_style.py` & `quality-result-gui-1.1.6/src/quality_result_gui/style/default_style.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/style/quality_layer_error_symbol.py` & `quality-result-gui-1.1.6/src/quality_result_gui/style/quality_layer_error_symbol.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_error_tree_view.py` & `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_error_tree_view.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_errors_dock.py` & `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_errors_dock.ui` & `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_dock.ui`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py` & `quality-result-gui-1.1.6/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/utils/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/utils/layer_utils.py` & `quality-result-gui-1.1.6/src/quality_result_gui/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui/utils/styling_utils.py` & `quality-result-gui-1.1.6/src/quality_result_gui/utils/styling_utils.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui.egg-info/PKG-INFO` & `quality-result-gui-1.1.6/src/quality_result_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quality-result-gui
-Version: 1.1.5
+Version: 1.1.6
 Summary: QGIS plugin for visualizing quality check results.
 Home-page: https://github.com/nlsfi/quality-result-gui
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/quality-result-gui/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -95,14 +95,18 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [1.1.6] - 2023-05-23
+
+- Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
+
 ## [1.1.5] - 2023-03-29
 
 - Fix: Do not zoom to error when geometry is null geometry
 
 ## [1.1.4] - 2023-03-08
 
 - Fix: Show correct error count when errors are filtered
@@ -162,7 +166,8 @@
 [1.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.0.0
 [1.1.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.0
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
+[1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
```

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui.egg-info/SOURCES.txt` & `quality-result-gui-1.1.6/src/quality_result_gui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/quality_result_gui/__init__.py
+src/quality_result_gui/layer_mapping.py
 src/quality_result_gui/py.typed
 src/quality_result_gui/quality_data_fetcher.py
 src/quality_result_gui/quality_error_manager.py
+src/quality_result_gui/quality_error_manager_settings.py
 src/quality_result_gui/quality_error_visualizer.py
 src/quality_result_gui/quality_errors_filters.py
 src/quality_result_gui/quality_errors_tree_model.py
 src/quality_result_gui/quality_layer.py
 src/quality_result_gui.egg-info/PKG-INFO
 src/quality_result_gui.egg-info/SOURCES.txt
 src/quality_result_gui.egg-info/dependency_links.txt
```

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/__init__.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/mock_api_client.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/mock_api_client.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/dev_tools/response_parser.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/dev_tools/response_parser.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/env.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/env.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/metadata.txt` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/metadata.txt`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/plugin.py` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-1.1.5/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg` & `quality-result-gui-1.1.6/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg`

 * *Files identical despite different names*

