# Comparing `tmp/dev-gpt-0.18.41.dev9.tar.gz` & `tmp/dev-gpt-0.18.42.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.41.dev9.tar", last modified: Mon May 15 15:27:54 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.42.dev1.tar", last modified: Mon May 22 22:05:58 2023, max compression
```

## Comparing `dev-gpt-0.18.41.dev9.tar` & `dev-gpt-0.18.42.dev1.tar`

### file list

```diff
@@ -1,88 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.621939 dev-gpt-0.18.41.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-05-15 15:27:54.621939 dev-gpt-0.18.41.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20391 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.613939 dev-gpt-0.18.41.dev9/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 15:27:54.000000 dev-gpt-0.18.41.dev9/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.613939 dev-gpt-0.18.41.dev9/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.613939 dev-gpt-0.18.41.dev9/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.613939 dev-gpt-0.18.41.dev9/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.613939 dev-gpt-0.18.41.dev9/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/auto_refine_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/extract_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/get_user_input_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/pm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/pm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/pm/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/pm/task_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/prompt_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.613939 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.613939 dev-gpt-0.18.41.dev9/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-05-15 15:27:54.000000 dev-gpt-0.18.41.dev9/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-15 15:27:54.000000 dev-gpt-0.18.41.dev9/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:27:54.000000 dev-gpt-0.18.41.dev9/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 15:27:54.000000 dev-gpt-0.18.41.dev9/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-15 15:27:54.000000 dev-gpt-0.18.41.dev9/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 15:27:54.000000 dev-gpt-0.18.41.dev9/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:27:54.621939 dev-gpt-0.18.41.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:54.617939 dev-gpt-0.18.41.dev9/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/unit/test_construct_sub_task_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-15 15:27:49.000000 dev-gpt-0.18.41.dev9/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.191062 dev-gpt-0.18.42.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-05-22 22:05:58.191062 dev-gpt-0.18.42.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 22:05:57.000000 dev-gpt-0.18.42.dev1/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/auto_refine_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/extract_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/get_user_input_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/conversation_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31796 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/pm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/pm/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/pm/task_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/prompt_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.183062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/app_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/microservice/google_custom_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/templates_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.191062 dev-gpt-0.18.42.dev1/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.187062 dev-gpt-0.18.42.dev1/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-05-22 22:05:58.000000 dev-gpt-0.18.42.dev1/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-22 22:05:58.000000 dev-gpt-0.18.42.dev1/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:05:58.000000 dev-gpt-0.18.42.dev1/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-22 22:05:58.000000 dev-gpt-0.18.42.dev1/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-22 22:05:58.000000 dev-gpt-0.18.42.dev1/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 22:05:58.000000 dev-gpt-0.18.42.dev1/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:05:58.191062 dev-gpt-0.18.42.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.191062 dev-gpt-0.18.42.dev1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.191062 dev-gpt-0.18.42.dev1/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:58.191062 dev-gpt-0.18.42.dev1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/unit/test_construct_sub_task_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/unit/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/unit/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-22 22:05:51.000000 dev-gpt-0.18.42.dev1/test/unit/test_tools.py
```

### Comparing `dev-gpt-0.18.41.dev9/LICENSE` & `dev-gpt-0.18.42.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/PKG-INFO` & `dev-gpt-0.18.42.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.41.dev9
+Version: 0.18.42.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -65,33 +65,39 @@
 </a>
 <a href="https://github.com/tiangolo/dev-gpt/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://img.shields.io/badge/platform-mac%20%7C%20linux%20%7C%20windows-blue" alt="Supported platforms">
 </a>
 <a href="https://pypistats.org/packages/dev-gpt" target="_blank">
     <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
-<a href="https://discord.gg/tBrFhx384D" target="_blank">
-    <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
-</a>
+<a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
+
 
 </p>
 
-Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
+Welcome to Dev-GPT, where we bring your ideas to life with the power of advanced artificial intelligence! 
+Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. 
+Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
 ## Quickstart
 
 ```bash
 pip install dev-gpt
 dev-gpt generate
 ```
 
 ### Requirements
 - OpenAI key with access to gpt-3.5-turbo or gpt-4
+- if you want to enable your microservice to search for web content, 
+you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID environment variables.
+More information can be found [here](https://developers.google.com/custom-search/v1/overview).
 ```bash
-dev-gpt configure --key <your openai api key>
+dev-gpt configure --openai_api_key <your openai api key>
+dev-gpt configure --google_api_key <google api key> (optional if you want to use google search)
+dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google search)
 ```
 
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ## Docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.41.dev9 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.42.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -12,27 +12,34 @@
             ****** Dev GPT: Your Automated Development Team ******
                 â ï¸ This is an experimental version. â ï¸
                     [Product Manager] [Developer] [DevOps]
                      Product Manager   Developer   DevOps
 Tell your AI team what microservice you want to build, and they will do it for
                       you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
-                     platforms] [Downloads] [Discord_Chat]
-Welcome to Dev GPT, where we bring your ideas to life with the power of
+            platforms] [Downloads] [https://img.shields.io/discord/
+      1106542220112302130?logo=discord&logoColor=white&style=flat-square]
+Welcome to Dev-GPT, where we bring your ideas to life with the power of
 advanced artificial intelligence! Our automated development team is designed to
 create microservices tailored to your specific needs, making your software
 development process seamless and efficient. Comprised of a virtual Product
 Manager, Developer, and DevOps, our AI team ensures that every aspect of your
 project is covered, from concept to deployment. ## Quickstart ```bash pip
 install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
-to gpt-3.5-turbo or gpt-4 ```bash dev-gpt configure --key  ``` If you set the
-environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
-Your api key must have access to gpt-4 to use this tool. We are working on a
-way to use gpt-3.5-turbo as well. ## Docs ### Generate Microservice ```bash
-dev-gpt generate \ --description "" \ --model
+to gpt-3.5-turbo or gpt-4 - if you want to enable your microservice to search
+for web content, you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID
+environment variables. More information can be found [here](https://
+developers.google.com/custom-search/v1/overview). ```bash dev-gpt configure --
+openai_api_key  dev-gpt configure --google_api_key  (optional if you want to
+use google search) dev-gpt configure --google_cse_id  (optional if you want to
+use google search) ``` If you set the environment variable `OPENAI_API_KEY`,
+the configuration step can be skipped. Your api key must have access to gpt-
+4 to use this tool. We are working on a way to use gpt-3.5-turbo as well. ##
+Docs ### Generate Microservice ```bash dev-gpt generate \ --description "" \ --
+model
 5-turbo or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5-turbo` or `gpt-4`. `gpt-3.5-
 turbo` is ~10x cheaper, but will not be able to generate as complex
 microservices. (default: largest you have access to) - A `path` on the local
 drive where the microservice will be generated. (default: ./microservice) The
```

### Comparing `dev-gpt-0.18.41.dev9/README.md` & `dev-gpt-0.18.42.dev1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,33 +45,39 @@
 </a>
 <a href="https://github.com/tiangolo/dev-gpt/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://img.shields.io/badge/platform-mac%20%7C%20linux%20%7C%20windows-blue" alt="Supported platforms">
 </a>
 <a href="https://pypistats.org/packages/dev-gpt" target="_blank">
     <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
-<a href="https://discord.gg/tBrFhx384D" target="_blank">
-    <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
-</a>
+<a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
+
 
 </p>
 
-Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
+Welcome to Dev-GPT, where we bring your ideas to life with the power of advanced artificial intelligence! 
+Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. 
+Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
 ## Quickstart
 
 ```bash
 pip install dev-gpt
 dev-gpt generate
 ```
 
 ### Requirements
 - OpenAI key with access to gpt-3.5-turbo or gpt-4
+- if you want to enable your microservice to search for web content, 
+you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID environment variables.
+More information can be found [here](https://developers.google.com/custom-search/v1/overview).
 ```bash
-dev-gpt configure --key <your openai api key>
+dev-gpt configure --openai_api_key <your openai api key>
+dev-gpt configure --google_api_key <google api key> (optional if you want to use google search)
+dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google search)
 ```
 
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ## Docs
```

#### html2text {}

```diff
@@ -1,27 +1,34 @@
             ****** Dev GPT: Your Automated Development Team ******
                 â ï¸ This is an experimental version. â ï¸
                     [Product Manager] [Developer] [DevOps]
                      Product Manager   Developer   DevOps
 Tell your AI team what microservice you want to build, and they will do it for
                       you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
-                     platforms] [Downloads] [Discord_Chat]
-Welcome to Dev GPT, where we bring your ideas to life with the power of
+            platforms] [Downloads] [https://img.shields.io/discord/
+      1106542220112302130?logo=discord&logoColor=white&style=flat-square]
+Welcome to Dev-GPT, where we bring your ideas to life with the power of
 advanced artificial intelligence! Our automated development team is designed to
 create microservices tailored to your specific needs, making your software
 development process seamless and efficient. Comprised of a virtual Product
 Manager, Developer, and DevOps, our AI team ensures that every aspect of your
 project is covered, from concept to deployment. ## Quickstart ```bash pip
 install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
-to gpt-3.5-turbo or gpt-4 ```bash dev-gpt configure --key  ``` If you set the
-environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
-Your api key must have access to gpt-4 to use this tool. We are working on a
-way to use gpt-3.5-turbo as well. ## Docs ### Generate Microservice ```bash
-dev-gpt generate \ --description "" \ --model
+to gpt-3.5-turbo or gpt-4 - if you want to enable your microservice to search
+for web content, you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID
+environment variables. More information can be found [here](https://
+developers.google.com/custom-search/v1/overview). ```bash dev-gpt configure --
+openai_api_key  dev-gpt configure --google_api_key  (optional if you want to
+use google search) dev-gpt configure --google_cse_id  (optional if you want to
+use google search) ``` If you set the environment variable `OPENAI_API_KEY`,
+the configuration step can be skipped. Your api key must have access to gpt-
+4 to use this tool. We are working on a way to use gpt-3.5-turbo as well. ##
+Docs ### Generate Microservice ```bash dev-gpt generate \ --description "" \ --
+model
 5-turbo or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5-turbo` or `gpt-4`. `gpt-3.5-
 turbo` is ~10x cheaper, but will not be able to generate as complex
 microservices. (default: largest you have access to) - A `path` on the local
 drive where the microservice will be generated. (default: ./microservice) The
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.42.dev1/dev_gpt/apis/gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 from langchain.schema import HumanMessage, SystemMessage, BaseMessage, AIMessage
 from openai.error import RateLimitError
 from requests.exceptions import ConnectionError, ChunkedEncodingError
 from urllib3.exceptions import InvalidChunkLength
 
 from dev_gpt.constants import PRICING_GPT4_PROMPT, PRICING_GPT4_GENERATION, PRICING_GPT3_5_TURBO_PROMPT, \
     PRICING_GPT3_5_TURBO_GENERATION, CHARS_PER_TOKEN
+from dev_gpt.options.generate.conversation_logger import ConversationLogger
 from dev_gpt.options.generate.templates_system import template_system_message_base
 from dev_gpt.utils.string_tools import print_colored, get_template_parameters
 
 
 def configure_openai_api_key():
     if 'OPENAI_API_KEY' not in os.environ:
         print_colored('You need to set OPENAI_API_KEY in your environment.', '''
 Run:
-dev-gpt configure --key <your_openai_api_key>
+dev-gpt configure --openai_api_key <your_openai_api_key>
 
 If you have updated it already, please restart your terminal.
 ''', 'red')
         exit(1)
     openai.api_key = os.environ['OPENAI_API_KEY']
 
 
@@ -37,35 +38,39 @@
     _initialized = False
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super(GPTSession, cls).__new__(cls)
         return cls._instance
 
-    def __init__(self, model: str = 'gpt-4', ):
+    def __init__(self, log_file_path: str, model: str = 'gpt-4', ):
         if GPTSession._initialized:
             return
+        self.conversation_logger = ConversationLogger(log_file_path)
         if model == 'gpt-4' and self.is_gpt4_available():
             self.pricing_prompt = PRICING_GPT4_PROMPT
             self.pricing_generation = PRICING_GPT4_GENERATION
         else:
             if model == 'gpt-4':
                 print_colored('GPT version info', 'GPT-4 is not available. Using GPT-3.5-turbo instead.', 'yellow')
             model = 'gpt-3.5-turbo'
             self.pricing_prompt = PRICING_GPT3_5_TURBO_PROMPT
             self.pricing_generation = PRICING_GPT3_5_TURBO_GENERATION
         self.model_name = model
         self.chars_prompt_so_far = 0
         self.chars_generation_so_far = 0
         GPTSession._initialized = True
 
+
+
+
     def get_conversation(self, messages: List[BaseMessage] = [], print_stream: bool = True, print_costs: bool = True):
         messages = deepcopy(messages)
         return _GPTConversation(
-            self.model_name, self.cost_callback, messages, print_stream, print_costs
+            self.model_name, self.cost_callback, messages, print_stream, print_costs, self.conversation_logger
         )
 
     @staticmethod
     def is_gpt4_available():
         try:
             for i in range(5):
                 try:
@@ -103,26 +108,27 @@
 class AssistantStreamingStdOutCallbackHandler(StreamingStdOutCallbackHandler):
     def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Run on new LLM token. Only available when streaming is enabled."""
         print_colored('', token, 'green', end='')
 
 
 class _GPTConversation:
-    def __init__(self, model: str, cost_callback, messages: List[BaseMessage], print_stream, print_costs):
+    def __init__(self, model: str, cost_callback, messages: List[BaseMessage], print_stream, print_costs, conversation_logger: ConversationLogger = None):
         self._chat = ChatOpenAI(
             model_name=model,
             streaming=True,
             callback_manager=CallbackManager([AssistantStreamingStdOutCallbackHandler()] if print_stream else []),
             verbose=True,
             temperature=0,
         )
         self.cost_callback = cost_callback
         self.messages = messages
         self.print_stream = print_stream
         self.print_costs = print_costs
+        self.conversation_logger = conversation_logger
 
     def print_messages(self, messages):
         for i, message in enumerate(messages):
             if os.environ['VERBOSE'].lower() == 'true':
                 if isinstance(message, SystemMessage):
                     print_colored(f'({i}) system - prompt', message.content, 'magenta')
                 elif isinstance(message, HumanMessage):
@@ -137,14 +143,15 @@
         self.print_messages(self.messages)
         if self.print_stream:
             print_colored('assistant', '', 'green', end='')
         print('thinking...')
         for i in range(10):
             try:
                 response = self._chat(self.messages)
+                self.conversation_logger.log(self.messages, response)
                 break
             except (ConnectionError, InvalidChunkLength, ChunkedEncodingError) as e:
                 print('There was a connection error. Retrying...')
                 if i == 9:
                     raise e
                 sleep(10)
 
@@ -169,15 +176,15 @@
         raise ValueError(
             f'Prompt template parameters {set(template_parameters)} do not match provided parameters {set(kwargs.keys())}'
         )
     for key, value in kwargs.items():
         if isinstance(value, dict):
             kwargs[key] = json.dumps(value, indent=4)
     prompt = prompt_template.format(**kwargs)
-    conversation = GPTSession().get_conversation(
+    conversation = GPTSession._instance.get_conversation(
         [],
         print_stream=os.environ['VERBOSE'].lower() == 'true',
         print_costs=False
     )
     agent_response_raw = conversation.chat(prompt, role='user')
     agent_response = parser(agent_response_raw)
     return agent_response
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.42.dev1/dev_gpt/apis/jina_cloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,19 +94,24 @@
     md5_hash.update(content)
     md5_digest = md5_hash.hexdigest()
 
     form_data = {
         'public': 'True',
         'private': 'False',
         'verbose': 'True',
-        'buildEnv': f'{{"OPENAI_API_KEY": "{os.environ["OPENAI_API_KEY"]}"}}',
+        'buildEnv': f'{{"OPENAI_API_KEY": "{os.environ["OPENAI_API_KEY"]}", "GOOGLE_API_KEY": "{os.environ.get("GOOGLE_API_KEY","")}", "GOOGLE_CSE_ID": "{os.environ.get("GOOGLE_CSE_ID","")}"}}',
         'md5sum': md5_digest,
     }
     with suppress_stdout():
         headers = get_request_header()
+        headers['jinameta-platform'] = 'Darwin'
+        headers['jinameta-platform-release'] = '21.1.0'
+        headers['jinameta-platform-version'] = 'Darwin Kernel Version 21.1.0: Wed Oct 13 17:33:23 PDT 2021; root:xnu-8019.41.5~1/RELEASE_X86_64'
+        headers['jinameta-architecture'] = 'x86_64'
+        headers['jinameta-processor'] = 'i386'
 
     resp = upload_file(
         'https://api.hubble.jina.ai/v2/rpc/executor.push',
         'filename',
         content,
         dict_data=form_data,
         headers=headers,
@@ -247,15 +252,17 @@
     {f"uses: {prefix}://{get_user_name(DEMO_TOKEN)}/Gateway{executor_name}:latest" if use_custom_gateway else ""}
     {"" if use_docker else "install-requirements: True"}
 executors:
   - name: {executor_name.lower()}
     uses: {prefix}://{get_user_name(DEMO_TOKEN)}/{executor_name}:latest
     {"" if use_docker else "install-requirements: True"}
     env:
-      OPENAI_API_KEY: {os.environ['OPENAI_API_KEY']}
+      OPENAI_API_KEY: ${{{{ ENV.OPENAI_API_KEY }}}}
+      GOOGLE_API_KEY: ${{{{ ENV.GOOGLE_API_KEY }}}}
+      GOOGLE_CSE_ID: ${{{{ ENV.GOOGLE_CSE_ID }}}}
     jcloud:
       resources:
         instance: C2
         capacity: spot
 '''
     full_flow_path = os.path.join(dest_folder,
                                   'flow.yml')
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.42.dev1/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/cli.py` & `dev-gpt-0.18.42.dev1/dev_gpt/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,14 +88,21 @@
     jina_auth_login()
     from dev_gpt.options.deploy.deployer import Deployer
     path = os.path.expanduser(path)
     path = os.path.abspath(path)
     Deployer().deploy(path)
 
 @main.command()
-@click.option('--key', required=True, help='Your OpenAI API key.')
-def configure(key):
-    set_api_key(key)
+@click.option('--openai-api-key', default=None, help='Your OpenAI API key.')
+@click.option('--google-api-key', default=None, help='Your Google API key.')
+@click.option('--google-cse-id', default=None, help='Your Google CSE ID.')
+def configure(openai_api_key, google_api_key, google_cse_id):
+    if openai_api_key:
+        set_api_key('OPENAI_API_KEY', openai_api_key)
+    if google_api_key:
+        set_api_key('GOOGLE_API_KEY', google_api_key)
+    if google_cse_id:
+        set_api_key('GOOGLE_CSE_ID', google_cse_id)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/constants.py` & `dev-gpt-0.18.42.dev1/dev_gpt/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,20 @@
     (TEST_EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_TAG),
     (REQUIREMENTS_FILE_NAME, REQUIREMENTS_FILE_TAG),
     (DOCKER_FILE_NAME, DOCKER_FILE_TAG),
     (CLIENT_FILE_NAME, CLIENT_FILE_TAG),
     (STREAMLIT_FILE_NAME, STREAMLIT_FILE_TAG)
 ]
 
+INDICATOR_TO_IMPORT_STATEMENT = {
+    'io.BytesIO': 'import io',
+    'BytesIO': 'from io import BytesIO',
+    'base64': 'import base64',
+}
+
 FLOW_URL_PLACEHOLDER = 'jcloud.jina.ai'
 
 PRICING_GPT4_PROMPT = 0.03
 PRICING_GPT4_GENERATION = 0.06
 PRICING_GPT3_5_TURBO_PROMPT = 0.002
 PRICING_GPT3_5_TURBO_GENERATION = 0.002
 
@@ -39,19 +45,24 @@
 MAX_DEBUGGING_ITERATIONS = 10
 
 DEMO_TOKEN = '45372338e04f5a41af949024db929d46'
 
 BLACKLISTED_PACKAGES = [
     'moderngl', 'pyopengl', 'pyglet', 'pythreejs', 'panda3d',  # because they need a screen,
     'tika',  # because it needs java
+    'clearbit'  # because of installation issues on latest version
 ]
 UNNECESSARY_PACKAGES = [
     'fastapi', 'uvicorn', 'starlette'  # because the wrappers are used instead
 ]
 
 LANGUAGE_PACKAGES = [
-    'allennlp', 'bertopic', 'fasttext', 'flair', 'gensim', 'nltk', 'openai',
+    'allennlp', 'bertopic', 'GPT-3', 'fasttext', 'flair', 'gensim', 'nltk', 'openai',
     'pattern', 'polyglot', 'pytorch-transformers', 'rasa', 'sentence-transformers',
     'spacy', 'stanza', 'summarizer', 'sumy', 'textblob', 'textstat', 'transformers',
     'vadersentiment'
 ]
 
+SEARCH_PACKAGES = [
+    'googlesearch-python', 'google', 'googlesearch', 'google-api-python-client', 'pygooglenews', 'google-cloud'
+]
+
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/__init__.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/configure/key_handling.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,105 +36,105 @@
 
         return None
     except Exception as e:
         click.echo(f"Error detecting shell: {e}")
         return None
 
 
-def get_shell_config(key):
+def get_shell_config(name, key):
     return {
-        "bash": {"config_file": "~/.bashrc", "export_line": f"export OPENAI_API_KEY={key}"},
-        "zsh": {"config_file": "~/.zshrc", "export_line": f"export OPENAI_API_KEY={key}"},
-        "sh": {"config_file": "~/.profile", "export_line": f"export OPENAI_API_KEY={key}"},
+        "bash": {"config_file": "~/.bashrc", "export_line": f"export {name}={key}"},
+        "zsh": {"config_file": "~/.zshrc", "export_line": f"export {name}={key}"},
+        "sh": {"config_file": "~/.profile", "export_line": f"export {name}={key}"},
         "fish": {
             "config_file": "~/.config/fish/config.fish",
-            "export_line": f"set -gx OPENAI_API_KEY {key}",
+            "export_line": f"set -gx {name} {key}",
         },
-        "csh": {"config_file": "~/.cshrc", "export_line": f"setenv OPENAI_API_KEY {key}"},
-        "tcsh": {"config_file": "~/.tcshrc", "export_line": f"setenv OPENAI_API_KEY {key}"},
-        "ksh": {"config_file": "~/.kshrc", "export_line": f"export OPENAI_API_KEY={key}"},
-        "dash": {"config_file": "~/.profile", "export_line": f"export OPENAI_API_KEY={key}"}
+        "csh": {"config_file": "~/.cshrc", "export_line": f"setenv {name} {key}"},
+        "tcsh": {"config_file": "~/.tcshrc", "export_line": f"setenv {name} {key}"},
+        "ksh": {"config_file": "~/.kshrc", "export_line": f"export {name}={key}"},
+        "dash": {"config_file": "~/.profile", "export_line": f"export {name}={key}"}
     }
 
 
-def set_env_variable(shell, key):
-    shell_config = get_shell_config(key)
+def set_env_variable(shell, name, key):
+    shell_config = get_shell_config(name, key)
     if shell not in shell_config:
-        click.echo("Sorry, your shell is not supported. Please add the key OPENAI_API_KEY manually.")
+        click.echo(f"Sorry, your shell is not supported. Please add the key {name} manually.")
         return
 
     config_file = os.path.expanduser(shell_config[shell]["config_file"])
 
     try:
         with open(config_file, "r", encoding='utf-8') as file:
             content = file.read()
 
         export_line = shell_config[shell]['export_line']
 
         # Update the existing API key if it exists, otherwise append it to the config file
-        if f"OPENAI_API_KEY" in content:
-            content = re.sub(r'OPENAI_API_KEY=.*', f'OPENAI_API_KEY={key}', content, flags=re.MULTILINE)
+        if f"{name}" in content:
+            content = re.sub(rf'{name}=.*', f'{name}={key}', content, flags=re.MULTILINE)
 
             with open(config_file, "w", encoding='utf-8') as file:
                 file.write(content)
         else:
             with open(config_file, "a", encoding='utf-8') as file:
                 file.write(f"\n{export_line}\n")
 
         click.echo(f'''
-✅ Success, OPENAI_API_KEY has been set in {config_file}.
+✅ Success, {name} has been set in {config_file}.
 Please restart your shell to apply the changes or run:
 source {config_file}
 '''
                    )
 
     except FileNotFoundError:
         click.echo(f"Error: {config_file} not found. Please set the environment variable manually.")
 
 
-def set_api_key(key):
+def set_api_key(name, key):
     system_platform = platform.system().lower()
 
     if system_platform == "windows":
-        set_env_variable_command = f'setx OPENAI_API_KEY "{key}"'
+        set_env_variable_command = f'setx {name} "{key}"'
         subprocess.call(set_env_variable_command, shell=True)
-        click.echo('''
-✅ Success, OPENAI_API_KEY has been set.
+        click.echo(f'''
+✅ Success, {name} has been set.
 Please restart your Command Prompt to apply the changes.
 '''
                    )
 
     elif system_platform in ["linux", "darwin"]:
-        if "OPENAI_API_KEY" in os.environ or is_key_set_in_config_file(key):
-            if not click.confirm("OPENAI_API_KEY is already set. Do you want to overwrite it?"):
+        if f"{name}" in os.environ or is_key_set_in_config_file(key):
+            if not click.confirm(f"{name} is already set. Do you want to overwrite it?"):
                 click.echo("Aborted.")
                 return
 
         shell = get_shell()
         if shell is None:
             click.echo(
                 "Error: Unable to detect your shell or psutil is not available. Please set the environment variable manually.")
             return
 
-        set_env_variable(shell, key)
+        set_env_variable(shell, name, key)
     else:
         click.echo("Sorry, this platform is not supported.")
 
 
-def is_key_set_in_config_file(key):
+def is_key_set_in_config_file(name, key):
     shell = get_shell()
     if shell is None:
         return False
 
-    shell_config = get_shell_config(key)
+    shell_config = get_shell_config(name, key)
 
     config_file = os.path.expanduser(shell_config[shell]["config_file"])
 
     try:
         with open(config_file, "r", encoding='utf-8') as file:
             content = file.read()
-            if f"OPENAI_API_KEY" in content:
+            if f"{name}" in content:
                 return True
     except FileNotFoundError:
         pass
 
     return False
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/auto_refine_description.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/auto_refine_description.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
 from dev_gpt.apis.gpt import ask_gpt
 from dev_gpt.options.generate.parser import identity_parser
 from dev_gpt.options.generate.prompt_factory import context_to_string
-
+from dev_gpt.options.generate.tools.tools import get_available_tools
 
 
 def auto_refine_description(context):
     context['microservice_description'] = ask_gpt(
         better_description_prompt,
         identity_parser,
         context_string=context_to_string(context)
@@ -32,26 +32,29 @@
     #     context['microservice_description'] += '\n\nAdditional information:' + json.dumps(details, indent=4)
     # del context['details']
 
 
 better_description_prompt = f'''{{context_string}}
 Update the description of the Microservice to make it more precise without adding or removing information.
 Note: the output must be a list of tasks the Microservice has to perform.
-Example for the description: "return the average temperature of the 5 days weather forecast for a given location."
+Note: you can uses two tools if necessary:
+{get_available_tools()}
+Example for the description: "return a description of the average temperature of the 5 days weather forecast for a given location."
 1. get the 5 days weather forcast from the https://openweathermap.org/ API
 2. extract the temperature from the response
 3. calculate the average temperature'''
 
 generate_request_schema_prompt = '''{context_string}
 Generate the lean request json schema of the Microservice.
 Note: If you are not sure about the details, then come up with the minimal number of parameters possible.'''
 
 generate_output_schema_prompt = '''{context_string}
 Generate the lean response json schema for the Microservice.
-Note: If you are not sure about the details, then come up with the minimal number of parameters possible.'''
+Note: If you are not sure about the details, then come up with the minimal number of parameters possible.
+Note: If you can decide to return files as URLs or as base64 encoded strings, then choose the base64 encoded strings.'''
 
 summarize_description_and_schemas_prompt = '''{context_string}
 Write an updated microservice description by incorporating information about the request and response parameters in a concise way without losing any information.
 Note: You must not mention any details about algorithms or the technical implementation.
 Note: You must not mention that there is a request and response JSON schema
 Note: You must not use any formatting like triple backticks.
 Note: If an external API is mentioned in the description, then you must mention the API in the updated description as well.'''
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/extract_information.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/extract_information.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/get_user_input_if_needed.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/get_user_input_if_needed.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/translation.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/translation.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 import json
 import os
 import random
 import re
 import shutil
+import sys
 from typing import Callable
 from typing import List, Text, Optional
 
 from langchain import PromptTemplate
+from langchain.schema import SystemMessage, AIMessage
 from pydantic.dataclasses import dataclass
 
 from dev_gpt.apis import gpt
 from dev_gpt.apis.gpt import _GPTConversation
 from dev_gpt.apis.jina_cloud import process_error_message, push_executor, is_executor_in_hub
 from dev_gpt.apis.pypi import is_package_on_pypi, clean_requirements_txt
 from dev_gpt.constants import FILE_AND_TAG_PAIRS, NUM_IMPLEMENTATION_STRATEGIES, MAX_DEBUGGING_ITERATIONS, \
     BLACKLISTED_PACKAGES, EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_TAG, \
     REQUIREMENTS_FILE_NAME, REQUIREMENTS_FILE_TAG, DOCKER_FILE_NAME, IMPLEMENTATION_FILE_NAME, \
-    IMPLEMENTATION_FILE_TAG, LANGUAGE_PACKAGES, UNNECESSARY_PACKAGES, DOCKER_BASE_IMAGE_VERSION
+    IMPLEMENTATION_FILE_TAG, LANGUAGE_PACKAGES, UNNECESSARY_PACKAGES, DOCKER_BASE_IMAGE_VERSION, SEARCH_PACKAGES, \
+    INDICATOR_TO_IMPORT_STATEMENT
 from dev_gpt.options.generate.pm.pm import PM
 from dev_gpt.options.generate.templates_user import template_generate_microservice_name, \
     template_generate_possible_packages, \
-    template_solve_code_issue, \
+    template_implement_solution_code_issue, \
     template_solve_pip_dependency_issue, template_is_dependency_issue, template_generate_playground, \
-    template_generate_function, template_generate_test, template_generate_requirements, \
+    template_generate_function_constructor, template_generate_test, template_generate_requirements, \
     template_chain_of_thought, template_summarize_error, \
-    template_solve_apt_get_dependency_issue
+    template_solve_apt_get_dependency_issue, \
+    template_suggest_solutions_code_issue, template_was_error_seen_before, \
+    template_was_solution_tried_before, response_format_was_error_seen_before, \
+    response_format_was_solution_tried_before, response_format_suggest_solutions
 from dev_gpt.utils.io import persist_file, get_all_microservice_files_with_content, get_microservice_path
 from dev_gpt.utils.string_tools import print_colored
 
 
 @dataclass
 class TaskSpecification:
     task: Optional[Text]
     test: Optional[Text]
 
 
 class Generator:
-    def __init__(self, task_description, path, model='gpt-4'):
-        self.gpt_session = gpt.GPTSession(model=model)
+    def __init__(self, task_description, path, model='gpt-4', self_healing=True):
+        self.gpt_session = gpt.GPTSession(os.path.join(path, 'log.json'), model=model)
         self.microservice_specification = TaskSpecification(task=task_description, test=None)
+        self.self_healing = self_healing
         self.microservice_root_path = path
+        self.microservice_name = None
+        self.previous_microservice_path = None
+        self.cur_microservice_path = None
+        self.previous_errors = []
+        self.previous_solutions = []
 
     @staticmethod
     def extract_content_from_result(plain_text, file_name, match_single_block=False, can_contain_code_block=True):
         optional_line_break = '\n' if can_contain_code_block else ''  # the \n at the end makes sure that ``` within the generated code is not matched because it is not right before a line break
         pattern = fr"(?:\*|\*\*| ){file_name}\*?\*?\n```(?:\w+\n)?([\s\S]*?){optional_line_break}```"
         matches = re.findall(pattern, plain_text, re.MULTILINE)
         if matches:
@@ -84,144 +96,185 @@
 
         return _default_parse_result_fn
 
     def generate_and_persist_file(
             self,
             section_title: str,
             template: PromptTemplate,
-            destination_folder: str,
+            destination_folder: str = None,
             file_name_s: List[str] = None,
             parse_result_fn: Callable = None,
+            use_custom_system_message: bool = True,
+            response_format_example: str = None,
+            post_process_fn: Callable = None,
             **template_kwargs
     ):
         """This function generates file(s) using the given template and persists it/them in the given destination folder.
         It also returns the generated content as a dictionary mapping file_name to its content.
 
         Args:
             section_title (str): The title of the section to be printed in the console.
             template (PromptTemplate): The template to be used for generating the file(s).
-            destination_folder (str): The destination folder where the generated file(s) should be persisted.
+            destination_folder (str): The destination folder where the generated file(s) should be persisted. If None,
+                the current microservice path is used. Defaults to None.
             file_name_s (List[str], optional): The name of the file(s) to be generated. Defaults to None.
             parse_result_fn (Callable, optional): A function that parses the generated content and returns a dictionary
                 mapping file_name to its content. If no content could be extract, it returns an empty dictionary.
                 Defaults to None. If None, default parsing is used which uses the file_name to extract from the generated content.
+            use_custom_system_message (bool, optional): whether to use custom system message or not. Defaults to True.
             **template_kwargs: The keyword arguments to be passed to the template.
         """
+        if destination_folder is None:
+            destination_folder = self.cur_microservice_path
+
         if parse_result_fn is None:
             parse_result_fn = self.get_default_parse_result_fn(file_name_s)
 
         print_colored('', f'\n\n############# {section_title} #############', 'blue')
-        system_introduction_message = _GPTConversation._create_system_message(
-            self.microservice_specification.task,
-            self.microservice_specification.test
+        if use_custom_system_message:
+            system_introduction_message = _GPTConversation._create_system_message(
+                self.microservice_specification.task,
+                self.microservice_specification.test
+            )
+        else:
+            system_introduction_message = SystemMessage(content='You are a helpful assistant.')
+        conversation = self.gpt_session.get_conversation(
+            messages=[system_introduction_message] if use_custom_system_message else []
         )
-        conversation = self.gpt_session.get_conversation(messages=[system_introduction_message])
         template_kwargs = {k: v for k, v in template_kwargs.items() if k in template.input_variables}
         if 'file_name' in template.input_variables and len(file_name_s) == 1:
             template_kwargs['file_name'] = file_name_s[0]
         content_raw = conversation.chat(
             template.format(
                 **template_kwargs
             )
         )
         content = parse_result_fn(content_raw)
+        if post_process_fn is not None:
+            content = post_process_fn(content)
         if content == {}:
+            conversation = self.gpt_session.get_conversation(
+                messages=[SystemMessage(content='You are a helpful assistant.'), AIMessage(content=content_raw)]
+            )
+            if response_format_example is not None:
+                file_wrapping_example = response_format_example
+            elif len(file_name_s) == 1:
+                file_ending = file_name_s[0].split('.')[-1]
+                if file_ending == 'py':
+                    tag = 'python'
+                elif file_ending == 'json':
+                    tag = 'json'
+                else:
+                    tag = ''
+                file_wrapping_example = f'''**{file_name_s[0]}**
+```{tag}
+<content_of_file>
+```'''
+            else:
+                file_wrapping_example = '''**file_name.file_ending**
+```<json|py|...
+<content_of_file>
+```'''
             content_raw = conversation.chat(
-                'You must add the content in the format shown above' + (f' for {file_name_s[0]}' if len(file_name_s) == 1 else ''))
+                'Based on your previous response, only output the content' + (f' for `{file_name_s[0]}`' if len(file_name_s) == 1 else '') +
+                '. Like this:\n' +
+                file_wrapping_example
+            )
             content = parse_result_fn(content_raw)
         for _file_name, _file_content in content.items():
             persist_file(_file_content, os.path.join(destination_folder, _file_name))
         return content
 
     def generate_microservice(
             self,
-            microservice_name,
             packages,
             num_approach,
     ):
-        MICROSERVICE_FOLDER_v1 = get_microservice_path(self.microservice_root_path, microservice_name, packages,
-                                                       num_approach, 1)
-        os.makedirs(MICROSERVICE_FOLDER_v1)
+        self.cur_microservice_path = get_microservice_path(
+            self.microservice_root_path, self.microservice_name, packages, num_approach, 1
+        )
+        os.makedirs(self.cur_microservice_path)
 
         with open(os.path.join(os.path.dirname(__file__), 'static_files', 'microservice', 'jina_wrapper.py'), 'r', encoding='utf-8') as f:
             microservice_executor_boilerplate = f.read()
-        microservice_executor_code = microservice_executor_boilerplate.replace('class DevGPTExecutor(Executor):',
-                                                                               f'class {microservice_name}(Executor):')
-        persist_file(microservice_executor_code, os.path.join(MICROSERVICE_FOLDER_v1, EXECUTOR_FILE_NAME))
-
-        with open(os.path.join(os.path.dirname(__file__), 'static_files', 'microservice', 'apis.py'), 'r', encoding='utf-8') as f:
-            persist_file(f.read(), os.path.join(MICROSERVICE_FOLDER_v1, 'apis.py'))
+        microservice_executor_code = microservice_executor_boilerplate \
+            .replace('class DevGPTExecutor(Executor):', f'class {self.microservice_name}(Executor):')
+        persist_file(microservice_executor_code, os.path.join(self.cur_microservice_path, EXECUTOR_FILE_NAME))
+
+        for additional_file in ['google_custom_search.py', 'gpt_3_5_turbo.py']:
+            with open(os.path.join(os.path.dirname(__file__), 'static_files', 'microservice', additional_file), 'r', encoding='utf-8') as f:
+                persist_file(f.read(), os.path.join(self.cur_microservice_path, additional_file))
 
+        is_using_gpt_3_5_turbo = 'gpt_3_5_turbo' in packages or 'gpt-3-5-turbo' in packages
+        is_using_google_custom_search = 'google_custom_search' in packages or 'google-custom-search' in packages
         microservice_content = self.generate_and_persist_file(
             section_title='Microservice',
-            template=template_generate_function,
-            destination_folder=MICROSERVICE_FOLDER_v1,
+            template=template_generate_function_constructor(is_using_gpt_3_5_turbo, is_using_google_custom_search),
             microservice_description=self.microservice_specification.task,
             test_description=self.microservice_specification.test,
             packages=packages,
             file_name_purpose=IMPLEMENTATION_FILE_NAME,
             tag_name=IMPLEMENTATION_FILE_TAG,
             file_name_s=[IMPLEMENTATION_FILE_NAME],
+            post_process_fn=self.add_missing_imports_post_process_fn,
         )[IMPLEMENTATION_FILE_NAME]
 
         test_microservice_content = self.generate_and_persist_file(
             'Test Microservice',
             template_generate_test,
-            MICROSERVICE_FOLDER_v1,
             code_files_wrapped=self.files_to_string({EXECUTOR_FILE_NAME: microservice_content}),
-            microservice_name=microservice_name,
+            microservice_name=self.microservice_name,
             microservice_description=self.microservice_specification.task,
             test_description=self.microservice_specification.test,
             file_name_purpose=TEST_EXECUTOR_FILE_NAME,
             tag_name=TEST_EXECUTOR_FILE_TAG,
             file_name_s=[TEST_EXECUTOR_FILE_NAME],
+            post_process_fn=self.add_missing_imports_post_process_fn,
         )[TEST_EXECUTOR_FILE_NAME]
 
-        requirements_content = self.generate_and_persist_file(
+        self.generate_and_persist_file(
             'Requirements',
             template_generate_requirements,
-            MICROSERVICE_FOLDER_v1,
             code_files_wrapped=self.files_to_string({
                 IMPLEMENTATION_FILE_NAME: microservice_content,
                 TEST_EXECUTOR_FILE_NAME: test_microservice_content,
             }),
             file_name_purpose=REQUIREMENTS_FILE_NAME,
             file_name_s=[REQUIREMENTS_FILE_NAME],
             parse_result_fn=self.parse_result_fn_requirements,
             tag_name=REQUIREMENTS_FILE_TAG,
-        )[REQUIREMENTS_FILE_NAME]
-
-        # I deactivated this because 3.5-turbo was hallucinating packages that were not needed
-        # now, in the first iteration the default dockerfile is used
-        # self.generate_and_persist_file(
-        #     section_title='Generate Dockerfile',
-        #     template=template_generate_apt_get_install,
-        #     destination_folder=MICROSERVICE_FOLDER_v1,
-        #     file_name_s=None,
-        #     parse_result_fn=self.parse_result_fn_dockerfile,
-        #     docker_file_wrapped=self.read_docker_template(),
-        #     requirements_file_wrapped=self.files_to_string({
-        #         REQUIREMENTS_FILE_NAME: requirements_content,
-        #     })
-        # )
+        )
 
         with open(os.path.join(os.path.dirname(__file__), 'static_files', 'microservice', 'Dockerfile'), 'r',
                   encoding='utf-8') as f:
             docker_file_template_lines = f.readlines()
         docker_file_template_lines = [
             line.replace('{{APT_GET_PACKAGES}}', '').replace('{{DOCKER_BASE_IMAGE_VERSION}}', DOCKER_BASE_IMAGE_VERSION)
             for line in docker_file_template_lines
         ]
-        docker_file_content = '\n'.join(docker_file_template_lines)
-        persist_file(docker_file_content, os.path.join(MICROSERVICE_FOLDER_v1, 'Dockerfile'))
+        docker_file_content = ''.join(docker_file_template_lines)
+        persist_file(docker_file_content, os.path.join(self.cur_microservice_path, 'Dockerfile'))
 
-        self.write_config_yml(microservice_name, MICROSERVICE_FOLDER_v1)
+        self.write_config_yml(self.microservice_name, self.cur_microservice_path)
 
         print('\nFirst version of the microservice generated. Start iterating on it to make the tests pass...')
 
+
+    def add_missing_imports_post_process_fn(self, content_dict: dict):
+        for file_name, file_content in content_dict.items():
+            file_content = self.add_missing_imports_for_file(file_content)
+            content_dict[file_name] = file_content
+        return content_dict
+
+    def add_missing_imports_for_file(self, file_content):
+        for indicator, import_statement in INDICATOR_TO_IMPORT_STATEMENT.items():
+            if indicator in file_content and import_statement not in file_content:
+                file_content = f'{import_statement}\n{file_content}'
+        return file_content
+
     @staticmethod
     def read_docker_template():
         with open(os.path.join(os.path.dirname(__file__), 'static_files', 'microservice', 'Dockerfile'), 'r', encoding='utf-8') as f:
             return f.read()
 
     def parse_result_fn_dockerfile(self, content_raw: str):
         json_string = self.extract_content_from_result(content_raw, 'apt-get-packages.json', match_single_block=True)
@@ -240,23 +293,26 @@
         content_modified = f'''jina==3.15.1.dev14
 docarray==0.21.0
 openai==0.27.5
 pytest
 {os.linesep.join(lines)}'''
         return {REQUIREMENTS_FILE_NAME: content_modified}
 
-    def generate_playground(self, microservice_name, microservice_path):
+    def generate_playground(self):
         print_colored('', '\n\n############# Playground #############', 'blue')
 
-        file_name_to_content = get_all_microservice_files_with_content(microservice_path)
+        with open(os.path.join(os.path.dirname(__file__), 'static_files', 'gateway', 'app_template.py'), 'r', encoding='utf-8') as f:
+            playground_template = f.read()
+        file_name_to_content = get_all_microservice_files_with_content(self.cur_microservice_path)
         conversation = self.gpt_session.get_conversation()
         conversation.chat(
             template_generate_playground.format(
-                code_files_wrapped=self.files_to_string(file_name_to_content, ['test_microservice.py']),
-                microservice_name=microservice_name,
+                code_files_wrapped=self.files_to_string(file_name_to_content, ['test_microservice.py', 'microservice.py']),
+                microservice_name=self.microservice_name,
+                playground_template=playground_template,
             )
         )
         playground_content_raw = conversation.chat(
             template_chain_of_thought.format(
                 file_name_purpose='app.py/the playground',
                 file_name='app.py',
                 tag_name='python',
@@ -264,21 +320,22 @@
         )
         playground_content = self.extract_content_from_result(playground_content_raw, 'app.py', match_single_block=True)
         if playground_content == '':
             content_raw = conversation.chat(f'You must add the app.py code. You most not output any other code')
             playground_content = self.extract_content_from_result(
                 content_raw, 'app.py', match_single_block=True
             )
+        playground_content = self.add_missing_imports_for_file(playground_content)
 
-        gateway_path = os.path.join(microservice_path, 'gateway')
+        gateway_path = os.path.join(self.cur_microservice_path, 'gateway')
         shutil.copytree(os.path.join(os.path.dirname(__file__), 'static_files', 'gateway'), gateway_path)
         persist_file(playground_content, os.path.join(gateway_path, 'app.py'))
 
         # fill-in name of microservice
-        gateway_name = f'Gateway{microservice_name}'
+        gateway_name = f'Gateway{self.microservice_name}'
         custom_gateway_path = os.path.join(gateway_path, 'custom_gateway.py')
         with open(custom_gateway_path, 'r', encoding='utf-8') as f:
             custom_gateway_content = f.read()
         custom_gateway_content = custom_gateway_content.replace(
             'class CustomGateway(CompositeGateway):',
             f'class {gateway_name}(CompositeGateway):'
         )
@@ -288,91 +345,153 @@
         # write config.yml
         self.write_config_yml(gateway_name, gateway_path, 'custom_gateway.py')
 
         # push the gateway
         print('Final step...')
         hubble_log = push_executor(gateway_path)
         if not is_executor_in_hub(gateway_name):
-            raise Exception(f'{microservice_name} not in hub. Hubble logs: {hubble_log}')
+            raise Exception(f'{self.microservice_name} not in hub. Hubble logs: {hubble_log}')
 
-    def debug_microservice(self, microservice_name, num_approach, packages):
+    def debug_microservice(self, num_approach, packages, self_healing):
         for i in range(1, MAX_DEBUGGING_ITERATIONS):
             print('Debugging iteration', i)
             print('Trying to debug the microservice. Might take a while...')
-            previous_microservice_path = get_microservice_path(self.microservice_root_path, microservice_name, packages,
-                                                               num_approach, i)
-            next_microservice_path = get_microservice_path(self.microservice_root_path, microservice_name, packages,
-                                                           num_approach, i + 1)
-            clean_requirements_txt(previous_microservice_path)
-            log_hubble = push_executor(previous_microservice_path)
+            clean_requirements_txt(self.cur_microservice_path)
+            log_hubble = push_executor(self.cur_microservice_path)
             error = process_error_message(log_hubble)
             if error:
+                if not self_healing:
+                    print(error)
+                    raise Exception('Self-healing is disabled. Please fix the error manually.')
                 print('An error occurred during the build process. Feeding the error back to the assistant...')
-                self.do_debug_iteration(error, next_microservice_path, previous_microservice_path)
+                self.previous_microservice_path = self.cur_microservice_path
+                self.cur_microservice_path = get_microservice_path(
+                    self.microservice_root_path, self.microservice_name, packages, num_approach, i + 1
+                )
+                os.makedirs(self.cur_microservice_path)
+                self.do_debug_iteration(error)
                 if i == MAX_DEBUGGING_ITERATIONS - 1:
                     raise self.MaxDebugTimeReachedException('Could not debug the microservice.')
             else:
                 # at the moment, there can be cases where no error log is extracted but the executor is still not published
                 # it leads to problems later on when someone tries a run or deployment
-                if is_executor_in_hub(microservice_name):
+                if is_executor_in_hub(self.microservice_name):
                     print('Successfully build microservice.')
                     break
                 else:
-                    raise Exception(f'{microservice_name} not in hub. Hubble logs: {log_hubble}')
+                    raise Exception(f'{self.microservice_name} not in hub. Hubble logs: {log_hubble}')
 
-        return get_microservice_path(self.microservice_root_path, microservice_name, packages, num_approach, i)
-
-    def do_debug_iteration(self, error, next_microservice_path, previous_microservice_path):
-        os.makedirs(next_microservice_path)
-        file_name_to_content = get_all_microservice_files_with_content(previous_microservice_path)
+    def do_debug_iteration(self, error):
+        file_name_to_content = get_all_microservice_files_with_content(self.previous_microservice_path)
         for file_name, content in file_name_to_content.items():
-            persist_file(content, os.path.join(next_microservice_path, file_name))
+            persist_file(content, os.path.join(self.cur_microservice_path, file_name))
 
         summarized_error = self.summarize_error(error)
         dock_req_string = self.files_to_string({
             key: val for key, val in file_name_to_content.items() if
             key in ['requirements.txt', 'Dockerfile']
         })
 
         is_apt_get_dependency_issue = self.is_dependency_issue(summarized_error, dock_req_string, 'apt-get')
         if is_apt_get_dependency_issue:
             self.generate_and_persist_file(
                 section_title='Debugging apt-get dependency issue',
                 template=template_solve_apt_get_dependency_issue,
-                destination_folder=next_microservice_path,
                 file_name_s=['apt-get-packages.json'],
                 parse_result_fn=self.parse_result_fn_dockerfile,
                 summarized_error=summarized_error,
                 all_files_string=dock_req_string,
             )
             print('Dockerfile updated')
         else:
             is_pip_dependency_issue = self.is_dependency_issue(summarized_error, dock_req_string, 'PIP')
             if is_pip_dependency_issue:
                 self.generate_and_persist_file(
                     section_title='Debugging pip dependency issue',
                     template=template_solve_pip_dependency_issue,
-                    destination_folder=next_microservice_path,
                     file_name_s=[REQUIREMENTS_FILE_NAME],
                     summarized_error=summarized_error,
                     all_files_string=dock_req_string,
                 )
             else:
+                all_files_string = self.files_to_string(
+                    {key: val for key, val in file_name_to_content.items() if key != EXECUTOR_FILE_NAME}
+                )
+
+                suggested_solution = self.generate_solution_suggestion(summarized_error, all_files_string)
+
                 self.generate_and_persist_file(
-                    section_title='Debugging code issue',
-                    template=template_solve_code_issue,
-                    destination_folder=next_microservice_path,
+                    section_title='Implementing suggestion solution for code issue',
+                    template=template_implement_solution_code_issue,
                     file_name_s=[IMPLEMENTATION_FILE_NAME, TEST_EXECUTOR_FILE_NAME, REQUIREMENTS_FILE_NAME],
                     summarized_error=summarized_error,
                     task_description=self.microservice_specification.task,
                     test_description=self.microservice_specification.test,
-                    all_files_string=self.files_to_string(
-                        {key: val for key, val in file_name_to_content.items() if key != EXECUTOR_FILE_NAME}),
+                    all_files_string=all_files_string,
+                    suggested_solution=suggested_solution,
                 )
 
+                self.previous_errors.append(summarized_error)
+                self.previous_solutions.append(suggested_solution)
+
+    def generate_solution_suggestion(self, summarized_error, all_files_string):
+        suggested_solutions = json.loads(
+            self.generate_and_persist_file(
+                section_title='Suggest solution for code issue',
+                template=template_suggest_solutions_code_issue,
+                file_name_s=['solutions.json'],
+                summarized_error=summarized_error,
+                task_description=self.microservice_specification.task,
+                test_description=self.microservice_specification.test,
+                all_files_string=all_files_string,
+                response_format_example=response_format_suggest_solutions,
+            )['solutions.json']
+        )
+
+        if len(self.previous_errors) > 0:
+            was_error_seen_before = json.loads(
+                self.generate_and_persist_file(
+                    section_title='Check if error was seen before',
+                    template=template_was_error_seen_before,
+                    file_name_s=['was_error_seen_before.json'],
+                    summarized_error=summarized_error,
+                    previous_errors='- "' + f'"{os.linesep}- "'.join(self.previous_errors) + '"',
+                    use_custom_system_message=False,
+                    response_format_example=response_format_was_error_seen_before,
+                )['was_error_seen_before.json']
+            )['was_error_seen_before'].lower() == 'yes'
+
+            suggested_solution = None
+            if was_error_seen_before:
+                for _num_solution in range(1, len(suggested_solutions) + 1):
+                    _suggested_solution = suggested_solutions[str(_num_solution)]
+                    was_solution_tried_before = json.loads(
+                        self.generate_and_persist_file(
+                            section_title='Check if solution was tried before',
+                            template=template_was_solution_tried_before,
+                            file_name_s=['will_lead_to_different_actions.json'],
+                            tried_solutions='- "' + f'"{os.linesep}- "'.join(self.previous_solutions) + '"',
+                            suggested_solution=_suggested_solution,
+                            use_custom_system_message=False,
+                            response_format_example=response_format_was_solution_tried_before,
+                        )['will_lead_to_different_actions.json']
+                    )['will_lead_to_different_actions'].lower() == 'no'
+                    if not was_solution_tried_before:
+                        suggested_solution = _suggested_solution
+                        break
+            else:
+                suggested_solution = suggested_solutions['1']
+
+            if suggested_solution is None:
+                suggested_solution = f"solve error: {summarized_error}"
+        else:
+            suggested_solution = suggested_solutions['1']
+
+        return suggested_solution
+
     class MaxDebugTimeReachedException(BaseException):
         pass
 
     def is_dependency_issue(self, summarized_error, dock_req_string: str, package_manager: str):
         # a few heuristics to quickly jump ahead
         if any([error_message in summarized_error for error_message in
                 ['AttributeError', 'NameError', 'AssertionError']]):
@@ -408,60 +527,63 @@
             section_title='Generate possible packages',
             template=template_generate_possible_packages,
             destination_folder=self.microservice_root_path,
             file_name_s=['strategies.json'],
             description=self.microservice_specification.task
         )['strategies.json']
         packages_list = [[pkg.strip().lower() for pkg in packages] for packages in json.loads(packages_json_string)]
-        packages_list = [[self.replace_with_gpt_3_5_turbo_if_possible(pkg) for pkg in packages] for packages in
+        packages_list = [[self.replace_with_tool_if_possible(pkg) for pkg in packages] for packages in
                          packages_list]
 
         packages_list = self.filter_packages_list(packages_list)
         packages_list = self.remove_duplicates_from_packages_list(packages_list)
         packages_list = packages_list[:NUM_IMPLEMENTATION_STRATEGIES]
         return packages_list
     # '/private/var/folders/f5/whmffl4d7q79s29jpyb6719m0000gn/T/pytest-of-florianhonicke/pytest-128/test_generation_level_0_mock_i0'
     # '/private/var/folders/f5/whmffl4d7q79s29jpyb6719m0000gn/T/pytest-of-florianhonicke/pytest-129/test_generation_level_0_mock_i0'
     def generate(self):
-        self.microservice_specification.task, self.microservice_specification.test = PM().refine_specification(self.microservice_specification.task)
         os.makedirs(self.microservice_root_path)
+        self.microservice_specification.task, self.microservice_specification.test = PM().refine_specification(self.microservice_specification.task)
         generated_name = self.generate_microservice_name(self.microservice_specification.task)
-        microservice_name = f'{generated_name}{random.randint(0, 10_000_000)}'
+        self.microservice_name = f'{generated_name}{random.randint(0, 10_000_000)}'
         packages_list = self.get_possible_packages()
         for num_approach, packages in enumerate(packages_list):
             try:
-                self.generate_microservice(microservice_name, packages, num_approach)
-                final_version_path = self.debug_microservice(microservice_name, num_approach, packages)
-                self.generate_playground(microservice_name, final_version_path)
+                self.generate_microservice(packages, num_approach)
+                self.debug_microservice(num_approach, packages, self.self_healing)
+                self.generate_playground()
             except self.MaxDebugTimeReachedException:
                 print('Could not debug the Microservice with the approach:', packages)
                 if num_approach == len(packages_list) - 1:
                     print_colored('',
                                   f'Could not debug the Microservice with any of the approaches: {packages} giving up.',
                                   'red')
                     return -1
                 continue
+            command = 'dev-gpt' if sys.argv[0] == 'dev-gpt' else 'python main.py'
             print(f'''
 You can now run or deploy your microservice:
-dev-gpt run --path {self.microservice_root_path}
-dev-gpt deploy --path {self.microservice_root_path}
+{command} run --path {self.microservice_root_path}
+{command} deploy --path {self.microservice_root_path}
 '''
                   )
             return 0
 
     def summarize_error(self, error):
         conversation = self.gpt_session.get_conversation()
         error_summary = conversation.chat(template_summarize_error.format(error=error))
         return error_summary
 
 
     @staticmethod
-    def replace_with_gpt_3_5_turbo_if_possible(pkg):
+    def replace_with_tool_if_possible(pkg):
         if pkg in LANGUAGE_PACKAGES:
             return 'gpt_3_5_turbo'
+        if pkg in SEARCH_PACKAGES:
+            return 'google_custom_search'
         return pkg
 
     @staticmethod
     def filter_packages_list(packages_list):
         # filter out complete package lists
         packages_list = [
             packages for packages in packages_list if all([
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/pm/pm.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/pm/pm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from dev_gpt.apis import gpt
 from dev_gpt.apis.gpt import ask_gpt
 from dev_gpt.options.generate.chains.auto_refine_description import auto_refine_description
 from dev_gpt.options.generate.chains.question_answering import is_question_true
 from dev_gpt.options.generate.chains.translation import translation
 from dev_gpt.options.generate.chains.user_confirmation_feedback_loop import user_feedback_loop
 from dev_gpt.options.generate.chains.get_user_input_if_needed import get_user_input_if_needed
-from dev_gpt.options.generate.parser import identity_parser
+from dev_gpt.options.generate.parser import identity_parser, json_parser
+from dev_gpt.options.generate.pm.task_tree_schema import TaskTree
 from dev_gpt.options.generate.prompt_factory import make_prompt_friendly
 from dev_gpt.options.generate.ui import get_random_employee
 
 
 class PM:
     def refine_specification(self, microservice_description):
         pm = get_random_employee('pm')
@@ -31,17 +32,17 @@
         print()
         while not val:
             val = input('you: ')
         return val
 
     def refine(self, microservice_description):
         microservice_description, test_description = self.refine_description(microservice_description)
-        return microservice_description, test_description
-        # sub_task_tree = self.construct_sub_task_tree(microservice_description)
+        # sub_task_tree = construct_sub_task_tree(microservice_description)
         # return sub_task_tree
+        return microservice_description, test_description
 
     def refine_description(self, microservice_description):
         context = {'microservice_description': microservice_description}
         auto_refine_description(context)
         microservice_description = user_feedback_loop(context, context['microservice_description'])
 
         test_description = ask_gpt(
@@ -56,15 +57,16 @@
             condition_question='Does the request schema provided include a property that represents a file?',
             question_gen='Generate a question that requests for an example file url.',
             extension_name='Input Example',
         )
         microservice_description += self.user_input_extension_if_needed(
             context,
             microservice_description,
-            condition_question='Does the microservice send requests to an API?',
+            condition_question='''\
+Does the microservice send requests to an API beside the Google Custom Search API and gpt-3.5-turbo?''',
             question_gen='Generate a question that asks for the endpoint of the external API and an example of a request and response when interacting with the external API.',
             extension_name='Example of API usage',
             post_transformation_fn=translation(from_format='api instruction', to_format='python code snippet raw without formatting')
         )
         return microservice_description, test_description
 
     def user_input_extension_if_needed(
@@ -123,52 +125,52 @@
 # def get_nlp_fns(self, microservice_description):
 #     return ask_gpt(
 #         get_nlp_fns_prompt,
 #         json_parser,
 #         microservice_description=microservice_description
 #     )
 #
-# def construct_sub_task_tree(self, microservice_description):
-#     """
-#     takes a microservice description and recursively constructs a tree of sub-tasks that need to be done to implement the microservice
-#     """
-#     #
-#     # nlp_fns = self.get_nlp_fns(
-#     #     microservice_description
-#     # )
-#
-#     sub_task_tree_dict = ask_gpt(
-#         construct_sub_task_tree_prompt, json_parser,
-#         microservice_description=microservice_description,
-#         # nlp_fns=nlp_fns
-#     )
-#     reflections = ask_gpt(
-#         sub_task_tree_reflections_prompt, identity_parser,
-#         microservice_description=microservice_description,
-#         # nlp_fns=nlp_fns,
-#         sub_task_tree=sub_task_tree_dict,
-#     )
-#     solutions = ask_gpt(
-#         sub_task_tree_solutions_prompt, identity_parser,
-#         # nlp_fns=nlp_fns,
-#         microservice_description=microservice_description, sub_task_tree=sub_task_tree_dict,
-#         reflections=reflections,
-#     )
-#     sub_task_tree_updated = ask_gpt(
-#         sub_task_tree_update_prompt,
-#         json_parser,
-#         microservice_description=microservice_description,
-#         # nlp_fns=nlp_fns,
-#         sub_task_tree=sub_task_tree_dict, solutions=solutions
-#     )
-#     # for task_dict in self.iterate_over_sub_tasks(sub_task_tree_updated):
-#     #     task_dict.update(self.get_additional_task_info(task_dict['task']))
-#
-#     sub_task_tree = TaskTree.parse_obj(sub_task_tree_updated)
-#     return sub_task_tree
+def construct_sub_task_tree(self, microservice_description):
+    """
+    takes a microservice description and recursively constructs a tree of sub-tasks that need to be done to implement the microservice
+    """
+    #
+    # nlp_fns = self.get_nlp_fns(
+    #     microservice_description
+    # )
+
+    sub_task_tree_dict = ask_gpt(
+        construct_sub_task_tree_prompt, json_parser,
+        microservice_description=microservice_description,
+        # nlp_fns=nlp_fns
+    )
+    reflections = ask_gpt(
+        sub_task_tree_reflections_prompt, identity_parser,
+        microservice_description=microservice_description,
+        # nlp_fns=nlp_fns,
+        sub_task_tree=sub_task_tree_dict,
+    )
+    solutions = ask_gpt(
+        sub_task_tree_solutions_prompt, identity_parser,
+        # nlp_fns=nlp_fns,
+        microservice_description=microservice_description, sub_task_tree=sub_task_tree_dict,
+        reflections=reflections,
+    )
+    sub_task_tree_updated = ask_gpt(
+        sub_task_tree_update_prompt,
+        json_parser,
+        microservice_description=microservice_description,
+        # nlp_fns=nlp_fns,
+        sub_task_tree=sub_task_tree_dict, solutions=solutions
+    )
+    # for task_dict in self.iterate_over_sub_tasks(sub_task_tree_updated):
+    #     task_dict.update(self.get_additional_task_info(task_dict['task']))
+
+    sub_task_tree = TaskTree.parse_obj(sub_task_tree_updated)
+    return sub_task_tree
 
 # def get_additional_task_info(self, sub_task_description):
 #     additional_info_dict = self.get_additional_infos(
 #         description=sub_task_description,
 #         parameter={
 #             'display_name': 'Task description',
 #             'text': sub_task_description,
@@ -276,79 +278,79 @@
 # Make the description more concise without losing any information.
 # Note: You must not mention any details about algorithms or the technical implementation.
 # Note: You must ignore facts that are not specified.
 # Note: You must ignore facts that are not relevant.
 # Note: You must ignore facts that are unknown.
 # Note: You must ignore facts that are unclear.'''
 
-# construct_sub_task_tree_prompt = client_description + '''
-# Recursively constructs a tree of functions that need to be implemented for the endpoint_function that retrieves a json string and returns a json string.
-# Example:
-# Input: "Input: list of integers, Output: Audio file of short story where each number is mentioned exactly once."
-# Output:
-# {{
-#     "description": "Create an audio file containing a short story in which each integer from the provided list is seamlessly incorporated, ensuring that every integer is mentioned exactly once.",
-#     "python_fn_signature": "def generate_integer_story_audio(numbers: List[int]) -> str:",
-#     "sub_fns": [
-#         {{
-#             "description": "Generate sentence from integer.",
-#             "python_fn_signature": "def generate_sentence_from_integer(number: int) -> int:",
-#             "sub_fns": []
-#         }},
-#         {{
-#             "description": "Convert the story into an audio file.",
-#             "python_fn_signature": "def convert_story_to_audio(story: str) -> bytes:",
-#             "sub_fns": []
-#         }}
-#     ]
-# }}
-#
-# Note: you must only output the json string - nothing else.
-# Note: you must pretty print the json string.'''
+construct_sub_task_tree_prompt = client_description + '''
+Recursively constructs a tree of functions that need to be implemented for the endpoint_function that retrieves a json string and returns a json string.
+Example:
+Input: "Input: list of integers, Output: Audio file of short story where each number is mentioned exactly once."
+Output:
+{{
+    "description": "Create an audio file containing a short story in which each integer from the provided list is seamlessly incorporated, ensuring that every integer is mentioned exactly once.",
+    "python_fn_signature": "def generate_integer_story_audio(numbers: List[int]) -> str:",
+    "sub_fns": [
+        {{
+            "description": "Generate sentence from integer.",
+            "python_fn_signature": "def generate_sentence_from_integer(number: int) -> int:",
+            "sub_fns": []
+        }},
+        {{
+            "description": "Convert the story into an audio file.",
+            "python_fn_signature": "def convert_story_to_audio(story: str) -> bytes:",
+            "sub_fns": []
+        }}
+    ]
+}}
 
-# sub_task_tree_reflections_prompt = client_description + '''
-# Sub task tree:
-# ```
-# {sub_task_tree}
-# ```
-# Write down 3 arguments why the sub task tree might not perfectly represents the information mentioned in the microservice description. (5 words per argument)'''
-#
-# sub_task_tree_solutions_prompt = client_description + '''
-# Sub task tree:
-# ```
-# {sub_task_tree}
-# ```
-# Reflections:
-# ```
-# {reflections}
-# ```
-# For each constructive criticism, write a solution (5 words) that address the criticism.'''
-#
-# sub_task_tree_update_prompt = client_description + '''
-# Sub task tree:
-# ```
-# {sub_task_tree}
-# ```
-# Solutions:
-# ```
-# {solutions}
-# ```
-# Update the sub task tree by applying the solutions. (pretty print the json string)'''
-#
-# ask_questions_prompt = client_description + '''
-# Request json schema:
-# ```
-# {request_schema}
-# ```
-# Response json schema:
-# ```
-# {response_schema}
-# ```
-# Ask the user up to 5 unique detailed questions (5 words) about the microservice description that are not yet answered.
-# '''
+Note: you must only output the json string - nothing else.
+Note: you must pretty print the json string.'''
+
+sub_task_tree_reflections_prompt = client_description + '''
+Sub task tree:
+```
+{sub_task_tree}
+```
+Write down 3 arguments why the sub task tree might not perfectly represents the information mentioned in the microservice description. (5 words per argument)'''
+
+sub_task_tree_solutions_prompt = client_description + '''
+Sub task tree:
+```
+{sub_task_tree}
+```
+Reflections:
+```
+{reflections}
+```
+For each constructive criticism, write a solution (5 words) that address the criticism.'''
+
+sub_task_tree_update_prompt = client_description + '''
+Sub task tree:
+```
+{sub_task_tree}
+```
+Solutions:
+```
+{solutions}
+```
+Update the sub task tree by applying the solutions. (pretty print the json string)'''
+
+ask_questions_prompt = client_description + '''
+Request json schema:
+```
+{request_schema}
+```
+Response json schema:
+```
+{response_schema}
+```
+Ask the user up to 5 unique detailed questions (5 words) about the microservice description that are not yet answered.
+'''
 
 # answer_questions_prompt = client_description + '''
 # Request json schema:
 # ```
 # {request_schema}
 # ```
 # Response json schema:
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/pm/task_tree_schema.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/pm/task_tree_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# from typing import Dict, List, Union, Optional
-# from pydantic import BaseModel, Field
-#
-# class JSONSchema(BaseModel):
-#     type: str
-#     format: Union[str, None] = None
-#     items: Union['JSONSchema', None] = None
-#     properties: Dict[str, 'JSONSchema'] = Field(default_factory=dict)
-#     additionalProperties: Union[bool, 'JSONSchema'] = True
-#     required: List[str] = Field(default_factory=list)
-#
-#     class Config:
-#         arbitrary_types_allowed = True
-#
-# class TaskTree(BaseModel):
-#     description: Optional[str]
-#     python_fn_signature: str
-#     sub_fns: List['TaskTree']
-#
-# JSONSchema.update_forward_refs()
-# TaskTree.update_forward_refs()
+from typing import Dict, List, Union, Optional
+from pydantic import BaseModel, Field
+
+class JSONSchema(BaseModel):
+    type: str
+    format: Union[str, None] = None
+    items: Union['JSONSchema', None] = None
+    properties: Dict[str, 'JSONSchema'] = Field(default_factory=dict)
+    additionalProperties: Union[bool, 'JSONSchema'] = True
+    required: List[str] = Field(default_factory=list)
+
+    class Config:
+        arbitrary_types_allowed = True
+
+class TaskTree(BaseModel):
+    description: Optional[str]
+    python_fn_signature: str
+    sub_fns: List['TaskTree']
+
+JSONSchema.update_forward_refs()
+TaskTree.update_forward_refs()
 #
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import openai
 
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
 
 class GPT_3_5_Turbo:
-    def __init__(self, system: str = ''):
-        self.system = system
+    def __init__(self, system_string: str = ''):
+        self.system = system_string
 
-    def __call__(self, prompt: str) -> str:
+    def __call__(self, prompt_string: str) -> str:
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=[{
                 "role": 'system',
                 "content": self.system
             }, {
                 "role": 'user',
-                "content": prompt
+                "content": prompt_string
             }]
         )
         return response.choices[0]['message']['content']
+
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/templates_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 Note that the Dockerfile runs the test_microservice.py during the build process.
 The Dockerfile must not attach a virtual display when running test_microservice.py.'''
 
 
 not_allowed_function_string = '''The implemented function and the test must not use the GPU.
 The implemented function and the test must not access a database.
 The implemented function and the test must not access a display.
-The implemented function and the test must not access external apis except unless it is explicitly mentioned in the description or test case (e.g. by mentioning the api that should be used or by providing a URL to access the data). 
-The implemented function and the test must not load data from the local file system unless it was created by the implemented function itself.
+The implemented function and the test must not access external apis unless it is explicitly mentioned.
+The implemented function and the test must not be based on a large collection of hard-coded strings.
+The implemented function and the test must not open files from the local file system unless it was created by the implemented function itself.
 The implemented function and the test must not use a pre-trained model unless it is explicitly mentioned in the description.
 The implemented function and the test must not train a model.
 The implemented function and the test must not contain prototype or placeholder implementations.
 The implemented function and the test must run in a docker container based on debian.
 The implemented function and the test must not use libraries like Flask.
 The implemented function and the test must not have a __main__ function.
 The implemented function and the test must use gpt_3_5_turbo if the task requires the processing of language (e.g., understanding, generation, summarization, transformation, translation, modification or classification). Other language models are not allowed.
@@ -33,18 +34,23 @@
 "{description}"
 The executor name must fulfill the following criteria:
 - camel case
 - start with a capital letter
 - only consists of lower and upper case characters
 - end with Executor.
 
-The output is a the raw string wrapped into ``` and starting with **name.txt** like this:
+Your response must exactly match the following block code format (double asterisks for the file name and triple backticks for the file block):
 **name.txt**
 ```
-PDFParserExecutor
+<name here>
+```
+Example for: "Get a png as input and return a vectorized version as svg.":
+**name.txt**
+```
+PngToSvgExecutor
 ```'''
 )
 
 # todo split into multiple calls. One for brainstorming - one for the final answer
 template_generate_possible_packages = PromptTemplate.from_template(
     '''Here is the task description of the problem you need to solve:
 "{description}"
@@ -58,15 +64,15 @@
 d) can solve the task when running in a docker container
 e) the implementation of the core problem using the package would obey the following rules:
 ''' + not_allowed_function_string + '''
 
 When answering, just write "yes" or "no".
 
 4. For each approach, list the required python package combinations as discibed in the following.
-You must output the package combinations as json wrapped into tripple backticks ``` and name it **strategies.json**. \
+You must output the package combinations as json wrapped into triple backticks ``` and name it **strategies.json**. \
 Note that you can also leave a list empty to indicate that one of the strategies does not require any package and can be done in plain python.
 Write the output using double asterisks and triple backticks like this:
 **strategies.json**
 ```
 [
   ["package1", "package2", "package3"],
   ["package4", "package5"],
@@ -74,78 +80,102 @@
   [],
   ["package10"]
 ]
 ```''')
 
 
 template_code_wrapping_string = '''The code will go into {file_name_purpose}.
-Note that you must obey the double asterisk and tripple backtick syntax from like this:
+Note that you must obey the double asterisk and triple backtick syntax from like this:
 **{file_name}**
 ```{tag_name}
 ...code...
 ```
-You must provide the complete file with the exact same syntax to wrap the code.'''
+You must provide the complete {file_name} wrapped with the exact syntax shown above.'''
 
 
-gpt_35_turbo_usage_string = """If need to use gpt_3_5_turbo, then this is an example on how to use it:
+gpt_35_turbo_usage_string = """If you need to use gpt_3_5_turbo, then use it like shown in the following example:
 ```
-from .apis import GPT_3_5_Turbo
+from .gpt_3_5_turbo import GPT_3_5_Turbo
 
 gpt_3_5_turbo = GPT_3_5_Turbo(
-    system=\'\'\'
+    system_string=\'\'\'
 You are a tv-reporter who is specialized in C-list celebrities.
-When you get asked something like 'Who was having a date with <X>?', then you answer with a json like '{{"dates": ["<Y>", "<Z>"]}}'. 
+When you get asked something like 'Who was having a date with <X>?', then you answer with a string like "<y>, <z> were having a date with <x>"'. 
 You must not answer something else - only the json.
 \'\'\')
 
-generated_string = gpt(prompt)  # fill-in the prompt (str); the output is a string
+generated_string = gpt_3_5_turbo(prompt_string="example user prompt") # prompt_string is the only parameter
 ```
 """
 
+google_custom_search_usage_string = """If you need to use google_custom_search, then use it like shown in the following example:
+a) when searching for text:
+```
+from .google_custom_search import search_web
 
-template_generate_function = PromptTemplate.from_template(
-    general_guidelines_string + '''
+# input: search term (str), top_n (int)
+# output: list of strings
+string_list = search_web('<search term>', top_n=10)
+```
+b) when searching for images:
+```
+from .google_custom_search import search_images
+
+# input: search term (str), top_n (int)
+# output: list of image urls
+image_url_list = search_images('<search term>', top_n=10)
+```
+"""
+
+linebreak = '\n'
+def template_generate_function_constructor(is_using_gpt_3_5_turbo, is_using_google_custom_search):
+    return PromptTemplate.from_template(
+    general_guidelines_string + f'''
 
 Write a python function which receives as \
-input json string (that can be parsed with the python function json.loads) and \
-outputs a json string (that can be parsed with the python function json.loads). \
-The function is called 'func'.
-The function must fulfill the following description: '{microservice_description}'.
-It will be tested with the following scenario: '{test_description}'.
-For the implementation use the following package(s): '{packages}'.
+input json dictionary string (that can be parsed with the python function json.loads) and \
+outputs a json dictionary string (that can be parsed with the python function json.loads). \
+The function is called 'func' and has the following signature:
+def func(input_json_dict_string: str) -> str:
+The function must fulfill the following description: '{{microservice_description}}'.
+It will be tested with the following scenario: '{{test_description}}'.
+For the implementation use the following package(s): '{{packages}}'.
 
 The code must start with the following imports:
-```
-from .apis import GPT_3_5_Turbo
+```{linebreak +'from .gpt_3_5_turbo import GPT_3_5_Turbo' if is_using_gpt_3_5_turbo else ""}{linebreak + 'from .google_custom_search import search_web, search_images' if is_using_google_custom_search else ""}
 import json
+import requests
 ```
 Obey the following rules:
-''' + not_allowed_function_string + '''
+{not_allowed_function_string}
 
 Your approach:
 1. Identify the core challenge when implementing the function.
 2. Think about solutions for these challenges.
 3. Decide for one of the solutions.
 4. Write the code for the function. Don't write code for the test.
-''' + gpt_35_turbo_usage_string + '\n' + template_code_wrapping_string
-)
+{gpt_35_turbo_usage_string if is_using_gpt_3_5_turbo else ''}
+{google_custom_search_usage_string if is_using_google_custom_search else ''}
+{template_code_wrapping_string}'''
+    )
 
 
 template_generate_test = PromptTemplate.from_template(
     general_guidelines_string + '''
 
 {code_files_wrapped}
 
 Write a single pytest case that tests the following scenario: '{test_description}'. In case the test scenario is not precise enough, test a general case without any assumptions.
 Start the test with an extensive comment about the test case. If gpt_3_5_turbo is used in the executor, then the test must not check the exact output of the executor as it is not deterministic. 
 
 The test must start with the following imports:
 ```
 from .microservice import func
 import json
+import requests
 ```
 ''' + not_allowed_function_string + '''
 The test must not open local files.
 The test must not mock a function of the executor.
 The test must not use other data than the one provided in the test scenario.
 The test must not set any environment variables which require a key.
 ''' + '\n' + template_code_wrapping_string
@@ -202,18 +232,19 @@
 {{"packages": []}}
 ```
 '''
 )
 
 
 template_summarize_error = PromptTemplate.from_template(
-    '''Here is an error message I encountered during the docker build process:
+    '''Your task is to condense an error encountered during the docker build process. The error message is as follows:
 "{error}"
 Your task is to summarize the error message as compact and informative as possible \
 while maintaining all information necessary to debug the core issue (100 words).
+It should also provide some additional context regarding the specific file and line number where the error occurred. \
 Note that you must not suggest a solution to the error.
 Warnings are not worth mentioning.'''
 )
 
 
 template_is_dependency_issue = PromptTemplate.from_template(
     '''Your task is to assist in identifying the root cause of a Docker build error for a python application.
@@ -230,15 +261,15 @@
 2. Write down one bullet point on why it is unlikely that the error happens because a PACKAGE_MANAGER package is missing or failed to install.
 3. Write down your final answer.
 4. Write down your final answer as json in the following format:
 **response.json**
 ```json
 {{"dependency_installation_failure": "<yes/no>"}}
 ```
-Note that you must obey the double asterisk and tripple backtick syntax from above.
+Note that you must obey the double asterisk and triple backtick syntax from above.
 '''
 )
 
 
 template_solve_pip_dependency_issue = PromptTemplate.from_template(
     '''Your task is to provide guidance on how to solve an error that occurred during the Docker build process. 
 Here is the summary of the error that occurred:
@@ -290,22 +321,31 @@
 Example:
 Error is about missing package `libgl1-mesa-glx`.
 The output is:
 **apt-get-packages.json**
 ```json
 {{"packages": [libgl1-mesa-glx]}}
 ```
-Note that you must not output the content of any other files like the Dockerfile or requirements.txt. 
-Only output the apt-get-packages.json file.
-Note that the first line you output must be: **apt-get-packages.json**
+Only output content of the apt-get-packages.json file. Ensure the response can be parsed by Python json.loads
+Note: you must not output the content of any other. Especially don't output the Dockerfile or requirements.txt. 
+Note: the first line you output must be: **apt-get-packages.json**
 '''
 )
 
 
-template_solve_code_issue = PromptTemplate.from_template(
+response_format_suggest_solutions = '''**solutions.json**
+```json
+{{
+    "1": "<best solution>",
+    "2": "<2nd best solution>"
+}}
+```'''
+
+
+template_suggest_solutions_code_issue = PromptTemplate.from_template(
     '''General rules:
 ''' + not_allowed_function_string + '''
 
 Here is the description of the task the function must solve:
 {task_description}
 
 Here is the test scenario the function must pass:
@@ -313,92 +353,130 @@
 Here are all the files I use:
 {all_files_string}
 
 
 Here is the summary of the error that occurred:
 {summarized_error}
 
-To solve this error, you should:
-1. Suggest 3 to 5 possible solutions on how to solve it. You have no access to the documentation of the package.
-2. Decide for the best solution and explain it in detail.
-3. Write down the files that need to be changed, but not files that don't need to be changed.
-Note that any changes needed to make the test pass must be written under the constraint that ''' + IMPLEMENTATION_FILE_NAME +  ''' will be used in a different file as well.
+You should suggest 3 to 5 possible solution approaches on how to solve it.
 Obey the following rules:
+Do not implement the solution.
+You have no access to the documentation of the package.
+You must not change the Dockerfile.
+Note that any changes needed to make the test pass must be written under the constraint that ''' + IMPLEMENTATION_FILE_NAME +  ''' will be used in a different file as well.
 ''' + f'{not_allowed_function_string}\n{not_allowed_docker_string}\n{gpt_35_turbo_usage_string}' + '''
 
+
+After thinking about the possible solutions, output them as JSON ranked from best to worst.
+You must use the following format:
+''' + response_format_suggest_solutions + '''
+Ensure the response starts with **solutions.json** and can be parsed by Python json.loads'''
+)
+
+
+response_format_was_error_seen_before = '''**was_error_seen_before.json**
+```json
+{{"was_error_seen_before": "<yes/no>"}}
+```'''
+
+
+template_was_error_seen_before = PromptTemplate.from_template(
+    '''Previously encountered error messages:
+{previous_errors}
+
+Now encountered error message: "{summarized_error}"
+Was this error message encountered before?
+
+Write down your final answer as json in the following format:
+''' + response_format_was_error_seen_before + '''
+Note that you must obey the double asterisk and triple backtick syntax from above. Ensure the response can be parsed by Python json.loads
+'''
+)
+
+
+response_format_was_solution_tried_before = '''**will_lead_to_different_actions.json**
+```json
+{{"will_lead_to_different_actions": "<yes/no>"}}
+```'''
+
+
+template_was_solution_tried_before = PromptTemplate.from_template(
+    '''Previously tried solutions:
+{tried_solutions}
+
+Suggested solution: "{suggested_solution}"
+
+Will the suggested solution lead to different actions than the previously tried solutions?
+
+Write down your final answer as json in the following format:
+''' + response_format_was_solution_tried_before + '''
+Note that you must obey the double asterisk and triple backtick syntax from above. Ensure the response can be parsed by Python json.loads'''
+)
+
+
+template_implement_solution_code_issue = PromptTemplate.from_template(
+    '''Here is the description of the task the function must solve:
+{task_description}
+
+Here is the test scenario the function must pass:
+{test_description}
+Here are all the files I use:
+{all_files_string}
+
+Implemented the suggested solution: {suggested_solution}
+
 Output all the files that need change. You must not change the Dockerfile. 
 Don't output files that don't need change. If you output a file, then write the complete file.
 Use the exact following syntax to wrap the code:
 
 **...**
 ```...
 ...code...
 ```
 
 Example:
-
-**microservice.py**
+**implementation.py**
 ```python
 import json
 
-def func(json_input: str) -> str:
-    return json_input['img_base64']
+def func(input_json_dict_string: str) -> str:
+    return json.dumps('output_param1': input_json_dict_string['img_base64'])
 ```'''
 )
 
 
 template_generate_playground = PromptTemplate.from_template(
     general_guidelines_string + '''👨‍💻
 
 {code_files_wrapped}
 
-Create a playground for the executor {microservice_name} using streamlit.
-The playground must look like it was made by a professional designer.
-All the ui elements are well thought out to make them visually appealing and easy to use.
-Don't mention the word Playground in the title.
-The playground contains many emojis that fit the theme of the playground and has an emoji as favicon.
-The playground encourages the user to deploy their own microservice by clicking on this link: https://github.com/jina-ai/dev-gpt
-The playground uses the following code to send a request to the microservice:
-```
-from jina import Client, Document, DocumentArray
-client = Client(host='http://localhost:8080')
-d = Document(text=json.dumps(INPUT_DICTIONARY)) # fill-in dictionary which takes input
-response = client.post('/', inputs=DocumentArray([d])) # always use '/'
-print(response[0].text) # can also be blob in case of image/audio..., this should be visualized in the streamlit app
-```
-Note that the response will always be in response[0].text
-The playground displays a code block containing the microservice specific curl code that can be used to send the request to the microservice.
-While the exact payload in the curl might change, the host and deployment ID always stay the same. Example: 
-```
-deployment_id = os.environ.get("K8S_NAMESPACE_NAME", "")
-host = f'https://dev-gpt-{{deployment_id.split("-")[1]}}.wolf.jina.ai/post' if deployment_id else "http://localhost:8080/post"
-with st.expander("See curl command"):
-    st.code(
-        f'curl -X \\'POST\\' \\'host\\' -H \\'accept: application/json\\' -H \\'Content-Type: application/json\\' -d \\'{{{{"data": [{{{{"text": "hello, world!"}}}}]}}}}\\'',
-        language='bash'
-    )
+1. Write down the json request model required by microservice.py.
+2. Generate a playground for the microservice {microservice_name} using the following streamlit template by replacing all the placeholders (<...>) with the correct values:
+**app_template.py**
+```python
+{playground_template}
 ```
-You must provide the complete app.py file using the following syntax to wrap the code:
+Note: Don't mention the word Playground in the title.
+Most importantly: You must generate the complete app.py file using the following syntax to wrap the code:
 **app.py**
 ```python
 ...
-```
-The playground (app.py) must always use the host on http://localhost:8080  and must not let the user configure the host on the UI.
-The playground (app.py) must not import the executor.
-'''
+```'''
 )
 
 
 template_chain_of_thought = PromptTemplate.from_template(
-    '''First, write down an extensive list of obvious and non-obvious observations about {file_name_purpose} that could need an adjustment. Explain why.
-Think if all the changes are required and finally decide for the changes you want to make, but you are not allowed disregard the instructions in the previous message.
-Be very hesitant to change the code. Only make a change if you are sure that it is necessary.
-
-Output only {file_name_purpose}
-Write the whole content of {file_name_purpose} - even if you decided to change only a small thing or even nothing.
+    '''\
+1. write down an extensive list (5 words per item) of obvious and non-obvious observations about {file_name_purpose} that could need an adjustment. 
+2. Explain why. (5 words per item)
+3. Think if all the changes are required
+4. decide for the changes you want to make, but you are not allowed disregard the instructions in the previous message.
+5. Write the whole content of {file_name_purpose} - even if you decided to change only a small thing or even nothing.
+Note: Be very hesitant to change the code. Only make a change if you are sure that it is necessary.
+Note: Output only {file_name_purpose}
 ''' + '\n' + template_code_wrapping_string + '''
 
 Remember: 
 The playground (app.py) must always use the host on http://localhost:8080 and must not let the user configure the host on the UI.
 The playground (app.py) must not import the executor.
 '''
 )
@@ -423,15 +501,15 @@
     "example_input": "<example input file or string here if mentioned before otherwise n/a>",
     "code_samples": "<code samples from the client here>",
     "documentation_info": "<documentation info here>",
     "credentials: "<credentials here>"
 }}
 ``` 
 Note that your response must be either prompt.json or final.json. You must not write both.
-Note that you must obey the double asterisk and tripple backtick syntax from above.
+Note that you must obey the double asterisk and triple backtick syntax from above.
 Note that the last sequence of characters in your response must be ``` (triple backtick).
 Note that prompt.json must not only contain one question.
 Note that if urls, secrets, database names, etc. are mentioned, they must be part of the summary.
 {custom_suffix}
 '''
 )
 
@@ -467,14 +545,14 @@
 ```json
 {{
     "input": "<input here>",
     "assertion": "the output contains the result that is of type <type here>"
 }}
 ```
 Note that your response must be either prompt.json or final.json. You must not write both.
-Note that you must obey the double asterisk and tripple backtick syntax from above.
+Note that you must obey the double asterisk and triple backtick syntax from above.
 Note that the last sequence of characters in your response must be ``` (triple backtick).
 Note that your response must start with the character sequence ** (double asterisk).
 Note that prompt.json must only contain one question.
 {custom_suffix}
 '''
 )
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.42.dev1/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/utils/io.py` & `dev-gpt-0.18.42.dev1/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.42.dev1/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.42.dev1/dev_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.41.dev9
+Version: 0.18.42.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -65,33 +65,39 @@
 </a>
 <a href="https://github.com/tiangolo/dev-gpt/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://img.shields.io/badge/platform-mac%20%7C%20linux%20%7C%20windows-blue" alt="Supported platforms">
 </a>
 <a href="https://pypistats.org/packages/dev-gpt" target="_blank">
     <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
-<a href="https://discord.gg/tBrFhx384D" target="_blank">
-    <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
-</a>
+<a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
+
 
 </p>
 
-Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
+Welcome to Dev-GPT, where we bring your ideas to life with the power of advanced artificial intelligence! 
+Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. 
+Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
 ## Quickstart
 
 ```bash
 pip install dev-gpt
 dev-gpt generate
 ```
 
 ### Requirements
 - OpenAI key with access to gpt-3.5-turbo or gpt-4
+- if you want to enable your microservice to search for web content, 
+you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID environment variables.
+More information can be found [here](https://developers.google.com/custom-search/v1/overview).
 ```bash
-dev-gpt configure --key <your openai api key>
+dev-gpt configure --openai_api_key <your openai api key>
+dev-gpt configure --google_api_key <google api key> (optional if you want to use google search)
+dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google search)
 ```
 
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ## Docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.41.dev9 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.42.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -12,27 +12,34 @@
             ****** Dev GPT: Your Automated Development Team ******
                 â ï¸ This is an experimental version. â ï¸
                     [Product Manager] [Developer] [DevOps]
                      Product Manager   Developer   DevOps
 Tell your AI team what microservice you want to build, and they will do it for
                       you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
-                     platforms] [Downloads] [Discord_Chat]
-Welcome to Dev GPT, where we bring your ideas to life with the power of
+            platforms] [Downloads] [https://img.shields.io/discord/
+      1106542220112302130?logo=discord&logoColor=white&style=flat-square]
+Welcome to Dev-GPT, where we bring your ideas to life with the power of
 advanced artificial intelligence! Our automated development team is designed to
 create microservices tailored to your specific needs, making your software
 development process seamless and efficient. Comprised of a virtual Product
 Manager, Developer, and DevOps, our AI team ensures that every aspect of your
 project is covered, from concept to deployment. ## Quickstart ```bash pip
 install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
-to gpt-3.5-turbo or gpt-4 ```bash dev-gpt configure --key  ``` If you set the
-environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
-Your api key must have access to gpt-4 to use this tool. We are working on a
-way to use gpt-3.5-turbo as well. ## Docs ### Generate Microservice ```bash
-dev-gpt generate \ --description "" \ --model
+to gpt-3.5-turbo or gpt-4 - if you want to enable your microservice to search
+for web content, you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID
+environment variables. More information can be found [here](https://
+developers.google.com/custom-search/v1/overview). ```bash dev-gpt configure --
+openai_api_key  dev-gpt configure --google_api_key  (optional if you want to
+use google search) dev-gpt configure --google_cse_id  (optional if you want to
+use google search) ``` If you set the environment variable `OPENAI_API_KEY`,
+the configuration step can be skipped. Your api key must have access to gpt-
+4 to use this tool. We are working on a way to use gpt-3.5-turbo as well. ##
+Docs ### Generate Microservice ```bash dev-gpt generate \ --description "" \ --
+model
 5-turbo or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5-turbo` or `gpt-4`. `gpt-3.5-
 turbo` is ~10x cheaper, but will not be able to generate as complex
 microservices. (default: largest you have access to) - A `path` on the local
 drive where the microservice will be generated. (default: ./microservice) The
```

### Comparing `dev-gpt-0.18.41.dev9/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.42.dev1/dev_gpt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 dev_gpt/apis/pypi.py
 dev_gpt/options/__init__.py
 dev_gpt/options/configure/__init__.py
 dev_gpt/options/configure/key_handling.py
 dev_gpt/options/deploy/__init__.py
 dev_gpt/options/deploy/deployer.py
 dev_gpt/options/generate/__init__.py
+dev_gpt/options/generate/conversation_logger.py
 dev_gpt/options/generate/generator.py
 dev_gpt/options/generate/parser.py
 dev_gpt/options/generate/prompt_factory.py
 dev_gpt/options/generate/templates_system.py
 dev_gpt/options/generate/templates_user.py
 dev_gpt/options/generate/ui.py
 dev_gpt/options/generate/chains/__init__.py
@@ -40,28 +41,34 @@
 dev_gpt/options/generate/pm/__init__.py
 dev_gpt/options/generate/pm/pm.py
 dev_gpt/options/generate/pm/task_tree_schema.py
 dev_gpt/options/generate/static_files/base_image/Dockerfile
 dev_gpt/options/generate/static_files/gateway/Dockerfile
 dev_gpt/options/generate/static_files/gateway/__init__.py
 dev_gpt/options/generate/static_files/gateway/app_config.toml
+dev_gpt/options/generate/static_files/gateway/app_template.py
 dev_gpt/options/generate/static_files/gateway/custom_gateway.py
 dev_gpt/options/generate/static_files/gateway/nginx.conf
 dev_gpt/options/generate/static_files/gateway/requirements.txt
 dev_gpt/options/generate/static_files/microservice/Dockerfile
 dev_gpt/options/generate/static_files/microservice/__init__.py
-dev_gpt/options/generate/static_files/microservice/apis.py
+dev_gpt/options/generate/static_files/microservice/google_custom_search.py
+dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py
 dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+dev_gpt/options/generate/tools/__init__.py
+dev_gpt/options/generate/tools/tools.py
 dev_gpt/options/run/__init__.py
 dev_gpt/options/run/runner.py
 dev_gpt/utils/__init__.py
 dev_gpt/utils/io.py
 dev_gpt/utils/string_tools.py
 test/__init__.py
 test/conftest.py
 test/integration/__init__.py
 test/integration/test_generator.py
 test/unit/__init__.py
 test/unit/test_api.py
 test/unit/test_construct_sub_task_tree.py
 test/unit/test_response_parsing.py
-test/unit/test_strings.py
+test/unit/test_search.py
+test/unit/test_strings.py
+test/unit/test_tools.py
```

### Comparing `dev-gpt-0.18.41.dev9/setup.py` & `dev-gpt-0.18.42.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/test/conftest.py` & `dev-gpt-0.18.42.dev1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/test/integration/test_generator.py` & `dev-gpt-0.18.42.dev1/test/integration/test_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     APIs: ❌
     Databases: ❌
     """
     os.environ['VERBOSE'] = 'true'
     generator = Generator(
         "The microservice is very simple, it does not take anything as input and only outputs the word 'test'",
         microservice_dir,
-        'gpt-3.5-turbo'
+        'gpt-3.5-turbo',
+        self_healing=False,
     )
     assert generator.generate() == 0
 
 
-
 @pytest.mark.parametrize('mock_input_sequence', [['y']], indirect=True)
 def test_generation_level_1(microservice_dir, mock_input_sequence):
     """
     Requirements:
     coding challenge: ❌
     pip packages: ❌
     environment: ❌
@@ -42,38 +42,64 @@
     os.environ['VERBOSE'] = 'true'
     generator = Generator(
         '''Input is a tweet that might contain passive aggressive language. The output is the positive version of that tweet.
 Example tweet: 
 \'When your coworker microwaves fish in the break room... AGAIN. 🐟🤢 
 But hey, at least SOMEONE's enjoying their lunch. #officelife\'''',
         str(microservice_dir),
-        'gpt-3.5-turbo'
+        'gpt-3.5-turbo',
+        # self_healing=False,
     )
     assert generator.generate() == 0
 
 
-@pytest.mark.parametrize('mock_input_sequence', [['y', 'https://www.africau.edu/images/default/sample.pdf']], indirect=True)
+@pytest.mark.parametrize('mock_input_sequence', [['y', 'https://www.africau.edu/images/default/sample.pdf']],
+                         indirect=True)
 def test_generation_level_2(microservice_dir, mock_input_sequence):
     """
     Requirements:
     coding challenge: ❌
     pip packages: ✅ (pdf parser)
     environment: ❌
     GPT-3.5-turbo: ✅ (for summarizing the text)
     APIs: ❌
     Databases: ❌
     """
     os.environ['VERBOSE'] = 'true'
     generator = Generator(
         "The input is a PDF and the output the summarized text (50 words).",
         str(microservice_dir),
-        'gpt-3.5-turbo'
+        'gpt-3.5-turbo',
+        # self_healing=False,
     )
     assert generator.generate() == 0
 
+
+@pytest.mark.parametrize('mock_input_sequence', [
+    ['y', 'https://upload.wikimedia.org/wikipedia/commons/4/47/PNG_transparency_demonstration_1.png']], indirect=True)
+def test_generation_level_2_svg(microservice_dir, mock_input_sequence):
+    """
+    Requirements:
+    coding challenge: ✅
+    pip packages: ✅
+    environment: ❌
+    GPT-3.5-turbo: ❌
+    APIs: ❌
+    Databases: ❌
+    """
+    os.environ['VERBOSE'] = 'true'
+    generator = Generator(
+        "Get a png as input and return a vectorized version as svg.",
+        str(microservice_dir),
+        'gpt-3.5-turbo',
+        # self_healing=False,
+    )
+    assert generator.generate() == 0
+
+
 @pytest.mark.parametrize('mock_input_sequence', [['y', 'yfinance.Ticker("MSFT").info']], indirect=True)
 def test_generation_level_3(microservice_dir, mock_input_sequence):
     """
     Requirements:
     coding challenge: ✅ (calculate the average closing price)
     pip packages: ❌
     environment: ❌
@@ -87,18 +113,20 @@
 1. Fetch stock data (open, high, low, close, volume) for the past 30 days using a financial data API Yahoo Finance.
 2. Calculate the average closing price over the 30 days.
 3. Generate a brief summary of the company's stock performance over the past 30 days, including the average closing price and the company name.
 4. Return the summary as a string.
 Example input: 'AAPL'
 ''',
         str(microservice_dir),
-        'gpt-3.5-turbo'
+        'gpt-3.5-turbo',
+        # self_healing=False,
     )
     assert generator.generate() == 0
 
+
 @pytest.mark.parametrize(
     'mock_input_sequence', [
         [
             'y',
             'https://www2.cs.uic.edu/~i101/SoundFiles/taunt.wav',
             f'''\
 import requests
@@ -131,31 +159,53 @@
         f'''Given an audio file (1min wav) of speech, 
 1. convert it to text using the Whisper API.
 2. Summarize the text (~50 words) while still maintaining the key facts.
 3. Create an audio file of the summarized text using a tts library.
 4. Return the the audio file as base64 encoded binary.
 ''',
         str(microservice_dir),
-        'gpt-4'
+        'gpt-4',
+        # self_healing=False,
+    )
+    assert generator.generate() == 0
+
+
+@pytest.mark.parametrize('mock_input_sequence', [['y']], indirect=True)
+def test_generation_level_5_company_logos(microservice_dir, mock_input_sequence):
+    os.environ['VERBOSE'] = 'true'
+    generator = Generator(
+        f'''\
+Given a list of email addresses, get all company names from them.
+For all companies, get the company logo.
+All logos need to be arranged on a square.
+The square is returned as png.
+''',
+        str(microservice_dir),
+        'gpt-3.5-turbo',
+        # self_healing=False,
     )
     assert generator.generate() == 0
 
-@pytest.mark.parametrize('mock_input_sequence', [['y', 'https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/PNG_transparency_demonstration_1.png/560px-PNG_transparency_demonstration_1.png']], indirect=True)
+
+@pytest.mark.parametrize('mock_input_sequence', [['y',
+                                                  'https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/PNG_transparency_demonstration_1.png/560px-PNG_transparency_demonstration_1.png']],
+                         indirect=True)
 def test_generation_level_5(microservice_dir, mock_input_sequence):
     """
     Requirements:
     coding challenge: ✅ (putting text on the image)
     pip packages: ✅ (Pillow for image processing)
     environment: ✅ (image library)
     GPT-3.5-turbo: ✅ (for writing the joke)
     APIs: ✅ (scenex for image description)
     Databases: ❌
     """
     os.environ['VERBOSE'] = 'true'
-    generator = Generator(f'''
+    generator = Generator(
+        f'''
 The input is an image.
 Use the following api to get the description of the image:
 Request:
 curl "https://us-central1-causal-diffusion.cloudfunctions.net/describe" \\
   -H "x-api-key: token {os.environ['SCENEX_API_KEY']}" \\
   -H "content-type: application/json" \\
   --data '{{"data":[
@@ -169,17 +219,18 @@
     }}
   ]
 }}
 The description is then used to generate a joke.
 The joke is the put on the image.
 The output is the image with the joke on it.
 ''',
-                          str(microservice_dir),
-                          'gpt-3.5-turbo'
-                          )
+        str(microservice_dir),
+        'gpt-3.5-turbo',
+        # self_healing=False,
+    )
     assert generator.generate() == 0
 
 # @pytest.fixture
 # def microservice_dir():
 #     return 'microservice'
```

### Comparing `dev-gpt-0.18.41.dev9/test/unit/test_api.py` & `dev-gpt-0.18.42.dev1/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.41.dev9/test/unit/test_response_parsing.py` & `dev-gpt-0.18.42.dev1/test/unit/test_response_parsing.py`

 * *Files identical despite different names*

