# Comparing `tmp/oarepo-cli-11.0.7.tar.gz` & `tmp/oarepo-cli-11.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-cli-11.0.7.tar", last modified: Fri Feb 24 08:36:45 2023, max compression
+gzip compressed data, was "oarepo-cli-11.0.8.tar", last modified: Fri Feb 24 09:15:57 2023, max compression
```

## Comparing `oarepo-cli-11.0.7.tar` & `oarepo-cli-11.0.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.058465 oarepo-cli-11.0.7/oarepo_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.058465 oarepo-cli-11.0.7/oarepo_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.058465 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_01_initialize_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_02_deployment_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_03_create_monorepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_04_install_invenio_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_05_install_oarepo_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_06_primary_site_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.058465 oarepo-cli-11.0.7/oarepo_cli/cli/model/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/model/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/model/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/model/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/model/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/model/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.058465 oarepo-cli-11.0.7/oarepo_cli/cli/run/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/cli/site/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_01_install_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_02_check_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_03_fixup_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_04_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_05_create_pipenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_06_install_invenio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_07_init_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/step_08_next_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/site/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/cli/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/ui/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/ui/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/ui/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/templates/repo/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/cookiecutter
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.envrc
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/invenio-cli
--rwxr-xr-x   0 runner    (1001) docker     (123)      261 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/nrp-cli
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/oarepo_cli/ui/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/wizard/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/wizard/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/ui/wizard/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/oarepo_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:36:45.058465 oarepo-cli-11.0.7/oarepo_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-24 08:36:45.000000 oarepo-cli-11.0.7/oarepo_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-24 08:36:45.000000 oarepo-cli-11.0.7/oarepo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 08:36:45.000000 oarepo-cli-11.0.7/oarepo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-24 08:36:45.000000 oarepo-cli-11.0.7/oarepo_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-24 08:36:45.000000 oarepo-cli-11.0.7/oarepo_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 08:36:45.000000 oarepo-cli-11.0.7/oarepo_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-24 08:36:45.062465 oarepo-cli-11.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-24 08:36:41.000000 oarepo-cli-11.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.797679 oarepo-cli-11.0.8/oarepo_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_01_initialize_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_02_deployment_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_03_create_monorepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_04_install_invenio_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_05_install_oarepo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_06_primary_site_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli/cli/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/cli/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/cli/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_01_install_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_02_check_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_03_fixup_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_04_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_05_create_pipenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_06_install_invenio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_07_init_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_08_next_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/cli/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/templates/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/cookiecutter
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.envrc
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/invenio-cli
+-rwxr-xr-x   0 runner    (1001) docker     (123)      261 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/nrp-cli
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/setup.py
```

### Comparing `oarepo-cli-11.0.7/PKG-INFO` & `oarepo-cli-11.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-cli
-Version: 11.0.7
+Version: 11.0.8
 Summary: Utilities for managing invenio monorepo
 Description-Content-Type: text/markdown
 
 # oarepo-cli
 
 Work in progress.
```

### Comparing `oarepo-cli-11.0.7/README.md` & `oarepo-cli-11.0.8/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/initialize/__init__.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_01_initialize_directory.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_01_initialize_directory.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_02_deployment_type.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_02_deployment_type.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_03_create_monorepo.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_03_create_monorepo.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_04_install_invenio_cli.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_04_install_invenio_cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_05_install_oarepo_cli.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_05_install_oarepo_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if oarepo_cli_dir.exists():
             shutil.rmtree(oarepo_cli_dir)
         venv.main([str(oarepo_cli_dir)])
 
         pip_install(
             oarepo_cli_dir / "bin" / "pip",
             "OAREPO_CLI_VERSION",
-            "oarepo-cli==11",
+            "oarepo-cli>=11.0.8,<12",
             "https://github.com/oarepo/oarepo-cli",
         )
 
         with open(oarepo_cli_dir / ".check.ok", "w") as f:
             f.write("oarepo check ok")
         commit_git(
             self.data.project_dir,
```

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/initialize/step_06_primary_site_name.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_06_primary_site_name.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/model/add.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/model/add.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/model/compile.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/model/compile.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/model/install.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/model/install.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/model/load.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/model/load.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/run/__init__.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/add.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/add.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_01_install_site.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_01_install_site.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_02_check_requirements.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_02_check_requirements.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_03_fixup_code.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_03_fixup_code.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_04_start_containers.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_04_start_containers.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_05_create_pipenv.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_05_create_pipenv.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_06_install_invenio.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_06_install_invenio.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_07_init_database.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_07_init_database.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/site/step_08_next_steps.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_08_next_steps.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/ui/add.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/ui/add.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/ui/install.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/ui/install.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/cli/utils.py` & `oarepo-cli-11.0.8/oarepo_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/config.py` & `oarepo-cli-11.0.8/oarepo_cli/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore` & `oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/invenio-cli` & `oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/invenio-cli`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/ui/input.py` & `oarepo-cli-11.0.8/oarepo_cli/ui/input.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/ui/radio.py` & `oarepo-cli-11.0.8/oarepo_cli/ui/radio.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/ui/wizard/steps.py` & `oarepo-cli-11.0.8/oarepo_cli/ui/wizard/steps.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli/utils.py` & `oarepo-cli-11.0.8/oarepo_cli/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/oarepo_cli.egg-info/PKG-INFO` & `oarepo-cli-11.0.8/oarepo_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-cli
-Version: 11.0.7
+Version: 11.0.8
 Summary: Utilities for managing invenio monorepo
 Description-Content-Type: text/markdown
 
 # oarepo-cli
 
 Work in progress.
```

### Comparing `oarepo-cli-11.0.7/oarepo_cli.egg-info/SOURCES.txt` & `oarepo-cli-11.0.8/oarepo_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.0.7/setup.cfg` & `oarepo-cli-11.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-cli
-version = 11.0.7
+version = 11.0.8
 description = Utilities for managing invenio monorepo
 authors = Miroslav Simek <simeki@vscht.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

