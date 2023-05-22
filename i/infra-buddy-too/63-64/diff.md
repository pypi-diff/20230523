# Comparing `tmp/infra-buddy-too-63.tar.gz` & `tmp/infra-buddy-too-64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infra-buddy-too-63.tar", last modified: Fri May 12 17:54:16 2023, max compression
+gzip compressed data, was "infra-buddy-too-64.tar", last modified: Mon May 22 14:07:04 2023, max compression
```

## Comparing `infra-buddy-too-63.tar` & `infra-buddy-too-64.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.433896 infra-buddy-too-63/
--rw-rw-r--   0 runner    (1001) docker     (123)       56 2023-05-12 17:54:15.000000 infra-buddy-too-63/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 17:54:16.433896 infra-buddy-too-63/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.425896 infra-buddy-too-63/infra_buddy_too/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/aws/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/aws/cloudwatch_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/aws/ecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5271 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commandline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/bootstrap/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/deploy_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/deploy_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/deploy_cloudformation/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/deploy_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/deploy_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/deploy_service/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/generate_artifact_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/generate_artifact_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/generate_artifact_manifest/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/generate_service_definition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/generate_service_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/generate_service_definition/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/introspect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/introspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/introspect/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/commands/validate_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/validate_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/commands/validate_template/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/context/artifact_definition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14267 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/context/deploy_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/context/monitor_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/context/service_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.433896 infra-buddy-too-63/infra_buddy_too/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/deploy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17041 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/deploy/cloudformation_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/deploy/datadog_monitor_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/deploy/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/deploy/ecs_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/deploy/s3_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.433896 infra-buddy-too-63/infra_buddy_too/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/notifier/datadog_notifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.433896 infra-buddy-too-63/infra_buddy_too/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/template/builtin-templates.json
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/template/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8950 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/template/template_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.433896 infra-buddy-too-63/infra_buddy_too/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/utility/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9442 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/utility/helper_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/utility/print_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-12 17:53:40.000000 infra-buddy-too-63/infra_buddy_too/utility/waitfor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.429896 infra-buddy-too-63/infra_buddy_too.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 17:54:16.000000 infra-buddy-too-63/infra_buddy_too.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-12 17:54:16.000000 infra-buddy-too-63/infra_buddy_too.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:16.000000 infra-buddy-too-63/infra_buddy_too.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:16.000000 infra-buddy-too-63/infra_buddy_too.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 17:54:16.000000 infra-buddy-too-63/infra_buddy_too.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 17:54:16.000000 infra-buddy-too-63/infra_buddy_too.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:16.000000 infra-buddy-too-63/infra_buddy_too.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:16.433896 infra-buddy-too-63/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-12 17:54:15.000000 infra-buddy-too-63/scripts/infra-buddy
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:54:16.433896 infra-buddy-too-63/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-05-12 17:54:15.000000 infra-buddy-too-63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.559401 infra-buddy-too-64/
+-rw-rw-r--   0 runner    (1001) docker     (123)       56 2023-05-22 14:07:03.000000 infra-buddy-too-64/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 14:07:04.559401 infra-buddy-too-64/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/aws/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/aws/cloudwatch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/aws/ecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5271 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commandline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/bootstrap/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/deploy_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/deploy_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/deploy_cloudformation/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/deploy_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/deploy_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/deploy_service/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/generate_artifact_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/generate_artifact_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/generate_artifact_manifest/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/generate_service_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/generate_service_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/generate_service_definition/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/introspect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/introspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/introspect/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/commands/validate_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/validate_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/commands/validate_template/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/context/artifact_definition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14267 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/context/deploy_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/context/monitor_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/context/service_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/deploy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17041 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/deploy/cloudformation_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/deploy/datadog_monitor_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/deploy/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/deploy/ecs_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/deploy/s3_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.559401 infra-buddy-too-64/infra_buddy_too/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/notifier/datadog_notifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.559401 infra-buddy-too-64/infra_buddy_too/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/template/builtin-templates.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/template/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8950 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/template/template_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.559401 infra-buddy-too-64/infra_buddy_too/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/utility/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9442 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/utility/helper_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/utility/print_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-22 14:06:28.000000 infra-buddy-too-64/infra_buddy_too/utility/waitfor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.555401 infra-buddy-too-64/infra_buddy_too.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 14:07:04.000000 infra-buddy-too-64/infra_buddy_too.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-22 14:07:04.000000 infra-buddy-too-64/infra_buddy_too.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:07:04.000000 infra-buddy-too-64/infra_buddy_too.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:07:04.000000 infra-buddy-too-64/infra_buddy_too.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 14:07:04.000000 infra-buddy-too-64/infra_buddy_too.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 14:07:04.000000 infra-buddy-too-64/infra_buddy_too.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:07:04.000000 infra-buddy-too-64/infra_buddy_too.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:07:04.559401 infra-buddy-too-64/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-22 14:07:03.000000 infra-buddy-too-64/scripts/infra-buddy
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:07:04.559401 infra-buddy-too-64/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-05-22 14:07:03.000000 infra-buddy-too-64/setup.py
```

### Comparing `infra-buddy-too-63/infra_buddy_too/aws/cloudformation.py` & `infra-buddy-too-64/infra_buddy_too/aws/cloudformation.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/aws/cloudwatch_logs.py` & `infra-buddy-too-64/infra_buddy_too/aws/cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/aws/config.py` & `infra-buddy-too-64/infra_buddy_too/aws/config.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/aws/ecs.py` & `infra-buddy-too-64/infra_buddy_too/aws/ecs.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/aws/s3.py` & `infra-buddy-too-64/infra_buddy_too/aws/s3.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/commandline.py` & `infra-buddy-too-64/infra_buddy_too/commandline.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
               type=click.Path(exists=True),
               help='A directory where a service definition (service.json) and supporting files can be found.')
 @click.option("--application", envvar='APPLICATION', help='The application name.')
 @click.option("--role", envvar='ROLE', help='The role name')
 @click.option("--environment", envvar='ENVIRONMENT', help='The environment the deployment should target.')
 @click.option("--configuration-defaults", envvar='CONFIG_DEFAULTS', type=click.Path(exists=True),
               help='A json file with a dictionary of the default values, if defaults.json is in CWD it will be used.')
-@click.option("--verbose", is_flag=True, help='Print verbose status messages')
+@click.option("--verbose", envvar='IB_DEBUG', is_flag=True, help='Print verbose status messages')
 @click.pass_context
 def cli(ctx, artifact_directory, application, role, environment, configuration_defaults, verbose):
     # type: (object, str, str, str, str, str, bool) -> None
     """
     CLI for managing the infrastructure for deploying micro-services in AWS.
     """
     print_utility.configure(verbose)
```

### Comparing `infra-buddy-too-63/infra_buddy_too/commands/bootstrap/command.py` & `infra-buddy-too-64/infra_buddy_too/commands/bootstrap/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/commands/deploy_cloudformation/command.py` & `infra-buddy-too-64/infra_buddy_too/commands/deploy_cloudformation/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/commands/deploy_service/command.py` & `infra-buddy-too-64/infra_buddy_too/commands/deploy_service/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/commands/generate_artifact_manifest/command.py` & `infra-buddy-too-64/infra_buddy_too/commands/generate_artifact_manifest/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/commands/generate_service_definition/command.py` & `infra-buddy-too-64/infra_buddy_too/commands/generate_service_definition/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/commands/introspect/command.py` & `infra-buddy-too-64/infra_buddy_too/commands/introspect/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/commands/validate_template/command.py` & `infra-buddy-too-64/infra_buddy_too/commands/validate_template/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/context/artifact_definition.py` & `infra-buddy-too-64/infra_buddy_too/context/artifact_definition.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/context/deploy_ctx.py` & `infra-buddy-too-64/infra_buddy_too/context/deploy_ctx.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/context/monitor_definition.py` & `infra-buddy-too-64/infra_buddy_too/context/monitor_definition.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/context/service_definition.py` & `infra-buddy-too-64/infra_buddy_too/context/service_definition.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/deploy/cloudformation_deploy.py` & `infra-buddy-too-64/infra_buddy_too/deploy/cloudformation_deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/deploy/datadog_monitor_deploy.py` & `infra-buddy-too-64/infra_buddy_too/deploy/datadog_monitor_deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/deploy/deploy.py` & `infra-buddy-too-64/infra_buddy_too/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/deploy/ecs_deploy.py` & `infra-buddy-too-64/infra_buddy_too/deploy/ecs_deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/deploy/s3_deploy.py` & `infra-buddy-too-64/infra_buddy_too/deploy/s3_deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/notifier/datadog_notifier.py` & `infra-buddy-too-64/infra_buddy_too/notifier/datadog_notifier.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/template/builtin-templates.json` & `infra-buddy-too-64/infra_buddy_too/template/builtin-templates.json`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/template/template.py` & `infra-buddy-too-64/infra_buddy_too/template/template.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/template/template_manager.py` & `infra-buddy-too-64/infra_buddy_too/template/template_manager.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/utility/helper_functions.py` & `infra-buddy-too-64/infra_buddy_too/utility/helper_functions.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/utility/print_utility.py` & `infra-buddy-too-64/infra_buddy_too/utility/print_utility.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too/utility/waitfor.py` & `infra-buddy-too-64/infra_buddy_too/utility/waitfor.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/infra_buddy_too.egg-info/SOURCES.txt` & `infra-buddy-too-64/infra_buddy_too.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-63/setup.py` & `infra-buddy-too-64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'infra-buddy-too',
-        version = '63',
+        version = '64',
         description = 'CLI for deploying micro-services',
         long_description = 'CLI for deploying micro-services',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```

