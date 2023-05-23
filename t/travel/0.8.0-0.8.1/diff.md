# Comparing `tmp/travel-0.8.0.tar.gz` & `tmp/travel-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/travel-0.8.0.tar", last modified: Sat Nov 12 19:19:50 2022, max compression
+gzip compressed data, was "travel-0.8.1.tar", last modified: Tue May 23 09:55:44 2023, max compression
```

## Comparing `travel-0.8.0.tar` & `travel-0.8.1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-12 19:19:49.000000 travel-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5298 2022-11-12 19:19:50.000000 travel-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-11-12 19:19:49.000000 travel-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-12 19:19:49.000000 travel-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-12 19:19:50.000000 travel-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-12 19:19:50.000000 travel-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-11-12 19:19:49.000000 travel-0.8.0/travel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-11-12 19:19:49.000000 travel-0.8.0/travel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/adder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/cli/console/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/console/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/packer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/planner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/setupper.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/takeoffer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-11-12 19:19:49.000000 travel-0.8.0/travel/cli/utils/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/config/environment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/environment/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/environment/python.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/config/sanitizers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/sanitizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/sanitizers/asserter.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/sanitizers/name_sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/sanitizers/pip_sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/sanitizers/python_sanitizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/config/subconfigs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/subconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/subconfigs/pip.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-11-12 19:19:49.000000 travel-0.8.0/travel/config/subconfigs/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/custom/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/custom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/custom/scopes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/custom/scopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-11-12 19:19:49.000000 travel-0.8.0/travel/custom/scopes/scoped_venvs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/custom/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/custom/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-11-12 19:19:49.000000 travel-0.8.0/travel/custom/tasks/performer.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-11-12 19:19:49.000000 travel-0.8.0/travel/custom/tasks/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7504 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/base_venv.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/executable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel/tools/outputs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/outputs/latest_updates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/pip.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/python.py
--rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-11-12 19:19:49.000000 travel-0.8.0/travel/tools/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:19:50.000000 travel-0.8.0/travel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5298 2022-11-12 19:19:50.000000 travel-0.8.0/travel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-11-12 19:19:50.000000 travel-0.8.0/travel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 19:19:50.000000 travel-0.8.0/travel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-12 19:19:50.000000 travel-0.8.0/travel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-12 19:19:50.000000 travel-0.8.0/travel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-12 19:19:50.000000 travel-0.8.0/travel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.780441 travel-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-05-23 09:55:42.000000 travel-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 09:55:42.000000 travel-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-23 09:55:44.780441 travel-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-23 09:55:42.000000 travel-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 09:55:42.000000 travel-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:55:44.780441 travel-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-23 09:55:43.000000 travel-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.772441 travel-0.8.1/travel/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-23 09:55:42.000000 travel-0.8.1/travel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-23 09:55:42.000000 travel-0.8.1/travel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.772441 travel-0.8.1/travel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.772441 travel-0.8.1/travel/cli/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/console/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/setupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/takeoffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.772441 travel-0.8.1/travel/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-23 09:55:42.000000 travel-0.8.1/travel/cli/utils/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.776441 travel-0.8.1/travel/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.776441 travel-0.8.1/travel/config/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/environment/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/environment/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.776441 travel-0.8.1/travel/config/sanitizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/sanitizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/sanitizers/asserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/sanitizers/name_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/sanitizers/pip_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/sanitizers/python_sanitizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.776441 travel-0.8.1/travel/config/subconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/subconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/subconfigs/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 09:55:42.000000 travel-0.8.1/travel/config/subconfigs/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.776441 travel-0.8.1/travel/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/custom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.776441 travel-0.8.1/travel/custom/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/custom/scopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-23 09:55:42.000000 travel-0.8.1/travel/custom/scopes/scoped_venvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.776441 travel-0.8.1/travel/custom/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/custom/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-23 09:55:42.000000 travel-0.8.1/travel/custom/tasks/performer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 09:55:42.000000 travel-0.8.1/travel/custom/tasks/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.780441 travel-0.8.1/travel/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/base_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/executable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.780441 travel-0.8.1/travel/tools/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/outputs/latest_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 09:55:42.000000 travel-0.8.1/travel/tools/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:55:44.772441 travel-0.8.1/travel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-23 09:55:44.000000 travel-0.8.1/travel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-23 09:55:44.000000 travel-0.8.1/travel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:55:44.000000 travel-0.8.1/travel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 09:55:44.000000 travel-0.8.1/travel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 09:55:44.000000 travel-0.8.1/travel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:55:44.000000 travel-0.8.1/travel.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `travel-0.8.0/PKG-INFO` & `travel-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: travel
-Version: 0.8.0
+Version: 0.8.1
 Summary: A software manager for easy development and distribution of Python code
 Home-page: https://github.com/travel-tools/travel
 Author: Federico Pugliese
 Author-email: federico.pugliese.wr@gmail.com
 License: Apache Software License, Version 2.0
 Description: # Travel
```

### Comparing `travel-0.8.0/README.md` & `travel-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/setup.py` & `travel-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     readme = f.read()
 
 
 # Package configuration
 _NAME = "travel"
 setup(
     name=_NAME,
-    version="0.8.0",
+    version="0.8.1",
     description="A software manager for easy development and distribution of Python code",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     python_requires=">=3.7",
     entry_points={
         'console_scripts': [
```

### Comparing `travel-0.8.0/travel/__init__.py` & `travel-0.8.1/travel/__init__.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/__main__.py` & `travel-0.8.1/travel/__main__.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/adder.py` & `travel-0.8.1/travel/cli/adder.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/base.py` & `travel-0.8.1/travel/cli/base.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/cleaner.py` & `travel-0.8.1/travel/cli/cleaner.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/configurer.py` & `travel-0.8.1/travel/cli/configurer.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/packer.py` & `travel-0.8.1/travel/cli/packer.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/planner.py` & `travel-0.8.1/travel/cli/planner.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/setupper.py` & `travel-0.8.1/travel/cli/setupper.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/cli/takeoffer.py` & `travel-0.8.1/travel/cli/takeoffer.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/config/bag.py` & `travel-0.8.1/travel/config/bag.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/config/environment/configuration.py` & `travel-0.8.1/travel/config/environment/configuration.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/config/environment/python.py` & `travel-0.8.1/travel/config/environment/python.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/config/reader.py` & `travel-0.8.1/travel/config/reader.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/config/sanitizers/pip_sanitizer.py` & `travel-0.8.1/travel/config/sanitizers/pip_sanitizer.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/config/subconfigs/scopes.py` & `travel-0.8.1/travel/config/subconfigs/scopes.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/custom/scopes/scoped_venvs.py` & `travel-0.8.1/travel/custom/scopes/scoped_venvs.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/custom/tasks/performer.py` & `travel-0.8.1/travel/custom/tasks/performer.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/custom/tasks/task.py` & `travel-0.8.1/travel/custom/tasks/task.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/tools/base_venv.py` & `travel-0.8.1/travel/tools/base_venv.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/tools/outputs/latest_updates.py` & `travel-0.8.1/travel/tools/outputs/latest_updates.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/tools/pip.py` & `travel-0.8.1/travel/tools/pip.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/tools/python.py` & `travel-0.8.1/travel/tools/python.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/tools/shell.py` & `travel-0.8.1/travel/tools/shell.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel/tools/venv.py` & `travel-0.8.1/travel/tools/venv.py`

 * *Files identical despite different names*

### Comparing `travel-0.8.0/travel.egg-info/PKG-INFO` & `travel-0.8.1/travel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: travel
-Version: 0.8.0
+Version: 0.8.1
 Summary: A software manager for easy development and distribution of Python code
 Home-page: https://github.com/travel-tools/travel
 Author: Federico Pugliese
 Author-email: federico.pugliese.wr@gmail.com
 License: Apache Software License, Version 2.0
 Description: # Travel
```

### Comparing `travel-0.8.0/travel.egg-info/SOURCES.txt` & `travel-0.8.1/travel.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 travel/__init__.py
 travel/__main__.py
 travel.egg-info/PKG-INFO
```

