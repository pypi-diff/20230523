# Comparing `tmp/azure-cli-core-2.9.0.tar.gz` & `tmp/azure-cli-core-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vsts/work/1/a/azure-cli-core-2.9.0.tar", last modified: Fri Jul 10 07:14:01 2020, max compression
+gzip compressed data, was "/home/vsts/work/1/a/azure-cli-core-2.9.1.tar", last modified: Thu Jul 16 08:10:08 2020, max compression
```

## Comparing `azure-cli-core-2.9.0.tar` & `azure-cli-core-2.9.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/
--rw-r--r--   0 vsts      (1001) docker     (118)    15113 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (118)       42 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (118)    20233 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)       67 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure/
--rw-r--r--   0 vsts      (1001) docker     (118)      408 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure/cli/
--rw-r--r--   0 vsts      (1001) docker     (118)      408 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure/cli/core/
--rw-r--r--   0 vsts      (1001) docker     (118)    42023 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      777 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)      574 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_config.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2255 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_debug.py
--rw-r--r--   0 vsts      (1001) docker     (118)      518 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_environment.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16880 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8992 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_help_loaders.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1663 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_msal.py
--rw-r--r--   0 vsts      (1001) docker     (118)      783 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_output.py
--rw-r--r--   0 vsts      (1001) docker     (118)    61623 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_profile.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3729 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/_session.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4499 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/adal_authentication.py
--rw-r--r--   0 vsts      (1001) docker     (118)      637 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/api.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure/cli/core/auth_landing_pages/
--rw-r--r--   0 vsts      (1001) docker     (118)      343 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/auth_landing_pages/fail.html
--rw-r--r--   0 vsts      (1001) docker     (118)      421 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/auth_landing_pages/ok.html
--rw-r--r--   0 vsts      (1001) docker     (118)     9223 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/azlogging.py
--rw-r--r--   0 vsts      (1001) docker     (118)    26977 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/cloud.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure/cli/core/commands/
--rw-r--r--   0 vsts      (1001) docker     (118)    63045 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    51403 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/arm.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9645 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2215 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)      866 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/events.py
--rw-r--r--   0 vsts      (1001) docker     (118)    20368 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/parameters.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5283 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/progress.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7594 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/template_create.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2359 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/transform.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4828 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/commands/validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2738 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/decorators.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure/cli/core/extension/
--rw-r--r--   0 vsts      (1001) docker     (118)    12648 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/extension/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2086 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/extension/_homebrew_patch.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2308 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/extension/_index.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4392 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/extension/_resolve.py
--rw-r--r--   0 vsts      (1001) docker     (118)    19572 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/extension/operations.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4322 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/file_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3202 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/keys.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9030 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/local_context.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2061 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/mock.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15949 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/parser.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure/cli/core/profiles/
--rw-r--r--   0 vsts      (1001) docker     (118)     5740 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/profiles/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    23867 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/profiles/_shared.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17669 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (118)    39671 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure/cli/core/util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2358 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/azure_bdist_wheel.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure_cli_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (118)    20233 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)     1683 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure_cli_core.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (118)      457 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure_cli_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        6 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/azure_cli_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (118)       95 2020-07-10 07:14:01.000000 azure-cli-core-2.9.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (118)     3345 2020-07-10 07:13:51.000000 azure-cli-core-2.9.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/
+-rw-r--r--   0 vsts      (1001) docker     (118)    15141 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)       42 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (118)    20293 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)       67 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure/
+-rw-r--r--   0 vsts      (1001) docker     (118)      408 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure/cli/
+-rw-r--r--   0 vsts      (1001) docker     (118)      408 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure/cli/core/
+-rw-r--r--   0 vsts      (1001) docker     (118)    42225 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      777 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      574 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2255 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_debug.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      518 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16880 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8992 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_help_loaders.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1663 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_msal.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      783 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_output.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    61804 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_profile.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3729 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/_session.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4499 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/adal_authentication.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      637 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/api.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure/cli/core/auth_landing_pages/
+-rw-r--r--   0 vsts      (1001) docker     (118)      343 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/auth_landing_pages/fail.html
+-rw-r--r--   0 vsts      (1001) docker     (118)      421 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/auth_landing_pages/ok.html
+-rw-r--r--   0 vsts      (1001) docker     (118)     9223 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/azlogging.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    26977 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/cloud.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure/cli/core/commands/
+-rw-r--r--   0 vsts      (1001) docker     (118)    63045 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    51403 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/arm.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9645 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2215 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      866 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/events.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    20368 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/parameters.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5283 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7594 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/template_create.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2359 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/transform.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4828 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/commands/validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2738 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/decorators.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure/cli/core/extension/
+-rw-r--r--   0 vsts      (1001) docker     (118)    12648 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/extension/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2086 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/extension/_homebrew_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2312 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/extension/_index.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4392 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/extension/_resolve.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    19600 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/extension/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4322 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/file_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3202 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/keys.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9030 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/local_context.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2061 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/mock.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15949 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/parser.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure/cli/core/profiles/
+-rw-r--r--   0 vsts      (1001) docker     (118)     5740 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/profiles/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    23867 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/profiles/_shared.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    17669 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    40205 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure/cli/core/util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2358 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/azure_bdist_wheel.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/azure_cli_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (118)    20293 2020-07-16 08:10:07.000000 azure-cli-core-2.9.1/azure_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)     1683 2020-07-16 08:10:07.000000 azure-cli-core-2.9.1/azure_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-16 08:10:07.000000 azure-cli-core-2.9.1/azure_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-16 08:10:07.000000 azure-cli-core-2.9.1/azure_cli_core.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (118)      457 2020-07-16 08:10:07.000000 azure-cli-core-2.9.1/azure_cli_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        6 2020-07-16 08:10:07.000000 azure-cli-core-2.9.1/azure_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)       95 2020-07-16 08:10:08.000000 azure-cli-core-2.9.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (118)     3345 2020-07-16 08:09:55.000000 azure-cli-core-2.9.1/setup.py
```

### Comparing `azure-cli-core-2.9.0/HISTORY.rst` & `azure-cli-core-2.9.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 Release History
 ===============
 
+2.9.1
+++++++
+* Minor fixes
+
 2.9.0
 ++++++
 * Fix get_token() issue in msi login and `expiresIn` key error in cloud shell login credentials for track 2 SDK related commands (#14187)
 
 2.8.0
 ++++++
 * Add get_command_loader() entry to support to load customized CommandLoader (#13763)
```

### Comparing `azure-cli-core-2.9.0/PKG-INFO` & `azure-cli-core-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: azure-cli-core
-Version: 2.9.0
+Version: 2.9.1
 Summary: Microsoft Azure Command-Line Tools Core Module
 Home-page: https://github.com/Azure/azure-cli
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Description: Microsoft Azure CLI Core Module
         ==================================
         
         
         .. :changelog:
         
         Release History
         ===============
         
+        2.9.1
+        ++++++
+        * Minor fixes
+        
         2.9.0
         ++++++
         * Fix get_token() issue in msi login and `expiresIn` key error in cloud shell login credentials for track 2 SDK related commands (#14187)
         
         2.8.0
         ++++++
         * Add get_command_loader() entry to support to load customized CommandLoader (#13763)
```

### Comparing `azure-cli-core-2.9.0/azure/cli/core/__init__.py` & `azure-cli-core-2.9.1/azure/cli/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 # pylint: disable=line-too-long
 
 from __future__ import print_function
 
-__version__ = "2.9.0"
+__version__ = "2.9.1"
 
 import os
 import sys
 import timeit
 
 import six
 
@@ -251,17 +251,14 @@
             :param ext_suppressions: Extension suppression information.
             :param extension_modname: Command modules to load, in the format like ['azext_timeseriesinsights'].
              If None, will do extension discovery and load all extensions.
              If [], only ALWAYS_LOADED_EXTENSIONS will be loaded.
              Otherwise, the list will be extended using ALWAYS_LOADED_EXTENSIONS.
              If the extensions in the list are not installed, it will be skipped.
             """
-
-            from azure.cli.core.extension.operations import check_version_compatibility
-
             def _handle_extension_suppressions(extensions):
                 filtered_extensions = []
                 for ext in extensions:
                     should_include = True
                     for suppression in ext_suppressions:
                         if should_include and suppression.handle_suppress(ext):
                             should_include = False
@@ -295,14 +292,17 @@
                 cumulative_group_count = 0
                 cumulative_command_count = 0
                 logger.debug("Loading extensions:")
                 logger.debug(self.header_ext)
 
                 for ext in allowed_extensions:
                     try:
+                        # Import in the `for` loop because `allowed_extensions` can be []. In such case we
+                        # don't need to import `check_version_compatibility` at all.
+                        from azure.cli.core.extension.operations import check_version_compatibility
                         check_version_compatibility(ext.get_metadata())
                     except CLIError as ex:
                         # issue warning and skip loading extensions that aren't compatible with the CLI core
                         logger.warning(ex)
                         continue
                     ext_name = ext.name
                     ext_dir = ext.path or get_extension_path(ext_name)
```

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_completers.py` & `azure-cli-core-2.9.1/azure/cli/core/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_config.py` & `azure-cli-core-2.9.1/azure/cli/core/_config.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_debug.py` & `azure-cli-core-2.9.1/azure/cli/core/_debug.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_environment.py` & `azure-cli-core-2.9.1/azure/cli/core/_environment.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_help.py` & `azure-cli-core-2.9.1/azure/cli/core/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_help_loaders.py` & `azure-cli-core-2.9.1/azure/cli/core/_help_loaders.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_msal.py` & `azure-cli-core-2.9.1/azure/cli/core/_msal.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_output.py` & `azure-cli-core-2.9.1/azure/cli/core/_output.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_profile.py` & `azure-cli-core-2.9.1/azure/cli/core/_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 
 from azure.cli.core._environment import get_config_dir
 from azure.cli.core._session import ACCOUNT
 from azure.cli.core.util import get_file_json, in_cloud_console, open_page_in_browser, can_launch_browser,\
     is_windows, is_wsl
 from azure.cli.core.cloud import get_active_cloud, set_cloud_subscription
 
-from .adal_authentication import MSIAuthenticationWrapper
-
 from knack.log import get_logger
 from knack.util import CLIError
 
 logger = get_logger(__name__)
 
 # Names below are used by azure-xplat-cli to persist account information into
 # ~/.azure/azureProfile.json or osx/keychainer or windows secure storage,
@@ -305,14 +303,15 @@
 
     def find_subscriptions_in_vm_with_msi(self, identity_id=None, allow_no_subscriptions=None):
         # pylint: disable=too-many-statements
 
         import jwt
         from requests import HTTPError
         from msrestazure.tools import is_valid_resource_id
+        from azure.cli.core.adal_authentication import MSIAuthenticationWrapper
         resource = self.cli_ctx.cloud.endpoints.active_directory_resource_id
 
         if identity_id:
             if is_valid_resource_id(identity_id):
                 msi_creds = MSIAuthenticationWrapper(resource=resource, msi_res_id=identity_id)
                 identity_type = MsiAccountTypes.user_assigned_resource_id
             else:
@@ -384,14 +383,15 @@
         consolidated = self._normalize_properties(user, subscriptions, is_service_principal=False)
         for s in consolidated:
             s[_USER_ENTITY][_CLOUD_SHELL_ID] = True
         self._set_subscriptions(consolidated)
         return deepcopy(consolidated)
 
     def _get_token_from_cloud_shell(self, resource):  # pylint: disable=no-self-use
+        from azure.cli.core.adal_authentication import MSIAuthenticationWrapper
         auth = MSIAuthenticationWrapper(resource=resource)
         auth.set_token()
         token_entry = auth.token
         return (token_entry['token_type'], token_entry['access_token'], token_entry)
 
     def _set_subscriptions(self, new_subscriptions, merge=True, secondary_key_name=None):
 
@@ -769,14 +769,15 @@
     @staticmethod
     def valid_msi_account_types():
         return [MsiAccountTypes.system_assigned, MsiAccountTypes.user_assigned_client_id,
                 MsiAccountTypes.user_assigned_object_id, MsiAccountTypes.user_assigned_resource_id]
 
     @staticmethod
     def msi_auth_factory(cli_account_name, identity, resource):
+        from azure.cli.core.adal_authentication import MSIAuthenticationWrapper
         if cli_account_name == MsiAccountTypes.system_assigned:
             return MSIAuthenticationWrapper(resource=resource)
         if cli_account_name == MsiAccountTypes.user_assigned_client_id:
             return MSIAuthenticationWrapper(resource=resource, client_id=identity)
         if cli_account_name == MsiAccountTypes.user_assigned_object_id:
             return MSIAuthenticationWrapper(resource=resource, object_id=identity)
         if cli_account_name == MsiAccountTypes.user_assigned_resource_id:
```

### Comparing `azure-cli-core-2.9.0/azure/cli/core/_session.py` & `azure-cli-core-2.9.1/azure/cli/core/_session.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/adal_authentication.py` & `azure-cli-core-2.9.1/azure/cli/core/adal_authentication.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/api.py` & `azure-cli-core-2.9.1/azure/cli/core/api.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/azlogging.py` & `azure-cli-core-2.9.1/azure/cli/core/azlogging.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/cloud.py` & `azure-cli-core-2.9.1/azure/cli/core/cloud.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/__init__.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/arm.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/arm.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/client_factory.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/constants.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/constants.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/events.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/events.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/parameters.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/parameters.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/progress.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/progress.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/template_create.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/template_create.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/transform.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/transform.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/commands/validators.py` & `azure-cli-core-2.9.1/azure/cli/core/commands/validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/decorators.py` & `azure-cli-core-2.9.1/azure/cli/core/decorators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/extension/__init__.py` & `azure-cli-core-2.9.1/azure/cli/core/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/extension/_homebrew_patch.py` & `azure-cli-core-2.9.1/azure/cli/core/extension/_homebrew_patch.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/extension/_index.py` & `azure-cli-core-2.9.1/azure/cli/core/extension/_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
-import requests
 
 from knack.log import get_logger
 from knack.util import CLIError
 
 logger = get_logger(__name__)
 
 DEFAULT_INDEX_URL = "https://aka.ms/azure-cli-extension-index-v1"
@@ -18,14 +17,15 @@
 
 ERR_UNABLE_TO_GET_EXTENSIONS = 'Unable to get extensions from index. Improper index format.'
 TRIES = 3
 
 
 # pylint: disable=inconsistent-return-statements
 def get_index(index_url=None):
+    import requests
     from azure.cli.core.util import should_disable_connection_verify
     index_url = index_url or DEFAULT_INDEX_URL
 
     for try_number in range(TRIES):
         try:
             response = requests.get(index_url, verify=(not should_disable_connection_verify()))
             if response.status_code == 200:
```

### Comparing `azure-cli-core-2.9.0/azure/cli/core/extension/_resolve.py` & `azure-cli-core-2.9.1/azure/cli/core/extension/_resolve.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/extension/operations.py` & `azure-cli-core-2.9.1/azure/cli/core/extension/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import shutil
 import zipfile
 import traceback
 import hashlib
 from subprocess import check_output, STDOUT, CalledProcessError
 from six.moves.urllib.parse import urlparse  # pylint: disable=import-error
 
-import requests
 from pkg_resources import parse_version
 
 from azure.cli.core import CommandIndex
 from azure.cli.core.util import CLIError, reload_module
 from azure.cli.core.extension import (extension_exists, build_extension_path, get_extensions, get_extension_modname,
                                       get_extension, ext_compat_with_cli,
                                       EXT_METADATA_ISPREVIEW, EXT_METADATA_ISEXPERIMENTAL,
@@ -60,14 +59,15 @@
         if "PermissionError: [WinError 5]" in e.output:
             logger.warning("You do not have the permission to add extensions in the target directory%s. You may need to rerun on a shell as administrator.", ': ' + os.path.split(extension_path)[0] if extension_path else '')
         returncode = e.returncode
     return returncode
 
 
 def _whl_download_from_url(url_parse_result, ext_file):
+    import requests
     from azure.cli.core.util import should_disable_connection_verify
     url = url_parse_result.geturl()
     r = requests.get(url, stream=True, verify=(not should_disable_connection_verify()))
     if r.status_code != 200:
         raise CLIError("Request to {} failed with {}".format(url, r.status_code))
     with open(ext_file, 'wb') as f:
         for chunk in r.iter_content(chunk_size=1024):
@@ -102,14 +102,15 @@
         raise CLIError('The extension {} already exists.'.format(extension_name))
     ext_file = None
     if is_url:
         # Download from URL
         tmp_dir = tempfile.mkdtemp()
         ext_file = os.path.join(tmp_dir, whl_filename)
         logger.debug('Downloading %s to %s', source, ext_file)
+        import requests
         try:
             cmd.cli_ctx.get_progress_controller().add(message='Downloading')
             _whl_download_from_url(url_parse_result, ext_file)
         except (requests.exceptions.ConnectionError, requests.exceptions.HTTPError) as err:
             raise CLIError('Please ensure you have network connection. Error detail: {}'.format(str(err)))
         logger.debug('Downloaded to %s', ext_file)
     else:
```

### Comparing `azure-cli-core-2.9.0/azure/cli/core/file_util.py` & `azure-cli-core-2.9.1/azure/cli/core/file_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/keys.py` & `azure-cli-core-2.9.1/azure/cli/core/keys.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/local_context.py` & `azure-cli-core-2.9.1/azure/cli/core/local_context.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/mock.py` & `azure-cli-core-2.9.1/azure/cli/core/mock.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/parser.py` & `azure-cli-core-2.9.1/azure/cli/core/parser.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/profiles/__init__.py` & `azure-cli-core-2.9.1/azure/cli/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/profiles/_shared.py` & `azure-cli-core-2.9.1/azure/cli/core/profiles/_shared.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/telemetry.py` & `azure-cli-core-2.9.1/azure/cli/core/telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure/cli/core/util.py` & `azure-cli-core-2.9.1/azure/cli/core/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -731,42 +731,47 @@
     # https://management.azure.com + /subscriptions/xxx/resourcegroups/xxx?api-version=2019-07-01
     if '://' not in url:
         url = endpoints.resource_manager.rstrip('/') + url
 
     # Replace common tokens with real values. It is for smooth experience if users copy and paste the url from
     # Azure Rest API doc
     from azure.cli.core._profile import Profile
-    profile = Profile()
+    profile = Profile(cli_ctx=cli_ctx)
     if '{subscriptionId}' in url:
         url = url.replace('{subscriptionId}', cli_ctx.data['subscription_id'] or profile.get_subscription_id())
 
+    # Prepare the Bearer token for `Authorization` header
     if not skip_authorization_header and url.lower().startswith('https://'):
-        # Prepare `resource`
+        # Prepare `resource` for `get_raw_token`
         if not resource:
-            # If url starts with ARM endpoint, like https://management.azure.com/,
-            # use active_directory_resource_id for resource.
-            # This follows the same behavior as azure.cli.core.commands.client_factory._get_mgmt_service_client
+            # If url starts with ARM endpoint, like `https://management.azure.com/`,
+            # use `active_directory_resource_id` for resource, like `https://management.core.windows.net/`.
+            # This follows the same behavior as `azure.cli.core.commands.client_factory._get_mgmt_service_client`
             if url.lower().startswith(endpoints.resource_manager.rstrip('/')):
                 resource = endpoints.active_directory_resource_id
             else:
                 from azure.cli.core.cloud import CloudEndpointNotSetException
                 for p in [x for x in dir(endpoints) if not x.startswith('_')]:
                     try:
                         value = getattr(endpoints, p)
                     except CloudEndpointNotSetException:
                         continue
                     if isinstance(value, six.string_types) and url.lower().startswith(value.lower()):
                         resource = value
                         break
         if resource:
-            # If this is an ARM request, extract subscription ID from the URL.
-            # In the future when multi-tenant subscription is supported, we won't be able to uniquely identity the token
-            # from subscription anymore.
+            # Prepare `subscription` for `get_raw_token`
+            # If this is an ARM request, try to extract subscription ID from the URL.
+            # But there are APIs which don't require subscription ID, like /subscriptions, /tenants
+            # TODO: In the future when multi-tenant subscription is supported, we won't be able to uniquely identify
+            #   the token from subscription anymore.
+            token_subscription = None
             if url.lower().startswith(endpoints.resource_manager.rstrip('/')):
                 token_subscription = _extract_subscription_id(url)
+            if token_subscription:
                 logger.debug('Retrieving token for resource %s, subscription %s', resource, token_subscription)
                 token_info, _, _ = profile.get_raw_token(resource, subscription=token_subscription)
             else:
                 logger.debug('Retrieving token for resource %s', resource)
                 token_info, _, _ = profile.get_raw_token(resource)
             token_type, token, _ = token_info
             headers = headers or {}
@@ -800,17 +805,20 @@
     return r
 
 
 def _extract_subscription_id(url):
     """Extract the subscription ID from an ARM request URL."""
     subscription_regex = '/subscriptions/([0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12})'
     match = re.search(subscription_regex, url, re.IGNORECASE)
-    if not match:
-        raise CLIError('No subscription ID specified in the URL')
-    return match.groups()[0]
+    if match:
+        subscription_id = match.groups()[0]
+        logger.debug('Found subscription ID %s in the URL %s', subscription_id, url)
+        return subscription_id
+    logger.debug('No subscription ID specified in the URL %s', url)
+    return None
 
 
 def _log_request(request):
     """Log a client request. Copied from msrest
     https://github.com/Azure/msrest-for-python/blob/3653d29fc44da408898b07c710290a83d196b777/msrest/http_logger.py#L39
     """
     if not logger.isEnabledFor(logging.DEBUG):
```

### Comparing `azure-cli-core-2.9.0/azure_bdist_wheel.py` & `azure-cli-core-2.9.1/azure_bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/azure_cli_core.egg-info/PKG-INFO` & `azure-cli-core-2.9.1/azure_cli_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: azure-cli-core
-Version: 2.9.0
+Version: 2.9.1
 Summary: Microsoft Azure Command-Line Tools Core Module
 Home-page: https://github.com/Azure/azure-cli
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Description: Microsoft Azure CLI Core Module
         ==================================
         
         
         .. :changelog:
         
         Release History
         ===============
         
+        2.9.1
+        ++++++
+        * Minor fixes
+        
         2.9.0
         ++++++
         * Fix get_token() issue in msi login and `expiresIn` key error in cloud shell login credentials for track 2 SDK related commands (#14187)
         
         2.8.0
         ++++++
         * Add get_command_loader() entry to support to load customized CommandLoader (#13763)
```

### Comparing `azure-cli-core-2.9.0/azure_cli_core.egg-info/SOURCES.txt` & `azure-cli-core-2.9.1/azure_cli_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-core-2.9.0/setup.py` & `azure-cli-core-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from azure_bdist_wheel import cmdclass
 except ImportError:
     from distutils import log as logger
 
     logger.warn("Wheel is not available, disabling bdist_wheel hook")
     cmdclass = {}
 
-VERSION = "2.9.0"
+VERSION = "2.9.1"
 # If we have source, validate that our version numbers match
 # This should prevent uploading releases with mismatched versions.
 try:
     with open('azure/cli/core/__init__.py', 'r', encoding='utf-8') as f:
         content = f.read()
 except OSError:
     pass
```

