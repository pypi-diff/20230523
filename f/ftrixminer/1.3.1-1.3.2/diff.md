# Comparing `tmp/ftrixminer-1.3.1.tar.gz` & `tmp/ftrixminer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrixminer-1.3.1.tar", last modified: Mon May 22 17:39:33 2023, max compression
+gzip compressed data, was "ftrixminer-1.3.2.tar", last modified: Tue May 23 05:00:19 2023, max compression
```

## Comparing `ftrixminer-1.3.1.tar` & `ftrixminer-1.3.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.498530 ftrixminer-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.486529 ftrixminer-1.3.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-22 17:39:33.498530 ftrixminer-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.486529 ftrixminer-1.3.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.490529 ftrixminer-1.3.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:39:33.498530 ftrixminer-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.486529 ftrixminer-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/src/ftrixminer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-22 17:39:33.000000 ftrixminer-1.3.1/src/ftrixminer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-22 17:39:33.000000 ftrixminer-1.3.1/src/ftrixminer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:39:33.000000 ftrixminer-1.3.1/src/ftrixminer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 17:39:33.000000 ftrixminer-1.3.1/src/ftrixminer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 17:39:33.000000 ftrixminer-1.3.1/src/ftrixminer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 17:39:33.000000 ftrixminer-1.3.1/src/ftrixminer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/src/ftrixminer_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/src/ftrixminer_api/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/src/ftrixminer_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/explore1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.494529 ftrixminer-1.3.1/src/ftrixminer_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 17:39:33.000000 ftrixminer-1.3.1/src/ftrixminer_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.498530 ftrixminer-1.3.1/src/ftrixminer_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.498530 ftrixminer-1.3.1/src/ftrixminer_lib/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/miners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/miners/direct_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/src/ftrixminer_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.498530 ftrixminer-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:39:33.498530 ftrixminer-1.3.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-22 17:39:25.000000 ftrixminer-1.3.1/tests/test_miner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.078558 ftrixminer-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.066558 ftrixminer-1.3.2/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.066558 ftrixminer-1.3.2/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.066558 ftrixminer-1.3.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.066558 ftrixminer-1.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.062558 ftrixminer-1.3.2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.066558 ftrixminer-1.3.2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.066558 ftrixminer-1.3.2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-23 05:00:19.078558 ftrixminer-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.062558 ftrixminer-1.3.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 05:00:19.078558 ftrixminer-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.066558 ftrixminer-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.070557 ftrixminer-1.3.2/src/ftrixminer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-23 05:00:19.000000 ftrixminer-1.3.2/src/ftrixminer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-23 05:00:19.000000 ftrixminer-1.3.2/src/ftrixminer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 05:00:19.000000 ftrixminer-1.3.2/src/ftrixminer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 05:00:19.000000 ftrixminer-1.3.2/src/ftrixminer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 05:00:19.000000 ftrixminer-1.3.2/src/ftrixminer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 05:00:19.000000 ftrixminer-1.3.2/src/ftrixminer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.074558 ftrixminer-1.3.2/src/ftrixminer_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.074558 ftrixminer-1.3.2/src/ftrixminer_api/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.074558 ftrixminer-1.3.2/src/ftrixminer_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.074558 ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/explore1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.074558 ftrixminer-1.3.2/src/ftrixminer_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 05:00:18.000000 ftrixminer-1.3.2/src/ftrixminer_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.074558 ftrixminer-1.3.2/src/ftrixminer_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.074558 ftrixminer-1.3.2/src/ftrixminer_lib/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/miners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/miners/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/src/ftrixminer_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.078558 ftrixminer-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:00:19.078558 ftrixminer-1.3.2/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-23 05:00:11.000000 ftrixminer-1.3.2/tests/test_miner.py
```

### Comparing `ftrixminer-1.3.1/.dae-devops/Makefile` & `ftrixminer-1.3.2/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.dae-devops/docs/conventions.rst` & `ftrixminer-1.3.2/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.dae-devops/docs/developing.rst` & `ftrixminer-1.3.2/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.dae-devops/docs/devops.rst` & `ftrixminer-1.3.2/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.dae-devops/docs/docs_structure.rst` & `ftrixminer-1.3.2/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.dae-devops/docs/installing.rst` & `ftrixminer-1.3.2/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.dae-devops/docs/testing.rst` & `ftrixminer-1.3.2/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.dae-devops/project.yaml` & `ftrixminer-1.3.2/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.devcontainer/Dockerfile` & `ftrixminer-1.3.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.devcontainer/devcontainer.json` & `ftrixminer-1.3.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/CONTRIBUTING.rst` & `ftrixminer-1.3.2/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/actions/install_requirements/action.yml` & `ftrixminer-1.3.2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/dependabot.yml` & `ftrixminer-1.3.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/pages/make_switcher.py` & `ftrixminer-1.3.2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/workflows/code.yml` & `ftrixminer-1.3.2/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/workflows/docs.yml` & `ftrixminer-1.3.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/workflows/docs_clean.yml` & `ftrixminer-1.3.2/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.github/workflows/linkcheck.yml` & `ftrixminer-1.3.2/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.gitignore` & `ftrixminer-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.gitlab-ci.yml` & `ftrixminer-1.3.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/.vscode/launch.json` & `ftrixminer-1.3.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/LICENSE` & `ftrixminer-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/PKG-INFO` & `ftrixminer-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrixminer
-Version: 1.3.1
+Version: 1.3.2
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ftrixminer-1.3.1/README.rst` & `ftrixminer-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/docs/conf.py` & `ftrixminer-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/docs/images/dls-favicon.ico` & `ftrixminer-1.3.2/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/docs/images/dls-logo.svg` & `ftrixminer-1.3.2/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/docs/index.rst` & `ftrixminer-1.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/docs/user/explanations/25-docs-structure.rst` & `ftrixminer-1.3.2/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/docs/user/index.rst` & `ftrixminer-1.3.2/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/pyproject.toml` & `ftrixminer-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer.egg-info/PKG-INFO` & `ftrixminer-1.3.2/src/ftrixminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrixminer
-Version: 1.3.1
+Version: 1.3.2
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ftrixminer-1.3.1/src/ftrixminer.egg-info/SOURCES.txt` & `ftrixminer-1.3.2/src/ftrixminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_api/context_base.py` & `ftrixminer-1.3.2/src/ftrixminer_api/context_base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_api/exceptions.py` & `ftrixminer-1.3.2/src/ftrixminer_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_api/miners/aiohttp.py` & `ftrixminer-1.3.2/src/ftrixminer_api/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_api/miners/context.py` & `ftrixminer-1.3.2/src/ftrixminer_api/miners/context.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_api/miners/miners.py` & `ftrixminer-1.3.2/src/ftrixminer_api/miners/miners.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_api/thing.py` & `ftrixminer-1.3.2/src/ftrixminer_api/thing.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_api/things.py` & `ftrixminer-1.3.2/src/ftrixminer_api/things.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_cli/main.py` & `ftrixminer-1.3.2/src/ftrixminer_cli/main.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/base.py` & `ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/explore1.py` & `ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/explore1.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_cli/subcommands/service.py` & `ftrixminer-1.3.2/src/ftrixminer_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_cli/version.py` & `ftrixminer-1.3.2/src/ftrixminer_cli/version.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/__main__.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/contexts/base.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/exceptions.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/miners/aiohttp.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/miners/base.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/miners/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/miners/context.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/miners/context.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/miners/direct_poll.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/miners/direct_poll.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
         cursor = connection.cursor()
         cursor.execute(sql)
         rows = cursor.fetchall()
 
         if self.__query_count % 60 == 0:
             logger.debug(
-                f"query #{self.__query_count}. got {len(rows)} rows from\n{sql}"
+                f"[FTRIXMINER POLL] query #{self.__query_count}. got {len(rows)} rows from\n{sql}"
             )
 
         self.__query_count += 1
 
         return rows
 
     # ----------------------------------------------------------------------------------------
```

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/miners/miners.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/miners/miners.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/src/ftrixminer_lib/version.py` & `ftrixminer-1.3.2/src/ftrixminer_lib/version.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/tests/base.py` & `ftrixminer-1.3.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/tests/configurations/direct_poll.yaml` & `ftrixminer-1.3.2/tests/configurations/direct_poll.yaml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/tests/configurations/service.yaml` & `ftrixminer-1.3.2/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/tests/conftest.py` & `ftrixminer-1.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.3.1/tests/test_miner.py` & `ftrixminer-1.3.2/tests/test_miner.py`

 * *Files identical despite different names*

