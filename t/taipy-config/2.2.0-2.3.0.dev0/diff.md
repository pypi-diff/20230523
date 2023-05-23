# Comparing `tmp/taipy-config-2.2.0.tar.gz` & `tmp/taipy-config-2.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-config-2.2.0.tar", last modified: Wed Apr 12 08:49:33 2023, max compression
+gzip compressed data, was "taipy-config-2.3.0.dev0.tar", last modified: Tue May 23 11:54:05 2023, max compression
```

## Comparing `taipy-config-2.2.0.tar` & `taipy-config-2.3.0.dev0.tar`

### file list

```diff
@@ -1,59 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.866582 taipy-config-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-12 08:49:19.000000 taipy-config-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 08:49:19.000000 taipy-config-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-12 08:49:33.866582 taipy-config-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-12 08:49:19.000000 taipy-config-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:49:33.866582 taipy-config-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 08:49:19.000000 taipy-config-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.846582 taipy-config-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.850582 taipy-config-2.2.0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.854582 taipy-config-2.2.0/src/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_config_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_toml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.854582 taipy-config-2.2.0/src/taipy/config/checker/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.858582 taipy-config-2.2.0/src/taipy/config/checker/_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/_auth_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/issue_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_classproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_config_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_template_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_validate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    33812 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/config/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/config/global_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/global_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/global_app/global_app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/section.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/unique_section.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/logger/_taipy_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.866582 taipy-config-2.2.0/src/taipy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:49:25.000000 taipy-config-2.2.0/src/taipy_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.220262 taipy-config-2.3.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.224262 taipy-config-2.3.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.224262 taipy-config-2.3.0.dev0/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.224262 taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/_cli/_base_cli/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.228262 taipy-config-2.3.0.dev0/src/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.228262 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/_comparator_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/_config_comparator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.232262 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_toml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.232262 taipy-config-2.3.0.dev0/src/taipy/config/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.232262 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/checker/issue_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_config_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_template_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/_validate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/common/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35297 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/config/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/config/global_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/global_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/global_app/global_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/unique_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 11:53:50.000000 taipy-config-2.3.0.dev0/src/taipy/logger/_taipy_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:54:05.236262 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:53:56.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 11:54:05.000000 taipy-config-2.3.0.dev0/src/taipy_config.egg-info/top_level.txt
```

### Comparing `taipy-config-2.2.0/LICENSE` & `taipy-config-2.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/PKG-INFO` & `taipy-config-2.3.0.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.2.0
+Version: 2.3.0.dev0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Taipy config
 
 ## License
@@ -72,9 +71,10 @@
     - `tests`: Unit tests following the `taipy/` structure.
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-config_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy-config_.
 - `INSTALLATION.md`: Instructions to install _taipy-config_.
 - `LICENSE`: The Apache 2.0 License.
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies.
 - `README.md`: Current file.
+- `contributors.txt`: The list of contributors.
 - `setup.py`: The setup script managing building, distributing, and installing _taipy-config_.
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-config-2.2.0/README.md` & `taipy-config-2.3.0.dev0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -51,9 +51,10 @@
     - `tests`: Unit tests following the `taipy/` structure.
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-config_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy-config_.
 - `INSTALLATION.md`: Instructions to install _taipy-config_.
 - `LICENSE`: The Apache 2.0 License.
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies.
 - `README.md`: Current file.
+- `contributors.txt`: The list of contributors.
 - `setup.py`: The setup script managing building, distributing, and installing _taipy-config_.
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-config-2.2.0/setup.py` & `taipy-config-2.3.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     description="A Taipy package dedicated to easily configure a Taipy application.",
     install_requires=requirements,
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     license="Apache License 2.0",
```

### Comparing `taipy-config-2.2.0/src/taipy/__init__.py` & `taipy-config-2.3.0.dev0/src/taipy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,32 +9,43 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from importlib.util import find_spec
 
 if find_spec("taipy"):
     if find_spec("taipy.config"):
-        from taipy.config import Config
-        from taipy.config import Scope
-        from taipy.config import Frequency
+        from taipy.config import Config, Frequency, Scope
 
     if find_spec("taipy.core"):
+        from taipy.core._core import Core
+        from taipy.core.cycle.cycle import Cycle
+        from taipy.core.cycle.cycle_id import CycleId
+        from taipy.core.data.data_node import DataNode
+        from taipy.core.data.data_node_id import DataNodeId
+        from taipy.core.job.job import Job
+        from taipy.core.job.job_id import JobId
+        from taipy.core.job.status import Status
+        from taipy.core.pipeline.pipeline import Pipeline
+        from taipy.core.pipeline.pipeline_id import PipelineId
+        from taipy.core.scenario.scenario import Scenario
+        from taipy.core.scenario.scenario_id import ScenarioId
         from taipy.core.taipy import (
             cancel_job,
             clean_all_entities,
             clean_all_entities_by_version,
             compare_scenarios,
             create_pipeline,
             create_scenario,
             delete,
             delete_job,
             delete_jobs,
             export_scenario,
             get,
             get_cycles,
+            get_cycles_scenarios,
             get_data_nodes,
             get_jobs,
             get_latest_job,
             get_parents,
             get_pipelines,
             get_primary,
             get_primary_scenarios,
@@ -46,23 +57,16 @@
             subscribe_pipeline,
             subscribe_scenario,
             tag,
             unsubscribe_pipeline,
             unsubscribe_scenario,
             untag,
         )
-        from taipy.core._core import Core
-        from taipy.core.common.alias import CycleId, DataNodeId, JobId, PipelineId, ScenarioId, TaskId
-        from taipy.core.cycle.cycle import Cycle
-        from taipy.core.data.data_node import DataNode
-        from taipy.core.job.job import Job
-        from taipy.core.job.status import Status
-        from taipy.core.pipeline.pipeline import Pipeline
-        from taipy.core.scenario.scenario import Scenario
         from taipy.core.task.task import Task
+        from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
```

### Comparing `taipy-config-2.2.0/src/taipy/config/__init__.py` & `taipy-config-2.3.0.dev0/src/taipy/config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,47 +19,57 @@
 """
 
 import os
 from typing import List
 
 from .checker.issue import Issue
 from .checker.issue_collector import IssueCollector
-from .section import Section
-from .unique_section import UniqueSection
+from .common.frequency import Frequency
+from .common.scope import Scope
 from .config import Config
 from .global_app.global_app_config import GlobalAppConfig
-from .common.scope import Scope
-from .common.frequency import Frequency
+from .section import Section
+from .unique_section import UniqueSection
 from .version import _get_version
 
 __version__ = _get_version()
 
 
 def _config_doc(func):
-    def func_with_doc(section, attribute_name, default, configuration_methods):
+    def func_with_doc(section, attribute_name, default, configuration_methods, add_to_unconflicted_sections=False):
         if os.environ.get("GENERATING_TAIPY_DOC", None) and os.environ["GENERATING_TAIPY_DOC"] == "true":
-            with open('config_doc.txt', 'a') as f:
+            with open("config_doc.txt", "a") as f:
                 from inspect import signature
+
                 for exposed_configuration_method, configuration_method in configuration_methods:
                     annotation = "    @staticmethod\n"
                     sign = "    def " + exposed_configuration_method + str(signature(configuration_method)) + ":\n"
                     doc = '        """' + configuration_method.__doc__ + '"""\n'
-                    content = '        pass\n\n'
+                    content = "        pass\n\n"
                     f.write(annotation + sign + doc + content)
-        return func(section, attribute_name, default, configuration_methods)
+        return func(section, attribute_name, default, configuration_methods, add_to_unconflicted_sections)
 
     return func_with_doc
 
 
 @_config_doc
-def _inject_section(section_clazz, attribute_name: str, default: Section, configuration_methods: List[tuple]):
+def _inject_section(
+    section_clazz,
+    attribute_name: str,
+    default: Section,
+    configuration_methods: List[tuple],
+    add_to_unconflicted_sections: bool = False,
+):
     Config._register_default(default)
 
     if issubclass(section_clazz, UniqueSection):
         setattr(Config, attribute_name, Config.unique_sections[section_clazz.name])
     elif issubclass(section_clazz, Section):
         setattr(Config, attribute_name, Config.sections[section_clazz.name])
     else:
         raise TypeError
 
+    if add_to_unconflicted_sections:
+        Config._comparator._add_unconflicted_section(section_clazz.name)
+
     for exposed_configuration_method, configuration_method in configuration_methods:
         setattr(Config, exposed_configuration_method, configuration_method)
```

### Comparing `taipy-config-2.2.0/src/taipy/config/_base_serializer.py` & `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_base_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 import inspect
 import re
 import types
 from abc import abstractmethod
 from datetime import datetime, timedelta
 from typing import Any, Dict, Optional
 
-from . import Section
-from ._config import _Config
-from .common._template_handler import _TemplateHandler
-from .common._validate_id import _validate_id
-from .common.frequency import Frequency
-from .common.scope import Scope
-from .exceptions.exceptions import LoadingError
-from .global_app.global_app_config import GlobalAppConfig
-from .unique_section import UniqueSection
+from .._config import _Config
+from ..common._template_handler import _TemplateHandler
+from ..common._validate_id import _validate_id
+from ..common.frequency import Frequency
+from ..common.scope import Scope
+from ..exceptions.exceptions import LoadingError
+from ..global_app.global_app_config import GlobalAppConfig
+from ..section import Section
+from ..unique_section import UniqueSection
 
 
 class _BaseSerializer(object):
     """Base serializer class for taipy configuration."""
 
     _GLOBAL_NODE_NAME = "TAIPY"
     _section_class = {_GLOBAL_NODE_NAME: GlobalAppConfig}
```

### Comparing `taipy-config-2.2.0/src/taipy/config/_config.py` & `taipy-config-2.3.0.dev0/src/taipy/config/_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/_json_serializer.py` & `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_json_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import json  # type: ignore
 
+from .._config import _Config
+from ..exceptions.exceptions import LoadingError
 from ._base_serializer import _BaseSerializer
-from ._config import _Config
-from .exceptions.exceptions import LoadingError
 
 
 class _JsonSerializer(_BaseSerializer):
     """Convert configuration from JSON representation to Python Dict and reciprocally."""
 
     @classmethod
     def _write(cls, configuration: _Config, filename: str):
```

### Comparing `taipy-config-2.2.0/src/taipy/config/_toml_serializer.py` & `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/_toml_serializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import toml  # type: ignore
 
+from .._config import _Config
+from ..exceptions.exceptions import LoadingError
 from ._base_serializer import _BaseSerializer
-from ._config import _Config
-from .exceptions.exceptions import LoadingError
 
 
 class _TomlSerializer(_BaseSerializer):
     """Convert configuration from TOML representation to Python Dict and reciprocally."""
 
     @classmethod
     def _write(cls, configuration: _Config, filename: str):
```

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/__init__.py` & `taipy-config-2.3.0.dev0/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/_checker.py` & `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/_checkers/__init__.py` & `taipy-config-2.3.0.dev0/src/taipy/config/_config_comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/_checkers/_auth_config_checker.py` & `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/_checkers/_config_checker.py` & `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from typing import Any, List
 
 from ..._config import _Config
 from ..issue_collector import IssueCollector
 
 
 class _ConfigChecker:
+
+    _PREDEFINED_PROPERTIES_KEYS = ["_entity_owner"]
+
     def __init__(self, config: _Config, collector):
         self._collector = collector
         self._config = config
 
     @abc.abstractmethod
     def _check(self) -> IssueCollector:
         raise NotImplementedError
@@ -35,27 +38,36 @@
         self._collector._add_info(field, value, message, self.__class__.__name__)
 
     def _check_children(self, parent_config_class, config_id: str, config_key: str, config_value, child_config_class):
         if not config_value:
             self._warning(
                 config_key,
                 config_value,
-                f"{config_key} field of {parent_config_class.__name__} {config_id} is empty.",
+                f"{config_key} field of {parent_config_class.__name__} `{config_id}` is empty.",
             )
         else:
             if not (
                 isinstance(config_value, List) and all(map(lambda x: isinstance(x, child_config_class), config_value))
             ):
                 self._error(
                     config_key,
                     config_value,
-                    f"{config_key} field of {parent_config_class.__name__} {config_id} must be populated with a list "
+                    f"{config_key} field of {parent_config_class.__name__} `{config_id}` must be populated with a list "
                     f"of {child_config_class.__name__} objects.",
                 )
 
     def _check_existing_config_id(self, config):
         if not config.id:
             self._error(
                 "config_id",
                 config.id,
-                f"config_id of {config.__name__} {config.id} is empty.",
+                f"config_id of {config.__class__.__name__} `{config.id}` is empty.",
             )
+
+    def _check_if_entity_property_key_used_is_predefined(self, config):
+        for key, value in config._properties.items():
+            if key in self._PREDEFINED_PROPERTIES_KEYS:
+                self._error(
+                    key,
+                    value,
+                    f"Properties of {config.__class__.__name__} `{config.id}` cannot have `{key}` as its property.",
+                )
```

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py` & `taipy-config-2.3.0.dev0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from ..._config import _Config
-from ._config_checker import _ConfigChecker
-from ..issue_collector import IssueCollector
-from ...global_app.global_app_config import GlobalAppConfig
-from ...exceptions.exceptions import InconsistentEnvVariableError
 from ...common._template_handler import _TemplateHandler as tpl
+from ...exceptions.exceptions import InconsistentEnvVariableError
+from ...global_app.global_app_config import GlobalAppConfig
+from ..issue_collector import IssueCollector
+from ._config_checker import _ConfigChecker
 
 
 class _GlobalConfigChecker(_ConfigChecker):
     def __init__(self, config: _Config, collector: IssueCollector):
         super().__init__(config, collector)
 
     def _check(self) -> IssueCollector:
@@ -40,9 +40,10 @@
             except InconsistentEnvVariableError:
                 pass
         if isinstance(value, bool):
             return
         self._error(
             global_config._CLEAN_ENTITIES_ENABLED_KEY,
             value,
-            f"{global_config._CLEAN_ENTITIES_ENABLED_KEY} field must be populated with a boolean value.",
+            f"`{global_config._CLEAN_ENTITIES_ENABLED_KEY}` field of GlobalAppConfig "
+            "must be populated with a boolean value.",
         )
```

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/issue.py` & `taipy-config-2.3.0.dev0/src/taipy/config/unique_section.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,29 +5,21 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-from dataclasses import dataclass
-from typing import Any, Optional
+from abc import ABC
 
+from .common._validate_id import _validate_id
+from .section import Section
 
-@dataclass
-class Issue:
-    """
-    An issue detected in the configuration.
 
-    Attributes:
-        level (str): Level of the issue among ERROR, WARNING, INFO.
-        field (str): Configuration field on which the issue has been detected.
-        value (Any): Value of the field on which the issue has been detected.
-        message (str): Human readable message to help the user fix the issue.
-        tag (Optional[str]): Optional tag to be used to filter issues.
+class UniqueSection(Section, ABC):
+    """A UniqueSection is a configuration `Section^` that can have only one instance.
+
+    A UniqueSection is only defined by the section name.
     """
 
-    level: str
-    field: str
-    value: Any
-    message: str
-    tag: Optional[str]
+    def __init__(self, **properties):
+        super().__init__(_validate_id(self.name), **properties)
```

### Comparing `taipy-config-2.2.0/src/taipy/config/checker/issue_collector.py` & `taipy-config-2.3.0.dev0/src/taipy/config/checker/issue_collector.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/common/_classproperty.py` & `taipy-config-2.3.0.dev0/src/taipy/config/common/_classproperty.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/common/_config_blocker.py` & `taipy-config-2.3.0.dev0/src/taipy/config/common/_config_blocker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/common/_repr_enum.py` & `taipy-config-2.3.0.dev0/src/taipy/config/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/common/_template_handler.py` & `taipy-config-2.3.0.dev0/src/taipy/config/common/_template_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/common/_validate_id.py` & `taipy-config-2.3.0.dev0/src/taipy/config/common/_validate_id.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/common/frequency.py` & `taipy-config-2.3.0.dev0/src/taipy/config/common/frequency.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/common/scope.py` & `taipy-config-2.3.0.dev0/src/taipy/config/common/scope.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/config.py` & `taipy-config-2.3.0.dev0/src/taipy/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # specific language governing permissions and limitations under the License.
 
 import os
 from typing import Dict, Union
 
 from ..logger._taipy_logger import _TaipyLogger
 from ._config import _Config
-from ._json_serializer import _JsonSerializer
-from ._toml_serializer import _TomlSerializer
+from ._config_comparator._config_comparator import _ConfigComparator
+from ._serializer._json_serializer import _JsonSerializer
+from ._serializer._toml_serializer import _TomlSerializer
 from .checker._checker import _Checker
 from .checker.issue_collector import IssueCollector
 from .common._classproperty import _Classproperty
 from .common._config_blocker import _ConfigBlocker
-from .exceptions.exceptions import ConfigurationIssueError
 from .global_app.global_app_config import GlobalAppConfig
 from .section import Section
 from .unique_section import UniqueSection
 
 
 class Config:
     """Configuration singleton."""
@@ -35,14 +35,15 @@
     _python_config = _Config()
     _file_config = None
     _env_file_config = None
     _applied_config = _Config._default_config()
     _collector = IssueCollector()
     _serializer = _TomlSerializer()
     __json_serializer = _JsonSerializer()
+    _comparator: _ConfigComparator = _ConfigComparator()
 
     @_Classproperty
     def unique_sections(cls) -> Dict[str, UniqueSection]:
         """Return all unique sections."""
         return cls._applied_config._unique_sections
 
     @_Classproperty
@@ -184,18 +185,15 @@
         if isinstance(default_section, UniqueSection):
             if cls._default_config._unique_sections.get(default_section.name, None):
                 cls._default_config._unique_sections[default_section.name]._update(default_section._to_dict())
             else:
                 cls._default_config._unique_sections[default_section.name] = default_section
         else:
             if def_sections := cls._default_config._sections.get(default_section.name, None):
-                if def_sections.get(default_section.id, None):
-                    def_sections[default_section.id]._update(default_section._to_dict())
-                else:
-                    def_sections[default_section.id] = default_section
+                def_sections[default_section.id] = default_section
             else:
                 cls._default_config._sections[default_section.name] = {default_section.id: default_section}
         cls._serializer._section_class[default_section.name] = default_section.__class__  # type: ignore
         cls.__json_serializer._section_class[default_section.name] = default_section.__class__  # type: ignore
         cls.__compile_configs()
 
     @classmethod
@@ -243,15 +241,15 @@
         for issue in config._collector._warnings:
             cls.__logger.warning(str(issue))
         for issue in config._collector._infos:
             cls.__logger.info(str(issue))
         for issue in config._collector._errors:
             cls.__logger.error(str(issue))
         if len(config._collector._errors) != 0:
-            raise ConfigurationIssueError("Configuration issues found.")
+            raise SystemExit("Configuration errors found. Please check the error log for more information.")
 
     @classmethod
     def _to_json(cls, _config: _Config) -> str:
         return cls.__json_serializer._serialize(_config)
 
     @classmethod
     def _from_json(cls, config_as_str: str) -> _Config:
```

### Comparing `taipy-config-2.2.0/src/taipy/config/config.pyi` & `taipy-config-2.3.0.dev0/src/taipy/config/config.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -6,63 +6,65 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import json
-from typing import Any, Callable, Dict, List, Union, Optional
+from typing import Any, Callable, Dict, List, Optional, Union
+
+from taipy.core.config import DataNodeConfig, JobConfig, PipelineConfig, ScenarioConfig, TaskConfig
 
 from .checker.issue_collector import IssueCollector
 from .common._classproperty import _Classproperty
 from .common._config_blocker import _ConfigBlocker
-from .common.scope import Scope
 from .common.frequency import Frequency
+from .common.scope import Scope
 from .global_app.global_app_config import GlobalAppConfig
 from .section import Section
 from .unique_section import UniqueSection
 
-from taipy.core.config import (
-    DataNodeConfig,
-    JobConfig,
-    TaskConfig,
-    PipelineConfig,
-    ScenarioConfig,
-)
 
 class Config:
+    """Configuration singleton."""
     @_Classproperty
     def unique_sections(cls) -> Dict[str, UniqueSection]:
         """Return all unique sections."""
+
     @_Classproperty
     def sections(cls) -> Dict[str, Dict[str, Section]]:
         """Return all non unique sections."""
+
     @_Classproperty
     def global_config(cls) -> GlobalAppConfig:
         """Return configuration values related to the global application as a `GlobalAppConfig^`."""
+
     @classmethod
     @_ConfigBlocker._check()
     def load(cls, filename):
         """Load a configuration file to replace the current python config and trigger the Config compilation.
+
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     def export(cls, filename):
         """Export a configuration.
 
         The export is done in a toml file.
 
         The exported configuration is taken from the python code configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
             If _filename_ already exists, it is overwritten.
         """
+
     @classmethod
     def backup(cls, filename):
         """Backup a configuration.
 
         The backup is done in a toml file.
 
         The backed up configuration is a compilation from the three possible methods to configure
@@ -70,53 +72,52 @@
         configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
             If _filename_ already exists, it is overwritten.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def restore(cls, filename):
         """Restore a configuration file and replace the current applied configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def override(cls, filename):
         """Load a configuration from a file and overrides the current config.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     def block_update(cls):
         """Block update on the configuration signgleton."""
+
     @classmethod
     def unblock_update(cls):
         """Unblock update on the configuration signgleton."""
+
     @classmethod
     @_ConfigBlocker._check()
-    def _register_default(cls, default_section: Section):
-        """"""
-    @classmethod
-    @_ConfigBlocker._check()
-    def _register(cls, section):
-        """"""
-    @classmethod
     def configure_global_app(
         cls,
-        root_folder: str = ...,
-        storage_folder: str = ...,
-        clean_entities_enabled: Union[bool, str] = ...,
-        **properties: Dict[str, Any],
+        root_folder: str = None,
+        storage_folder: str = None,
+        clean_entities_enabled: Union[bool, str] = None,
+        **properties,
     ) -> GlobalAppConfig:
         """Configure the global application.
+
         Parameters:
             root_folder (Optional[str]): The path of the base folder for the Taipy application.
             storage_folder (Optional[str]): The folder name used to store Taipy data.
                 It is used in conjunction with the root_folder field: the storage path is
                 "<root_folder><storage_folder>".
             clean_entities_enabled (Optional[str]): The field to activate or deactivate the
                 'clean entities' feature. The default value is False.
@@ -130,577 +131,640 @@
 
         This method logs issue messages and returns an issue collector.
 
         Returns:
             Collector containing the info, warning and error issues.
         """
 
-    @_Classproperty
+    @classmethod
+    @_ConfigBlocker._check()
+    def _register_default(cls, default_section: Section):
+        """"""
+
+    @classmethod
+    @_ConfigBlocker._check()
+    def _register(cls, section):
+        """"""
+
+    @classmethod
+    def _override_env_file(cls):
+        """"""
+
+    @classmethod
+    def _to_json(cls, _config: _Config) -> str:
+        """"""
+
+    @classmethod
+    def _from_json(cls, config_as_str: str) -> _Config:
+        """"""
+
+    def job_config(cls) -> JobConfig:
+        """"""
+
     def data_nodes(cls) -> Dict[str, DataNodeConfig]:
-        """Return all data node configurations grouped by id in a dictionary.
+        """"""
 
-        `Config.data_nodes()` is an alias for `Config.sections["DATA_NODE"]`
-        """
+    def tasks(cls) -> Dict[str, TaskConfig]:
+        """"""
+
+    def pipelines(cls) -> Dict[str, PipelineConfig]:
+        """"""
+
+    def scenarios(cls) -> Dict[str, ScenarioConfig]:
+        """"""
 
     @staticmethod
-    def configure_data_node(
+    def configure_scenario(
         id: str,
-        storage_type: str = ...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new data node configuration.
+        pipeline_configs: List[PipelineConfig],
+        frequency: Optional[Frequency] = None,
+        comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
+        **properties,
+    ) -> "ScenarioConfig":
+        """Configure a new scenario configuration.
+
         Parameters:
-            id (str): The unique identifier of the new data node configuration.
-            storage_type (str): The data node configuration storage type. The possible values
-                are _"pickle"_ (which the default value, unless it has been overloaded by the
-                _storage_type_ value set in the default data node configuration
-                (see `(Config.)configure_default_data_node()^`)), _"csv"_, _"excel"_, _"sql_table"_, _"sql"_, _"json"_,
-                _"parquet"_, _"mongo_collection"_, _"in_memory"_, or _"generic"_.
-            scope (Scope^): The scope of the data node configuration. The default value is
-                `Scope.SCENARIO` (or the one specified in
-                `(Config.)configure_default_data_node()^`).
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new scenario configuration.
+            pipeline_configs (List[PipelineConfig^]): The list of pipeline configurations used
+                by this new scenario configuration.
+            frequency (Optional[Frequency^]): The scenario frequency.<br/>
+                It corresponds to the recurrence of the scenarios instantiated from this
+                configuration. Based on this frequency each scenario will be attached to the
+                relevant cycle.
+            comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
+                functions used to compare scenarios. A comparator function is attached to a
+                scenario's data node configuration. The key of the dictionary parameter
+                corresponds to the data node configuration id. During the scenarios'
+                comparison, each comparator is applied to all the data nodes instantiated from
+                the data node configuration attached to the comparator. See
+                `(taipy.)compare_scenarios()^` more more details.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new data node configuration.
+            The new scenario configuration.
         """
 
     @staticmethod
-    def configure_default_data_node(
-        storage_type: str,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure the default values for data node configurations.
-        This function creates the _default data node configuration_ object,
-        where all data node configuration objects will find their default
-        values when needed.
+    def configure_scenario_from_tasks(
+        id: str,
+        task_configs: List[TaskConfig],
+        frequency: Optional[Frequency] = None,
+        comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
+        pipeline_id: Optional[str] = None,
+        **properties,
+    ) -> "ScenarioConfig":
+        """Configure a new scenario configuration made of a single new pipeline configuration.
+
+        A new pipeline configuration is created as well. If *pipeline_id* is not provided,
+        the new pipeline configuration identifier is set to the scenario configuration identifier
+        post-fixed by '_pipeline'.
+
         Parameters:
-            storage_type (str): The default storage type for all data node configurations.
-                The possible values are _"pickle"_ (the default value), _"csv"_, _"excel"_,
-                _"sql"_, _"mongo_collection"_, _"in_memory"_, _"json"_, _"parquet"_ or _"generic"_.
-            scope (Scope^): The default scope for all data node configurations.
-                The default value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the scenario configuration.
+            task_configs (List[TaskConfig^]): The list of task configurations used by the
+                new pipeline configuration that is created.
+            frequency (Optional[Frequency^]): The scenario frequency.
+                It corresponds to the recurrence of the scenarios instantiated from this
+                configuration. Based on this frequency each scenario will be attached to the
+                relevant cycle.
+            comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
+                functions used to compare scenarios. A comparator function is attached to a
+                scenario's data node configuration. The key of the dictionary parameter
+                corresponds to the data node configuration id. During the scenarios'
+                comparison, each comparator is applied to all the data nodes instantiated from
+                the data node configuration attached to the comparator. See
+                `(taipy.)compare_scenarios()` more more details.
+            pipeline_id (Optional[str]): The identifier of the new pipeline configuration to be configured.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The default data node configuration.
+            The new scenario configuration.
         """
 
     @staticmethod
-    def configure_csv_data_node(
-        id: str,
-        default_path: str = ...,
-        has_header: bool = ...,
-        exposed_type=...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new CSV data node configuration.
+    def configure_default_scenario(
+        pipeline_configs: List[PipelineConfig],
+        frequency: Optional[Frequency] = None,
+        comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
+        **properties,
+    ) -> "ScenarioConfig":
+        """Configure the default values for scenario configurations.
+
+        This function creates the *default scenario configuration* object,
+        where all scenario configuration objects will find their default
+        values when needed.
+
         Parameters:
-            id (str): The unique identifier of the new CSV data node configuration.
-            default_path (str): The default path of the CSV file.
-            has_header (bool): If True, indicates that the CSV file has a header.
-            exposed_type: The exposed type of the data read from CSV file. The default value is `pandas`.
-            scope (Scope^): The scope of the CSV data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            pipeline_configs (List[PipelineConfig^]): The list of pipeline configurations used
+                by this scenario configuration.
+            frequency (Optional[Frequency^]): The scenario frequency.
+                It corresponds to the recurrence of the scenarios instantiated from this
+                configuration. Based on this frequency each scenario will be attached to
+                the relevant cycle.
+            comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
+                functions used to compare scenarios. A comparator function is attached to a
+                scenario's data node configuration. The key of the dictionary parameter
+                corresponds to the data node configuration id. During the scenarios'
+                comparison, each comparator is applied to all the data nodes instantiated from
+                the data node configuration attached to the comparator. See
+                `taipy.compare_scenarios()^` more more details.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new CSV data node configuration.
+            The new default scenario configuration.
         """
 
     @staticmethod
-    def configure_json_data_node(
-        id: str,
-        default_path: str = ...,
-        encoder: json.JSONEncoder = ...,
-        decoder: json.JSONDecoder = ...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new JSON data node configuration.
+    def configure_pipeline(id: str, task_configs: Union[TaskConfig, List[TaskConfig]], **properties) -> "PipelineConfig":
+        """Configure a new pipeline configuration.
+
         Parameters:
-            id (str): The unique identifier of the new JSON data node configuration.
-            default_path (str): The default path of the JSON file.
-            encoder (json.JSONEncoder): The JSON encoder used to write data into the JSON file.
-            decoder (json.JSONDecoder): The JSON decoder used to read data from the JSON file.
-            scope (Scope^): The scope of the JSON data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new pipeline configuration.
+            task_configs (Union[TaskConfig^, List[TaskConfig^]]): The list of the task
+                configurations that make this new pipeline. This can be a single task
+                configuration object is this pipeline holds a single task.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new JSON data node configuration.
+            The new pipeline configuration.
         """
 
     @staticmethod
-    def configure_parquet_data_node(
-        id: str,
-        default_path: str = ...,
-        exposed_type=...,
-        engine: Optional[str] = ...,
-        compression: Optional[str] = ...,
-        read_kwargs: Dict = ...,
-        write_kwargs: Dict = ...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new Parquet data node configuration.
+    def configure_default_pipeline(task_configs: Union[TaskConfig, List[TaskConfig]], **properties) -> "PipelineConfig":
+        """Configure the default values for pipeline configurations.
+
+        This function creates the *default pipeline configuration* object,
+        where all pipeline configuration objects will find their default
+        values when needed.
+
         Parameters:
-            id (str): The unique identifier of the new Parquet data node configuration.
-            default_path (str): The default path of the Parquet file.
-            exposed_type: The exposed type of the data read from Parquet file. The default value is `pandas`.
-            engine (Optional[str]): Parquet library to use. Possible values are _"fastparquet"_ or _"pyarrow"_.
-                The default value is _"pyarrow"_.
-            compression (Optional[str]): Name of the compression to use. Use None for no compression.
-                `{'snappy', 'gzip', 'brotli', None}`, default `'snappy'`.
-            read_kwargs (Optional[Dict]): Additional parameters passed to the `pandas.read_parquet` method.
-            write_kwargs (Optional[Dict]): Additional parameters passed to the `pandas.DataFrame.write_parquet` method.
-                The parameters in "read_kwargs" and "write_kwargs" have a **higher precedence** than the top-level parameters which are also
-                passed to Pandas.
-            scope (Scope^): The scope of the Parquet data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            task_configs (Union[TaskConfig^, List[TaskConfig^]]): The list of the task
+                configurations that make the default pipeline configuration. This can be
+                a single task configuration object is this pipeline holds a single task.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
-            `DataNodeConfig^`: The new Parquet data node configuration.
+            The default pipeline configuration.
         """
 
     @staticmethod
-    def configure_sql_table_data_node(
-        id: str,
-        db_username: str,
-        db_password: str,
-        db_name: str,
-        db_engine: str,
-        table_name: str = ...,
-        db_port: int = ...,
-        db_host: str = ...,
-        db_driver: str = ...,
-        db_extra_args: Dict[str, Any] = ...,
-        exposed_type=...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new SQL table data node configuration.
+    def configure_default_data_node(storage_type: str, scope: Optional[Scope] = None, **properties) -> "DataNodeConfig":
+        """Configure the default values for data node configurations.
+
+        This function creates the _default data node configuration_ object,
+        where all data node configuration objects will find their default
+        values when needed.
+
         Parameters:
-            id (str): The unique identifier of the new SQL data node configuration.
-            db_username (str): The database username.
-            db_password (str): The database password.
-            db_name (str): The database name.
-            db_host (str): The database host. The default value is _"localhost"_.
-            db_engine (str): The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or _"postgresql"_.
-            db_driver (str): The database driver. The default value is
-                _"ODBC Driver 17 for SQL Server"_.
-            db_port (int): The database port. The default value is 1433.
-            db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database
-                connection string.
-            table_name (str): The name of the SQL table.
-            exposed_type: The exposed type of the data read from SQL query. The default value is `pandas`.
-            scope (Scope^): The scope of the SQL data node configuration. The default value is
-                `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            storage_type (str): The default storage type for all data node configurations.
+                The possible values are *"pickle"* (the default value), *"csv"*, *"excel"*,
+                *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"* or
+                *"generic"*.
+            scope (Optional[Scope^]): The default scope for all data node configurations.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new SQL data node configuration.
+            The default data node configuration.
         """
 
-    @staticmethod
-    def configure_sql_data_node(
-        id: str,
-        db_username: str,
-        db_password: str,
-        db_name: str,
-        db_engine: str,
-        db_port: int = ...,
-        db_host: str = ...,
-        db_driver: str = ...,
-        db_extra_args: Dict[str, Any] = ...,
-        read_query: str = ...,
-        write_query_builder: Callable = ...,
-        exposed_type=...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new SQL data node configuration.
+    @classmethod
+    def configure_data_node(
+        cls, id: str, storage_type: Optional[str] = None, scope: Optional[Scope] = None, **properties
+    ) -> "DataNodeConfig":
+        """Configure a new data node configuration.
+
         Parameters:
-            id (str): The unique identifier of the new SQL data node configuration.
-            db_username (str): The database username.
-            db_password (str): The database password.
-            db_name (str): The database name.
-            db_engine (str): The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or _"postgresql"_.
-            db_port (int): The database port. The default value is 1433.
-            db_host (str): The database host. The default value is _"localhost"_.
-            db_driver (str): The database driver. The default value is
-                _"ODBC Driver 17 for SQL Server"_.
-            db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database
-                connection string.
-            read_query (str): The SQL query string used to read the data from the database.
-            write_query_builder (Callable): A callback function that takes the data as an input parameter and returns a list of SQL queries.
-            exposed_type: The exposed type of the data read from SQL query. The default value is `pandas`.
-            scope (Scope^): The scope of the SQL data node configuration. The default value is
-                `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new data node configuration.
+            storage_type (Optional[str]): The data node configuration storage type. The possible values
+                are None (which is the default value of *"pickle"*, unless it has been overloaded by the
+                *storage_type* value set in the default data node configuration
+                (see `(Config.)configure_default_data_node()^`)), *"pickle"*, *"csv"*, *"excel"*,
+                *"sql_table"*, *"sql"*, *"json"*, *"parquet"*, *"mongo_collection"*, *"in_memory"*, or
+                *"generic"*.
+            scope (Optional[Scope^]): The scope of the data node configuration.<br/>
+                The default value is `Scope.SCENARIO` (or the one specified in
+                `(Config.)configure_default_data_node()^`).
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new SQL data node configuration.
+            The new data node configuration.
         """
 
-    @staticmethod
-    def configure_mongo_collection_data_node(
+    @classmethod
+    def configure_csv_data_node(
+        cls,
         id: str,
-        db_name: str,
-        collection_name: str,
-        custom_document: Any = ...,
-        db_username: str = ...,
-        db_password: str = ...,
-        db_host: str = ...,
-        db_port: int = ...,
-        db_extra_args: Dict[str, Any] = ...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new Mongo collection data node configuration.
+        default_path: Optional[str] = None,
+        has_header: Optional[bool] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new CSV data node configuration.
+
         Parameters:
-            id (str): The unique identifier of the new Mongo collection data node configuration.
-            db_name (str): The database name.
-            collection_name (str): The collection in the database to read from and to write the data to.
-            custom_document (Any): The custom document class to store, encode, and decode data when reading and writing to a Mongo collection.
-                The custom_document can have optional `decode` method to decode data in the Mongo collection to a custom object,
-                and `encode` method to encode the object's properties to the Mongo collection when writing.
-            db_username (str): The database username.
-            db_password (str): The database password.
-            db_host (str): The database host. The default value is _"localhost"_.
-            db_port (int): The database port. The default value is 27017.
-            db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database connection string.
-            scope (Scope^): The scope of the Mongo collection data node configuration. The default value is
-                `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new CSV data node configuration.
+            default_path (Optional[str]): The default path of the CSV file.
+            has_header (Optional[bool]): If True, indicates that the CSV file has a header.
+            exposed_type (Optional[str]): The exposed type of the data read from CSV file.<br/>
+                The default value is `pandas`.
+            scope (Optional[Scope^]): The scope of the CSV data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new Mongo collection data node configuration.
+            The new CSV data node configuration.
         """
 
-    @staticmethod
-    def configure_in_memory_data_node(
+    @classmethod
+    def configure_json_data_node(
+        cls,
         id: str,
-        default_data: Optional[Any] = ...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new _in_memory_ data node configuration.
+        default_path: Optional[str] = None,
+        encoder: Optional[json.JSONEncoder] = None,
+        decoder: Optional[json.JSONDecoder] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new JSON data node configuration.
+
         Parameters:
-            id (str): The unique identifier of the new in_memory data node configuration.
-            default_data (Optional[Any]): The default data of the data nodes instantiated from
-                this in_memory data node configuration.
-            scope (Scope^): The scope of the in_memory data node configuration. The default
-                value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new JSON data node configuration.
+            default_path (Optional[str]): The default path of the JSON file.
+            encoder (Optional[json.JSONEncoder]): The JSON encoder used to write data into the JSON file.
+            decoder (Optional[json.JSONDecoder]): The JSON decoder used to read data from the JSON file.
+            scope (Optional[Scope^]): The scope of the JSON data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
-            `DataNodeConfig^`: The new _in_memory_ data node configuration.
+            The new JSON data node configuration.
         """
 
-    @staticmethod
-    def configure_pickle_data_node(
+    @classmethod
+    def configure_parquet_data_node(
+        cls,
         id: str,
-        default_data: Optional[Any] = ...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
-        """Configure a new pickle data node configuration.
+        default_path: Optional[str] = None,
+        engine: Optional[str] = None,
+        compression: Optional[str] = None,
+        read_kwargs: Optional[Dict] = None,
+        write_kwargs: Optional[Dict] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new Parquet data node configuration.
+
         Parameters:
-            id (str): The unique identifier of the new pickle data node configuration.
-            default_data (Optional[Any]): The default data of the data nodes instantiated from
-                this pickle data node configuration.
-            scope (Scope^): The scope of the pickle data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new Parquet data node configuration.
+            default_path (Optional[str]): The default path of the Parquet file.
+            engine (Optional[str]): Parquet library to use. Possible values are *"fastparquet"* or
+                *"pyarrow"*.<br/>
+                The default value is *"pyarrow"*.
+            compression (Optional[str]): Name of the compression to use. Possible values are *"snappy"*,
+                *"gzip"*, *"brotli"*, or *"none"* (no compression). The default value is *"snappy"*.
+            read_kwargs (Optional[dict]): Additional parameters passed to the `pandas.read_parquet()`
+                function.
+            write_kwargs (Optional[dict]): Additional parameters passed to the
+                `pandas.DataFrame.write_parquet()` function.<br/>
+                The parameters in *read_kwargs* and *write_kwargs* have a **higher precedence** than the
+                top-level parameters which are also passed to Pandas.
+            exposed_type (Optional[str]): The exposed type of the data read from Parquet file.<br/>
+                The default value is `pandas`.
+            scope (Optional[Scope^]): The scope of the Parquet data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new pickle data node configuration.
+            The new Parquet data node configuration.
         """
 
-    @staticmethod
+    @classmethod
     def configure_excel_data_node(
+        cls,
         id: str,
-        default_path: str = ...,
-        has_header: bool = True,
-        sheet_name: Union[List[str], str] = ...,
-        exposed_type=...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
+        default_path: Optional[str] = None,
+        has_header: Optional[bool] = None,
+        sheet_name: Optional[Union[List[str], str]] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
         """Configure a new Excel data node configuration.
+
         Parameters:
             id (str): The unique identifier of the new Excel data node configuration.
-            default_path (str): The path of the Excel file.
-            has_header (bool): If True, indicates that the Excel file has a header.
-            sheet_name (Union[List[str], str]): The list of sheet names to be used. This
-                can be a unique name.
-            exposed_type: The exposed type of the data read from Excel file. The default value is `pandas`.
-            scope (Scope^): The scope of the Excel data node configuration. The default
-                value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            default_path (Optional[str]): The path of the Excel file.
+            has_header (Optional[bool]): If True, indicates that the Excel file has a header.
+            sheet_name (Optional[Union[List[str], str]]): The list of sheet names to be used.
+                This can be a unique name.
+            exposed_type (Optional[str]): The exposed type of the data read from Excel file.<br/>
+                The default value is `pandas`.
+            scope (Optional[Scope^]): The scope of the Excel data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new CSV data node configuration.
+            The new Excel data node configuration.
         """
 
-    @staticmethod
+    @classmethod
     def configure_generic_data_node(
+        cls,
         id: str,
-        read_fct: Callable = ...,
-        write_fct: Callable = ...,
-        read_fct_params: List = ...,
-        write_fct_params: List = ...,
-        scope: Scope = ...,
-        **properties: Dict[str, Any],
-    ) -> DataNodeConfig:
+        read_fct: Optional[Callable] = None,
+        write_fct: Optional[Callable] = None,
+        read_fct_args: Optional[List] = None,
+        write_fct_args: Optional[List] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
         """Configure a new generic data node configuration.
+
         Parameters:
             id (str): The unique identifier of the new generic data node configuration.
             read_fct (Optional[Callable]): The Python function called to read the data.
             write_fct (Optional[Callable]): The Python function called to write the data.
-                The provided function must have at least one parameter that receives the data
-                to be written.
-            read_fct_params (Optional[List]): The parameters that are passed to _read_fct_
-                to read the data.
-            write_fct_params (Optional[List]): The parameters that are passed to _write_fct_
-                to write the data.
-            scope (Optional[Scope^]): The scope of the Generic data node configuration.
+                The provided function must have at least one parameter that receives the data to be written.
+            read_fct_args (Optional[List]): The list of arguments that are passed to the function
+                *read_fct* to read data.
+            write_fct_args (Optional[List]): The list of arguments that are passed to the function
+                *write_fct* to write the data.
+            scope (Optional[Scope^]): The scope of the Generic data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
-            `DataNodeConfig^`: The new Generic data node configuration.
+            The new Generic data node configuration.
         """
 
-    @_Classproperty
-    def job_config(cls) -> JobConfig:
-        """Return the job execution configuration `JobConfig^`."""
+    @classmethod
+    def configure_in_memory_data_node(
+        cls, id: str, default_data: Optional[Any] = None, scope: Optional[Scope] = None, **properties
+    ) -> "DataNodeConfig":
+        """Configure a new *in-memory* data node configuration.
 
-    @staticmethod
-    def configure_job_executions(
-        mode: str = ...,
-        nb_of_workers: Union[int, str] = ...,
-        max_nb_of_workers: Union[int, str] = ...,
-        **properties: Dict[str, Any],
-    ) -> JobConfig:
-        """Configure job execution.
         Parameters:
-            mode (Optional[str]): The job execution mode.
-                Possible values are: _"standalone"_ (the default value) or
-                _"development"_.
-            max_nb_of_workers (Optional[int, str]): Parameter used only in default _"standalone"_ mode. The maximum
-                number of jobs able to run in parallel. The default value is 1.<br/>
-                A string can be provided to dynamically set the value using an environment
-                variable. The string must follow the pattern: `ENV[&lt;env_var&gt;]` where
-                `&lt;env_var&gt;` is the name of environment variable.
-            nb_of_workers (Optional[int, str]): Deprecated. Use max_nb_of_workers instead.
+            id (str): The unique identifier of the new in_memory data node configuration.
+            default_data (Optional[any]): The default data of the data nodes instantiated from
+                this in_memory data node configuration.
+            scope (Optional[Scope^]): The scope of the in_memory data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `JobConfig^`: The job execution configuration.
+            The new *in-memory* data node configuration.
         """
 
-    @_Classproperty
-    def pipelines(cls) -> Dict[str, PipelineConfig]:
-        """Return all pipeline configurations grouped by id in a dictionary.
-
-        `Config.pipelines()` is an alias for `Config.sections["PIPELINE"]`
-        """
+    @classmethod
+    def configure_pickle_data_node(
+        cls,
+        id: str,
+        default_path: Optional[str] = None,
+        default_data: Optional[Any] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new pickle data node configuration.
 
-    @staticmethod
-    def configure_pipeline(id: str, task_configs: Union[TaskConfig, List[TaskConfig]], **properties: Dict[str, Any]) -> PipelineConfig:  # type: ignore
-        """Configure a new pipeline configuration.
         Parameters:
-            id (str): The unique identifier of the new pipeline configuration.
-            task_configs (Union[TaskConfig^, List[TaskConfig^]]): The list of the task
-                configurations that make this new pipeline. This can be a single task
-                configuration object is this pipeline holds a single task.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `PipelineConfig^`: The new pipeline configuration.
-        """
+            id (str): The unique identifier of the new pickle data node configuration.
+            default_path (Optional[str]): The path of the pickle file.
+            default_data (Optional[any]): The default data of the data nodes instantiated from
+                this pickle data node configuration.
+            scope (Optional[Scope^]): The scope of the pickle data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
-    @staticmethod
-    def configure_default_pipeline(task_configs: Union[TaskConfig, List[TaskConfig]], **properties: Dict[str, Any]) -> PipelineConfig:  # type: ignore
-        """Configure the default values for pipeline configurations.
-        This function creates the _default pipeline configuration_ object,
-        where all pipeline configuration objects will find their default
-        values when needed.
-        Parameters:
-            task_configs (Union[TaskConfig^, List[TaskConfig^]]): The list of the task
-                configurations that make the default pipeline configuration. This can be
-                a single task configuration object is this pipeline holds a single task.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
         Returns:
-            `PipelineConfig^`: The default pipeline configuration.
-        """
-
-    @_Classproperty
-    def scenarios(cls) -> Dict[str, ScenarioConfig]:
-        """Return all scenario configurations grouped by id in a dictionary.
-
-        `Config.scenarios()` is an alias for `Config.sections["SCENARIO"]`
+            The new pickle data node configuration.
         """
 
-    @staticmethod
-    def configure_scenario(
+    @classmethod
+    def configure_sql_table_data_node(
+        cls,
         id: str,
-        pipeline_configs: List[PipelineConfig],  # type: ignore
-        frequency: Optional[Frequency] = ...,
-        comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = ...,
-        **properties: Dict[str, Any],
-    ) -> ScenarioConfig:
-        """Configure a new scenario configuration.
-        Parameters:
-            id (str): The unique identifier of the new scenario configuration.
-            pipeline_configs (List[PipelineConfig^]): The list of pipeline configurations used
-                by this new scenario configuration.
-            frequency (Optional[Frequency^]): The scenario frequency.
-                It corresponds to the recurrence of the scenarios instantiated from this
-                configuration. Based on this frequency each scenario will be attached to the
-                relevant cycle.
-            comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
-                functions used to compare scenarios. A comparator function is attached to a
-                scenario's data node configuration. The key of the dictionary parameter
-                corresponds to the data node configuration id. During the scenarios'
-                comparison, each comparator is applied to all the data nodes instantiated from
-                the data node configuration attached to the comparator. See
-                `(taipy.)compare_scenarios()^` more more details.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `ScenarioConfig^`: The new scenario configuration.
-        """
+        db_name: str,
+        db_engine: str,
+        table_name: str,
+        db_username: Optional[str] = None,
+        db_password: Optional[str] = None,
+        db_host: Optional[str] = None,
+        db_port: Optional[int] = None,
+        db_driver: Optional[str] = None,
+        sqlite_folder_path: Optional[str] = None,
+        sqlite_file_extension: Optional[str] = None,
+        db_extra_args: Optional[Dict[str, Any]] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new SQL table data node configuration.
 
-    @staticmethod
-    def configure_default_scenario(
-        pipeline_configs: List[PipelineConfig],  # type: ignore
-        frequency: Optional[Frequency] = ...,
-        comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = ...,
-        **properties: Dict[str, Any],
-    ) -> ScenarioConfig:
-        """Configure the default values for scenario configurations.
-        This function creates the _default scenario configuration_ object,
-        where all scenario configuration objects will find their default
-        values when needed.
         Parameters:
-            pipeline_configs (List[PipelineConfig^]): The list of pipeline configurations used
-                by this scenario configuration.
-            frequency (Optional[Frequency^]): The scenario frequency.
-                It corresponds to the recurrence of the scenarios instantiated from this
-                configuration. Based on this frequency each scenario will be attached to
-                the relevant cycle.
-            comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
-                functions used to compare scenarios. A comparator function is attached to a
-                scenario's data node configuration. The key of the dictionary parameter
-                corresponds to the data node configuration id. During the scenarios'
-                comparison, each comparator is applied to all the data nodes instantiated from
-                the data node configuration attached to the comparator. See
-                `taipy.compare_scenarios()^` more more details.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new SQL data node configuration.
+            db_name (str): The database name, or the name of the SQLite database file.
+            db_engine (str): The database engine. Possible values are *"sqlite"*, *"mssql"*, *"mysql"*,
+                or *"postgresql"*.
+            table_name (str): The name of the SQL table.
+            db_username (Optional[str]): The database username. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_password (Optional[str]): The database password. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_host (Optional[str]): The database host.<br/>
+                The default value is "localhost".
+            db_port (Optional[int]): The database port.<br/>
+                The default value is 1433.
+            db_driver (Optional[str]): The database driver.
+            sqlite_folder_path (Optional[str]): The path to the folder that contains SQLite file.<br/>
+                The default value is the current working folder.
+            sqlite_file_extension (Optional[str]): The file extension of the SQLite file.<br/>
+                The default value is ".db".
+            db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into database connection string.
+            exposed_type (Optional[str]): The exposed type of the data read from SQL table.<br/>
+                The default value is "pandas".
+            scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `ScenarioConfig^`: The default scenario configuration.
+            The new SQL data node configuration.
         """
 
-    @staticmethod
-    def configure_scenario_from_tasks(
+    @classmethod
+    def configure_sql_data_node(
+        cls,
         id: str,
-        task_configs: List[TaskConfig],  # type: ignore
-        frequency: Optional[Frequency] = ...,
-        comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = ...,
-        pipeline_id: Optional[str] = ...,
-        **properties: Dict[str, Any],
-    ) -> ScenarioConfig:
-        """Configure a new scenario configuration made of a single new pipeline configuration.
-        A new pipeline configuration is created as well. If _pipeline_id_ is not provided,
-        the new pipeline configuration identifier is set to the scenario configuration identifier
-        post-fixed by '_pipeline'.
+        db_name: str,
+        db_engine: str,
+        read_query: str,
+        write_query_builder: Callable,
+        db_username: Optional[str] = None,
+        db_password: Optional[str] = None,
+        db_host: Optional[str] = None,
+        db_port: Optional[int] = None,
+        db_driver: Optional[str] = None,
+        sqlite_folder_path: Optional[str] = None,
+        sqlite_file_extension: Optional[str] = None,
+        db_extra_args: Optional[Dict[str, Any]] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new SQL data node configuration.
+
         Parameters:
-            id (str): The unique identifier of the scenario configuration.
-            task_configs (List[TaskConfig^]): The list of task configurations used by the
-                new pipeline configuration that is created.
-            frequency (Optional[Frequency^]): The scenario frequency.
-                It corresponds to the recurrence of the scenarios instantiated from this
-                configuration. Based on this frequency each scenario will be attached to the
-                relevant cycle.
-            comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
-                functions used to compare scenarios. A comparator function is attached to a
-                scenario's data node configuration. The key of the dictionary parameter
-                corresponds to the data node configuration id. During the scenarios'
-                comparison, each comparator is applied to all the data nodes instantiated from
-                the data node configuration attached to the comparator. See
-                `(taipy.)compare_scenarios()` more more details.
-            pipeline_id (str): The identifier of the new pipeline configuration to be
-                configured.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            id (str): The unique identifier of the new SQL data node configuration.
+            db_name (str): The database name, or the name of the SQLite database file.
+            db_engine (str): The database engine. Possible values are *"sqlite"*, *"mssql"*, *"mysql"*,
+                or *"postgresql"*.
+            read_query (str): The SQL query string used to read the data from the database.
+            write_query_builder (Callable): A callback function that takes the data as an input parameter
+                and returns a list of SQL queries.
+            db_username (Optional[str]): The database username. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_password (Optional[str]): The database password. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_host (Optional[str]): The database host.<br/>
+                The default value is "localhost".
+            db_port (Optional[int]): The database port.<br/>
+                The default value is 1433.
+            db_driver (Optional[str]): The database driver.
+            sqlite_folder_path (Optional[str]): The path to the folder that contains SQLite file.<br/>
+                The default value is the current working folder.
+            sqlite_file_extension (Optional[str]): The file extension of the SQLite file.<br/>
+                The default value is ".db".
+            db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into database connection string.
+            exposed_type (Optional[str]): The exposed type of the data read from SQL query.<br/>
+                The default value is "pandas".
+            scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
-            `ScenarioConfig^`: The new scenario configuration.
+            The new SQL data node configuration.
         """
 
-    @_Classproperty
-    def tasks(cls) -> Dict[str, TaskConfig]:
-        """Return all task configurations grouped by id in a dictionary.
+    @classmethod
+    def configure_mongo_collection_data_node(
+        cls,
+        id: str,
+        db_name: str,
+        collection_name: str,
+        custom_document: Optional[Any] = None,
+        db_username: Optional[str] = None,
+        db_password: Optional[str] = None,
+        db_host: Optional[str] = None,
+        db_port: Optional[int] = None,
+        db_extra_args: Optional[Dict[str, Any]] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new Mongo collection data node configuration.
 
-        `Config.tasks()` is an alias for `Config.sections["TASK"]`
+        Parameters:
+            id (str): The unique identifier of the new Mongo collection data node configuration.
+            db_name (str): The database name.
+            collection_name (str): The collection in the database to read from and to write the data to.
+            custom_document (Optional[any]): The custom document class to store, encode, and decode data
+                when reading and writing to a Mongo collection. The custom_document can have an optional
+                *decode()* method to decode data in the Mongo collection to a custom object, and an
+                optional *encode()*) method to encode the object's properties to the Mongo collection
+                when writing.
+            db_username (Optional[str]): The database username.
+            db_password (Optional[str]): The database password.
+            db_host (Optional[str]): The database host.<br/>
+                The default value is "localhost".
+            db_port (Optional[int]): The database port.<br/>
+                The default value is 27017.
+            db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into database connection string.
+            scope (Optional[Scope^]): The scope of the Mongo collection data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
+        Returns:
+            The new Mongo collection data node configuration.
         """
 
     @staticmethod
     def configure_task(
         id: str,
-        function: Callable,
-        input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = ...,  # type: ignore
-        output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = ...,  # type: ignore
-        skippable: Optional[bool] = ...,  # type: ignore
-        **properties: Dict[str, Any],
-    ) -> TaskConfig:
+        function,
+        input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
+        output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
+        skippable: Optional[bool] = False,
+        **properties,
+    ) -> "TaskConfig":
         """Configure a new task configuration.
+
         Parameters:
             id (str): The unique identifier of this task configuration.
             function (Callable): The python function called by Taipy to run the task.
             input (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 function input data node configurations. This can be a unique data node
                 configuration if there is a single input data node, or None if there are none.
             output (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 function output data node configurations. This can be a unique data node
                 configuration if there is a single output data node, or None if there are none.
             skippable (bool): If True, indicates that the task can be skipped if no change has
-                been made on inputs. The default value is _False_.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+                been made on inputs.<br/>
+                The default value is False.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `TaskConfig^`: The new task configuration.
+            The new task configuration.
         """
 
     @staticmethod
     def configure_default_task(
-        function: Callable,
-        input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = ...,  # type: ignore
-        output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = ...,  # type: ignore
-        skippable: Optional[bool] = ...,  # type: ignore
-        **properties: Dict[str, Any],
-    ) -> TaskConfig:
+        function,
+        input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
+        output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
+        skippable: Optional[bool] = False,
+        **properties,
+    ) -> "TaskConfig":
         """Configure the default values for task configurations.
-        This function creates the _default task configuration_ object,
+
+        This function creates the *default task configuration* object,
         where all task configuration objects will find their default
         values when needed.
+
         Parameters:
             function (Callable): The python function called by Taipy to run the task.
             input (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 input data node configurations. This can be a unique data node
                 configuration if there is a single input data node, or None if there are none.
             output (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 output data node configurations. This can be a unique data node
                 configuration if there is a single output data node, or None if there are none.
             skippable (bool): If True, indicates that the task can be skipped if no change has
-                been made on inputs. The default value is _False_.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
+                been made on inputs.<br/>
+                The default value is False.
+            **properties (dict[str, any]): A keyworded variable length list of additional
                 arguments.
         Returns:
-            `TaskConfig^`: The default task configuration.
+            The default task configuration.
         """
+
+    @staticmethod
+    def configure_job_executions(
+        mode: str = None, nb_of_workers: Union[int, str] = None, max_nb_of_workers: Union[int, str] = None, **properties
+    ) -> "JobConfig":
+        """Configure job execution.
+
+        Parameters:
+            mode (Optional[str]): The job execution mode.
+                Possible values are: *"standalone"* (the default value) or *"development"*.
+            max_nb_of_workers (Optional[int, str]): Parameter used only in default *"standalone"* mode.
+                This indicates the maximum number of jobs able to run in parallel.<br/>
+                The default value is 1.<br/>
+                A string can be provided to dynamically set the value using an environment
+                variable. The string must follow the pattern: `ENV[&lt;env_var&gt;]` where
+                `&lt;env_var&gt;` is the name of an environment variable.
+            nb_of_workers (Optional[int, str]): Deprecated. Use *max_nb_of_workers* instead.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
+        Returns:
+            The new job execution configuration.
+        """
+
```

### Comparing `taipy-config-2.2.0/src/taipy/config/exceptions/__init__.py` & `taipy-config-2.3.0.dev0/src/taipy/config/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/exceptions/exceptions.py` & `taipy-config-2.3.0.dev0/src/taipy/config/exceptions/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 # specific language governing permissions and limitations under the License.
 
 
 class LoadingError(Exception):
     """Raised if an error occurs while loading the configuration file."""
 
 
-class ConfigurationIssueError(Exception):
-    """Raised if an inconsistency has been detected in the configuration."""
-
-
 class InconsistentEnvVariableError(Exception):
     """Inconsistency value has been detected in an environment variable referenced by the configuration."""
 
 
 class MissingEnvVariableError(Exception):
     """Environment variable referenced in configuration is missing."""
```

### Comparing `taipy-config-2.2.0/src/taipy/config/global_app/global_app_config.py` & `taipy-config-2.3.0.dev0/src/taipy/config/global_app/global_app_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/config/section.py` & `taipy-config-2.3.0.dev0/src/taipy/config/section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/logger/__init__.py` & `taipy-config-2.3.0.dev0/src/taipy/config/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.2.0/src/taipy/logger/_taipy_logger.py` & `taipy-config-2.3.0.dev0/src/taipy/logger/_taipy_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,11 +31,11 @@
             logging.config.fileConfig(config_filename)
             cls.__logger = logging.getLogger("Taipy")
         else:
             cls.__logger = logging.getLogger("Taipy")
             cls.__logger.setLevel(logging.INFO)
             ch = logging.StreamHandler(sys.stdout)
             ch.setLevel(logging.INFO)
-            formatter = logging.Formatter("[%(asctime)s][%(name)s][%(levelname)s] %(message)s")
+            formatter = logging.Formatter("[%(asctime)s][%(name)s][%(levelname)s] %(message)s", "%Y-%m-%d %H:%M:%S")
             ch.setFormatter(formatter)
             cls.__logger.addHandler(ch)
         return cls.__logger
```

### Comparing `taipy-config-2.2.0/src/taipy_config.egg-info/PKG-INFO` & `taipy-config-2.3.0.dev0/src/taipy_config.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.2.0
+Version: 2.3.0.dev0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Taipy config
 
 ## License
@@ -72,9 +71,10 @@
     - `tests`: Unit tests following the `taipy/` structure.
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-config_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy-config_.
 - `INSTALLATION.md`: Instructions to install _taipy-config_.
 - `LICENSE`: The Apache 2.0 License.
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies.
 - `README.md`: Current file.
+- `contributors.txt`: The list of contributors.
 - `setup.py`: The setup script managing building, distributing, and installing _taipy-config_.
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-config-2.2.0/src/taipy_config.egg-info/SOURCES.txt` & `taipy-config-2.3.0.dev0/src/taipy_config.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/taipy/__init__.py
+src/taipy/_cli/__init__.py
+src/taipy/_cli/_base_cli/__init__.py
+src/taipy/_cli/_base_cli/_cli.py
 src/taipy/config/__init__.py
-src/taipy/config/_base_serializer.py
 src/taipy/config/_config.py
-src/taipy/config/_config_comparator.py
-src/taipy/config/_json_serializer.py
-src/taipy/config/_toml_serializer.py
 src/taipy/config/config.py
 src/taipy/config/config.pyi
 src/taipy/config/section.py
 src/taipy/config/unique_section.py
 src/taipy/config/version.json
 src/taipy/config/version.py
+src/taipy/config/_config_comparator/__init__.py
+src/taipy/config/_config_comparator/_comparator_result.py
+src/taipy/config/_config_comparator/_config_comparator.py
+src/taipy/config/_serializer/__init__.py
+src/taipy/config/_serializer/_base_serializer.py
+src/taipy/config/_serializer/_json_serializer.py
+src/taipy/config/_serializer/_toml_serializer.py
 src/taipy/config/checker/__init__.py
 src/taipy/config/checker/_checker.py
 src/taipy/config/checker/issue.py
 src/taipy/config/checker/issue_collector.py
 src/taipy/config/checker/_checkers/__init__.py
 src/taipy/config/checker/_checkers/_auth_config_checker.py
 src/taipy/config/checker/_checkers/_config_checker.py
 src/taipy/config/checker/_checkers/_gLobal_config_checker.py
 src/taipy/config/common/__init__.py
-src/taipy/config/common/_argparser.py
 src/taipy/config/common/_classproperty.py
 src/taipy/config/common/_config_blocker.py
 src/taipy/config/common/_repr_enum.py
 src/taipy/config/common/_template_handler.py
 src/taipy/config/common/_validate_id.py
 src/taipy/config/common/frequency.py
 src/taipy/config/common/scope.py
```

