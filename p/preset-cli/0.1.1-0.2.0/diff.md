# Comparing `tmp/preset-cli-0.1.1.tar.gz` & `tmp/preset-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preset-cli-0.1.1.tar", last modified: Tue Sep 13 23:39:13 2022, max compression
+gzip compressed data, was "preset-cli-0.2.0.tar", last modified: Tue May 23 17:55:28 2023, max compression
```

## Comparing `preset-cli-0.1.1.tar` & `preset-cli-0.2.0.tar`

### file list

```diff
@@ -1,146 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.212025 preset-cli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.188024 preset-cli-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.196024 preset-cli-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-09-13 23:39:00.000000 preset-cli-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-13 23:39:00.000000 preset-cli-0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-13 23:39:00.000000 preset-cli-0.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13862 2022-09-13 23:39:00.000000 preset-cli-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-13 23:39:00.000000 preset-cli-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-09-13 23:39:00.000000 preset-cli-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    19280 2022-09-13 23:39:13.212025 preset-cli-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18673 2022-09-13 23:39:00.000000 preset-cli-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-13 23:39:00.000000 preset-cli-0.1.1/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-09-13 23:39:00.000000 preset-cli-0.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.196024 preset-cli-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.196024 preset-cli-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9753 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.196024 preset-cli-0.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)   271378 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/images/export_dashboards.png
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-09-13 23:39:00.000000 preset-cli-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.188024 preset-cli-0.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.196024 preset-cli-0.1.1/examples/exports/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.196024 preset-cli-0.1.1/examples/exports/charts/
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-09-13 23:39:00.000000 preset-cli-0.1.1/examples/exports/charts/Total_count_134.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/examples/exports/dashboards/
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-09-13 23:39:00.000000 preset-cli-0.1.1/examples/exports/dashboards/White_label_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/examples/exports/databases/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-09-13 23:39:00.000000 preset-cli-0.1.1/examples/exports/databases/Google_Sheets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.188024 preset-cli-0.1.1/examples/exports/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/examples/exports/datasets/Google_Sheets/
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-09-13 23:39:00.000000 preset-cli-0.1.1/examples/exports/datasets/Google_Sheets/country_cnt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/examples/exports/functions/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-13 23:39:00.000000 preset-cli-0.1.1/examples/exports/functions/demo.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-13 23:39:00.000000 preset-cli-0.1.1/examples/exports/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-09-13 23:39:00.000000 preset-cli-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-13 23:39:00.000000 preset-cli-0.1.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-09-13 23:39:00.000000 preset-cli-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-09-13 23:39:13.216025 preset-cli-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-13 23:39:00.000000 preset-cli-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.188024 preset-cli-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/src/preset_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/src/preset_cli/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/src/preset_cli/api/clients/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19440 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/api/clients/dbt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4580 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/api/clients/preset.py
--rw-r--r--   0 runner    (1001) docker     (121)    25783 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/api/clients/superset.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/api/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.204025 preset-cli-0.1.1/src/preset_cli/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/auth/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/auth/lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.204025 preset-cli-0.1.1/src/preset_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9342 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.204025 preset-cli-0.1.1/src/preset_cli/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4625 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/import_.py
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.204025 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.208025 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5746 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/databases.py
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/exposures.py
--rw-r--r--   0 runner    (1001) docker     (121)    11006 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.208025 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6400 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/cli/superset/sync/native/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-13 23:39:00.000000 preset-cli-0.1.1/src/preset_cli/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.200024 preset-cli-0.1.1/src/preset_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19280 2022-09-13 23:39:13.000000 preset-cli-0.1.1/src/preset_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-09-13 23:39:13.000000 preset-cli-0.1.1/src/preset_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 23:39:13.000000 preset-cli-0.1.1/src/preset_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-13 23:39:13.000000 preset-cli-0.1.1/src/preset_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 23:39:12.000000 preset-cli-0.1.1/src/preset_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-13 23:39:13.000000 preset-cli-0.1.1/src/preset_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-13 23:39:13.000000 preset-cli-0.1.1/src/preset_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.208025 preset-cli-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.208025 preset-cli-0.1.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.208025 preset-cli-0.1.1/tests/api/clients/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41534 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/api/clients/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/api/clients/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    63743 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/api/clients/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.208025 preset-cli-0.1.1/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/auth/jwt_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2220 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/auth/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/auth/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.208025 preset-cli-0.1.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15964 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.212025 preset-cli-0.1.1/tests/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9337 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/export_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/import_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/main_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11781 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sql_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.212025 preset-cli-0.1.1/tests/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.212025 preset-cli-0.1.1/tests/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13313 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/command_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10330 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8354 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    22290 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/exposures_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10880 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9054 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/dbt/metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:13.212025 preset-cli-0.1.1/tests/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13206 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/cli/superset/sync/native/command_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-09-13 23:39:00.000000 preset-cli-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 17:55:16.000000 preset-cli-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-05-23 17:55:16.000000 preset-cli-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-23 17:55:16.000000 preset-cli-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 17:55:16.000000 preset-cli-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 17:55:16.000000 preset-cli-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-23 17:55:28.988757 preset-cli-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-05-23 17:55:16.000000 preset-cli-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 17:55:16.000000 preset-cli-0.2.0/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-23 17:55:16.000000 preset-cli-0.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/images/export_dashboards.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/charts/Total_count_134.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/dashboards/White_label_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/databases/Google_Sheets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/examples/exports/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/datasets/Google_Sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/datasets/Google_Sheets/country_cnt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/functions/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 17:55:16.000000 preset-cli-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 17:55:16.000000 preset-cli-0.2.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-23 17:55:16.000000 preset-cli-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-23 17:55:28.988757 preset-cli-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-23 17:55:16.000000 preset-cli-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35266 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/superset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/exposures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/native/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47038 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87530 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/jwt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/password_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/preset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sql_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32583 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/exposures_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/native/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tox.ini
```

### Comparing `preset-cli-0.1.1/.coveragerc` & `preset-cli-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/.github/workflows/python-package-daily.yml` & `preset-cli-0.2.0/.github/workflows/python-package-daily.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.8, 3.9, '3.10', '3.11.0-beta.5']
+        python-version: [3.8, 3.9, '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `preset-cli-0.1.1/.github/workflows/python-package.yml` & `preset-cli-0.2.0/.github/workflows/python-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.8, 3.9, '3.10']
+        python-version: [3.8, 3.9, '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip wheel
         python -m pip install -r dev-requirements.txt
     - name: Test with pytest
       run: |
+        pre-commit run --all-files
         pytest --cov-fail-under=100 --cov=src/preset_cli -vv tests/
```

### Comparing `preset-cli-0.1.1/.github/workflows/python-publish.yml` & `preset-cli-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/.gitignore` & `preset-cli-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/.pre-commit-config.yaml` & `preset-cli-0.2.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 exclude: '^docs/conf.py'
 
 repos:
-- repo: git://github.com/pre-commit/pre-commit-hooks
+- repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v3.4.0
   hooks:
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
@@ -25,32 +25,32 @@
 #     args: [
 #       --in-place,
 #       --remove-all-unused-imports,
 #       --remove-unused-variables,
 #     ]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.7.0
+  rev: 5.11.5
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 20.8b1
+  rev: 22.10.0
   hooks:
   - id: black
     language_version: python3
 
 ## If like to embrace black styles even in the docs:
 # - repo: https://github.com/asottile/blacken-docs
 #   rev: v1.9.1
 #   hooks:
 #   - id: blacken-docs
 #     additional_dependencies: [black]
 
-- repo: https://gitlab.com/pycqa/flake8
+- repo: https://github.com/PyCQA/flake8
   rev: 3.9.2
   hooks:
   - id: flake8
   ## You can add flake8 plugins via `additional_dependencies`:
   #  additional_dependencies: [flake8-bugbear]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
@@ -70,15 +70,15 @@
   - id: add-trailing-comma
 #- repo: https://github.com/asottile/reorder_python_imports
 #  rev: v2.5.0
 #  hooks:
 #  - id: reorder-python-imports
 #    args: [--application-directories=.:src]
 - repo: https://github.com/hadialqattan/pycln
-  rev: v1.0.3 # Possible releases: https://github.com/hadialqattan/pycln/tags
+  rev: v2.1.2 # Possible releases: https://github.com/hadialqattan/pycln/tags
   hooks:
   - id: pycln
     args: [--config=pyproject.toml]
 - repo: local
   hooks:
   - id: pylint
     name: pylint
```

### Comparing `preset-cli-0.1.1/CONTRIBUTING.rst` & `preset-cli-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/Makefile` & `preset-cli-0.2.0/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 clean:
 	pyenv virtualenv-delete backend-sdk
 
 spellcheck:
 	codespell -S "*.json" src/preset_cli docs/*rst tests templates
 
-requirements.txt: .python-version requirements.in
+requirements.txt: .python-version requirements.in setup.cfg
 	pip install --upgrade pip
 	pip-compile --no-annotate
 
-dev-requirements.txt: dev-requirements.in
+dev-requirements.txt: dev-requirements.in setup.cfg
 	pip-compile dev-requirements.in --no-annotate
 
 check:
 	pre-commit run --all-files
```

### Comparing `preset-cli-0.1.1/PKG-INFO` & `preset-cli-0.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: preset-cli
-Version: 0.1.1
-Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
-Home-page: https://github.com/preset-io/preset-cli
-Author: Beto Dealmeida
-Author-email: beto@preset.io
-License: Other/Proprietary License
-Project-URL: Documentation, https://github.com/preset-io/preset-cli/blob/master/README.rst
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: License :: Other/Proprietary License
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 ==========
 preset-cli
 ==========
 
     A CLI to interact with Preset workspaces.
 
 This tool is a command line interface (CLI) to interact with your Preset workspaces. Currently it can be used to sync resources (databases, datasets, charts, dashboards) from source control, either in native format or from a `dbt <https://www.getdbt.com/>`_ project. It can also be used to run SQL against any database in any workspace. In the future, the CLI will also allow you to manage your workspaces and users.
@@ -31,14 +14,20 @@
 .. code-block:: bash
 
     $ pip install -U setuptools setuptools_scm wheel  # for good measure
     $ pip install preset-cli
 
 Make sure you're using Python 3.8 or newer.
 
+You can also install from ``main``, if you need recent features:
+
+.. code-block:: bash
+
+     $ pip install "git+https://github.com/preset-io/backend-sdk.git"
+
 Authentication
 ==============
 
 The CLI requires an API key for authentication, composed of token and an associated secret. Both can be defined in your environment as ``PRESET_API_TOKEN`` and ``PRESET_API_SECRET``, respectively, or can be stored in a configuration file. To store the credentials in a configuration file simply run ``preset-cli auth``. This should open https://manage.app.preset.io/app/user in your browser so you can generate a new token, and it will prompt you for the token and its secret:
 
 .. code-block:: bash
 
@@ -120,20 +109,24 @@
 
 Commands
 ========
 
 The following commands are currently available:
 
 - ``preset-cli auth``: store authentication credentials.
+- ``preset-cli invite-users``: invite users to Preset.
+- ``preset-cli import-users``: automatically add users to Preset.
+- ``preset-cli list-group-membership``: List SCIM groups from a team and their memberships.
 - ``preset-cli superset sql``: run SQL interactively or programmatically against an analytical database.
-- ``preset-cli superset export-assets``: export resources (databases, datasets, charts, dashboards) into a directory as YAML files.
+- ``preset-cli superset export-assets`` (alternatively, ``preset-cli superset export``): export resources (databases, datasets, charts, dashboards) into a directory as YAML files.
 - ``preset-cli superset export-ownership``: export resource ownership (UUID -> email) into a YAML file.
 - ``preset-cli superset export-rls``: export RLS rules into a YAML file.
+- ``preset-cli superset export-roles``: export user roles into a YAML file.
 - ``preset-cli superset export-users``: export users (name, username, email, roles) into a YAML file.
-- ``preset-cli superset sync native``: synchronize the workspace from a directory of templated configuration files.
+- ``preset-cli superset sync native`` (alternatively, ``preset-cli superset import-assets``): synchronize the workspace from a directory of templated configuration files.
 - ``preset-cli superset sync dbt-core``: synchronize the workspace from a dbt Core project.
 - ``preset-cli superset sync dbt-cloud``: synchronize the workspace from a dbt Cloud project.
 
 All the ``superset`` sub-commands can also be executed against a standalone Superset instance, using the ``superset-cli`` command. This means that if you are running an instance of Superset at https://superset.example.org/ you can export its resources with the command:
 
 .. code-block:: bash
 
@@ -304,53 +297,119 @@
 .. code-block:: yaml
 
     slice_name: {{ functions.demo.hello_world() }}
     viz_type: big_number_total
     params:
       ...
 
+Disabling Jinja Templating
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Both the CLI and Superset support Jinja templating. To prevent the CLI from loading Superset Jinja syntax, the export operation automatically escapes Jinja syntax from YAML files. As a consequence, this query:
+
+.. code-block:: yaml
+
+    sql: 'SELECT action, count(*) as times
+        FROM logs
+        {% if filter_values(''action_type'')|length %}
+            WHERE action is null
+            {% for action in filter_values(''action_type'') %}
+                or action = ''{{ action }}''
+            {% endfor %}
+        {% endif %}
+        GROUP BY action'
+
+Becomes this:
+
+.. code-block:: yaml
+
+    sql: 'SELECT action, count(*) as times
+        FROM logs
+        {{ '{% if' }} filter_values(''action_type'')|length {{ '%}' }}
+            WHERE action is null
+            {{ '{% for' }} action in filter_values(''action_type'') {{ '%}' }}
+                or action = ''{{ '{{' }} action {{ '}}' }}''
+            {{ '{% endfor %}' }}
+        {{ '{% endif %}' }}
+        GROUP BY action'
+
+When performing the import, the CLI would load any templating syntax that isn't escaped, and remove escaping. However, this escaping syntax isn't compatible with UI imports. 
+To avoid issues when running migrations using both the CLI and the UI, you can use:
+
+- ``--disable-jinja-escaping`` flag with the ``export-assets`` command to disable the escaping (so that exported assets can be imported via the UI)
+- ``--disable-jinja-templating`` flag with the ``sync native`` command to disable jinja templating (so that assets exported via the UI can be imported via the CLI)
+
+Note that using these flags would remove the ability to dynamically modify the content through the CLI. 
+
 Synchronizing to and from dbt
 -----------------------------
 
 The CLI also allows you to synchronize models, and metrics from a `dbt <https://www.getdbt.com/>`_ project.
 
-If you're using dbt Core you can point the CLI to your compiled manifest and your profiles file, so that all the database is automatically created, together with all the models and metrics. The full command is:
+If you're using dbt Core you can point the CLI to your compiled manifest and your profiles file, so that the database is automatically created, together with all the models and metrics. The full command is:
 
 .. code-block:: bash
 
    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
    > superset sync dbt-core /path/to/dbt/my_project/target/manifest.json \
-   > --project=my_project --target=dev --profile=${HOME}/.dbt/profiles.yml \
+   > --project=my_project --target=dev --profiles=${HOME}/.dbt/profiles.yml \
    > --exposures=/path/to/dbt/my_project/models/exposures.yaml \
    > --import-db \
    > --external-url-prefix=http://localhost:8080/
 
 Running this command will:
 
 1. Read the dbt profile and create the ``$target`` database for the specified project in the Preset workspace.
 2. Every source in the project will be created as a dataset in the Preset workspace.
 3. Every model in the project will be created as a dataset in the Preset workspace.
 4. Any `metrics <https://docs.getdbt.com/docs/building-a-dbt-project/metrics>`_ will be added to the corresponding datasets.
 5. Every dashboard built on top of the dbt sources and/or models will be synchronized back to dbt as an `exposure <https://docs.getdbt.com/docs/building-a-dbt-project/exposures>`_.
 
 The ``--external-url-prefix`` should point to your dbt docs, so that the resources in the workspace can point to the source of truth where they are being managed. Similar to the native sync, the dbt sync also supports the ``--disallow-edits`` flag.
 
+By default, the CLI sync would create a new database on the destination workspace using below name structure:
+
+.. code-block:: python
+
+    f"{project_name}_{target_name}"
+
+If you want to sync data to an existing database connection on the workspace instead, you can specify the database connection name on the profiles YAML file. Add below structure under the ``<target-name>``:
+
+.. code-block:: yaml
+    
+    meta:
+      superset:
+        database_name: my DB name # <= specify the database connection/display name used on the workspace
+        
+Example:
+
+.. code-block:: yaml
+
+    jaffle_shop:
+      outputs:
+        dev:
+          meta:
+            superset:
+              database_name: Postgres - Production
+
+If  ``--import-db`` was passed and a database connection was found on the workspace, the operation would update the connection configuration with the dbt connection settings.
+
 If you're using dbt Cloud you can instead pass a job ID and a `service account access token <https://cloud.getdbt.com/#/accounts/72449/settings/service-tokens/new/>`_:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset sync dbt-cloud \
     > $TOKEN $JOB_ID \
     > --external-url-prefix=http://localhost:8080/
 
 The token only needs access to the "Metadata only" permission set for your project. You can see the job ID by going to the project URL in dbt Cloud and looking at the last ID in the URL. For example, if the URL is https://cloud.getdbt.com/#/accounts/12345/projects/567890/jobs/ the job ID is 567890.
 
-Before running the command you need to have a database already created in the Preset workspace, and the database should have the same name as the dbt Cloud database. You can run the command before creating the database to see what the name should be.
-
+When syncing from dbt Cloud, the database connection must already exist on the target workspace. The connection display name on the workspace must match the database name from dbt Cloud.
+              
 Selecting models
 ~~~~~~~~~~~~~~~~
 
 By default all the models will be synchronized to the workspace. The CLI supports a subset of the syntax used by the ``dbt`` command line to select which models should be synchronized. Models that should be synchronized can be specified via the ``--select`` flag:
 
 .. code-block:: bash
 
@@ -381,31 +440,61 @@
     % preset-cli --select my_model+ --exclude tag:test
 
 The command above synchronizes "my_model" and its children, as long as the models don't have the "test" tag.
 
 Exporting resources
 -------------------
 
-The CLI can also be used to export all resources (databases, datasets, charts, and dashboards) from a given Preset workspace (using ``preset-cli``) or Superset instance (using ``superset-cli``). This is useful for migrating resources between workspaces, from an existing Superset installation to Preset, or even from Preset to Superset (one of the advantages of Preset is no vendor lock in!).
+The CLI can also be used to export resources (databases, datasets, charts, and dashboards) from a given Preset workspace (using ``preset-cli``) or Superset instance (using ``superset-cli``). This is useful for migrating resources between workspaces, from an existing Superset installation to Preset, or even from Preset to Superset (one of the advantages of Preset is no vendor lock in!).
 
-The run the command on a self-hosted Superset instance:
+To export resources from a self-hosted Superset instance:
 
 .. code-block:: bash
 
     % superset-cli https://superset.example.org/ export /path/to/directory
 
 This will create a nice directory structure in ``/path/to/directory``, ready to be imported using the ``sync native`` command.
 
 To export resources from a Preset workspace:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset export /path/to/directory
 
+It's also possible to use the CLI to export specific resources:
+
+Use ``--asset-type`` to export all assets from a given type. Available options:
+
+- ``dashboard``
+- ``chart``
+- ``dataset``
+- ``database``
+
+For example, running below command would export all dashboards from this workspace (datasets, charts and DB connections wouldn't be included):
+
+.. code-block:: bash
+
+    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
+    > superset export /path/to/directory --asset-type=dashboard
+    
+Use ``--asset-ids`` to filter for specific assets. Available options:
+
+- ``dashboard-ids``
+- ``chart-ids``
+- ``dataset-ids``
+- ``database-ids``
+
+For example, running below command would export specified dashboards from this workspace (datasets, charts and DB connections would be included):
+
+.. code-block:: bash
+
+    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
+    > superset export /path/to/directory --dashboard-ids=9,10
+
 To import the exported resources into a Preset workspace:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset sync native /path/to/directory
 
@@ -436,18 +525,24 @@
     GROUP BY action
 
 So that when processed by ``preset-cli superset sync native`` the original Jinja2 is reconstructed correctly.
 
 Exporting users
 ~~~~~~~~~~~~~~~
 
-The ``preset-cli superset export-users`` command can be used to export a list of users. Currently there's no way to import this into a workspace, but work is in progress.
+The ``preset-cli superset export-users`` command can be used to export a list of users. These users can then be imported to Preset via the ``preset-cli import-users`` command.
+
+You can also export roles via ``preset-cli superset export-roles``, and import with ``import-roles``.
 
 Exporting RLS rules
 ~~~~~~~~~~~~~~~~~~~
 
 The ``preset-cli superset export-rls`` command can be used to export a list of RLS rules. Currently there's no way to import this into a workspace, but work is in progress.
 
 Exporting ownership
 ~~~~~~~~~~~~~~~~~~~
 
 The ``preset-cli superset export-ownership`` command generates a YAML file with information about ownership of different resources. The file maps resource UUIDs to user email address, and in the future will be used to recreate ownership on a different instance of Superset.
+
+Listing SCIM Groups
+~~~~~~~~~~~~~~~~~~~
+The ``preset-cli list-group-membership`` command prints all SCIM groups (including membership) associated with a Preset team. Instead of printing the results on the terminal (whcih can be useful for quick troubleshooting), it's possible to use ``--save-report=yaml`` or ``--save-report=csv`` to write results to a file. The file name would be ``{TeamSlug}__user_group_membership.{FileExtension}``.
```

### Comparing `preset-cli-0.1.1/README.rst` & `preset-cli-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: preset-cli
+Version: 0.2.0
+Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
+Home-page: https://github.com/preset-io/backend-sdk
+Author: Beto Dealmeida
+Author-email: beto@preset.io
+License: Other/Proprietary License
+Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Other/Proprietary License
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 ==========
 preset-cli
 ==========
 
     A CLI to interact with Preset workspaces.
 
 This tool is a command line interface (CLI) to interact with your Preset workspaces. Currently it can be used to sync resources (databases, datasets, charts, dashboards) from source control, either in native format or from a `dbt <https://www.getdbt.com/>`_ project. It can also be used to run SQL against any database in any workspace. In the future, the CLI will also allow you to manage your workspaces and users.
@@ -14,14 +35,20 @@
 .. code-block:: bash
 
     $ pip install -U setuptools setuptools_scm wheel  # for good measure
     $ pip install preset-cli
 
 Make sure you're using Python 3.8 or newer.
 
+You can also install from ``main``, if you need recent features:
+
+.. code-block:: bash
+
+     $ pip install "git+https://github.com/preset-io/backend-sdk.git"
+
 Authentication
 ==============
 
 The CLI requires an API key for authentication, composed of token and an associated secret. Both can be defined in your environment as ``PRESET_API_TOKEN`` and ``PRESET_API_SECRET``, respectively, or can be stored in a configuration file. To store the credentials in a configuration file simply run ``preset-cli auth``. This should open https://manage.app.preset.io/app/user in your browser so you can generate a new token, and it will prompt you for the token and its secret:
 
 .. code-block:: bash
 
@@ -103,20 +130,24 @@
 
 Commands
 ========
 
 The following commands are currently available:
 
 - ``preset-cli auth``: store authentication credentials.
+- ``preset-cli invite-users``: invite users to Preset.
+- ``preset-cli import-users``: automatically add users to Preset.
+- ``preset-cli list-group-membership``: List SCIM groups from a team and their memberships.
 - ``preset-cli superset sql``: run SQL interactively or programmatically against an analytical database.
-- ``preset-cli superset export-assets``: export resources (databases, datasets, charts, dashboards) into a directory as YAML files.
+- ``preset-cli superset export-assets`` (alternatively, ``preset-cli superset export``): export resources (databases, datasets, charts, dashboards) into a directory as YAML files.
 - ``preset-cli superset export-ownership``: export resource ownership (UUID -> email) into a YAML file.
 - ``preset-cli superset export-rls``: export RLS rules into a YAML file.
+- ``preset-cli superset export-roles``: export user roles into a YAML file.
 - ``preset-cli superset export-users``: export users (name, username, email, roles) into a YAML file.
-- ``preset-cli superset sync native``: synchronize the workspace from a directory of templated configuration files.
+- ``preset-cli superset sync native`` (alternatively, ``preset-cli superset import-assets``): synchronize the workspace from a directory of templated configuration files.
 - ``preset-cli superset sync dbt-core``: synchronize the workspace from a dbt Core project.
 - ``preset-cli superset sync dbt-cloud``: synchronize the workspace from a dbt Cloud project.
 
 All the ``superset`` sub-commands can also be executed against a standalone Superset instance, using the ``superset-cli`` command. This means that if you are running an instance of Superset at https://superset.example.org/ you can export its resources with the command:
 
 .. code-block:: bash
 
@@ -287,53 +318,119 @@
 .. code-block:: yaml
 
     slice_name: {{ functions.demo.hello_world() }}
     viz_type: big_number_total
     params:
       ...
 
+Disabling Jinja Templating
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Both the CLI and Superset support Jinja templating. To prevent the CLI from loading Superset Jinja syntax, the export operation automatically escapes Jinja syntax from YAML files. As a consequence, this query:
+
+.. code-block:: yaml
+
+    sql: 'SELECT action, count(*) as times
+        FROM logs
+        {% if filter_values(''action_type'')|length %}
+            WHERE action is null
+            {% for action in filter_values(''action_type'') %}
+                or action = ''{{ action }}''
+            {% endfor %}
+        {% endif %}
+        GROUP BY action'
+
+Becomes this:
+
+.. code-block:: yaml
+
+    sql: 'SELECT action, count(*) as times
+        FROM logs
+        {{ '{% if' }} filter_values(''action_type'')|length {{ '%}' }}
+            WHERE action is null
+            {{ '{% for' }} action in filter_values(''action_type'') {{ '%}' }}
+                or action = ''{{ '{{' }} action {{ '}}' }}''
+            {{ '{% endfor %}' }}
+        {{ '{% endif %}' }}
+        GROUP BY action'
+
+When performing the import, the CLI would load any templating syntax that isn't escaped, and remove escaping. However, this escaping syntax isn't compatible with UI imports. 
+To avoid issues when running migrations using both the CLI and the UI, you can use:
+
+- ``--disable-jinja-escaping`` flag with the ``export-assets`` command to disable the escaping (so that exported assets can be imported via the UI)
+- ``--disable-jinja-templating`` flag with the ``sync native`` command to disable jinja templating (so that assets exported via the UI can be imported via the CLI)
+
+Note that using these flags would remove the ability to dynamically modify the content through the CLI. 
+
 Synchronizing to and from dbt
 -----------------------------
 
 The CLI also allows you to synchronize models, and metrics from a `dbt <https://www.getdbt.com/>`_ project.
 
-If you're using dbt Core you can point the CLI to your compiled manifest and your profiles file, so that all the database is automatically created, together with all the models and metrics. The full command is:
+If you're using dbt Core you can point the CLI to your compiled manifest and your profiles file, so that the database is automatically created, together with all the models and metrics. The full command is:
 
 .. code-block:: bash
 
    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
    > superset sync dbt-core /path/to/dbt/my_project/target/manifest.json \
-   > --project=my_project --target=dev --profile=${HOME}/.dbt/profiles.yml \
+   > --project=my_project --target=dev --profiles=${HOME}/.dbt/profiles.yml \
    > --exposures=/path/to/dbt/my_project/models/exposures.yaml \
    > --import-db \
    > --external-url-prefix=http://localhost:8080/
 
 Running this command will:
 
 1. Read the dbt profile and create the ``$target`` database for the specified project in the Preset workspace.
 2. Every source in the project will be created as a dataset in the Preset workspace.
 3. Every model in the project will be created as a dataset in the Preset workspace.
 4. Any `metrics <https://docs.getdbt.com/docs/building-a-dbt-project/metrics>`_ will be added to the corresponding datasets.
 5. Every dashboard built on top of the dbt sources and/or models will be synchronized back to dbt as an `exposure <https://docs.getdbt.com/docs/building-a-dbt-project/exposures>`_.
 
 The ``--external-url-prefix`` should point to your dbt docs, so that the resources in the workspace can point to the source of truth where they are being managed. Similar to the native sync, the dbt sync also supports the ``--disallow-edits`` flag.
 
+By default, the CLI sync would create a new database on the destination workspace using below name structure:
+
+.. code-block:: python
+
+    f"{project_name}_{target_name}"
+
+If you want to sync data to an existing database connection on the workspace instead, you can specify the database connection name on the profiles YAML file. Add below structure under the ``<target-name>``:
+
+.. code-block:: yaml
+    
+    meta:
+      superset:
+        database_name: my DB name # <= specify the database connection/display name used on the workspace
+        
+Example:
+
+.. code-block:: yaml
+
+    jaffle_shop:
+      outputs:
+        dev:
+          meta:
+            superset:
+              database_name: Postgres - Production
+
+If  ``--import-db`` was passed and a database connection was found on the workspace, the operation would update the connection configuration with the dbt connection settings.
+
 If you're using dbt Cloud you can instead pass a job ID and a `service account access token <https://cloud.getdbt.com/#/accounts/72449/settings/service-tokens/new/>`_:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset sync dbt-cloud \
     > $TOKEN $JOB_ID \
     > --external-url-prefix=http://localhost:8080/
 
 The token only needs access to the "Metadata only" permission set for your project. You can see the job ID by going to the project URL in dbt Cloud and looking at the last ID in the URL. For example, if the URL is https://cloud.getdbt.com/#/accounts/12345/projects/567890/jobs/ the job ID is 567890.
 
-Before running the command you need to have a database already created in the Preset workspace, and the database should have the same name as the dbt Cloud database. You can run the command before creating the database to see what the name should be.
-
+When syncing from dbt Cloud, the database connection must already exist on the target workspace. The connection display name on the workspace must match the database name from dbt Cloud.
+              
 Selecting models
 ~~~~~~~~~~~~~~~~
 
 By default all the models will be synchronized to the workspace. The CLI supports a subset of the syntax used by the ``dbt`` command line to select which models should be synchronized. Models that should be synchronized can be specified via the ``--select`` flag:
 
 .. code-block:: bash
 
@@ -364,31 +461,61 @@
     % preset-cli --select my_model+ --exclude tag:test
 
 The command above synchronizes "my_model" and its children, as long as the models don't have the "test" tag.
 
 Exporting resources
 -------------------
 
-The CLI can also be used to export all resources (databases, datasets, charts, and dashboards) from a given Preset workspace (using ``preset-cli``) or Superset instance (using ``superset-cli``). This is useful for migrating resources between workspaces, from an existing Superset installation to Preset, or even from Preset to Superset (one of the advantages of Preset is no vendor lock in!).
+The CLI can also be used to export resources (databases, datasets, charts, and dashboards) from a given Preset workspace (using ``preset-cli``) or Superset instance (using ``superset-cli``). This is useful for migrating resources between workspaces, from an existing Superset installation to Preset, or even from Preset to Superset (one of the advantages of Preset is no vendor lock in!).
 
-The run the command on a self-hosted Superset instance:
+To export resources from a self-hosted Superset instance:
 
 .. code-block:: bash
 
     % superset-cli https://superset.example.org/ export /path/to/directory
 
 This will create a nice directory structure in ``/path/to/directory``, ready to be imported using the ``sync native`` command.
 
 To export resources from a Preset workspace:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset export /path/to/directory
 
+It's also possible to use the CLI to export specific resources:
+
+Use ``--asset-type`` to export all assets from a given type. Available options:
+
+- ``dashboard``
+- ``chart``
+- ``dataset``
+- ``database``
+
+For example, running below command would export all dashboards from this workspace (datasets, charts and DB connections wouldn't be included):
+
+.. code-block:: bash
+
+    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
+    > superset export /path/to/directory --asset-type=dashboard
+    
+Use ``--asset-ids`` to filter for specific assets. Available options:
+
+- ``dashboard-ids``
+- ``chart-ids``
+- ``dataset-ids``
+- ``database-ids``
+
+For example, running below command would export specified dashboards from this workspace (datasets, charts and DB connections would be included):
+
+.. code-block:: bash
+
+    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
+    > superset export /path/to/directory --dashboard-ids=9,10
+
 To import the exported resources into a Preset workspace:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset sync native /path/to/directory
 
@@ -419,18 +546,24 @@
     GROUP BY action
 
 So that when processed by ``preset-cli superset sync native`` the original Jinja2 is reconstructed correctly.
 
 Exporting users
 ~~~~~~~~~~~~~~~
 
-The ``preset-cli superset export-users`` command can be used to export a list of users. Currently there's no way to import this into a workspace, but work is in progress.
+The ``preset-cli superset export-users`` command can be used to export a list of users. These users can then be imported to Preset via the ``preset-cli import-users`` command.
+
+You can also export roles via ``preset-cli superset export-roles``, and import with ``import-roles``.
 
 Exporting RLS rules
 ~~~~~~~~~~~~~~~~~~~
 
 The ``preset-cli superset export-rls`` command can be used to export a list of RLS rules. Currently there's no way to import this into a workspace, but work is in progress.
 
 Exporting ownership
 ~~~~~~~~~~~~~~~~~~~
 
 The ``preset-cli superset export-ownership`` command generates a YAML file with information about ownership of different resources. The file maps resource UUIDs to user email address, and in the future will be used to recreate ownership on a different instance of Superset.
+
+Listing SCIM Groups
+~~~~~~~~~~~~~~~~~~~
+The ``preset-cli list-group-membership`` command prints all SCIM groups (including membership) associated with a Preset team. Instead of printing the results on the terminal (whcih can be useful for quick troubleshooting), it's possible to use ``--save-report=yaml`` or ``--save-report=csv`` to write results to a file. The file name would be ``{TeamSlug}__user_group_membership.{FileExtension}``.
```

### Comparing `preset-cli-0.1.1/dev-requirements.txt` & `preset-cli-0.2.0/dev-requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 #
 # This file is autogenerated by pip-compile with python 3.8
 # To update, run:
 #
 #    pip-compile --no-annotate dev-requirements.in
 #
 -e file:.
-aiohttp==3.8.1
+aiohttp==3.8.3
 aiosignal==1.2.0
 appdirs==1.4.4
+astroid==2.12.12
 async-timeout==4.0.2
 attrs==22.1.0
+backoff==2.2.1
 beautifulsoup4==4.11.1
 build==0.8.0
 certifi==2021.10.8
 cfgv==3.3.1
 charset-normalizer==2.0.12
 click==8.1.2
 codespell==2.1.0
 commonmark==0.9.1
 coverage[toml]==6.4.3
 cython==0.29.32
+dill==0.3.6
 distlib==0.3.5
 filelock==3.8.0
 freezegun==1.2.2
 frozenlist==1.3.1
-greenlet==1.1.2
+greenlet==1.1.3.post0
 identify==2.5.3
 idna==3.3
 iniconfig==1.1.1
+isort==5.10.1
 jinja2==3.1.2
+lazy-object-proxy==1.8.0
 markupsafe==2.1.1
 marshmallow==3.17.0
+mccabe==0.7.0
 multidict==6.0.2
 nodeenv==1.7.0
 numpy==1.23.1
 packaging==21.3
 pandas==1.4.3
 pep517==0.13.0
 pip-tools==6.8.0
@@ -42,36 +48,39 @@
 pluggy==1.0.0
 pre-commit==2.20.0
 prison==0.2.1
 prompt-toolkit==3.0.30
 py==1.11.0
 pyfakefs==4.6.3
 pygments==2.12.0
+pylint==2.15.5
 pyparsing==3.0.9
 pytest==7.1.2
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 python-dateutil==2.8.2
 python-graphql-client==0.4.3
 pytz==2022.2
 pyyaml==6.0
 requests==2.27.1
 requests-mock==1.9.3
 rich==12.5.1
 six==1.16.0
 soupsieve==2.3.2.post1
 sqlalchemy==1.4.40
-sqlparse==0.4.2
+sqlparse==0.4.3
 tabulate==0.8.10
 toml==0.10.2
 tomli==2.0.1
+tomlkit==0.11.6
 typing-extensions==4.3.0
 urllib3==1.26.9
 virtualenv==20.16.3
 wcwidth==0.2.5
 websockets==10.3
 wheel==0.37.1
+wrapt==1.14.1
 yarl==1.8.1
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `preset-cli-0.1.1/docs/Makefile` & `preset-cli-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/docs/conf.py` & `preset-cli-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/docs/images/export_dashboards.png` & `preset-cli-0.2.0/docs/images/export_dashboards.png`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/docs/index.rst` & `preset-cli-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/examples/exports/charts/Total_count_134.yaml` & `preset-cli-0.2.0/examples/exports/charts/Total_count_134.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/examples/exports/dashboards/White_label_test.yaml` & `preset-cli-0.2.0/examples/exports/dashboards/White_label_test.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/examples/exports/datasets/Google_Sheets/country_cnt.yaml` & `preset-cli-0.2.0/examples/exports/datasets/Google_Sheets/country_cnt.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/requirements.txt` & `preset-cli-0.2.0/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #
 # This file is autogenerated by pip-compile with python 3.8
 # To update, run:
 #
 #    pip-compile --no-annotate
 #
 -e file:.
-aiohttp==3.8.1
+aiohttp==3.8.3
 aiosignal==1.2.0
 appdirs==1.4.4
 async-timeout==4.0.2
 attrs==22.1.0
+backoff==2.2.1
 beautifulsoup4==4.11.1
 certifi==2021.10.8
 charset-normalizer==2.0.12
 click==8.1.2
 commonmark==0.9.1
 cython==0.29.28
 frozenlist==1.3.1
-greenlet==1.1.2
+greenlet==1.1.3.post0
 idna==3.3
 jinja2==3.1.1
 markupsafe==2.1.1
 marshmallow==3.17.0
 multidict==6.0.2
 numpy==1.22.3
 packaging==21.3
@@ -35,14 +36,14 @@
 pytz==2022.1
 pyyaml==6.0
 requests==2.27.1
 rich==12.3.0
 six==1.16.0
 soupsieve==2.3.2.post1
 sqlalchemy==1.4.35
-sqlparse==0.4.2
+sqlparse==0.4.3
 tabulate==0.8.9
 typing-extensions==4.2.0
 urllib3==1.26.9
 wcwidth==0.2.5
 websockets==10.3
 yarl==1.7.2
```

### Comparing `preset-cli-0.1.1/setup.cfg` & `preset-cli-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -3,51 +3,58 @@
 description = A CLI to interact with Preset (https://preset.io/) workspaces.
 author = Beto Dealmeida
 author_email = beto@preset.io
 license = Other/Proprietary License
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
-url = https://github.com/preset-io/preset-cli
+url = https://github.com/preset-io/backend-sdk
 project_urls = 
-	Documentation = https://github.com/preset-io/preset-cli/blob/master/README.rst
+	Documentation = https://github.com/preset-io/backend-sdk/blob/master/README.rst
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: Other/Proprietary License
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	Cython>=0.29.26
 	PyYAML>=6.0
 	appdirs>=1.4.4
+	backoff>=1.10.0
 	beautifulsoup4>=4.10.0
 	click>=8.0.3
 	jinja2>=3.0.3
 	marshmallow>=3.17.0
 	numpy>=1.21.5
 	pandas>=1.3.5
 	prison>=0.2.1
 	prompt-toolkit>=3.0.24
 	pygments>=2.11.2
 	python-graphql-client>=0.4.3
 	requests>=2.26.0
 	rich>=12.3.0
-	sqlalchemy>=1.4
-	sqlparse>=0.4.2
+	sqlalchemy>=1.4,<2
+	sqlparse>=0.4.3
 	tabulate>=0.8.9
 	typing-extensions>=4.0.1
 	yarl>=1.7.2
+	greenlet>=1.1.3  # required for Python 3.11
+	aiohttp>=3.8.3
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
@@ -58,14 +65,15 @@
 	pytest-cov
 	pytest-mock
 	pyfakefs
 	requests-mock
 	codespell
 	pre-commit
 	pip-tools>=6.6.0
+	pylint>=2.11.1
 
 [options.entry_points]
 console_scripts = 
 	preset-cli = preset_cli.cli.main:preset_cli
 	superset-cli = preset_cli.cli.superset.main:superset_cli
 
 [tool:pytest]
```

### Comparing `preset-cli-0.1.1/setup.py` & `preset-cli-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/src/preset_cli/api/clients/dbt.py` & `preset-cli-0.2.0/src/preset_cli/api/clients/dbt.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,36 @@
     - https://docs.getdbt.com/dbt-cloud/api-v2
     - https://docs.getdbt.com/docs/dbt-cloud/dbt-cloud-api/metadata/schema/metadata-schema-seeds
     - https://github.com/dbt-labs/dbt-cloud-openapi-spec/blob/master/openapi-v3.yaml
 """
 
 # pylint: disable=invalid-name, too-few-public-methods
 
+import logging
 from enum import Enum
-from typing import Any, Dict, List, Type, TypedDict
+from typing import Any, Dict, List, Optional, Type, TypedDict
 
 from marshmallow import INCLUDE, Schema, fields
 from python_graphql_client import GraphqlClient
 from yarl import URL
 
 from preset_cli import __version__
 from preset_cli.auth.main import Auth
 
+_logger = logging.getLogger(__name__)
+
 REST_ENDPOINT = URL("https://cloud.getdbt.com/")
 GRAPHQL_ENDPOINT = URL("https://metadata.cloud.getdbt.com/graphql")
 
 
 class PostelSchema(Schema):
     """
     Be liberal in what you accept, and conservative in what you send.
 
-    A schema that allows unknown fields. This way if they API returns new fields that
+    A schema that allows unknown fields. This way if the API returns new fields that
     the client is not expecting no errors will be thrown when validating the payload.
     """
 
     class Meta:
         """
         Allow unknown fields.
         """
@@ -527,14 +530,16 @@
     database = fields.String()
     schema = fields.String()
     description = fields.String()
     meta = fields.Raw()
     name = fields.String()
     unique_id = fields.String(data_key="uniqueId")
     tags = fields.List(fields.String())
+    columns = fields.Raw()
+    config = fields.Dict(fields.String(), fields.Raw(allow_none=True))
 
 
 class FilterSchema(PostelSchema):
     """
     Schema for a metric filter.
     """
 
@@ -553,14 +558,17 @@
     filters = fields.List(fields.Nested(FilterSchema))
     meta = fields.Raw()
     name = fields.String()
     label = fields.String()
     sql = fields.String()
     type = fields.String()
     unique_id = fields.String(data_key="uniqueId")
+    # dbt >= 1.3
+    calculation_method = fields.String()
+    expression = fields.String()
 
 
 class DataResponse(TypedDict):
     """
     Type for the GraphQL response.
     """
 
@@ -570,78 +578,85 @@
 class DBTClient:  # pylint: disable=too-few-public-methods
 
     """
     A client for the dbt API.
     """
 
     def __init__(self, auth: Auth):
-        self.auth = auth
-        self.auth.headers.update(
-            {
-                "User-Agent": "Preset CLI",
-                "X-Client-Version": __version__,
-            },
-        )
         self.graphql_client = GraphqlClient(endpoint=GRAPHQL_ENDPOINT)
         self.baseurl = REST_ENDPOINT
 
+        self.session = auth.session
+        self.session.headers.update(auth.get_headers())
+        self.session.headers["User-Agent"] = "Preset CLI"
+        self.session.headers["X-Client-Version"] = __version__
+        self.session.headers["X-dbt-partner-source"] = "preset"
+
     def execute(self, query: str, **variables: Any) -> DataResponse:
         """
         Run a GraphQL query.
         """
         return self.graphql_client.execute(
             query=query,
             variables=variables,
-            headers=self.auth.get_headers(),
+            headers=self.session.headers,
         )
 
     def get_accounts(self) -> List[AccountSchema]:
         """
         List all accounts.
         """
-        session = self.auth.get_session()
-        headers = self.auth.get_headers()
-        response = session.get(self.baseurl / "api/v2/accounts/", headers=headers)
+        url = self.baseurl / "api/v2/accounts/"
+        _logger.debug("GET %s", url)
+        response = self.session.get(url)
 
         payload = response.json()
 
+        if not response.ok:
+            raise Exception(payload["status"]["user_message"])
+
         account_schema = AccountSchema()
         return [account_schema.load(row) for row in payload["data"]]
 
     def get_projects(self, account_id: int) -> List[ProjectSchema]:
         """
         List all projects.
         """
-        session = self.auth.get_session()
-        headers = self.auth.get_headers()
-        response = session.get(
-            self.baseurl / "api/v2/accounts" / str(account_id) / "projects/",
-            headers=headers,
-        )
+        url = self.baseurl / "api/v2/accounts" / str(account_id) / "projects/"
+        _logger.debug("GET %s", url)
+        response = self.session.get(url)
 
         payload = response.json()
 
+        if not response.ok:
+            raise Exception(payload["status"]["user_message"])
+
         project_schema = ProjectSchema()
         projects = [project_schema.load(project) for project in payload["data"]]
 
         return projects
 
-    def get_jobs(self, account_id: int) -> List[JobSchema]:
-        """
-        List all jobs.
-        """
-        session = self.auth.get_session()
-        headers = self.auth.get_headers()
-        response = session.get(
-            self.baseurl / "api/v2/accounts" / str(account_id) / "jobs/",
-            headers=headers,
-        )
+    def get_jobs(
+        self,
+        account_id: int,
+        project_id: Optional[int] = None,
+    ) -> List[JobSchema]:
+        """
+        List all jobs, optionally for a project.
+        """
+        url = self.baseurl / "api/v2/accounts" / str(account_id) / "jobs/"
+        params = {"project_id": project_id} if project_id is not None else {}
+        _logger.debug("GET %s", url % params)
+        response = self.session.get(url, params=params)
 
         payload = response.json()
 
+        if not response.ok:
+            raise Exception(payload["status"]["user_message"])
+
         job_schema = JobSchema()
         jobs = [job_schema.load(job) for job in payload["data"]]
 
         return jobs
 
     def get_models(self, job_id: int) -> List[ModelSchema]:
         """
@@ -655,14 +670,18 @@
                     childrenL1
                     name
                     database
                     schema
                     description
                     meta
                     tags
+                    columns {
+                        name
+                        description
+                    }
                 }
             }
         """
         payload = self.execute(query, jobId=job_id)
 
         model_schema = ModelSchema()
         models = [model_schema.load(model) for model in payload["data"]["models"]]
```

### Comparing `preset-cli-0.1.1/src/preset_cli/auth/jwt.py` & `preset-cli-0.2.0/src/preset_cli/auth/jwt.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import yaml
 
 from preset_cli.auth.lib import get_access_token, get_credentials_path
 from preset_cli.auth.token import TokenAuth
 
 
-class JWTAuth(TokenAuth):  # pylint: disable=too-few-public-methods
+class JWTAuth(TokenAuth):  # pylint: disable=too-few-public-methods, abstract-method
     """
     Auth via JWT.
     """
 
     @classmethod
     def from_stored_credentials(cls) -> "JWTAuth":
         """
```

### Comparing `preset-cli-0.1.1/src/preset_cli/auth/lib.py` & `preset-cli-0.2.0/src/preset_cli/auth/lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,20 @@
     """
     Fetch the JWT access token.
     """
     if isinstance(baseurl, str):
         baseurl = URL(baseurl)
 
     response = requests.post(
-        baseurl / "api/v1/auth/",
+        baseurl / "v1/auth/",
         json={"name": api_token, "secret": api_secret},
         headers={"Content-Type": "application/json"},
+        timeout=60,
     )
+    response.raise_for_status()
     payload = response.json()
     return payload["payload"]["access_token"]
 
 
 def get_credentials_path() -> Path:
     """
     Return the system-dependent location of the credentials.
```

### Comparing `preset-cli-0.1.1/src/preset_cli/cli/superset/import_.py` & `preset-cli-0.2.0/src/preset_cli/cli/superset/import_.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,35 @@
             client.import_rls(rls)
 
 
 @click.command()
 @click.argument(
     "path",
     type=click.Path(resolve_path=True),
+    default="roles.yaml",
+)
+@click.pass_context
+def import_roles(ctx: click.core.Context, path: str) -> None:
+    """
+    Import roles from a YAML file.
+    """
+    auth = ctx.obj["AUTH"]
+    url = URL(ctx.obj["INSTANCE"])
+    client = SupersetClient(url, auth)
+
+    with open(path, encoding="utf-8") as input_:
+        config = yaml.load(input_, Loader=yaml.SafeLoader)
+        for role in config:
+            client.import_role(role)
+
+
+@click.command()
+@click.argument(
+    "path",
+    type=click.Path(resolve_path=True),
     default="ownership.yaml",
 )
 @click.pass_context
 def import_ownership(ctx: click.core.Context, path: str) -> None:
     """
     Import resource ownership from a YAML file.
     """
```

### Comparing `preset-cli-0.1.1/src/preset_cli/cli/superset/main.py` & `preset-cli-0.2.0/src/preset_cli/cli/superset/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,82 @@
 """
 Main entry point for Superset commands.
 """
-from typing import Any
+from typing import Any, Optional
 
 import click
 from yarl import URL
 
-from preset_cli.auth.main import UsernamePasswordAuth
+from preset_cli.auth.jwt import JWTAuth
+from preset_cli.auth.password import UsernamePasswordAuth
 from preset_cli.cli.superset.export import (
     export_assets,
     export_ownership,
     export_rls,
+    export_roles,
     export_users,
 )
-from preset_cli.cli.superset.import_ import import_ownership, import_rls
+from preset_cli.cli.superset.import_ import import_ownership, import_rls, import_roles
 from preset_cli.cli.superset.sql import sql
 from preset_cli.cli.superset.sync.main import sync
 from preset_cli.cli.superset.sync.native.command import native
+from preset_cli.lib import setup_logging
 
 
 @click.group()
 @click.argument("instance")
+@click.option("--jwt-token", default=None, help="JWT token")
 @click.option("-u", "--username", default="admin", help="Username")
 @click.option(
     "-p",
     "--password",
     prompt=True,
     prompt_required=False,
     default="admin",
     hide_input=True,
     help="Password (leave empty for prompt)",
 )
+@click.option("--loglevel", default="INFO")
+@click.version_option()
 @click.pass_context
-def superset_cli(
+def superset_cli(  # pylint: disable=too-many-arguments
     ctx: click.core.Context,
     instance: str,
-    username: str = "admin",
-    password: str = "admin",
+    jwt_token: Optional[str],
+    username: str,
+    password: str,
+    loglevel: str,
 ):
     """
     An Apache Superset CLI.
     """
+    setup_logging(loglevel)
+
     ctx.ensure_object(dict)
 
     ctx.obj["INSTANCE"] = instance
 
     # allow a custom authenticator to be passed via the context
     if "AUTH" not in ctx.obj:
-        ctx.obj["AUTH"] = UsernamePasswordAuth(URL(instance), username, password)
+        if jwt_token:
+            ctx.obj["AUTH"] = JWTAuth(jwt_token)
+        else:
+            ctx.obj["AUTH"] = UsernamePasswordAuth(URL(instance), username, password)
 
 
 superset_cli.add_command(sql)
 superset_cli.add_command(sync)
 superset_cli.add_command(export_assets)
 superset_cli.add_command(export_assets, name="export")  # for backwards compatibility
 superset_cli.add_command(export_users)
 superset_cli.add_command(export_rls)
+superset_cli.add_command(export_roles)
 superset_cli.add_command(export_ownership)
 superset_cli.add_command(import_rls)
+superset_cli.add_command(import_roles)
 superset_cli.add_command(import_ownership)
 superset_cli.add_command(native, name="import-assets")
 
 
 @click.group()
 @click.pass_context
 def superset(ctx: click.core.Context) -> None:
```

### Comparing `preset-cli-0.1.1/src/preset_cli/cli/superset/sql.py` & `preset-cli-0.2.0/src/preset_cli/cli/superset/sql.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/databases.py` & `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/databases.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,94 @@
 """
 Sync dbt database to Superset.
 """
 
 import logging
 from pathlib import Path
-from typing import Any
+from typing import Any, Optional
 
 from yarl import URL
 
 from preset_cli.api.clients.superset import SupersetClient
 from preset_cli.cli.superset.sync.dbt.lib import build_sqlalchemy_params, load_profiles
 from preset_cli.exceptions import DatabaseNotFoundError
 
 _logger = logging.getLogger(__name__)
 
 
 def sync_database(  # pylint: disable=too-many-locals, too-many-arguments
     client: SupersetClient,
     profiles_path: Path,
     project_name: str,
-    target_name: str,
+    profile_name: str,
+    target_name: Optional[str],
     import_db: bool,
     disallow_edits: bool,  # pylint: disable=unused-argument
     external_url_prefix: str,
 ) -> Any:
     """
     Read target database from a dbt profiles.yml and sync to Superset.
     """
     base_url = URL(external_url_prefix) if external_url_prefix else None
 
-    profiles = load_profiles(profiles_path, project_name, target_name)
-    project = profiles[project_name]
+    profiles = load_profiles(profiles_path, project_name, profile_name, target_name)
+    project = profiles[profile_name]
     outputs = project["outputs"]
+    if target_name is None:
+        target_name = project["target"]
     target = outputs[target_name]
 
     # read additional metadata that should be applied to the DB
     meta = target.get("meta", {}).get("superset", {})
 
-    if "connection_params" in meta:
-        connection_params = meta.pop("connection_params")
-    else:
-        connection_params = build_sqlalchemy_params(target)
-
     database_name = meta.pop("database_name", f"{project_name}_{target_name}")
     databases = client.get_databases(database_name=database_name)
     if len(databases) > 1:
         raise Exception("More than one database with the same name found")
 
     if base_url and "external_url" not in meta:
         meta["external_url"] = str(base_url.with_fragment("!/overview"))
 
-    if databases:
-        _logger.info("Found an existing database, updating it")
+    if import_db:
+        connection_params = meta.pop(
+            "connection_params",
+            build_sqlalchemy_params(target),
+        )
+
+        if databases:
+            _logger.info("Found an existing database connection, updating it")
+            database = databases[0]
+            meta.pop("uuid", None)
+
+            database = client.update_database(
+                database_id=database["id"],
+                database_name=database_name,
+                is_managed_externally=disallow_edits,
+                masked_encrypted_extra=connection_params.get("encrypted_extra"),
+                sqlalchemy_uri=connection_params["sqlalchemy_uri"],
+                **meta,
+            )
+
+        else:
+            _logger.info("No database connection found, creating it")
+
+            database = client.create_database(
+                database_name=database_name,
+                is_managed_externally=disallow_edits,
+                masked_encrypted_extra=connection_params.get("encrypted_extra"),
+                **connection_params,
+                **meta,
+            )
+
+        database["sqlalchemy_uri"] = connection_params["sqlalchemy_uri"]
+
+    elif databases:
+        _logger.info("Found an existing database connection, using it")
         database = databases[0]
+        database["sqlalchemy_uri"] = client.get_database(database["id"])[
+            "sqlalchemy_uri"
+        ]
 
-        database = client.update_database(
-            database_id=database["id"],
-            database_name=database_name,
-            is_managed_externally=disallow_edits,
-            masked_encrypted_extra=connection_params.get("encrypted_extra"),
-            sqlalchemy_uri=connection_params["sqlalchemy_uri"],
-            **meta,
-        )
-    elif not import_db:
-        raise DatabaseNotFoundError()
     else:
-        _logger.info("No database found, creating it")
-        database = client.create_database(
-            database_name=database_name,
-            is_managed_externally=disallow_edits,
-            **connection_params,
-            **meta,
-        )
+        raise DatabaseNotFoundError()
 
     return database
```

### Comparing `preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/exposures.py` & `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/exposures.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,123 +1,149 @@
 """
 Sync Superset dashboards as dbt exposures.
 """
 
 import json
 from pathlib import Path
-from typing import Any, List
+from typing import Any, Dict, List, NamedTuple, Optional
 
 import yaml
 
 from preset_cli.api.clients.superset import SupersetClient
 
 # XXX: DashboardResponseType and DatasetResponseType
 
 
-def get_chart_depends_on(client: SupersetClient, chart: Any) -> List[str]:
+class ModelKey(NamedTuple):
+    """
+    Model key, so they can be mapped from datasets.
+    """
+
+    schema: Optional[str]
+    table: str
+
+
+def get_chart_depends_on(
+    client: SupersetClient,
+    chart: Any,
+    model_map: Dict[ModelKey, str],
+) -> List[str]:
     """
     Get all the dbt dependencies for a given chart.
     """
 
     query_context = json.loads(chart["query_context"])
     dataset_id = query_context["datasource"]["id"]
     dataset = client.get_dataset(dataset_id)
-    extra = json.loads(dataset["result"]["extra"] or "{}")
+    extra = json.loads(dataset["extra"] or "{}")
     if "depends_on" in extra:
         return [extra["depends_on"]]
 
+    key = ModelKey(dataset["schema"], dataset["table_name"])
+    if dataset["datasource_type"] == "table" and key in model_map:
+        return [model_map[key]]
+
     return []
 
 
-def get_dashboard_depends_on(client: SupersetClient, dashboard: Any) -> List[str]:
+def get_dashboard_depends_on(
+    client: SupersetClient,
+    dashboard: Any,
+    model_map: Dict[ModelKey, str],
+) -> List[str]:
     """
     Get all the dbt dependencies for a given dashboard.
     """
 
     url = client.baseurl / "api/v1/dashboard" / str(dashboard["id"]) / "datasets"
 
-    session = client.auth.get_session()
+    session = client.auth.session
     headers = client.auth.get_headers()
     response = session.get(url, headers=headers)
     response.raise_for_status()
 
     payload = response.json()
 
     depends_on = []
     for dataset in payload["result"]:
         full_dataset = client.get_dataset(int(dataset["id"]))
         try:
-            extra = json.loads(full_dataset["result"]["extra"] or "{}")
+            extra = json.loads(full_dataset["extra"] or "{}")
         except json.decoder.JSONDecodeError:
             extra = {}
+
+        key = ModelKey(full_dataset["schema"], full_dataset["table_name"])
         if "depends_on" in extra:
             depends_on.append(extra["depends_on"])
+        elif full_dataset["datasource_type"] == "table" and key in model_map:
+            depends_on.append(model_map[key])
 
     return depends_on
 
 
 def sync_exposures(  # pylint: disable=too-many-locals
     client: SupersetClient,
     exposures_path: Path,
     datasets: List[Any],
+    model_map: Dict[ModelKey, str],
 ) -> None:
     """
     Write dashboards back to dbt as exposures.
     """
     exposures = []
     charts_ids = set()
     dashboards_ids = set()
 
     for dataset in datasets:
         url = client.baseurl / "api/v1/dataset" / str(dataset["id"]) / "related_objects"
 
-        session = client.auth.get_session()
+        session = client.auth.session
         headers = client.auth.get_headers()
         response = session.get(url, headers=headers)
         response.raise_for_status()
 
         payload = response.json()
         for chart in payload["charts"]["result"]:
             charts_ids.add(chart["id"])
         for dashboard in payload["dashboards"]["result"]:
             dashboards_ids.add(dashboard["id"])
 
     for chart_id in charts_ids:
-        chart = client.get_chart(chart_id)["result"]
+        chart = client.get_chart(chart_id)
         first_owner = chart["owners"][0]
         exposure = {
             "name": chart["slice_name"] + " [chart]",
             "type": "analysis",
             "maturity": "high" if chart["certified_by"] else "low",
             "url": str(
                 client.baseurl
                 / "superset/explore/"
                 % {"form_data": json.dumps({"slice_id": chart_id})},
             ),
             "description": chart["description"] or "",
-            "depends_on": get_chart_depends_on(client, chart),
+            "depends_on": get_chart_depends_on(client, chart, model_map),
             "owner": {
                 "name": first_owner["first_name"] + " " + first_owner["last_name"],
                 "email": first_owner.get("email", "unknown"),
             },
         }
         exposures.append(exposure)
 
     for dashboard_id in dashboards_ids:
-        dashboard = client.get_dashboard(dashboard_id)["result"]
+        dashboard = client.get_dashboard(dashboard_id)
         first_owner = dashboard["owners"][0]
         exposure = {
             "name": dashboard["dashboard_title"] + " [dashboard]",
             "type": "dashboard",
             "maturity": "high"
             if dashboard["published"] or dashboard["certified_by"]
             else "low",
             "url": str(client.baseurl / dashboard["url"].lstrip("/")),
             "description": "",
-            "depends_on": get_dashboard_depends_on(client, dashboard),
+            "depends_on": get_dashboard_depends_on(client, dashboard, model_map),
             "owner": {
                 "name": first_owner["first_name"] + " " + first_owner["last_name"],
                 "email": first_owner.get("email", "unknown"),
             },
         }
         exposures.append(exposure)
```

### Comparing `preset-cli-0.1.1/src/preset_cli/cli/superset/sync/dbt/lib.py` & `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
 def build_sqlalchemy_params(target: Dict[str, Any]) -> Dict[str, Any]:
     """
     Build the SQLAlchemy URI for a given target.
     """
     type_ = target.get("type")
 
-    if type_ in {"postgres", "redshift"}:
+    if type_ == "postgres":
         return build_postgres_sqlalchemy_params(target)
+    if type_ == "redshift":
+        return build_redshift_sqlalchemy_params(target)
     if type_ == "bigquery":
         return build_bigquery_sqlalchemy_params(target)
     if type_ == "snowflake":
         return build_snowflake_sqlalchemy_params(target)
 
     raise NotImplementedError(
         f"Unable to build a SQLAlchemy URI for a target of type {type_}. Please file an "
@@ -65,14 +67,44 @@
                 database=dbname,
                 query=query,
             ),
         ),
     }
 
 
+def build_redshift_sqlalchemy_params(target: Dict[str, Any]) -> Dict[str, Any]:
+    """
+    Build the SQLAlchemy URI for a Redshift target.
+    """
+    if "search_path" in target:
+        _logger.warning("Specifying a search path is not supported in Apache Superset")
+
+    username = target["user"]
+    password = target.get("password") or target.get("pass")
+    host = target["host"]
+    port = target["port"]
+    dbname = target["dbname"]
+
+    query = {"sslmode": target["sslmode"]} if "sslmode" in target else None
+
+    return {
+        "sqlalchemy_uri": str(
+            URL(
+                drivername="redshift+psycopg2",
+                username=username,
+                password=password,
+                host=host,
+                port=port,
+                database=dbname,
+                query=query,
+            ),
+        ),
+    }
+
+
 def build_bigquery_sqlalchemy_params(target: Dict[str, Any]) -> Dict[str, Any]:
     """
     Build the SQLAlchemy URI for a BigQuery target.
 
     Currently supports only configuration via ``keyfile``.
     """
     parameters: Dict[str, Any] = {}
@@ -111,32 +143,64 @@
 
 
 def build_snowflake_sqlalchemy_params(target: Dict[str, Any]) -> Dict[str, Any]:
     """
     Build the SQLAlchemy URI for a Snowflake target.
     """
     username = target["user"]
-    password = target["password"] or None
+    password = target.get("password", "") or None
     database = target["database"]
     host = target["account"]
     query = {"role": target["role"], "warehouse": target["warehouse"]}
 
-    return {
+    parameters = {
         "sqlalchemy_uri": str(
             URL(
                 drivername="snowflake",
                 username=username,
                 password=password,
                 host=host,
                 database=database,
                 query=query,
             ),
         ),
     }
 
+    authenticator = target.get("authenticator")
+    if authenticator:
+        if authenticator == "externalbrowser":
+            raise NotImplementedError("SSO not supported")
+        if authenticator.startswith("http"):
+            raise NotImplementedError("SSO not supported")
+        parameters["extra"] = json.dumps(
+            {
+                "engine_params": {
+                    "connect_args": {
+                        "passcode": authenticator,
+                    },
+                },
+            },
+        )
+
+    if "private_key_path" in target:
+        with open(target["private_key_path"], encoding="utf-8") as input_:
+            pk_body = input_.read()
+
+        parameters["encrypted_extra"] = json.dumps(
+            {
+                "auth_method": "keypair",
+                "auth_params": {
+                    "privatekey_body": pk_body,
+                    "privatekey_pass": target.get("private_key_passphrase", ""),
+                },
+            },
+        )
+
+    return parameters
+
 
 def env_var(var: str, default: Optional[str] = None) -> str:
     """
     Simplified version of dbt's ``env_var``.
 
     We need this to load the profile with secrets.
     """
@@ -163,38 +227,46 @@
     profile_name: str
     name: str
     schema: str
     type: str
     threads: int
 
 
-def load_profiles(path: Path, project_name: str, target_name: str) -> Dict[str, Any]:
+def load_profiles(
+    path: Path,
+    project_name: str,
+    profile_name: str,
+    target_name: Optional[str],
+) -> Dict[str, Any]:
     """
     Load the file and apply Jinja2 templating.
     """
     with open(path, encoding="utf-8") as input_:
         profiles = yaml.load(input_, Loader=yaml.SafeLoader)
 
-    if project_name not in profiles:
-        raise Exception(f"Project {project_name} not found in {path}")
-    project = profiles[project_name]
+    if profile_name not in profiles:
+        raise Exception(f"Project {profile_name} not found in {path}")
+    project = profiles[profile_name]
     outputs = project["outputs"]
+    if target_name is None:
+        target_name = project["target"]
     if target_name not in outputs:
         raise Exception(f"Target {target_name} not found in the outputs of {path}")
     target = outputs[target_name]
 
     env = Environment()
     env.filters["as_bool"] = bool
     env.filters["as_native"] = ast.literal_eval
     env.filters["as_number"] = as_number
     env.filters["as_text"] = str
 
     context = {
         "env_var": env_var,
         "project_name": project_name,
+        "profile_name": profile_name,
         "target": target,
     }
 
     def apply_templating(config: Any) -> Any:
         """
         Apply Jinja2 templating to dictionary values recursively.
         """
@@ -221,14 +293,22 @@
     See https://docs.getdbt.com/reference/node-selection/syntax.
     """
     # match by tag
     if condition.startswith("tag:"):
         tag = condition.split(":", 1)[1]
         return [model for model in models if tag in model["tags"]]
 
+    if condition.startswith("config"):
+        filtered_models = []
+        config_key, config_value = re.split(r"[.:]", condition)[1:]
+        for model in models:
+            if model.get("config", {}).get(config_key) == config_value:
+                filtered_models.append(model)
+        return filtered_models
+
     # simple match by name
     model_names = {model["name"]: model for model in models}
     if condition in model_names:
         return [model_names[condition]]
 
     # plus and n-plus operators
     if "+" in condition:
@@ -334,32 +414,34 @@
     models: List[ModelSchema],
     select: Tuple[str, ...],
     exclude: Tuple[str, ...],
 ) -> List[ModelSchema]:
     """
     Apply dbt node selection (https://docs.getdbt.com/reference/node-selection/syntax).
     """
-    if not select:
-        return models
-
     model_ids = {model["unique_id"]: model for model in models}
 
-    selected: Dict[str, ModelSchema] = {}
-    for selection in select:
-        ids = set.intersection(
-            *[
-                {model["unique_id"] for model in filter_models(models, condition)}
-                for condition in selection.split(",")
-            ]
-        )
-        selected.update({id_: model_ids[id_] for id_ in ids})
+    selected: Dict[str, ModelSchema]
+    if not select:
+        selected = {model["unique_id"]: model for model in models}
+    else:
+        selected = {}
+        for selection in select:
+            ids = set.intersection(
+                *[
+                    {model["unique_id"] for model in filter_models(models, condition)}
+                    for condition in selection.split(",")
+                ]
+            )
+            selected.update({id_: model_ids[id_] for id_ in ids})
 
     for selection in exclude:
         for id_ in set.intersection(
             *[
                 {model["unique_id"] for model in filter_models(models, condition)}
                 for condition in selection.split(",")
             ]
         ):
-            del selected[id_]
+            if id_ in selected:
+                del selected[id_]
 
     return list(selected.values())
```

### Comparing `preset-cli-0.1.1/src/preset_cli/exceptions.py` & `preset-cli-0.2.0/src/preset_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/src/preset_cli/lib.py` & `preset-cli-0.2.0/src/preset_cli/lib.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Basic helper functions.
 """
 
 import json
 import logging
 from pathlib import Path
-from typing import Any, Dict, List, cast
+from typing import Any, Dict, List, Optional, cast
 
+import click
 from requests import Response
 from rich.logging import RichHandler
 
 from preset_cli.exceptions import ErrorLevel, ErrorPayload, SupersetError
 
 _logger = logging.getLogger(__name__)
 
@@ -92,7 +93,32 @@
                 "error_type": "UNKNOWN_ERROR",
                 "level": ErrorLevel.ERROR,
             },
         ]
 
     _logger.error(message)
     raise SupersetError(errors=errors)
+
+
+def split_comma(  # pylint: disable=unused-argument
+    ctx: click.core.Context,
+    param: str,
+    value: Optional[str],
+) -> List[str]:
+    """
+    Split CLI option into multiple values.
+    """
+    if value is None:
+        return []
+
+    return [option.strip() for option in value.split(",")]
+
+
+def dict_merge(base: Dict[Any, Any], overrides: Dict[Any, Any]) -> None:
+    """
+    Recursive dict merge.
+    """
+    for k in overrides:  # pylint: disable=invalid-name
+        if k in base and isinstance(base[k], dict) and isinstance(overrides[k], dict):
+            dict_merge(base[k], overrides[k])
+        else:
+            base[k] = overrides[k]
```

### Comparing `preset-cli-0.1.1/src/preset_cli.egg-info/PKG-INFO` & `preset-cli-0.2.0/src/preset_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
-Home-page: https://github.com/preset-io/preset-cli
+Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
-Project-URL: Documentation, https://github.com/preset-io/preset-cli/blob/master/README.rst
+Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Other/Proprietary License
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 ==========
 preset-cli
@@ -31,14 +35,20 @@
 .. code-block:: bash
 
     $ pip install -U setuptools setuptools_scm wheel  # for good measure
     $ pip install preset-cli
 
 Make sure you're using Python 3.8 or newer.
 
+You can also install from ``main``, if you need recent features:
+
+.. code-block:: bash
+
+     $ pip install "git+https://github.com/preset-io/backend-sdk.git"
+
 Authentication
 ==============
 
 The CLI requires an API key for authentication, composed of token and an associated secret. Both can be defined in your environment as ``PRESET_API_TOKEN`` and ``PRESET_API_SECRET``, respectively, or can be stored in a configuration file. To store the credentials in a configuration file simply run ``preset-cli auth``. This should open https://manage.app.preset.io/app/user in your browser so you can generate a new token, and it will prompt you for the token and its secret:
 
 .. code-block:: bash
 
@@ -120,20 +130,24 @@
 
 Commands
 ========
 
 The following commands are currently available:
 
 - ``preset-cli auth``: store authentication credentials.
+- ``preset-cli invite-users``: invite users to Preset.
+- ``preset-cli import-users``: automatically add users to Preset.
+- ``preset-cli list-group-membership``: List SCIM groups from a team and their memberships.
 - ``preset-cli superset sql``: run SQL interactively or programmatically against an analytical database.
-- ``preset-cli superset export-assets``: export resources (databases, datasets, charts, dashboards) into a directory as YAML files.
+- ``preset-cli superset export-assets`` (alternatively, ``preset-cli superset export``): export resources (databases, datasets, charts, dashboards) into a directory as YAML files.
 - ``preset-cli superset export-ownership``: export resource ownership (UUID -> email) into a YAML file.
 - ``preset-cli superset export-rls``: export RLS rules into a YAML file.
+- ``preset-cli superset export-roles``: export user roles into a YAML file.
 - ``preset-cli superset export-users``: export users (name, username, email, roles) into a YAML file.
-- ``preset-cli superset sync native``: synchronize the workspace from a directory of templated configuration files.
+- ``preset-cli superset sync native`` (alternatively, ``preset-cli superset import-assets``): synchronize the workspace from a directory of templated configuration files.
 - ``preset-cli superset sync dbt-core``: synchronize the workspace from a dbt Core project.
 - ``preset-cli superset sync dbt-cloud``: synchronize the workspace from a dbt Cloud project.
 
 All the ``superset`` sub-commands can also be executed against a standalone Superset instance, using the ``superset-cli`` command. This means that if you are running an instance of Superset at https://superset.example.org/ you can export its resources with the command:
 
 .. code-block:: bash
 
@@ -304,53 +318,119 @@
 .. code-block:: yaml
 
     slice_name: {{ functions.demo.hello_world() }}
     viz_type: big_number_total
     params:
       ...
 
+Disabling Jinja Templating
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Both the CLI and Superset support Jinja templating. To prevent the CLI from loading Superset Jinja syntax, the export operation automatically escapes Jinja syntax from YAML files. As a consequence, this query:
+
+.. code-block:: yaml
+
+    sql: 'SELECT action, count(*) as times
+        FROM logs
+        {% if filter_values(''action_type'')|length %}
+            WHERE action is null
+            {% for action in filter_values(''action_type'') %}
+                or action = ''{{ action }}''
+            {% endfor %}
+        {% endif %}
+        GROUP BY action'
+
+Becomes this:
+
+.. code-block:: yaml
+
+    sql: 'SELECT action, count(*) as times
+        FROM logs
+        {{ '{% if' }} filter_values(''action_type'')|length {{ '%}' }}
+            WHERE action is null
+            {{ '{% for' }} action in filter_values(''action_type'') {{ '%}' }}
+                or action = ''{{ '{{' }} action {{ '}}' }}''
+            {{ '{% endfor %}' }}
+        {{ '{% endif %}' }}
+        GROUP BY action'
+
+When performing the import, the CLI would load any templating syntax that isn't escaped, and remove escaping. However, this escaping syntax isn't compatible with UI imports. 
+To avoid issues when running migrations using both the CLI and the UI, you can use:
+
+- ``--disable-jinja-escaping`` flag with the ``export-assets`` command to disable the escaping (so that exported assets can be imported via the UI)
+- ``--disable-jinja-templating`` flag with the ``sync native`` command to disable jinja templating (so that assets exported via the UI can be imported via the CLI)
+
+Note that using these flags would remove the ability to dynamically modify the content through the CLI. 
+
 Synchronizing to and from dbt
 -----------------------------
 
 The CLI also allows you to synchronize models, and metrics from a `dbt <https://www.getdbt.com/>`_ project.
 
-If you're using dbt Core you can point the CLI to your compiled manifest and your profiles file, so that all the database is automatically created, together with all the models and metrics. The full command is:
+If you're using dbt Core you can point the CLI to your compiled manifest and your profiles file, so that the database is automatically created, together with all the models and metrics. The full command is:
 
 .. code-block:: bash
 
    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
    > superset sync dbt-core /path/to/dbt/my_project/target/manifest.json \
-   > --project=my_project --target=dev --profile=${HOME}/.dbt/profiles.yml \
+   > --project=my_project --target=dev --profiles=${HOME}/.dbt/profiles.yml \
    > --exposures=/path/to/dbt/my_project/models/exposures.yaml \
    > --import-db \
    > --external-url-prefix=http://localhost:8080/
 
 Running this command will:
 
 1. Read the dbt profile and create the ``$target`` database for the specified project in the Preset workspace.
 2. Every source in the project will be created as a dataset in the Preset workspace.
 3. Every model in the project will be created as a dataset in the Preset workspace.
 4. Any `metrics <https://docs.getdbt.com/docs/building-a-dbt-project/metrics>`_ will be added to the corresponding datasets.
 5. Every dashboard built on top of the dbt sources and/or models will be synchronized back to dbt as an `exposure <https://docs.getdbt.com/docs/building-a-dbt-project/exposures>`_.
 
 The ``--external-url-prefix`` should point to your dbt docs, so that the resources in the workspace can point to the source of truth where they are being managed. Similar to the native sync, the dbt sync also supports the ``--disallow-edits`` flag.
 
+By default, the CLI sync would create a new database on the destination workspace using below name structure:
+
+.. code-block:: python
+
+    f"{project_name}_{target_name}"
+
+If you want to sync data to an existing database connection on the workspace instead, you can specify the database connection name on the profiles YAML file. Add below structure under the ``<target-name>``:
+
+.. code-block:: yaml
+    
+    meta:
+      superset:
+        database_name: my DB name # <= specify the database connection/display name used on the workspace
+        
+Example:
+
+.. code-block:: yaml
+
+    jaffle_shop:
+      outputs:
+        dev:
+          meta:
+            superset:
+              database_name: Postgres - Production
+
+If  ``--import-db`` was passed and a database connection was found on the workspace, the operation would update the connection configuration with the dbt connection settings.
+
 If you're using dbt Cloud you can instead pass a job ID and a `service account access token <https://cloud.getdbt.com/#/accounts/72449/settings/service-tokens/new/>`_:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset sync dbt-cloud \
     > $TOKEN $JOB_ID \
     > --external-url-prefix=http://localhost:8080/
 
 The token only needs access to the "Metadata only" permission set for your project. You can see the job ID by going to the project URL in dbt Cloud and looking at the last ID in the URL. For example, if the URL is https://cloud.getdbt.com/#/accounts/12345/projects/567890/jobs/ the job ID is 567890.
 
-Before running the command you need to have a database already created in the Preset workspace, and the database should have the same name as the dbt Cloud database. You can run the command before creating the database to see what the name should be.
-
+When syncing from dbt Cloud, the database connection must already exist on the target workspace. The connection display name on the workspace must match the database name from dbt Cloud.
+              
 Selecting models
 ~~~~~~~~~~~~~~~~
 
 By default all the models will be synchronized to the workspace. The CLI supports a subset of the syntax used by the ``dbt`` command line to select which models should be synchronized. Models that should be synchronized can be specified via the ``--select`` flag:
 
 .. code-block:: bash
 
@@ -381,31 +461,61 @@
     % preset-cli --select my_model+ --exclude tag:test
 
 The command above synchronizes "my_model" and its children, as long as the models don't have the "test" tag.
 
 Exporting resources
 -------------------
 
-The CLI can also be used to export all resources (databases, datasets, charts, and dashboards) from a given Preset workspace (using ``preset-cli``) or Superset instance (using ``superset-cli``). This is useful for migrating resources between workspaces, from an existing Superset installation to Preset, or even from Preset to Superset (one of the advantages of Preset is no vendor lock in!).
+The CLI can also be used to export resources (databases, datasets, charts, and dashboards) from a given Preset workspace (using ``preset-cli``) or Superset instance (using ``superset-cli``). This is useful for migrating resources between workspaces, from an existing Superset installation to Preset, or even from Preset to Superset (one of the advantages of Preset is no vendor lock in!).
 
-The run the command on a self-hosted Superset instance:
+To export resources from a self-hosted Superset instance:
 
 .. code-block:: bash
 
     % superset-cli https://superset.example.org/ export /path/to/directory
 
 This will create a nice directory structure in ``/path/to/directory``, ready to be imported using the ``sync native`` command.
 
 To export resources from a Preset workspace:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset export /path/to/directory
 
+It's also possible to use the CLI to export specific resources:
+
+Use ``--asset-type`` to export all assets from a given type. Available options:
+
+- ``dashboard``
+- ``chart``
+- ``dataset``
+- ``database``
+
+For example, running below command would export all dashboards from this workspace (datasets, charts and DB connections wouldn't be included):
+
+.. code-block:: bash
+
+    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
+    > superset export /path/to/directory --asset-type=dashboard
+    
+Use ``--asset-ids`` to filter for specific assets. Available options:
+
+- ``dashboard-ids``
+- ``chart-ids``
+- ``dataset-ids``
+- ``database-ids``
+
+For example, running below command would export specified dashboards from this workspace (datasets, charts and DB connections would be included):
+
+.. code-block:: bash
+
+    % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
+    > superset export /path/to/directory --dashboard-ids=9,10
+
 To import the exported resources into a Preset workspace:
 
 .. code-block:: bash
 
     % preset-cli --workspaces=https://abcdef12.us1a.app.preset.io/ \
     > superset sync native /path/to/directory
 
@@ -436,18 +546,24 @@
     GROUP BY action
 
 So that when processed by ``preset-cli superset sync native`` the original Jinja2 is reconstructed correctly.
 
 Exporting users
 ~~~~~~~~~~~~~~~
 
-The ``preset-cli superset export-users`` command can be used to export a list of users. Currently there's no way to import this into a workspace, but work is in progress.
+The ``preset-cli superset export-users`` command can be used to export a list of users. These users can then be imported to Preset via the ``preset-cli import-users`` command.
+
+You can also export roles via ``preset-cli superset export-roles``, and import with ``import-roles``.
 
 Exporting RLS rules
 ~~~~~~~~~~~~~~~~~~~
 
 The ``preset-cli superset export-rls`` command can be used to export a list of RLS rules. Currently there's no way to import this into a workspace, but work is in progress.
 
 Exporting ownership
 ~~~~~~~~~~~~~~~~~~~
 
 The ``preset-cli superset export-ownership`` command generates a YAML file with information about ownership of different resources. The file maps resource UUIDs to user email address, and in the future will be used to recreate ownership on a different instance of Superset.
+
+Listing SCIM Groups
+~~~~~~~~~~~~~~~~~~~
+The ``preset-cli list-group-membership`` command prints all SCIM groups (including membership) associated with a Preset team. Instead of printing the results on the terminal (whcih can be useful for quick troubleshooting), it's possible to use ``--save-report=yaml`` or ``--save-report=csv`` to write results to a file. The file name would be ``{TeamSlug}__user_group_membership.{FileExtension}``.
```

### Comparing `preset-cli-0.1.1/src/preset_cli.egg-info/SOURCES.txt` & `preset-cli-0.2.0/src/preset_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 src/preset_cli/api/clients/dbt.py
 src/preset_cli/api/clients/preset.py
 src/preset_cli/api/clients/superset.py
 src/preset_cli/auth/__init__.py
 src/preset_cli/auth/jwt.py
 src/preset_cli/auth/lib.py
 src/preset_cli/auth/main.py
+src/preset_cli/auth/password.py
+src/preset_cli/auth/preset.py
 src/preset_cli/auth/token.py
 src/preset_cli/cli/__init__.py
 src/preset_cli/cli/main.py
 src/preset_cli/cli/superset/__init__.py
 src/preset_cli/cli/superset/export.py
 src/preset_cli/cli/superset/import_.py
 src/preset_cli/cli/superset/main.py
@@ -87,14 +89,16 @@
 tests/api/clients/dbt_test.py
 tests/api/clients/preset_test.py
 tests/api/clients/superset_test.py
 tests/auth/__init__.py
 tests/auth/jwt_test.py
 tests/auth/lib_test.py
 tests/auth/main_test.py
+tests/auth/password_test.py
+tests/auth/preset_test.py
 tests/cli/__init__.py
 tests/cli/main_test.py
 tests/cli/superset/__init__.py
 tests/cli/superset/export_test.py
 tests/cli/superset/import_test.py
 tests/cli/superset/main_test.py
 tests/cli/superset/sql_test.py
```

### Comparing `preset-cli-0.1.1/tests/api/clients/dbt_test.py` & `preset-cli-0.2.0/tests/api/clients/dbt_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tests for the dbt client.
 """
 
-# pylint: disable=missing-class-docstring, invalid-name, line-too-long
+# pylint: disable=missing-class-docstring, invalid-name, line-too-long, too-many-lines
 
 import datetime
 from enum import Enum
 
 import pytest
 from marshmallow import fields
 from pytest_mock import MockerFixture
@@ -56,18 +56,15 @@
             }
         }
     """
     client.execute(query, jobId=1)
     GraphqlClient().execute.assert_called_with(
         query=query,
         variables={"jobId": 1},
-        headers={
-            "User-Agent": "Preset CLI",
-            "X-Client-Version": __version__,
-        },
+        headers=client.session.headers,
     )
 
 
 def test_dbt_client_get_accounts(requests_mock: Mocker) -> None:
     """
     Test the ``get_accounts`` method.
     """
@@ -176,14 +173,23 @@
             "git_auth_level": "team",
             "enterprise_unique_identifier": None,
             "queue_limit": 50,
             "pod_memory_request_mebibytes": 600,
         },
     ]
 
+    requests_mock.get(
+        "https://cloud.getdbt.com/api/v2/accounts/",
+        status_code=400,
+        json={"status": {"user_message": "A wild error appears!"}},
+    )
+    with pytest.raises(Exception) as excinfo:
+        client.get_accounts()
+    assert str(excinfo.value) == "A wild error appears!"
+
 
 def test_dbt_client_get_projects(requests_mock: Mocker) -> None:
     """
     Test the ``get_projects`` method.
     """
     requests_mock.get(
         "https://cloud.getdbt.com/api/v2/accounts/72449/projects/",
@@ -636,14 +642,23 @@
             "skipped_setup": False,
             "dbt_project_subdirectory": "jaffle_shop",
             "group_permissions": [],
             "name": "jaffle_shop",
         },
     ]
 
+    requests_mock.get(
+        "https://cloud.getdbt.com/api/v2/accounts/72449/projects/",
+        status_code=400,
+        json={"status": {"user_message": "A wild error appears!"}},
+    )
+    with pytest.raises(Exception) as excinfo:
+        client.get_projects(72449)
+    assert str(excinfo.value) == "A wild error appears!"
+
 
 def test_dbt_client_get_jobs(requests_mock: Mocker) -> None:
     """
     Test the ``get_jobs`` method.
     """
     requests_mock.get(
         "https://cloud.getdbt.com/api/v2/accounts/72449/jobs/",
@@ -706,14 +721,150 @@
         {
             "id": 108380,
             "deactivated": False,
             "triggers": {
                 "custom_branch_only": False,
                 "git_provider_webhook": False,
                 "github_webhook": False,
+                "schedule": True,
+            },
+            "next_run_humanized": "2 weeks, 2 days",
+            "generate_sources": False,
+            "execution": {"timeout_seconds": 0},
+            "environment_id": 107605,
+            "created_at": datetime.datetime(
+                2022,
+                7,
+                25,
+                22,
+                0,
+                11,
+                943460,
+                tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
+            ),
+            "account_id": 72449,
+            "state": 1,
+            "deferring_job_definition_id": None,
+            "generate_docs": True,
+            "cron_humanized": "Every hour",
+            "next_run": datetime.datetime(
+                2022,
+                7,
+                26,
+                23,
+                0,
+                tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
+            ),
+            "run_failure_count": 0,
+            "lifecycle_webhooks": False,
+            "settings": {"threads": 4, "target_name": "default"},
+            "execute_steps": ["dbt run", "dbt test"],
+            "project_id": 134905,
+            "is_deferrable": False,
+            "schedule": {
+                "cron": "0 * * * *",
+                "time": {"interval": 1, "type": "every_hour"},
+                "date": {"type": "every_day"},
+            },
+            "run_generate_sources": False,
+            "dbt_version": "1.0.0",
+            "updated_at": datetime.datetime(
+                2022,
+                7,
+                26,
+                22,
+                36,
+                23,
+                862370,
+                tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
+            ),
+            "lifecycle_webhooks_url": None,
+            "name": "Test job",
+        },
+    ]
+
+    requests_mock.get(
+        "https://cloud.getdbt.com/api/v2/accounts/72449/jobs/",
+        status_code=400,
+        json={"status": {"user_message": "A wild error appears!"}},
+    )
+    with pytest.raises(Exception) as excinfo:
+        client.get_jobs(72449)
+    assert str(excinfo.value) == "A wild error appears!"
+
+
+def test_dbt_client_get_jobs_for_project(requests_mock: Mocker) -> None:
+    """
+    Test the ``get_jobs`` method when passing a project.
+    """
+    requests_mock.get(
+        "https://cloud.getdbt.com/api/v2/accounts/72449/jobs/",
+        json={
+            "status": {
+                "code": 200,
+                "is_success": True,
+                "user_message": "Success!",
+                "developer_message": "",
+            },
+            "data": [
+                {
+                    "execution": {"timeout_seconds": 0},
+                    "generate_docs": True,
+                    "run_generate_sources": False,
+                    "id": 108380,
+                    "account_id": 72449,
+                    "project_id": 134905,
+                    "environment_id": 107605,
+                    "name": "Test job",
+                    "dbt_version": "1.0.0",
+                    "created_at": "2022-07-25T22:00:11.943460+00:00",
+                    "updated_at": "2022-07-26T22:36:23.862370+00:00",
+                    "execute_steps": ["dbt run", "dbt test"],
+                    "state": 1,
+                    "deactivated": False,
+                    "run_failure_count": 0,
+                    "deferring_job_definition_id": None,
+                    "lifecycle_webhooks": False,
+                    "lifecycle_webhooks_url": None,
+                    "triggers": {
+                        "github_webhook": False,
+                        "git_provider_webhook": False,
+                        "custom_branch_only": False,
+                        "schedule": True,
+                    },
+                    "settings": {"threads": 4, "target_name": "default"},
+                    "schedule": {
+                        "cron": "0 * * * *",
+                        "date": {"type": "every_day"},
+                        "time": {"type": "every_hour", "interval": 1},
+                    },
+                    "is_deferrable": False,
+                    "generate_sources": False,
+                    "cron_humanized": "Every hour",
+                    "next_run": "2022-07-26T23:00:00+00:00",
+                    "next_run_humanized": "2 weeks, 2 days",
+                },
+            ],
+            "extra": {
+                "filters": {"limit": 100, "offset": 0, "account_id": 72449},
+                "order_by": "id",
+                "pagination": {"count": 1, "total_count": 1},
+            },
+        },
+    )
+    auth = Auth()
+    client = DBTClient(auth)
+    assert client.get_jobs(72449, project_id=134905) == [
+        {
+            "id": 108380,
+            "deactivated": False,
+            "triggers": {
+                "custom_branch_only": False,
+                "git_provider_webhook": False,
+                "github_webhook": False,
                 "schedule": True,
             },
             "next_run_humanized": "2 weeks, 2 days",
             "generate_sources": False,
             "execution": {"timeout_seconds": 0},
             "environment_id": 107605,
             "created_at": datetime.datetime(
```

### Comparing `preset-cli-0.1.1/tests/api/clients/superset_test.py` & `preset-cli-0.2.0/tests/api/clients/superset_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """
 Tests for ``preset_cli.api.clients.superset``.
 """
-# pylint: disable=too-many-lines, trailing-whitespace
+# pylint: disable=too-many-lines, trailing-whitespace, line-too-long, use-implicit-booleaness-not-comparison
 
 import json
 from io import BytesIO
 from unittest import mock
+from urllib.parse import unquote_plus
 from uuid import UUID
 from zipfile import ZipFile, is_zipfile
 
 import pytest
 import yaml
 from pytest_mock import MockerFixture
 from requests_mock.mocker import Mocker
 from yarl import URL
 
 from preset_cli import __version__
 from preset_cli.api.clients.superset import (
+    RoleType,
     RuleType,
     SupersetClient,
     convert_to_adhoc_column,
     convert_to_adhoc_metric,
     parse_html_array,
 )
 from preset_cli.api.operators import OneToMany
 from preset_cli.auth.main import Auth
 from preset_cli.exceptions import ErrorLevel, SupersetError
 
 
-def test_run_query(requests_mock: Mocker) -> None:
+def test_run_query(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test the ``run_query`` method.
     """
+    _logger = mocker.patch("preset_cli.api.clients.superset._logger")
+    mocker.patch("preset_cli.api.clients.superset.shortid", return_value="5b8f4d8c89")
     requests_mock.post(
         "https://superset.example.org/superset/sql_json/",
         json={
             "query_id": 2,
             "status": "success",
             "data": [{"value": 1}],
             "columns": [{"name": "value", "type": "INT", "is_date": False}],
@@ -75,14 +79,33 @@
     )
 
     auth = Auth()
     client = SupersetClient("https://superset.example.org/", auth)
 
     results = client.run_query(database_id=1, sql="SELECT 1 AS value", limit=10)
     assert results.to_dict() == {"value": {0: 1}}
+    _logger.debug.assert_called_with(
+        "POST %s\n%s",
+        URL("https://superset.example.org/superset/sql_json/"),
+        """{
+    "client_id": "5b8f4d8c89",
+    "database_id": 1,
+    "json": true,
+    "runAsync": false,
+    "schema": null,
+    "sql": "SELECT 1 AS value",
+    "sql_editor_id": "1",
+    "tab": "Untitled Query 2",
+    "tmp_table_name": "",
+    "select_as_cta": false,
+    "ctas_method": "TABLE",
+    "queryLimit": 10,
+    "expand_data": true
+}""",
+    )
 
 
 def test_run_query_error(requests_mock: Mocker) -> None:
     """
     Test the ``run_query`` method when an error occurs.
     """
     errors = [
@@ -518,103 +541,92 @@
             26: 22,
             27: 87,
             28: 27,
         },
     }
 
 
-def test_get_data_parameters(mocker: MockerFixture) -> None:
+def test_get_data_parameters(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test different parameters passed to ``get_data``.
     """
-    auth = mocker.MagicMock()
-    session = auth.get_session()
-    session.get().json.return_value = {
-        "result": {
-            "columns": [],
-            "metrics": [],
-        },
-    }
-    session.post().json.return_value = {
-        "result": [
-            {
-                "data": [{"a": 1}],
+    requests_mock.get(
+        "https://superset.example.org/api/v1/dataset/27",
+        json={
+            "result": {
+                "columns": [],
+                "metrics": [],
             },
-        ],
-    }
+        },
+    )
+    post_mock = requests_mock.post(
+        "https://superset.example.org/api/v1/chart/data",
+        json={
+            "result": [
+                {
+                    "data": [{"a": 1}],
+                },
+            ],
+        },
+    )
     mocker.patch("preset_cli.api.clients.superset.uuid4", return_value=1234)
 
+    auth = Auth()
     client = SupersetClient("https://superset.example.org/", auth)
     client.get_data(
         27,
         ["cnt"],
         ["name"],
         time_column="ts",
         is_timeseries=True,
         granularity="P1M",
     )
 
-    session.post.assert_has_calls(
-        [
-            mock.call(),
-            mock.call(
-                URL("https://superset.example.org/api/v1/chart/data"),
-                json={
-                    "datasource": {"id": 27, "type": "table"},
-                    "force": False,
-                    "queries": [
-                        {
-                            "annotation_layers": [],
-                            "applied_time_extras": {},
-                            "columns": [{"label": "name", "sqlExpression": "name"}],
-                            "custom_form_data": {},
-                            "custom_params": {},
-                            "extras": {
-                                "having": "",
-                                "having_druid": [],
-                                "time_grain_sqla": "P1M",
-                                "where": "",
-                            },
-                            "filters": [],
-                            "granularity": "ts",
-                            "is_timeseries": True,
-                            "metrics": [
-                                {
-                                    "aggregate": None,
-                                    "column": None,
-                                    "expressionType": "SQL",
-                                    "hasCustomLabel": False,
-                                    "isNew": False,
-                                    "label": "cnt",
-                                    "optionName": "metric_1234",
-                                    "sqlExpression": "cnt",
-                                },
-                            ],
-                            "order_desc": True,
-                            "orderby": [],
-                            "row_limit": 10000,
-                            "time_range": "No filter",
-                            "timeseries_limit": 0,
-                            "url_params": {},
-                        },
-                    ],
-                    "result_format": "json",
-                    "result_type": "full",
-                },
-                headers={
-                    "Accept": "application/json",
-                    "Content-Type": "application/json",
-                    "User-Agent": f"Apache Superset Client ({__version__})",
-                    "Referer": "https://superset.example.org/",
+    assert post_mock.last_request.json() == {
+        "datasource": {"id": 27, "type": "table"},
+        "force": False,
+        "queries": [
+            {
+                "annotation_layers": [],
+                "applied_time_extras": {},
+                "columns": [{"label": "name", "sqlExpression": "name"}],
+                "custom_form_data": {},
+                "custom_params": {},
+                "extras": {
+                    "having": "",
+                    "having_druid": [],
+                    "where": "",
+                    "time_grain_sqla": "P1M",
                 },
-            ),
-            mock.call().ok.__bool__(),
-            mock.call().json(),
+                "filters": [],
+                "is_timeseries": True,
+                "metrics": [
+                    {
+                        "aggregate": None,
+                        "column": None,
+                        "expressionType": "SQL",
+                        "hasCustomLabel": False,
+                        "isNew": False,
+                        "label": "cnt",
+                        "optionName": "metric_1234",
+                        "sqlExpression": "cnt",
+                    },
+                ],
+                "order_desc": True,
+                "orderby": [],
+                "row_limit": 10000,
+                "time_range": "No filter",
+                "timeseries_limit": 0,
+                "url_params": {},
+                "granularity": "ts",
+            },
         ],
-    )
+        "result_format": "json",
+        "result_type": "full",
+    }
 
 
 def test_get_data_time_column_error(requests_mock: Mocker) -> None:
     """
     Test when the time column is ambiguous in ``get_data``.
     """
     requests_mock.get(
@@ -680,15 +692,15 @@
 def test_get_resource(requests_mock: Mocker) -> None:
     """
     Test the generic ``get_resource`` method.
     """
     # the payload schema is irrelevant, since it's passed through unmodified
     requests_mock.get(
         "https://superset.example.org/api/v1/database/1",
-        json={"Hello": "world"},
+        json={"result": {"Hello": "world"}},
     )
 
     auth = Auth()
     client = SupersetClient("https://superset.example.org/", auth)
 
     response = client.get_resource("database", 1)
     assert response == {"Hello": "world"}
@@ -973,15 +985,26 @@
     """
     auth = Auth()
     client = SupersetClient("https://superset.example.org/", auth)
     update_resource = mocker.patch.object(client, "update_resource")
 
     client.update_dataset(1, dataset_name="my_other_db")
     update_resource.assert_called_with(
-        "dataset", 1, {"override_columns": "true"}, dataset_name="my_other_db",
+        "dataset",
+        1,
+        {"override_columns": "false"},
+        dataset_name="my_other_db",
+    )
+
+    client.update_dataset(1, override_columns=True, dataset_name="my_other_db")
+    update_resource.assert_called_with(
+        "dataset",
+        1,
+        {"override_columns": "true"},
+        dataset_name="my_other_db",
     )
 
 
 def test_get_chart(mocker: MockerFixture) -> None:
     """
     Test the ``get_chart`` method.
     """
@@ -1306,27 +1329,27 @@
 
 def test_export_users_preset(requests_mock: Mocker) -> None:
     """
     Test ``export_users``.
     """
     requests_mock.get("https://superset.example.org/users/list/", status_code=404)
     requests_mock.get(
-        "https://manage.app.preset.io/api/v1/teams/",
+        "https://api.app.preset.io/v1/teams",
         json={
             "payload": [{"name": "team1"}],
         },
     )
     requests_mock.get(
-        "https://manage.app.preset.io/api/v1/teams/team1/workspaces/",
+        "https://api.app.preset.io/v1/teams/team1/workspaces",
         json={
             "payload": [{"id": 1, "hostname": "superset.example.org"}],
         },
     )
     requests_mock.get(
-        "https://manage.app.preset.io/api/v1/teams/team1/workspaces/1/memberships",
+        "https://api.app.preset.io/v1/teams/team1/workspaces/1/memberships",
         json={
             "payload": [
                 {
                     "user": {
                         "username": "adoe",
                         "first_name": "Alice",
                         "last_name": "Doe",
@@ -1372,14 +1395,279 @@
             "username": "bdoe",
             "email": "bdoe@example.com",
             "role": [],
         },
     ]
 
 
+def test_export_roles(mocker: MockerFixture, requests_mock: Mocker) -> None:
+    """
+    Test ``export_roles``.
+    """
+    requests_mock.get(
+        (
+            "https://superset.example.org/roles/list/?"
+            "psize_RoleModelView=100&"
+            "page_RoleModelView=0"
+        ),
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Name</th>
+      </tr>
+      <tr>
+        <td><input id="1" /></td>
+        <td>Admin</td>
+      </tr>
+      <tr>
+        <td><input id="2" /></td>
+        <td>Public</td>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        (
+            "https://superset.example.org/roles/list/?"
+            "psize_RoleModelView=100&"
+            "page_RoleModelView=1"
+        ),
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Name</th>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <input name="name" value="Admin" />
+    <select id="permissions">
+        <option selected="" value="1">can this</option>
+        <option selected="" value="2">can that</option>
+        <option value="3">cannot </option>
+    </select>
+    <select id="user">
+        <option selected="" value="1">Alice Doe</option>
+        <option value="2">Bob Doe</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/2",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <input name="name" value="Public" />
+    <select id="permissions">
+        <option value="1">can this</option>
+        <option value="2">can that</option>
+        <option value="3">cannot </option>
+    </select>
+    <select id="user">
+        <option value="1">Alice Doe</option>
+        <option value="2">Bob Doe</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
+    mocker.patch.object(
+        SupersetClient,
+        "export_users",
+        return_value=[
+            {"id": 1, "email": "adoe@example.com"},
+            {"id": 2, "email": "bdoe@example.com"},
+        ],
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    assert list(client.export_roles()) == [
+        {
+            "name": "Admin",
+            "permissions": ["can this", "can that"],
+            "users": ["adoe@example.com"],
+        },
+        {
+            "name": "Public",
+            "permissions": [],
+            "users": [],
+        },
+    ]
+
+
+def test_export_roles_anchor_role_id(
+    mocker: MockerFixture,
+    requests_mock: Mocker,
+) -> None:
+    """
+    Test ``export_roles``.
+    """
+    requests_mock.get(
+        (
+            "https://superset.example.org/roles/list/?"
+            "psize_RoleModelView=100&"
+            "page_RoleModelView=0"
+        ),
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Name</th>
+      </tr>
+      <tr>
+        <td><a href="/roles/edit/1">Edit</a></td>
+        <td>Admin</td>
+      </tr>
+      <tr>
+        <td><a href="/roles/edit/2">Edit</a></td>
+        <td>Public</td>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        (
+            "https://superset.example.org/roles/list/?"
+            "psize_RoleModelView=100&"
+            "page_RoleModelView=1"
+        ),
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Name</th>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <input name="name" value="Admin" />
+    <select id="permissions">
+        <option selected="" value="1">can this</option>
+        <option selected="" value="2">can that</option>
+        <option value="3">cannot </option>
+    </select>
+    <select id="user">
+        <option selected="" value="1">Alice Doe</option>
+        <option value="2">Bob Doe</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/2",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <input name="name" value="Public" />
+    <select id="permissions">
+        <option value="1">can this</option>
+        <option value="2">can that</option>
+        <option value="3">cannot </option>
+    </select>
+    <select id="user">
+        <option value="1">Alice Doe</option>
+        <option value="2">Bob Doe</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
+    mocker.patch.object(
+        SupersetClient,
+        "export_users",
+        return_value=[
+            {"id": 1, "email": "adoe@example.com"},
+            {"id": 2, "email": "bdoe@example.com"},
+        ],
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    assert list(client.export_roles()) == [
+        {
+            "name": "Admin",
+            "permissions": ["can this", "can that"],
+            "users": ["adoe@example.com"],
+        },
+        {
+            "name": "Public",
+            "permissions": [],
+            "users": [],
+        },
+    ]
+
+
 def test_export_rls(requests_mock: Mocker) -> None:
     """
     Test ``export_rls``.
     """
     requests_mock.get(
         (
             "https://superset.example.org/rowlevelsecurityfiltersmodelview/list/?"
@@ -1483,14 +1771,43 @@
             "roles": ["Gamma"],
             "group_key": "department",
             "clause": "client_id = 9",
         },
     ]
 
 
+def test_export_rls_no_rules(requests_mock: Mocker) -> None:
+    """
+    Test ``export_rls``.
+    """
+    requests_mock.get(
+        (
+            "https://superset.example.org/rowlevelsecurityfiltersmodelview/list/?"
+            "psize_RowLevelSecurityFiltersModelView=100&"
+            "page_RowLevelSecurityFiltersModelView=0"
+        ),
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    No records found
+  </body>
+</html>
+        """,
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    assert list(client.export_rls()) == []
+
+
 def test_export_ownership(mocker: MockerFixture) -> None:
     """
     Test ``export_ownership``.
     """
     mocker.patch.object(
         SupersetClient,
         "export_users",
@@ -1555,15 +1872,15 @@
         name = f"chart_export/chart/chart{i+1}.yaml"
         uuid = uuids[i]
         buf = BytesIO()
         with ZipFile(buf, "w") as bundle:
             with bundle.open("metadata.yaml", "w") as output:
                 output.write(b"Hello!")
             with bundle.open(name, "w") as output:
-                output.write(yaml.dump({"uuid": uuid}).encode())
+                output.write(yaml.dump({"uuid": uuid}).encode())  # type: ignore
         buf.seek(0)
 
         requests_mock.get(
             f"https://superset.example.org/api/v1/chart/export/?q=%21%28{i+1}%29",
             content=buf.getvalue(),
         )
 
@@ -1602,14 +1919,217 @@
                             public.FCC 2018 Survey
 """,
         )
         == ["main.sales", "public.FCC 2018 Survey"]
     )
 
 
+def test_import_role(mocker: MockerFixture, requests_mock: Mocker) -> None:
+    """
+    Test the ``import_role`` method.
+    """
+    _logger = mocker.patch("preset_cli.api.clients.superset._logger")
+    requests_mock.get(
+        "https://superset.example.org/roles/add",
+        text="""
+<select id="permissions">
+    <option value="1">All database access</option>
+    <option value="2">Schema access on Google Sheets.main</option>
+</select>
+    """,
+    )
+    requests_mock.post("https://superset.example.org/roles/add")
+    requests_mock.get(
+        "https://superset.example.org/roles/list/?_flt_3_name=Admin",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+  </body>
+</html>
+        """,
+    )
+    mocker.patch.object(
+        SupersetClient,
+        "export_users",
+        return_value=[
+            {"id": 1, "email": "admin@example.com"},
+            {"id": 2, "email": "adoe@example.com"},
+        ],
+    )
+
+    role: RoleType = {
+        "name": "Admin",
+        "permissions": [
+            "can do something that is not in Preset",
+            "all database access on all_database_access",
+            "schema access on [Google Sheets].[main]",
+            "database access on [Not added].(id:1)",
+            "datasource access on [Not added].[nope](id:42)",
+        ],
+        "users": ["admin@example.com", "adoe@example.com", "bdoe@example.com"],
+    }
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    client.import_role(role)
+
+    assert (
+        requests_mock.last_request.text
+        == "name=Admin&user=1&user=2&permissions=1&permissions=2"
+    )
+
+    assert _logger.warning.mock_calls == [
+        mock.call(
+            "Permission %s not found in target",
+            "can do something that is not in Preset",
+        ),
+        mock.call("Permission %s not found in target", "Database access on Not added"),
+        mock.call(
+            "Permission %s not found in target",
+            "Dataset access on Not added.nope",
+        ),
+    ]
+
+
+def test_import_role_update(mocker: MockerFixture, requests_mock: Mocker) -> None:
+    """
+    Test the ``import_role`` method on updates.
+    """
+    _logger = mocker.patch("preset_cli.api.clients.superset._logger")
+    requests_mock.get(
+        "https://superset.example.org/roles/add",
+        text="""
+<select id="permissions">
+    <option value="1">All database access</option>
+    <option value="2">Schema access on Google Sheets.main</option>
+</select>
+    """,
+    )
+    requests_mock.post("https://superset.example.org/roles/add")
+    requests_mock.post("https://superset.example.org/roles/edit/1")
+    requests_mock.post("https://superset.example.org/roles/edit/2")
+    requests_mock.get(
+        "https://superset.example.org/roles/list/?_flt_3_name=Admin",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Name</th>
+      </tr>
+      <tr>
+        <td><input id="1" /></td>
+        <td>Admin</td>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/list/?_flt_3_name=Public",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Name</th>
+      </tr>
+      <tr>
+        <td><a href="/roles/edit/2">Edit</a></td>
+        <td>Public</td>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/list/?_flt_3_name=Other",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table></table>
+  </body>
+</html>
+        """,
+    )
+    mocker.patch.object(
+        SupersetClient,
+        "export_users",
+        return_value=[
+            {"id": 1, "email": "admin@example.com"},
+            {"id": 2, "email": "adoe@example.com"},
+        ],
+    )
+
+    role: RoleType = {
+        "name": "Admin",
+        "permissions": [
+            "can do something that is not in Preset",
+            "all database access on all_database_access",
+            "schema access on [Google Sheets].[main]",
+            "database access on [Not added].(id:1)",
+            "datasource access on [Not added].[nope](id:42)",
+        ],
+        "users": ["admin@example.com", "adoe@example.com", "bdoe@example.com"],
+    }
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    client.import_role(role)
+
+    assert (
+        requests_mock.last_request.text
+        == "name=Admin&user=1&user=2&permissions=1&permissions=2"
+    )
+
+    assert _logger.warning.mock_calls == [
+        mock.call(
+            "Permission %s not found in target",
+            "can do something that is not in Preset",
+        ),
+        mock.call("Permission %s not found in target", "Database access on Not added"),
+        mock.call(
+            "Permission %s not found in target",
+            "Dataset access on Not added.nope",
+        ),
+    ]
+
+    # extra tests
+    role["name"] = "Public"
+    client.import_role(role)
+    assert requests_mock.last_request.url == "https://superset.example.org/roles/edit/2"
+    role["name"] = "Other"
+    client.import_role(role)
+    assert requests_mock.last_request.url == "https://superset.example.org/roles/add"
+
+
 def test_import_rls(requests_mock: Mocker) -> None:
     """
     Test the ``import_rls`` method.
     """
     requests_mock.get(
         "https://superset.example.org/api/v1/dataset/?q="
         "(filters:!((col:schema,opr:eq,value:main),"
@@ -1636,24 +2156,42 @@
   </head>
   <body>
     <table></table>
     <table>
       <tr>
         <td></td>
         <td>Name</td>
+        <td>Permissions</td>
       </tr>
       <tr>
         <td><input id="1" /></td>
         <td>Gamma</td>
+        <td>\n</td>
       </tr>
     </table>
   </body>
 </html>
         """,
     )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <select id="permissions">
+        <option value="1">some permission</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
     requests_mock.post(
         "https://superset.example.org/rowlevelsecurityfiltersmodelview/add",
     )
 
     rls: RuleType = {
         "clause": "client_id = 9",
         "description": "Rule description",
@@ -1675,14 +2213,155 @@
         "tables=1&"
         "roles=1&"
         "group_key=department&"
         "clause=client_id+%3D+9"
     )
 
 
+def test_import_rls_no_role_table(requests_mock: Mocker) -> None:
+    """
+    Test the ``import_rls`` method when there's no table for roles in the DOM.
+    """
+    requests_mock.get(
+        "https://superset.example.org/api/v1/dataset/?q="
+        "(filters:!((col:schema,opr:eq,value:main),"
+        "(col:table_name,opr:eq,value:test_table)),"
+        "order_column:changed_on_delta_humanized,"
+        "order_direction:desc,page:0,page_size:100)",
+        json={"result": [{"id": 1}]},
+    )
+    requests_mock.get(
+        "https://superset.example.org/api/v1/dataset/?q="
+        "(filters:!((col:schema,opr:eq,value:main),"
+        "(col:table_name,opr:eq,value:test_table)),"
+        "order_column:changed_on_delta_humanized,"
+        "order_direction:desc,page:1,page_size:100)",
+        json={"result": []},
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.post(
+        "https://superset.example.org/rowlevelsecurityfiltersmodelview/add",
+    )
+
+    rls: RuleType = {
+        "clause": "client_id = 9",
+        "description": "Rule description",
+        "filter_type": "Regular",
+        "group_key": "department",
+        "name": "Rule name",
+        "roles": ["Gamma"],
+        "tables": ["main.test_table"],
+    }
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    with pytest.raises(Exception) as excinfo:
+        client.import_rls(rls)
+    assert str(excinfo.value) == "Cannot find role: Gamma"
+
+
+def test_import_rls_invalid_role(requests_mock: Mocker) -> None:
+    """
+    Test the ``import_rls`` method when the role has permissions.
+    """
+    requests_mock.get(
+        "https://superset.example.org/api/v1/dataset/?q="
+        "(filters:!((col:schema,opr:eq,value:main),"
+        "(col:table_name,opr:eq,value:test_table)),"
+        "order_column:changed_on_delta_humanized,"
+        "order_direction:desc,page:0,page_size:100)",
+        json={"result": [{"id": 1}]},
+    )
+    requests_mock.get(
+        "https://superset.example.org/api/v1/dataset/?q="
+        "(filters:!((col:schema,opr:eq,value:main),"
+        "(col:table_name,opr:eq,value:test_table)),"
+        "order_column:changed_on_delta_humanized,"
+        "order_direction:desc,page:1,page_size:100)",
+        json={"result": []},
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <td></td>
+        <td>Name</td>
+        <td>Permissions</td>
+      </tr>
+      <tr>
+        <td><input id="1" /></td>
+        <td>Gamma</td>
+        <td>All database access</td>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <select id="permissions">
+        <option selected="" value="1">some permission</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.post(
+        "https://superset.example.org/rowlevelsecurityfiltersmodelview/add",
+    )
+
+    rls: RuleType = {
+        "clause": "client_id = 9",
+        "description": "Rule description",
+        "filter_type": "Regular",
+        "group_key": "department",
+        "name": "Rule name",
+        "roles": ["Gamma"],
+        "tables": ["main.test_table"],
+    }
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    with pytest.raises(Exception) as excinfo:
+        client.import_rls(rls)
+    assert str(excinfo.value) == (
+        "Role Gamma currently has permissions associated with it. "
+        "To use it with RLS it should have no permissions."
+    )
+
+
 def test_import_rls_no_schema(requests_mock: Mocker) -> None:
     """
     Test the ``import_rls`` method when the table has no schema.
     """
     requests_mock.get(
         "https://superset.example.org/api/v1/dataset/?q="
         "(filters:!((col:table_name,opr:eq,value:test_table)),"
@@ -1707,24 +2386,42 @@
   </head>
   <body>
     <table></table>
     <table>
       <tr>
         <td></td>
         <td>Name</td>
+        <td>Permissions</td>
       </tr>
       <tr>
         <td><input id="1" /></td>
         <td>Gamma</td>
+        <td>\n</td>
       </tr>
     </table>
   </body>
 </html>
         """,
     )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <select id="permissions">
+        <option value="1">some permission</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
     requests_mock.post(
         "https://superset.example.org/rowlevelsecurityfiltersmodelview/add",
     )
 
     rls: RuleType = {
         "clause": "client_id = 9",
         "description": "Rule description",
@@ -1978,24 +2675,42 @@
   </head>
   <body>
     <table></table>
     <table>
       <tr>
         <td></td>
         <td>Name</td>
+        <td>Permissions</td>
       </tr>
       <tr>
         <td><a href="/roles/edit/1">Edit</a></td>
         <td>Gamma</td>
+        <td>\n</td>
       </tr>
     </table>
   </body>
 </html>
         """,
     )
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <select id="permissions">
+        <option value="1">some permission</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
     requests_mock.post(
         "https://superset.example.org/rowlevelsecurityfiltersmodelview/add",
     )
 
     rls: RuleType = {
         "clause": "client_id = 9",
         "description": "Rule description",
@@ -2047,11 +2762,198 @@
         "dataset",
         [
             {
                 "name": "test_table",
                 "owners": ["admin@example.com", "adoe@example.com"],
                 "uuid": "e0d20af0-cef9-4bdb-80b4-745827f441bf",
             },
+            {
+                "name": "another_table",
+                "owners": ["admin@example.com", "adoe@example.com"],
+                "uuid": "1192072c-4bee-4535-b8ee-e9f5fc4eb6a2",
+            },
         ],
     )
 
     assert requests_mock.last_request.json() == {"owners": [1, 2]}
+
+
+def test_update_role(requests_mock: Mocker) -> None:
+    """
+    Test the ``update_role`` method.
+    """
+    requests_mock.get(
+        "https://superset.example.org/roles/edit/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <input name="name" value="Old Role" />
+    <select id="user">
+        <option selected="" value="1">Alice Doe</option>
+        <option value="2">Bob Doe</option>
+    </select>
+    <select id="permissions">
+        <option selected="" value="1">some permission</option>
+        <option value="2">another permission</option>
+    </select>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.post("https://superset.example.org/roles/edit/1")
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+
+    client.update_role(1, name="New Role")
+    assert requests_mock.last_request.text == "name=New+Role&user=1&permissions=1"
+
+    client.update_role(1, user=[2], permissions=[1, 2])
+    assert (
+        requests_mock.last_request.text
+        == "name=Old+Role&user=2&permissions=1&permissions=2"
+    )
+
+
+def test_create_virtual_dataset(requests_mock: Mocker) -> None:
+    """
+    Test the ``create_dataset`` method with virtual datasets.
+    """
+    requests_mock.post(
+        "https://superset.example.org/superset/sql_json/",
+        json={
+            "query_id": 137,
+            "status": "success",
+            "data": [
+                {
+                    "ID": 20,
+                    "FIRST_NAME": "Anna",
+                    "LAST_NAME": "A.",
+                    "ds": "2022-01-01",
+                    "complex": r"\x00",
+                },
+            ],
+            "columns": [
+                {"name": "ID", "type": "INTEGER", "is_dttm": False},
+                {"name": "FIRST_NAME", "type": "STRING", "is_dttm": False},
+                {"name": "LAST_NAME", "type": "STRING", "is_dttm": False},
+                {"name": "ds", "type": "DATETIME", "is_dttm": True},
+                {"name": "complex", "type": None, "is_dttm": False},
+            ],
+            "selected_columns": [
+                {"name": "ID", "type": "INTEGER", "is_dttm": False},
+                {"name": "FIRST_NAME", "type": "STRING", "is_dttm": False},
+                {"name": "LAST_NAME", "type": "STRING", "is_dttm": False},
+                {"name": "ds", "type": "DATETIME", "is_dttm": True},
+                {"name": "complex", "type": None, "is_dttm": False},
+            ],
+            "expanded_columns": [],
+            "query": {
+                "changedOn": "2022-10-04T00:54:22.174889",
+                "changed_on": "2022-10-04T00:54:22.174889",
+                "dbId": 6,
+                "db": "jaffle_shop_dev",
+                "endDttm": 1664844864497.491,
+                "errorMessage": None,
+                "executedSql": "-- 6dcd92a04feb50f14bbcf07c661680ba\nSELECT * FROM `dbt-tutorial`.jaffle_shop.customers LIMIT 2\n-- 6dcd92a04feb50f14bbcf07c661680ba",
+                "id": "eJfI9pxnh",
+                "queryId": 137,
+                "limit": 1,
+                "limitingFactor": "QUERY",
+                "progress": 100,
+                "rows": 1,
+                "schema": "dbt_beto",
+                "ctas": False,
+                "serverId": 137,
+                "sql": "SELECT * FROM `dbt-tutorial`.jaffle_shop.customers LIMIT 1;",
+                "sqlEditorId": "8",
+                "startDttm": 1664844861997.288000,
+                "state": "success",
+                "tab": "Query dbt_beto.customers",
+                "tempSchema": None,
+                "tempTable": None,
+                "userId": 2,
+                "user": "Beto Ferreira De Almeida",
+                "resultsKey": "313ec42b-3b76-40c7-8e90-31ed549174dd",
+                "trackingUrl": None,
+                "extra": {
+                    "progress": None,
+                    "columns": [
+                        {"name": "ID", "type": "INTEGER", "is_dttm": False},
+                        {"name": "FIRST_NAME", "type": "STRING", "is_dttm": False},
+                        {"name": "LAST_NAME", "type": "STRING", "is_dttm": False},
+                        {"name": "ds", "type": "DATETIME", "is_dttm": True},
+                        {"name": "complex", "type": None, "is_dttm": False},
+                    ],
+                },
+            },
+        },
+    )
+    requests_mock.post(
+        "https://superset.example.org/superset/sqllab_viz/",
+        json={"data": [1, 2, 3]},
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+
+    client.create_dataset(
+        database=1,
+        schema="public",
+        sql="SELECT * FROM `dbt-tutorial`.jaffle_shop.customers LIMIT 1;",
+        table_name="test virtual",
+    )
+
+    assert json.loads(
+        unquote_plus(requests_mock.last_request.text.split("=", 1)[1]),
+    ) == {
+        "sql": "SELECT * FROM `dbt-tutorial`.jaffle_shop.customers LIMIT 1;",
+        "dbId": 1,
+        "schema": "public",
+        "datasourceName": "test virtual",
+        "columns": [
+            {
+                "name": "ID",
+                "type": "INTEGER",
+                "is_dttm": False,
+                "column_name": "ID",
+                "groupby": True,
+                "type_generic": 0,
+            },
+            {
+                "name": "FIRST_NAME",
+                "type": "STRING",
+                "is_dttm": False,
+                "column_name": "FIRST_NAME",
+                "groupby": True,
+                "type_generic": 1,
+            },
+            {
+                "name": "LAST_NAME",
+                "type": "STRING",
+                "is_dttm": False,
+                "column_name": "LAST_NAME",
+                "groupby": True,
+                "type_generic": 1,
+            },
+            {
+                "name": "ds",
+                "type": "DATETIME",
+                "is_dttm": True,
+                "column_name": "ds",
+                "groupby": True,
+                "type_generic": 2,
+            },
+            {
+                "name": "complex",
+                "type": "UNKNOWN",
+                "is_dttm": False,
+                "column_name": "complex",
+                "groupby": True,
+                "type_generic": 1,
+            },
+        ],
+    }
```

### Comparing `preset-cli-0.1.1/tests/auth/jwt_test.py` & `preset-cli-0.2.0/tests/auth/jwt_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,32 +26,28 @@
     get_credentials_path().exists.return_value = True
     get_credentials_path().__str__.return_value = "/path/to/credentials.yaml"
 
     yaml = mocker.patch("preset_cli.auth.jwt.yaml")
     yaml.load.return_value = {
         "api_token": "TOKEN",
         "api_secret": "SECRET",
-        "baseurl": "https://manage.app.preset.io/",
+        "baseurl": "https://api.app.preset.io/",
     }
 
     get_access_token = mocker.patch("preset_cli.auth.jwt.get_access_token")
     get_access_token.return_value = "JWT_TOKEN"
 
     auth = JWTAuth.from_stored_credentials()
     assert auth.token == "JWT_TOKEN"
     get_access_token.assert_called_with(
-        baseurl="https://manage.app.preset.io/",
+        baseurl="https://api.app.preset.io/",
         api_token="TOKEN",
         api_secret="SECRET",
     )
 
-    # can also pass a URL
-    auth = JWTAuth.from_stored_credentials()
-    assert auth.token == "JWT_TOKEN"
-
     # test for error
     get_credentials_path().exists.return_value = False
     with pytest.raises(Exception) as excinfo:
         JWTAuth.from_stored_credentials()
     assert (
         str(excinfo.value)
         == "Could not load credentials from /path/to/credentials.yaml"
```

### Comparing `preset-cli-0.1.1/tests/auth/lib_test.py` & `preset-cli-0.2.0/tests/auth/lib_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
 
 def test_get_access_token(requests_mock: Mocker) -> None:
     """
     Test ``get_access_token``.
     """
     requests_mock.post(
-        "https://manage.app.preset.io/api/v1/auth/",
+        "https://api.app.preset.io/v1/auth/",
         json={"payload": {"access_token": "TOKEN"}},
     )
 
     access_token = get_access_token(
-        URL("https://manage.app.preset.io/"),
+        URL("https://api.app.preset.io/"),
         "API_TOKEN",
         "API_SECRET",
     )
     assert access_token == "TOKEN"
 
     access_token = get_access_token(
-        "https://manage.app.preset.io/",
+        "https://api.app.preset.io/",
         "API_TOKEN",
         "API_SECRET",
     )
     assert access_token == "TOKEN"
 
 
 def test_get_credentials_path(mocker: MockerFixture) -> None:
@@ -56,27 +56,27 @@
     """
     credentials_path = Path("/path/to/config/credentials.yaml")
 
     mocker.patch("preset_cli.auth.lib.input", side_effect=["invalid", "n"])
     store_credentials(
         "API_TOKEN",
         "API_SECRET",
-        URL("https://manage.app.preset.io/"),
+        URL("https://api.app.preset.io/"),
         credentials_path,
     )
     assert not credentials_path.exists()
 
     mocker.patch("preset_cli.auth.lib.input", return_value="y")
     store_credentials(
         "API_TOKEN",
         "API_SECRET",
-        URL("https://manage.app.preset.io/"),
+        URL("https://api.app.preset.io/"),
         credentials_path,
     )
     assert credentials_path.exists()
     with open(credentials_path, encoding="utf-8") as input_:
         contents = yaml.load(input_, Loader=yaml.SafeLoader)
     assert contents == {
         "api_secret": "API_SECRET",
         "api_token": "API_TOKEN",
-        "baseurl": "https://manage.app.preset.io/",
+        "baseurl": "https://api.app.preset.io/",
     }
```

### Comparing `preset-cli-0.1.1/tests/auth/main_test.py` & `preset-cli-0.2.0/tests/auth/password_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 """
-Test authentication mechanisms.
+Test username:password authentication mechanism.
 """
 
-from pytest_mock import MockerFixture
 from requests_mock.mocker import Mocker
 from yarl import URL
 
-from preset_cli.auth.main import Auth, UsernamePasswordAuth
-
-
-def test_auth(mocker: MockerFixture) -> None:
-    """
-    Tests for the base class ``Auth``.
-    """
-    requests = mocker.patch("preset_cli.auth.main.requests")
-
-    auth = Auth()
-    assert auth.get_session() == requests.Session()
+from preset_cli.auth.password import UsernamePasswordAuth
 
 
 def test_username_password_auth(requests_mock: Mocker) -> None:
     """
     Tests for the username/password authentication mechanism.
     """
     csrf_token = "CSFR_TOKEN"
@@ -39,7 +28,28 @@
         "X-CSRFToken": csrf_token,
     }
 
     assert (
         requests_mock.last_request.text
         == "username=admin&password=password123&csrf_token=CSFR_TOKEN"
     )
+
+
+def test_username_password_auth_no_csrf(requests_mock: Mocker) -> None:
+    """
+    Tests for the username/password authentication mechanism.
+    """
+    requests_mock.get(
+        "https://superset.example.org/login/",
+        text="<html><body>WTF_CSRF_ENABLED = False</body></html>",
+    )
+    requests_mock.post("https://superset.example.org/login/")
+
+    auth = UsernamePasswordAuth(
+        URL("https://superset.example.org/"),
+        "admin",
+        "password123",
+    )
+    # pylint: disable=use-implicit-booleaness-not-comparison
+    assert auth.get_headers() == {}
+
+    assert requests_mock.last_request.text == "username=admin&password=password123"
```

### Comparing `preset-cli-0.1.1/tests/cli/main_test.py` & `preset-cli-0.2.0/tests/cli/superset/sync/dbt/lib_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,516 +1,558 @@
 """
-Tests for ``preset_cli.cli.main``.
+Test for ``preset_cli.cli.superset.sync.dbt.lib``.
 """
-# pylint: disable=unused-argument, invalid-name, redefined-outer-name
+# pylint: disable=invalid-name
 
+import json
+import math
 from pathlib import Path
-from typing import Any, Dict
+from typing import List
 
 import pytest
-import yaml
-from click.testing import CliRunner
 from pyfakefs.fake_filesystem import FakeFilesystem
 from pytest_mock import MockerFixture
-from yarl import URL
 
-from preset_cli.cli.main import (
-    get_status_icon,
-    parse_selection,
-    preset_cli,
-    split_comma,
+from preset_cli.api.clients.dbt import ModelSchema
+from preset_cli.cli.superset.sync.dbt.lib import (
+    apply_select,
+    as_number,
+    build_sqlalchemy_params,
+    env_var,
+    filter_models,
+    load_profiles,
 )
 
 
-def test_split_comma(mocker: MockerFixture) -> None:
+def test_build_sqlalchemy_params_postgres(mocker: MockerFixture) -> None:
     """
-    Test ``split_comma``.
-
-    This is used to split workspaces passed in the CLI.
-    """
-    ctx = mocker.MagicMock()
-    assert split_comma(
-        ctx,
-        "workspaces",
-        "https://ws1.preset.io/,https://ws3.preset.io/, https://ws2.preset.io/",
-    ) == [
-        "https://ws1.preset.io/",
-        "https://ws3.preset.io/",
-        "https://ws2.preset.io/",
-    ]
-    assert split_comma(ctx, "workspaces", None) == []
-
-
-def test_get_status_icon() -> None:
-    """
-    Test ``get_status_icon``.
-    """
-    assert get_status_icon("READY") == "✅"
-    assert get_status_icon("LOADING_EXAMPLES") == "📊"
-    assert get_status_icon("CREATING_DB") == "💾"
-    assert get_status_icon("INITIALIZING_DB") == "💾"
-    assert get_status_icon("MIGRATING_DB") == "🚧"
-    assert get_status_icon("ROTATING_SECRETS") == "🕵️"
-    assert get_status_icon("UNKNOWN") == "❓"
-    assert get_status_icon("ERROR") == "❗️"
-    assert get_status_icon("UPGRADING") == "⤴️"
-    assert get_status_icon("INVALID") == "❓"
-
-
-def test_parse_selection() -> None:
-    """
-    Test ``parse_selection``.
-    """
-    assert parse_selection("1-4,7", 10) == [1, 2, 3, 4, 7]
-    assert parse_selection("-4", 10) == [1, 2, 3, 4]
-    assert parse_selection("4-", 10) == [4, 5, 6, 7, 8, 9, 10]
-
-    with pytest.raises(Exception) as excinfo:
-        parse_selection("1-20", 10)
-    assert str(excinfo.value) == "End 20 is greater than 10"
-    with pytest.raises(Exception) as excinfo:
-        parse_selection("20", 10)
-    assert str(excinfo.value) == "Number 20 is greater than 10"
-
-
-def test_auth(mocker: MockerFixture) -> None:
-    """
-    Test the ``auth`` command.
-    """
-    credentials_path = Path("/path/to/config/credentials.yaml")
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
-    )
-    webbrowser = mocker.patch("preset_cli.cli.main.webbrowser")
-    mocker.patch("preset_cli.cli.main.input", return_value="API_TOKEN")
-    getpass = mocker.patch("preset_cli.cli.main.getpass")
-    getpass.getpass.return_value = "API_SECRET"
-    store_credentials = mocker.patch("preset_cli.cli.main.store_credentials")
-
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "auth"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
-
-    webbrowser.open.assert_called_with("https://manage.app.preset.io/app/user")
-    store_credentials.assert_called_with(
-        "API_TOKEN",
-        "API_SECRET",
-        URL("https://manage.app.preset.io/"),
-        credentials_path,
-    )
-
-
-def test_auth_show(mocker: MockerFixture, fs: FakeFilesystem) -> None:
-    """
-    Test the ``auth --show`` command.
-    """
-    credentials_path = Path("/path/to/config/credentials.yaml")
-    fs.create_file(
-        credentials_path,
-        contents=yaml.dump(
-            {
-                "baseurl": "https://manage.app.preset.io/",
-                "api_secret": "XXX",
-                "api_token": "abc",
-            },
-        ),
-    )
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
-    )
-
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "auth", "--show"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
-    assert (
-        result.output
-        == """/path/to/config/credentials.yaml
-================================
-api_secret: XXX
-api_token: abc
-baseurl: https://manage.app.preset.io/
-
-"""
-    )
-
-
-def test_auth_show_no_credentials(mocker: MockerFixture, fs: FakeFilesystem) -> None:
-    """
-    Test the ``auth --show`` command when there are no credentials.
+    Test ``build_sqlalchemy_params`` for PostgreSQL.
     """
-    credentials_path = Path("/path/to/config/credentials.yaml")
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
-    )
-
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "auth", "--show"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 1
-    assert result.output == (
-        "The file /path/to/config/credentials.yaml doesn't exist. "
-        "Run ``preset-cli auth`` to create it.\n"
+    _logger = mocker.patch("preset_cli.cli.superset.sync.dbt.lib._logger")
+    config = {
+        "type": "postgres",
+        "user": "username",
+        "password": "password123",
+        "host": "localhost",
+        "port": 5432,
+        "dbname": "db",
+    }
+    assert build_sqlalchemy_params(config) == {
+        "sqlalchemy_uri": "postgresql+psycopg2://username:password123@localhost:5432/db",
+    }
+    _logger.warning.assert_not_called()
+    config["search_path"] = "test_schema"
+    build_sqlalchemy_params(config)
+    _logger.warning.assert_called_with(
+        "Specifying a search path is not supported in Apache Superset",
     )
 
 
-def test_auth_overwrite(mocker: MockerFixture, fs: FakeFilesystem) -> None:
-    """
-    Test the ``auth`` command when credentials already exist.
-    """
-    credentials_path = Path("/path/to/config/credentials.yaml")
-    fs.create_file(credentials_path)
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
+def test_build_sqlalchemy_params_redshift(mocker: MockerFixture) -> None:
+    """
+    Test ``build_sqlalchemy_params`` for Redshift.
+    """
+    _logger = mocker.patch("preset_cli.cli.superset.sync.dbt.lib._logger")
+    config = {
+        "type": "redshift",
+        "user": "username",
+        "password": "password123",
+        "host": "localhost",
+        "port": 5432,
+        "dbname": "db",
+    }
+    assert build_sqlalchemy_params(config) == {
+        "sqlalchemy_uri": "redshift+psycopg2://username:password123@localhost:5432/db",
+    }
+    _logger.warning.assert_not_called()
+    config["search_path"] = "test_schema"
+    build_sqlalchemy_params(config)
+    _logger.warning.assert_called_with(
+        "Specifying a search path is not supported in Apache Superset",
     )
 
-    runner = CliRunner()
 
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "auth"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 1
-
-    mocker.patch("preset_cli.cli.main.webbrowser")
-    mocker.patch("preset_cli.cli.main.input", return_value="API_TOKEN")
-    getpass = mocker.patch("preset_cli.cli.main.getpass")
-    getpass.getpass.return_value = "API_SECRET"
-    mocker.patch("preset_cli.cli.main.store_credentials")
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "auth", "--overwrite"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
-
-
-def test_auth_overwrite_expired_credentials(
-    mocker: MockerFixture,
-    fs: FakeFilesystem,
-) -> None:
+def test_build_sqlalchemy_params_bigquery(fs: FakeFilesystem) -> None:
     """
-    Test the ``auth`` command when overwriting expired credentials.
+    Test ``build_sqlalchemy_params`` for BigQuery.
     """
-    credentials_path = Path("/path/to/config/credentials.yaml")
     fs.create_file(
-        credentials_path,
-        contents=yaml.dump({"api_secret": "API_SECRET", "api_token": "API_TOKEN"}),
-    )
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
-    )
-    get_access_token = mocker.patch(
-        "preset_cli.cli.main.get_access_token",
-        side_effect=Exception("Unable to get access token"),
+        "/path/to/credentials.json",
+        contents=json.dumps({"Hello": "World!"}),
     )
+    config = {
+        "type": "bigquery",
+        "project": "my_project",
+        "keyfile": "/path/to/credentials.json",
+    }
+    assert build_sqlalchemy_params(config) == {
+        "sqlalchemy_uri": "bigquery://my_project/",
+        "encrypted_extra": json.dumps({"credentials_info": {"Hello": "World!"}}),
+    }
 
-    runner = CliRunner()
 
-    mocker.patch("preset_cli.cli.main.webbrowser")
-    mocker.patch("preset_cli.cli.main.input", return_value="API_TOKEN")
-    getpass = mocker.patch("preset_cli.cli.main.getpass")
-    getpass.getpass.return_value = "API_SECRET"
-    mocker.patch("preset_cli.cli.main.store_credentials")
-    result = runner.invoke(
-        preset_cli,
-        ["auth", "--overwrite"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
-    get_access_token.assert_called_with(
-        URL("https://manage.app.preset.io/"),
-        "API_TOKEN",
-        "API_SECRET",
-    )
-
-
-def test_jwt_token_credentials_exist(
-    mocker: MockerFixture,
-    fs: FakeFilesystem,
-) -> None:
-    """
-    Test the command when the credentials are stored.
+def test_build_sqlalchemy_params_bigquery_with_priority(fs: FakeFilesystem) -> None:
     """
-    credentials_path = Path("/path/to/config/credentials.yaml")
-    fs.create_file(
-        credentials_path,
-        contents=yaml.dump({"api_secret": "API_SECRET", "api_token": "API_TOKEN"}),
-    )
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
-    )
-    mocker.patch("preset_cli.cli.main.get_access_token", return_value="JWT_TOKEN")
-    JWTAuth = mocker.patch("preset_cli.cli.main.JWTAuth")
-
-    runner = CliRunner()
-    result = runner.invoke(preset_cli, ["auth", "--help"], catch_exceptions=False)
-    assert result.exit_code == 0
-    JWTAuth.assert_called_with("JWT_TOKEN")
+    Test ``build_sqlalchemy_params`` for BigQuery with priority parameter.
 
-
-def test_jwt_token_invalid_credentials(
-    mocker: MockerFixture,
-    fs: FakeFilesystem,
-) -> None:
+    Parameter should be uppercase.
     """
-    Test the command when the credentials are stored.
-    """
-    credentials_path = Path("/path/to/config/credentials.yaml")
     fs.create_file(
-        credentials_path,
-        contents=yaml.dump({"api_token": "API_TOKEN"}),
+        "/path/to/credentials.json",
+        contents=json.dumps({"Hello": "World!"}),
     )
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
+    config = {
+        "type": "bigquery",
+        "project": "my_project",
+        "keyfile": "/path/to/credentials.json",
+        "priority": "interactive",
+    }
+    assert build_sqlalchemy_params(config) == {
+        "sqlalchemy_uri": "bigquery://my_project/?priority=INTERACTIVE",
+        "encrypted_extra": json.dumps({"credentials_info": {"Hello": "World!"}}),
+    }
+
+
+def test_build_sqlalchemy_params_bigquery_no_keyfile() -> None:
+    """
+    Test ``build_sqlalchemy_params`` for BigQuery with priority parameter.
+
+    Parameter should be uppercase.
+    """
+    config = {
+        "type": "bigquery",
+        "project": "my_project",
+    }
+    with pytest.raises(Exception) as excinfo:
+        build_sqlalchemy_params(config)
+    assert (
+        str(excinfo.value)
+        == "Only service account auth is supported, you MUST pass `keyfile`."
     )
-    mocker.patch("preset_cli.cli.main.get_access_token", return_value="JWT_TOKEN")
-
-    runner = CliRunner()
-    result = runner.invoke(preset_cli, ["auth", "--help"], catch_exceptions=False)
-    assert result.exit_code == 1
 
 
-def test_jwt_token_prompt_for_credentials(
-    mocker: MockerFixture,
-    fs: FakeFilesystem,
-) -> None:
+def test_build_snowflake_sqlalchemy_params() -> None:
     """
-    Test the command when the credentials are stored.
+    Test ``build_snowflake_sqlalchemy_params`` for Snowflake.
     """
-    credentials_path = Path("/path/to/config/credentials.yaml")
-    mocker.patch(
-        "preset_cli.cli.main.get_credentials_path",
-        return_value=credentials_path,
-    )
-    mocker.patch("preset_cli.cli.main.webbrowser")
-    mocker.patch("preset_cli.cli.main.input", return_value="API_TOKEN")
-    getpass = mocker.patch("preset_cli.cli.main.getpass")
-    getpass.getpass.return_value = "API_SECRET"
-    mocker.patch("preset_cli.cli.main.store_credentials")
-    mocker.patch("preset_cli.cli.main.get_access_token", return_value="JWT_TOKEN")
-    JWTAuth = mocker.patch("preset_cli.cli.main.JWTAuth")
-
-    runner = CliRunner()
-    result = runner.invoke(preset_cli, ["auth", "--help"], catch_exceptions=False)
-    assert result.exit_code == 0
-    JWTAuth.assert_called_with("JWT_TOKEN")
+    config = {
+        "type": "snowflake",
+        "account": "abc123.eu-west-1.aws",
+        "user": "jdoe",
+        "password": "secret",
+        "role": "admin",
+        "database": "default",
+        "warehouse": "dunder-mifflin",
+    }
+    assert build_sqlalchemy_params(config) == {
+        "sqlalchemy_uri": (
+            "snowflake://jdoe:secret@abc123.eu-west-1.aws/default?"
+            "role=admin&warehouse=dunder-mifflin"
+        ),
+    }
 
 
-def test_jwt_token_credentials_passed(
-    mocker: MockerFixture,
-    fs: FakeFilesystem,
-) -> None:
+def test_build_snowflake_sqlalchemy_params_pk(fs: FakeFilesystem) -> None:
     """
-    Test the command when the credentials are stored.
+    Test ``build_snowflake_sqlalchemy_params`` for Snowflake with private keys.
     """
-    mocker.patch("preset_cli.cli.main.get_access_token", return_value="JWT_TOKEN")
-    JWTAuth = mocker.patch("preset_cli.cli.main.JWTAuth")
+    fs.create_file("/path/to/key", contents="-----BEGIN ENCRYPTED PRIVATE KEY")
 
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--api-token", "API_TOKEN", "--api-secret", "API_SECRET", "auth", "--help"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
-    JWTAuth.assert_called_with("JWT_TOKEN")
+    config = {
+        "type": "snowflake",
+        "account": "abc123.eu-west-1.aws",
+        "user": "jdoe",
+        "password": "secret",
+        "role": "admin",
+        "database": "default",
+        "warehouse": "dunder-mifflin",
+        "private_key_path": "/path/to/key",
+        "private_key_passphrase": "XXX",
+    }
+    assert build_sqlalchemy_params(config) == {
+        "sqlalchemy_uri": (
+            "snowflake://jdoe:secret@abc123.eu-west-1.aws/default?"
+            "role=admin&warehouse=dunder-mifflin"
+        ),
+        "encrypted_extra": json.dumps(
+            {
+                "auth_method": "keypair",
+                "auth_params": {
+                    "privatekey_body": "-----BEGIN ENCRYPTED PRIVATE KEY",
+                    "privatekey_pass": "XXX",
+                },
+            },
+        ),
+    }
 
 
-def test_workspaces(mocker: MockerFixture) -> None:
+def test_build_snowflake_sqlalchemy_params_mfa() -> None:
     """
-    Test that we prompt user for their workspaces if not specified.
+    Test ``build_snowflake_sqlalchemy_params`` for Snowflake with MFA.
     """
-    PresetClient = mocker.patch("preset_cli.cli.main.PresetClient")
-    client = PresetClient()
-    client.get_teams.return_value = [{"name": "botafogo", "title": "Alvinegro"}]
-    client.get_workspaces.return_value = [
-        {"workspace_status": "READY", "title": "My Workspace", "hostname": "ws1"},
-        {"workspace_status": "READY", "title": "My Other Workspace", "hostname": "ws2"},
-    ]
-    mocker.patch("preset_cli.cli.main.input", side_effect=["invalid", "-"])
-
-    runner = CliRunner()
-    obj: Dict[str, Any] = {}
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "superset", "--help"],
-        catch_exceptions=False,
-        obj=obj,
-    )
-    assert result.exit_code == 0
-    assert obj["WORKSPACES"] == ["https://ws1", "https://ws2"]
+    config = {
+        "type": "snowflake",
+        "account": "abc123.eu-west-1.aws",
+        "user": "jdoe",
+        "password": "secret",
+        "authenticator": "DUO code",
+        "role": "admin",
+        "database": "default",
+        "warehouse": "dunder-mifflin",
+    }
+    assert build_sqlalchemy_params(config) == {
+        "sqlalchemy_uri": (
+            "snowflake://jdoe:secret@abc123.eu-west-1.aws/default?"
+            "role=admin&warehouse=dunder-mifflin"
+        ),
+        "extra": json.dumps(
+            {"engine_params": {"connect_args": {"passcode": "DUO code"}}},
+        ),
+    }
 
 
-def test_workspaces_single_workspace(mocker: MockerFixture) -> None:
+def test_build_sqlalchemy_params_unsupported() -> None:
     """
-    Test that we don't prompt user for their workspaces if they have only one.
+    Test ``build_sqlalchemy_params`` for databases currently unsupported.
     """
-    PresetClient = mocker.patch("preset_cli.cli.main.PresetClient")
-    client = PresetClient()
-    client.get_teams.return_value = [{"name": "botafogo", "title": "Alvinegro"}]
-    client.get_workspaces.return_value = [
-        {"workspace_status": "READY", "title": "My Workspace", "hostname": "ws1"},
-    ]
-    parse_selection = mocker.patch(
-        "preset_cli.cli.main.parse_selection",
-    )
-
-    runner = CliRunner()
-    obj: Dict[str, Any] = {}
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "superset", "--help"],
-        catch_exceptions=False,
-        obj=obj,
-    )
-    assert result.exit_code == 0
-    assert obj["WORKSPACES"] == ["https://ws1"]
-    parse_selection.assert_not_called()
-
-
-def test_workspaces_no_workspaces(mocker: MockerFixture) -> None:
-    """
-    Test when no workspaces are available.
-    """
-    PresetClient = mocker.patch("preset_cli.cli.main.PresetClient")
-    client = PresetClient()
-    client.get_teams.return_value = [{"name": "botafogo", "title": "Alvinegro"}]
-    client.get_workspaces.return_value = []
-    mocker.patch("preset_cli.cli.main.input", side_effect=["invalid", "-"])
-
-    runner = CliRunner()
-    obj: Dict[str, Any] = {}
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token", "JWT_TOKEN", "superset", "--help"],
-        catch_exceptions=False,
-        obj=obj,
+    config = {"type": "mysql"}
+    with pytest.raises(Exception) as excinfo:
+        build_sqlalchemy_params(config)
+    assert str(excinfo.value) == (
+        "Unable to build a SQLAlchemy URI for a target of type mysql. Please file "
+        "an issue at https://github.com/preset-io/backend-sdk/issues/new?"
+        "labels=enhancement&title=Backend+for+mysql."
     )
-    assert result.exit_code == 1
 
 
-def test_invite_users(mocker: MockerFixture, fs: FakeFilesystem) -> None:
+def test_env_var(monkeypatch: pytest.MonkeyPatch) -> None:
     """
-    Test the ``invite_users`` command.
+    Test the ``env_var`` implementation.
     """
-    PresetClient = mocker.patch("preset_cli.cli.main.PresetClient")
-    client = PresetClient()
-    users = [
-        {"email": "adoe@example.com"},
-        {"email": "bdoe@example.com"},
-    ]
-    fs.create_file("users.yaml", contents=yaml.dump(users))
-
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token=XXX", "invite-users", "--teams=team1"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
+    monkeypatch.setenv("MY_USER", "Nanna")
 
-    client.invite_users.assert_called_with(
-        ["team1"],
-        ["adoe@example.com", "bdoe@example.com"],
-    )
+    assert env_var("MY_USER") == "Nanna"
+    assert env_var("YOUR_USER", "Jane Doe") == "Jane Doe"
+    with pytest.raises(Exception) as excinfo:
+        env_var("YOUR_USER")
+    assert str(excinfo.value) == "Env var required but not provided: 'YOUR_USER'"
 
 
-def test_invite_users_choose_teams(mocker: MockerFixture, fs: FakeFilesystem) -> None:
+def test_as_number() -> None:
     """
-    Test the ``invite_users`` command when no teams are passed.
+    Test ``as_number`` macro.
     """
-    PresetClient = mocker.patch("preset_cli.cli.main.PresetClient")
-    client = PresetClient()
-    client.get_teams.return_value = [
-        {"name": "botafogo", "title": "Alvinegro"},
-        {"name": "flamengo", "title": "Rubro-Negro"},
-    ]
-    mocker.patch("preset_cli.cli.main.input", side_effect=["invalid", "-"])
-    users = [
-        {"email": "adoe@example.com"},
-        {"email": "bdoe@example.com"},
-    ]
-    fs.create_file("users.yaml", contents=yaml.dump(users))
-
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token=XXX", "invite-users"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
-
-    client.invite_users.assert_called_with(
-        ["botafogo", "flamengo"],
-        ["adoe@example.com", "bdoe@example.com"],
-    )
+    assert as_number("1.0") == 1
+    assert as_number("1.1") == 1.1
+    assert as_number("2") == 2
+    assert math.isnan(as_number("nan"))
+    with pytest.raises(ValueError) as excinfo:
+        as_number("invalid")
+    assert str(excinfo.value) == "could not convert string to float: 'invalid'"
 
 
-def test_invite_users_no_teams(mocker: MockerFixture, fs: FakeFilesystem) -> None:
+def test_load_profiles(monkeypatch: pytest.MonkeyPatch, fs: FakeFilesystem) -> None:
     """
-    Test the ``invite_users`` command when no teams are available.
+    Test ``load_profiles``.
     """
-    PresetClient = mocker.patch("preset_cli.cli.main.PresetClient")
-    client = PresetClient()
-    client.get_teams.return_value = []
-    mocker.patch("preset_cli.cli.main.input", side_effect=["invalid", "-"])
-
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token=XXX", "invite-users"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 1
+    monkeypatch.setenv("REDSHIFT_HOST", "127.0.0.1")
+    monkeypatch.setenv("REDSHIFT_PORT", "1234")
+    monkeypatch.setenv("REDSHIFT_USER", "username")
+    monkeypatch.setenv("REDSHIFT_PASSWORD", "password123")
+    monkeypatch.setenv("REDSHIFT_DATABASE", "db")
+    monkeypatch.setenv("THREADS", "3")
+
+    path = Path("/path/to/profiles.yml")
+    fs.create_file(
+        path,
+        contents="""
+jaffle_shop:
+  outputs:
+    dev:
+      host: "{{ env_var('REDSHIFT_HOST') | as_text }}"
+      port: "{{ env_var('REDSHIFT_PORT') | as_number }}"
+      user: "{{ env_var('REDSHIFT_USER') }}"
+      pass: "{{ env_var('REDSHIFT_PASSWORD') }}"
+      dbname: "{{ env_var('REDSHIFT_DATABASE') }}"
+      schema: public
+      threads: "{{ env_var('THREADS') | as_native }}"
+      type: postgres
+      enabled: "{{ (target.name == 'prod') | as_bool }}"
+      a_list: [1, 2, 3]
+      a_value: 10
+  target: dev
+    """,
+    )
+
+    assert load_profiles(path, "jaffle_shop", "jaffle_shop", "dev") == {
+        "jaffle_shop": {
+            "outputs": {
+                "dev": {
+                    "host": "127.0.0.1",
+                    "port": 1234,
+                    "user": "username",
+                    "pass": "password123",
+                    "dbname": "db",
+                    "schema": "public",
+                    "threads": 3,
+                    "type": "postgres",
+                    "enabled": False,
+                    "a_list": [1, 2, 3],
+                    "a_value": 10,
+                },
+            },
+            "target": "dev",
+        },
+    }
 
 
-def test_invite_users_single_team(mocker: MockerFixture, fs: FakeFilesystem) -> None:
+def test_load_profiles_default_target(
+    monkeypatch: pytest.MonkeyPatch,
+    fs: FakeFilesystem,
+) -> None:
     """
-    Test the ``invite_users`` command doesn't prompt for teams when only one is available.
+    Test ``load_profiles`` when no target is specified.
     """
-    PresetClient = mocker.patch("preset_cli.cli.main.PresetClient")
-    client = PresetClient()
-    client.get_teams.return_value = [
-        {"name": "botafogo", "title": "Alvinegro"},
-    ]
-    mocker.patch("preset_cli.cli.main.input", side_effect=["invalid", "-"])
-    parse_selection = mocker.patch(
-        "preset_cli.cli.main.parse_selection",
-    )
-    users = [
-        {"email": "adoe@example.com"},
-        {"email": "bdoe@example.com"},
-    ]
-    fs.create_file("users.yaml", contents=yaml.dump(users))
-
-    runner = CliRunner()
-    result = runner.invoke(
-        preset_cli,
-        ["--jwt-token=XXX", "invite-users"],
-        catch_exceptions=False,
-    )
-    assert result.exit_code == 0
+    monkeypatch.setenv("REDSHIFT_HOST", "127.0.0.1")
+    monkeypatch.setenv("REDSHIFT_PORT", "1234")
+    monkeypatch.setenv("REDSHIFT_USER", "username")
+    monkeypatch.setenv("REDSHIFT_PASSWORD", "password123")
+    monkeypatch.setenv("REDSHIFT_DATABASE", "db")
+    monkeypatch.setenv("THREADS", "3")
 
-    client.invite_users.assert_called_with(
-        ["botafogo"],
-        ["adoe@example.com", "bdoe@example.com"],
-    )
-    parse_selection.assert_not_called()
+    path = Path("/path/to/profiles.yml")
+    fs.create_file(
+        path,
+        contents="""
+jaffle_shop:
+  outputs:
+    dev:
+      host: "{{ env_var('REDSHIFT_HOST') | as_text }}"
+      port: "{{ env_var('REDSHIFT_PORT') | as_number }}"
+      user: "{{ env_var('REDSHIFT_USER') }}"
+      pass: "{{ env_var('REDSHIFT_PASSWORD') }}"
+      dbname: "{{ env_var('REDSHIFT_DATABASE') }}"
+      schema: public
+      threads: "{{ env_var('THREADS') | as_native }}"
+      type: postgres
+      enabled: "{{ (target.name == 'prod') | as_bool }}"
+      a_list: [1, 2, 3]
+      a_value: 10
+  target: dev
+    """,
+    )
+
+    assert load_profiles(path, "jaffle_shop", "jaffle_shop", None) == {
+        "jaffle_shop": {
+            "outputs": {
+                "dev": {
+                    "host": "127.0.0.1",
+                    "port": 1234,
+                    "user": "username",
+                    "pass": "password123",
+                    "dbname": "db",
+                    "schema": "public",
+                    "threads": 3,
+                    "type": "postgres",
+                    "enabled": False,
+                    "a_list": [1, 2, 3],
+                    "a_value": 10,
+                },
+            },
+            "target": "dev",
+        },
+    }
+
+
+def test_filter_models() -> None:
+    """
+    Test ``filter_models``.
+    """
+    one = {
+        "name": "one",
+        "tags": ["test"],
+        "unique_id": "model.one",
+        "depends_on": ["source.zero"],
+        "children": ["model.two"],
+    }
+    two = {
+        "name": "two",
+        "tags": [],
+        "unique_id": "model.two",
+        "depends_on": ["model.one", "model.three"],
+    }
+    three = {
+        "name": "three",
+        "tags": [],
+        "unique_id": "model.three",
+        "depends_on": ["source.zero"],
+        "children": ["model.two"],
+        "config": {
+            "materialized": "view",
+            "persist_docs": {},
+            "quoting": {},
+            "column_types": {},
+        },
+    }
+    models: List[ModelSchema] = [one, two, three]  # type: ignore
+
+    assert {model["name"] for model in filter_models(models, "one")} == {"one"}
+    assert {model["name"] for model in filter_models(models, "one+")} == {
+        "one",
+        "two",
+    }
+    assert {model["name"] for model in filter_models(models, "+two")} == {
+        "one",
+        "two",
+        "three",
+    }
+    assert {model["name"] for model in filter_models(models, "tag:test")} == {"one"}
+    assert {model["name"] for model in filter_models(models, "@one")} == {
+        "one",
+        "two",
+        "three",
+    }
+
+    # testing config filtering
+    assert {
+        model["name"] for model in filter_models(models, "config.materialized:view")
+    } == {"three"}
+
+    with pytest.raises(NotImplementedError) as excinfo:
+        filter_models(models, "invalid")
+    assert str(excinfo.value) == (
+        "Unable to parse the selection invalid. Please file an issue at "
+        "https://github.com/preset-io/backend-sdk/issues/new?"
+        "labels=enhancement&title=dbt+select+invalid."
+    )
+
+
+def test_filter_models_seen() -> None:
+    """
+    Test that ``filter_models`` dedupes models.
+    """
+    one = {
+        "name": "one",
+        "tags": [],
+        "unique_id": "model.one",
+        "depends_on": ["source.zero"],
+        "children": ["model.two", "model.three"],
+    }
+    two = {
+        "name": "two",
+        "tags": [],
+        "unique_id": "model.two",
+        "depends_on": ["model.one"],
+        "children": ["model.four"],
+    }
+    three = {
+        "name": "three",
+        "tags": [],
+        "unique_id": "model.three",
+        "depends_on": ["model.one"],
+        "children": ["model.four"],
+    }
+    four = {
+        "name": "four",
+        "tags": [],
+        "unique_id": "model.four",
+        "depends_on": ["model.two", "model.three"],
+        "children": [],
+    }
+    models: List[ModelSchema] = [one, two, three, four]  # type: ignore
+
+    assert {model["name"] for model in filter_models(models, "+four")} == {
+        "one",
+        "two",
+        "three",
+        "four",
+    }
+    assert {model["name"] for model in filter_models(models, "one+")} == {
+        "one",
+        "two",
+        "three",
+        "four",
+    }
+    assert {model["name"] for model in filter_models(models, "1+four")} == {
+        "two",
+        "three",
+        "four",
+    }
+    assert {model["name"] for model in filter_models(models, "one+1")} == {
+        "one",
+        "two",
+        "three",
+    }
+
+
+def test_apply_select() -> None:
+    """
+    Test ``apply_select``.
+    """
+    one = {
+        "name": "one",
+        "tags": ["test"],
+        "unique_id": "model.one",
+        "depends_on": ["source.zero"],
+        "children": ["model.two"],
+    }
+    two = {
+        "name": "two",
+        "tags": [],
+        "unique_id": "model.two",
+        "depends_on": ["model.one", "model.three"],
+        "children": [],
+    }
+    three = {
+        "name": "three",
+        "tags": [],
+        "unique_id": "model.three",
+        "depends_on": ["source.zero"],
+        "children": ["model.two"],
+    }
+    models: List[ModelSchema] = [one, two, three]  # type: ignore
+
+    assert {model["name"] for model in apply_select(models, ("one", "two"), ())} == {
+        "one",
+        "two",
+    }
+    assert {model["name"] for model in apply_select(models, ("+two+",), ())} == {
+        "one",
+        "two",
+        "three",
+    }
+    assert {
+        model["name"] for model in apply_select(models, ("+two+,tag:test",), ())
+    } == {
+        "one",
+    }
+    assert {
+        model["name"] for model in apply_select(models, ("tag:test,+two+",), ())
+    } == {
+        "one",
+    }
+
+    assert {
+        model["name"]
+        for model in apply_select(models, ("+two+",), ("three", "tag:test"))
+    } == {
+        "two",
+    }
+
+
+def test_apply_select_exclude() -> None:
+    """
+    Custom tests for the ``exclude`` option.
+    """
+    a = dict(name="a", tags=[], unique_id="a", depends_on=[], children=["b", "c"])
+    b = dict(name="b", tags=[], unique_id="b", depends_on=["a"], children=["d"])
+    c = dict(name="c", tags=[], unique_id="c", depends_on=["a"], children=["d"])
+    d = dict(name="d", tags=[], unique_id="d", depends_on=["b", "c"], children=[])
+    models: List[ModelSchema] = [a, b, c, d]  # type: ignore
+
+    assert {model["name"] for model in apply_select(models, (), ("d",))} == {
+        "a",
+        "b",
+        "c",
+    }
+    assert {model["name"] for model in apply_select(models, (), ("b+", "c+"))} == {"a"}
+    assert {model["name"] for model in apply_select(models, ("a",), ("d",))} == {"a"}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `preset-cli-0.1.1/tests/cli/superset/import_test.py` & `preset-cli-0.2.0/tests/cli/superset/import_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,14 +39,40 @@
         catch_exceptions=False,
     )
     assert result.exit_code == 0
 
     client.import_rls.assert_called_with(rls[0])
 
 
+def test_import_roles(mocker: MockerFixture, fs: FakeFilesystem) -> None:
+    """
+    Test the ``import_roles`` command.
+    """
+    mocker.patch("preset_cli.cli.superset.main.UsernamePasswordAuth")
+    SupersetClient = mocker.patch("preset_cli.cli.superset.import_.SupersetClient")
+    client = SupersetClient()
+    roles = [
+        {
+            "name": "Role name",
+            "permissions": ["can do this", "can do that"],
+        },
+    ]
+    fs.create_file("roles.yaml", contents=yaml.dump(roles))
+
+    runner = CliRunner()
+    result = runner.invoke(
+        superset_cli,
+        ["https://superset.example.org/", "import-roles"],
+        catch_exceptions=False,
+    )
+    assert result.exit_code == 0
+
+    client.import_role.assert_called_with(roles[0])
+
+
 def test_import_ownership(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``import_ownership`` command.
     """
     mocker.patch("preset_cli.cli.superset.main.UsernamePasswordAuth")
     SupersetClient = mocker.patch("preset_cli.cli.superset.import_.SupersetClient")
     client = SupersetClient()
```

### Comparing `preset-cli-0.1.1/tests/cli/superset/sql_test.py` & `preset-cli-0.2.0/tests/cli/superset/sql_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.1.1/tests/cli/superset/sync/dbt/databases_test.py` & `preset-cli-0.2.0/tests/cli/superset/sync/dbt/databases_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,52 +16,91 @@
 
 def test_sync_database_new(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test ``sync_database`` when we want to import a new DB.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
-        contents=yaml.dump({"my_project": {"outputs": {"dev": {}}}}),
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
     )
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.databases.build_sqlalchemy_params",
         return_value={"sqlalchemy_uri": "dummy://"},
     )
     client = mocker.MagicMock()
     client.get_databases.return_value = []
 
     sync_database(
         client=client,
         profiles_path=Path("/path/to/.dbt/profiles.yml"),
         project_name="my_project",
+        profile_name="default",
         target_name="dev",
         import_db=True,
         disallow_edits=False,
         external_url_prefix="",
     )
 
     client.create_database.assert_called_with(
         database_name="my_project_dev",
+        is_managed_externally=False,
+        masked_encrypted_extra=None,
         sqlalchemy_uri="dummy://",
+    )
+
+
+def test_sync_database_new_default_target(
+    mocker: MockerFixture,
+    fs: FakeFilesystem,
+) -> None:
+    """
+    Test ``sync_database`` when we want to import a new DB using the default target.
+    """
+    fs.create_file(
+        "/path/to/.dbt/profiles.yml",
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}, "target": "dev"}}),
+    )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.databases.build_sqlalchemy_params",
+        return_value={"sqlalchemy_uri": "dummy://"},
+    )
+    client = mocker.MagicMock()
+    client.get_databases.return_value = []
+
+    sync_database(
+        client=client,
+        profiles_path=Path("/path/to/.dbt/profiles.yml"),
+        project_name="my_project",
+        profile_name="default",
+        target_name=None,
+        import_db=True,
+        disallow_edits=False,
+        external_url_prefix="",
+    )
+
+    client.create_database.assert_called_with(
+        database_name="my_project_dev",
         is_managed_externally=False,
+        masked_encrypted_extra=None,
+        sqlalchemy_uri="dummy://",
     )
 
 
 def test_sync_database_new_custom_sqlalchemy_uri(
     mocker: MockerFixture,
     fs: FakeFilesystem,
 ) -> None:
     """
     Test ``sync_database`` when we want to import a new DB.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
         contents=yaml.dump(
             {
-                "my_project": {
+                "default": {
                     "outputs": {
                         "dev": {
                             "meta": {
                                 "superset": {
                                     "connection_params": {
                                         "sqlalchemy_uri": "sqlite://",
                                     },
@@ -81,24 +120,26 @@
     client = mocker.MagicMock()
     client.get_databases.return_value = []
 
     sync_database(
         client=client,
         profiles_path=Path("/path/to/.dbt/profiles.yml"),
         project_name="my_project",
+        profile_name="default",
         target_name="dev",
         import_db=True,
         disallow_edits=False,
         external_url_prefix="",
     )
 
     client.create_database.assert_called_with(
         database_name="my_database",
-        sqlalchemy_uri="sqlite://",
         is_managed_externally=False,
+        masked_encrypted_extra=None,
+        sqlalchemy_uri="sqlite://",
     )
 
 
 def test_sync_database_env_var(
     mocker: MockerFixture,
     fs: FakeFilesystem,
     monkeypatch: pytest.MonkeyPatch,
@@ -108,15 +149,15 @@
     """
     monkeypatch.setenv("dsn", "sqlite://")
 
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
         contents=yaml.dump(
             {
-                "my_project": {
+                "default": {
                     "outputs": {
                         "dev": {
                             "meta": {
                                 "superset": {
                                     "connection_params": {
                                         "sqlalchemy_uri": '{{ env_var("dsn") }}',
                                     },
@@ -136,43 +177,46 @@
     client = mocker.MagicMock()
     client.get_databases.return_value = []
 
     sync_database(
         client=client,
         profiles_path=Path("/path/to/.dbt/profiles.yml"),
         project_name="my_project",
+        profile_name="default",
         target_name="dev",
         import_db=True,
         disallow_edits=False,
         external_url_prefix="",
     )
 
     client.create_database.assert_called_with(
         database_name="my_database",
-        sqlalchemy_uri="sqlite://",
         is_managed_externally=False,
+        masked_encrypted_extra=None,
+        sqlalchemy_uri="sqlite://",
     )
 
 
 def test_sync_database_no_project(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test ``sync_database`` when the project is invalid.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
-        contents=yaml.dump({"my_project": {"outputs": {"dev": {}}}}),
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
     )
     client = mocker.MagicMock()
     client.get_databases.return_value = []
 
     with pytest.raises(Exception) as excinfo:
         sync_database(
             client=client,
             profiles_path=Path("/path/to/.dbt/profiles.yml"),
-            project_name="my_other_project",
+            project_name="my_project",
+            profile_name="my_other_project",
             target_name="dev",
             import_db=True,
             disallow_edits=False,
             external_url_prefix="",
         )
     assert (
         str(excinfo.value)
@@ -182,24 +226,25 @@
 
 def test_sync_database_no_target(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test ``sync_database`` when the target is invalid.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
-        contents=yaml.dump({"my_project": {"outputs": {"dev": {}}}}),
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
     )
     client = mocker.MagicMock()
     client.get_databases.return_value = []
 
     with pytest.raises(Exception) as excinfo:
         sync_database(
             client=client,
             profiles_path=Path("/path/to/.dbt/profiles.yml"),
             project_name="my_project",
+            profile_name="default",
             target_name="prod",
             import_db=True,
             disallow_edits=False,
             external_url_prefix="",
         )
     assert (
         str(excinfo.value)
@@ -214,15 +259,15 @@
     """
     Test ``sync_database`` when multiple databases are found.
 
     This should not happen, since database names are unique.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
-        contents=yaml.dump({"my_project": {"outputs": {"dev": {}}}}),
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
     )
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.databases.build_sqlalchemy_params",
         return_value={"sqlalchemy_uri": "dummy://"},
     )
     client = mocker.MagicMock()
     client.get_databases.return_value = [
@@ -231,14 +276,15 @@
     ]
 
     with pytest.raises(Exception) as excinfo:
         sync_database(
             client=client,
             profiles_path=Path("/path/to/.dbt/profiles.yml"),
             project_name="my_project",
+            profile_name="default",
             target_name="dev",
             import_db=True,
             disallow_edits=False,
             external_url_prefix="",
         )
     assert str(excinfo.value) == "More than one database with the same name found"
 
@@ -248,62 +294,65 @@
     fs: FakeFilesystem,
 ) -> None:
     """
     Test ``sync_database`` with an external URL prefix.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
-        contents=yaml.dump({"my_project": {"outputs": {"dev": {}}}}),
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
     )
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.databases.build_sqlalchemy_params",
         return_value={"sqlalchemy_uri": "dummy://"},
     )
     client = mocker.MagicMock()
     client.get_databases.return_value = []
 
     sync_database(
         client=client,
         profiles_path=Path("/path/to/.dbt/profiles.yml"),
         project_name="my_project",
+        profile_name="default",
         target_name="dev",
         import_db=True,
         disallow_edits=True,
         external_url_prefix="https://dbt.example.org/",
     )
 
     client.create_database.assert_called_with(
         database_name="my_project_dev",
-        sqlalchemy_uri="dummy://",
-        external_url="https://dbt.example.org/#!/overview",
         is_managed_externally=True,
+        external_url="https://dbt.example.org/#!/overview",
+        sqlalchemy_uri="dummy://",
+        masked_encrypted_extra=None,
     )
 
 
 def test_sync_database_existing(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test ``sync_database`` when we want to import an existing DB.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
-        contents=yaml.dump({"my_project": {"outputs": {"dev": {}}}}),
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
     )
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.databases.build_sqlalchemy_params",
         return_value={"sqlalchemy_uri": "dummy://"},
     )
     client = mocker.MagicMock()
     client.get_databases.return_value = [
         {"id": 1, "database_name": "my_project_dev", "sqlalchemy_uri": "dummy://"},
     ]
 
     sync_database(
         client=client,
         profiles_path=Path("/path/to/.dbt/profiles.yml"),
         project_name="my_project",
+        profile_name="default",
         target_name="dev",
         import_db=True,
         disallow_edits=False,
         external_url_prefix="",
     )
 
     client.update_database.assert_called_with(
@@ -317,26 +366,61 @@
 
 def test_sync_database_new_no_import(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test ``sync_database`` when we want to import a new DB.
     """
     fs.create_file(
         "/path/to/.dbt/profiles.yml",
-        contents=yaml.dump({"my_project": {"outputs": {"dev": {}}}}),
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
     )
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.databases.build_sqlalchemy_params",
         return_value={"sqlalchemy_uri": "dummy://"},
     )
     client = mocker.MagicMock()
     client.get_databases.return_value = []
 
     with pytest.raises(DatabaseNotFoundError):
         sync_database(
             client=client,
             profiles_path=Path("/path/to/.dbt/profiles.yml"),
             project_name="my_project",
+            profile_name="default",
             target_name="dev",
             import_db=False,
             disallow_edits=False,
             external_url_prefix="",
         )
+
+
+def test_sync_database_reuse_connection(
+    mocker: MockerFixture,
+    fs: FakeFilesystem,
+) -> None:
+    """
+    Test ``sync_database`` when the connection already exists and --import-db wasn't passed.
+    """
+    fs.create_file(
+        "/path/to/.dbt/profiles.yml",
+        contents=yaml.dump({"default": {"outputs": {"dev": {}}}}),
+    )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.databases.build_sqlalchemy_params",
+        return_value={"sqlalchemy_uri": "dummy://"},
+    )
+    client = mocker.MagicMock()
+    client.get_databases.return_value = [
+        {"id": 1, "database_name": "my_project_dev", "sqlalchemy_uri": "dummy://"},
+    ]
+
+    sync_database(
+        client=client,
+        profiles_path=Path("/path/to/.dbt/profiles.yml"),
+        project_name="my_project",
+        profile_name="default",
+        target_name="dev",
+        import_db=False,
+        disallow_edits=False,
+        external_url_prefix="",
+    )
+
+    client.get_database.assert_called_with(1)
```

### Comparing `preset-cli-0.1.1/tests/cli/superset/sync/dbt/datasets_test.py` & `preset-cli-0.2.0/tests/cli/superset/sync/dbt/manifest.json`

 * *Files 23% similar despite different names*

```diff
@@ -1,523 +1,589 @@
-00000000: 2222 220a 5465 7374 7320 666f 7220 6060  """.Tests for ``
-00000010: 7072 6573 6574 5f63 6c69 2e63 6c69 2e73  preset_cli.cli.s
-00000020: 7570 6572 7365 742e 7379 6e63 2e64 6274  uperset.sync.dbt
-00000030: 2e64 6174 6173 6574 7360 602e 0a22 2222  .datasets``.."""
-00000040: 0a23 2070 796c 696e 743a 2064 6973 6162  .# pylint: disab
-00000050: 6c65 3d69 6e76 616c 6964 2d6e 616d 650a  le=invalid-name.
-00000060: 0a69 6d70 6f72 7420 6a73 6f6e 0a66 726f  .import json.fro
-00000070: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00000080: 4c69 7374 0a66 726f 6d20 756e 6974 7465  List.from unitte
-00000090: 7374 2069 6d70 6f72 7420 6d6f 636b 0a0a  st import mock..
-000000a0: 696d 706f 7274 2070 7974 6573 740a 6672  import pytest.fr
-000000b0: 6f6d 2070 7974 6573 745f 6d6f 636b 2069  om pytest_mock i
-000000c0: 6d70 6f72 7420 4d6f 636b 6572 4669 7874  mport MockerFixt
-000000d0: 7572 650a 0a66 726f 6d20 7072 6573 6574  ure..from preset
-000000e0: 5f63 6c69 2e61 7069 2e63 6c69 656e 7473  _cli.api.clients
-000000f0: 2e64 6274 2069 6d70 6f72 7420 4d65 7472  .dbt import Metr
-00000100: 6963 5363 6865 6d61 2c20 4d6f 6465 6c53  icSchema, ModelS
-00000110: 6368 656d 610a 6672 6f6d 2070 7265 7365  chema.from prese
-00000120: 745f 636c 692e 636c 692e 7375 7065 7273  t_cli.cli.supers
-00000130: 6574 2e73 796e 632e 6462 742e 6461 7461  et.sync.dbt.data
-00000140: 7365 7473 2069 6d70 6f72 7420 7379 6e63  sets import sync
-00000150: 5f64 6174 6173 6574 730a 0a6d 6574 7269  _datasets..metri
-00000160: 635f 7363 6865 6d61 203d 204d 6574 7269  c_schema = Metri
-00000170: 6353 6368 656d 6128 290a 6d65 7472 6963  cSchema().metric
-00000180: 733a 204c 6973 745b 4d65 7472 6963 5363  s: List[MetricSc
-00000190: 6865 6d61 5d20 3d20 5b0a 2020 2020 6d65  hema] = [.    me
-000001a0: 7472 6963 5f73 6368 656d 612e 6c6f 6164  tric_schema.load
-000001b0: 280a 2020 2020 2020 2020 7b0a 2020 2020  (.        {.    
-000001c0: 2020 2020 2020 2020 2264 6570 656e 6473          "depends
-000001d0: 5f6f 6e22 3a20 5b22 6d6f 6465 6c2e 7375  _on": ["model.su
-000001e0: 7065 7273 6574 5f65 7861 6d70 6c65 732e  perset_examples.
-000001f0: 6d65 7373 6167 6573 5f63 6861 6e6e 656c  messages_channel
-00000200: 7322 5d2c 0a20 2020 2020 2020 2020 2020  s"],.           
-00000210: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00000220: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
-00000230: 2266 696c 7465 7273 223a 205b 5d2c 0a20  "filters": [],. 
-00000240: 2020 2020 2020 2020 2020 2022 6d65 7461             "meta
-00000250: 223a 207b 7d2c 0a20 2020 2020 2020 2020  ": {},.         
-00000260: 2020 2022 6e61 6d65 223a 2022 636e 7422     "name": "cnt"
-00000270: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-00000280: 6162 656c 223a 2022 222c 0a20 2020 2020  abel": "",.     
-00000290: 2020 2020 2020 2022 7371 6c22 3a20 222a         "sql": "*
-000002a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000002b0: 7479 7065 223a 2022 636f 756e 7422 2c0a  type": "count",.
-000002c0: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-000002d0: 7175 655f 6964 223a 2022 6d65 7472 6963  que_id": "metric
-000002e0: 2e73 7570 6572 7365 745f 6578 616d 706c  .superset_exampl
-000002f0: 6573 2e63 6e74 222c 0a20 2020 2020 2020  es.cnt",.       
-00000300: 207d 2c0a 2020 2020 292c 0a5d 0a0a 6d6f   },.    ),.]..mo
-00000310: 6465 6c5f 7363 6865 6d61 203d 204d 6f64  del_schema = Mod
-00000320: 656c 5363 6865 6d61 2829 0a6d 6f64 656c  elSchema().model
-00000330: 733a 204c 6973 745b 4d6f 6465 6c53 6368  s: List[ModelSch
-00000340: 656d 615d 203d 205b 0a20 2020 206d 6f64  ema] = [.    mod
-00000350: 656c 5f73 6368 656d 612e 6c6f 6164 280a  el_schema.load(.
-00000360: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000370: 2020 2020 2020 2264 6174 6162 6173 6522        "database"
-00000380: 3a20 2265 7861 6d70 6c65 735f 6465 7622  : "examples_dev"
-00000390: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
-000003a0: 6368 656d 6122 3a20 2270 7562 6c69 6322  chema": "public"
-000003b0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-000003c0: 6573 6372 6970 7469 6f6e 223a 2022 222c  escription": "",
-000003d0: 0a20 2020 2020 2020 2020 2020 2022 6d65  .            "me
-000003e0: 7461 223a 207b 7d2c 0a20 2020 2020 2020  ta": {},.       
-000003f0: 2020 2020 2022 6e61 6d65 223a 2022 6d65       "name": "me
-00000400: 7373 6167 6573 5f63 6861 6e6e 656c 7322  ssages_channels"
-00000410: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
-00000420: 6e69 7175 655f 6964 223a 2022 6d6f 6465  nique_id": "mode
-00000430: 6c2e 7375 7065 7273 6574 5f65 7861 6d70  l.superset_examp
-00000440: 6c65 732e 6d65 7373 6167 6573 5f63 6861  les.messages_cha
-00000450: 6e6e 656c 7322 2c0a 2020 2020 2020 2020  nnels",.        
-00000460: 7d2c 0a20 2020 2029 2c0a 5d0a 0a0a 6465  },.    ),.]...de
-00000470: 6620 7465 7374 5f73 796e 635f 6461 7461  f test_sync_data
-00000480: 7365 7473 5f6e 6577 286d 6f63 6b65 723a  sets_new(mocker:
-00000490: 204d 6f63 6b65 7246 6978 7475 7265 2920   MockerFixture) 
-000004a0: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-000004b0: 0a20 2020 2054 6573 7420 6060 7379 6e63  .    Test ``sync
-000004c0: 5f64 6174 6173 6574 7360 6020 7768 656e  _datasets`` when
-000004d0: 206e 6f20 6461 7461 7365 7473 2065 7869   no datasets exi
-000004e0: 7374 2079 6574 2e0a 2020 2020 2222 220a  st yet..    """.
-000004f0: 2020 2020 636c 6965 6e74 203d 206d 6f63      client = moc
-00000500: 6b65 722e 4d61 6769 634d 6f63 6b28 290a  ker.MagicMock().
-00000510: 2020 2020 636c 6965 6e74 2e67 6574 5f64      client.get_d
-00000520: 6174 6173 6574 732e 7265 7475 726e 5f76  atasets.return_v
-00000530: 616c 7565 203d 205b 5d0a 2020 2020 636c  alue = [].    cl
-00000540: 6965 6e74 2e63 7265 6174 655f 6461 7461  ient.create_data
-00000550: 7365 742e 7369 6465 5f65 6666 6563 7420  set.side_effect 
-00000560: 3d20 5b7b 2269 6422 3a20 317d 2c20 7b22  = [{"id": 1}, {"
-00000570: 6964 223a 2032 7d2c 207b 2269 6422 3a20  id": 2}, {"id": 
-00000580: 337d 5d0a 0a20 2020 2073 796e 635f 6461  3}]..    sync_da
-00000590: 7461 7365 7473 280a 2020 2020 2020 2020  tasets(.        
-000005a0: 636c 6965 6e74 3d63 6c69 656e 742c 0a20  client=client,. 
-000005b0: 2020 2020 2020 206d 6f64 656c 733d 6d6f         models=mo
-000005c0: 6465 6c73 2c0a 2020 2020 2020 2020 6d65  dels,.        me
-000005d0: 7472 6963 733d 6d65 7472 6963 732c 0a20  trics=metrics,. 
-000005e0: 2020 2020 2020 2064 6174 6162 6173 653d         database=
-000005f0: 7b22 6964 223a 2031 7d2c 0a20 2020 2020  {"id": 1},.     
-00000600: 2020 2064 6973 616c 6c6f 775f 6564 6974     disallow_edit
-00000610: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-00000620: 2065 7874 6572 6e61 6c5f 7572 6c5f 7072   external_url_pr
-00000630: 6566 6978 3d22 222c 0a20 2020 2029 0a20  efix="",.    ). 
-00000640: 2020 2063 6c69 656e 742e 6372 6561 7465     client.create
-00000650: 5f64 6174 6173 6574 2e61 7373 6572 745f  _dataset.assert_
-00000660: 6861 735f 6361 6c6c 7328 0a20 2020 2020  has_calls(.     
-00000670: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00000680: 206d 6f63 6b2e 6361 6c6c 2864 6174 6162   mock.call(datab
-00000690: 6173 653d 312c 2073 6368 656d 613d 2270  ase=1, schema="p
-000006a0: 7562 6c69 6322 2c20 7461 626c 655f 6e61  ublic", table_na
-000006b0: 6d65 3d22 6d65 7373 6167 6573 5f63 6861  me="messages_cha
-000006c0: 6e6e 656c 7322 292c 0a20 2020 2020 2020  nnels"),.       
-000006d0: 205d 2c0a 2020 2020 290a 2020 2020 636c   ],.    ).    cl
-000006e0: 6965 6e74 2e75 7064 6174 655f 6461 7461  ient.update_data
-000006f0: 7365 742e 6173 7365 7274 5f68 6173 5f63  set.assert_has_c
-00000700: 616c 6c73 280a 2020 2020 2020 2020 5b0a  alls(.        [.
-00000710: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
-00000720: 2e63 616c 6c28 0a20 2020 2020 2020 2020  .call(.         
-00000730: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00000740: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00000750: 7074 696f 6e3d 2222 2c0a 2020 2020 2020  ption="",.      
-00000760: 2020 2020 2020 2020 2020 6578 7472 613d            extra=
-00000770: 6a73 6f6e 2e64 756d 7073 280a 2020 2020  json.dumps(.    
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000007a0: 2020 2020 2020 2020 2020 2275 6e69 7175            "uniqu
-000007b0: 655f 6964 223a 2022 6d6f 6465 6c2e 7375  e_id": "model.su
-000007c0: 7065 7273 6574 5f65 7861 6d70 6c65 732e  perset_examples.
-000007d0: 6d65 7373 6167 6573 5f63 6861 6e6e 656c  messages_channel
-000007e0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000007f0: 2020 2020 2020 2020 2020 2020 2264 6570              "dep
-00000800: 656e 6473 5f6f 6e22 3a20 2272 6566 2827  ends_on": "ref('
-00000810: 6d65 7373 6167 6573 5f63 6861 6e6e 656c  messages_channel
-00000820: 7327 2922 2c0a 2020 2020 2020 2020 2020  s')",.          
-00000830: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00000840: 6572 7469 6669 6361 7469 6f6e 223a 207b  ertification": {
-00000850: 2264 6574 6169 6c73 223a 2022 5468 6973  "details": "This
-00000860: 2074 6162 6c65 2069 7320 7072 6f64 7563   table is produc
-00000870: 6564 2062 7920 6462 7422 7d2c 0a20 2020  ed by dbt"},.   
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000008a0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-000008b0: 2020 2020 2020 2069 735f 6d61 6e61 6765         is_manage
-000008c0: 645f 6578 7465 726e 616c 6c79 3d46 616c  d_externally=Fal
-000008d0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-000008e0: 2020 2020 6d65 7472 6963 733d 5b5d 2c0a      metrics=[],.
-000008f0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00000900: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
-00000910: 6361 6c6c 280a 2020 2020 2020 2020 2020  call(.          
-00000920: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
-00000930: 2020 2020 2020 2020 206d 6574 7269 6373           metrics
-00000940: 3d5b 0a20 2020 2020 2020 2020 2020 2020  =[.             
-00000950: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2022 6578 7072 6573 7369 6f6e 223a 2022   "expression": "
-00000980: 434f 554e 5428 2a29 222c 0a20 2020 2020  COUNT(*)",.     
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2020 2022 6d65 7472 6963 5f6e 616d 6522     "metric_name"
-000009b0: 3a20 2263 6e74 222c 0a20 2020 2020 2020  : "cnt",.       
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2022 6d65 7472 6963 5f74 7970 6522 3a20   "metric_type": 
-000009e0: 2263 6f75 6e74 222c 0a20 2020 2020 2020  "count",.       
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2022 7665 7262 6f73 655f 6e61 6d65 223a   "verbose_name":
-00000a10: 2022 636e 7422 2c0a 2020 2020 2020 2020   "cnt",.        
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00000a40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000a50: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000a60: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00000a70: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00000a80: 2020 2020 5d2c 0a20 2020 2029 0a0a 0a64      ],.    )...d
-00000a90: 6566 2074 6573 745f 7379 6e63 5f64 6174  ef test_sync_dat
-00000aa0: 6173 6574 735f 6e6f 5f6d 6574 7269 6373  asets_no_metrics
-00000ab0: 286d 6f63 6b65 723a 204d 6f63 6b65 7246  (mocker: MockerF
-00000ac0: 6978 7475 7265 2920 2d3e 204e 6f6e 653a  ixture) -> None:
-00000ad0: 0a20 2020 2022 2222 0a20 2020 2054 6573  .    """.    Tes
-00000ae0: 7420 6060 7379 6e63 5f64 6174 6173 6574  t ``sync_dataset
-00000af0: 7360 6020 7768 656e 206e 6f20 6461 7461  s`` when no data
-00000b00: 7365 7473 2065 7869 7374 2079 6574 2e0a  sets exist yet..
-00000b10: 2020 2020 2222 220a 2020 2020 636c 6965      """.    clie
-00000b20: 6e74 203d 206d 6f63 6b65 722e 4d61 6769  nt = mocker.Magi
-00000b30: 634d 6f63 6b28 290a 2020 2020 636c 6965  cMock().    clie
-00000b40: 6e74 2e67 6574 5f64 6174 6173 6574 732e  nt.get_datasets.
-00000b50: 7265 7475 726e 5f76 616c 7565 203d 205b  return_value = [
-00000b60: 5d0a 2020 2020 636c 6965 6e74 2e63 7265  ].    client.cre
-00000b70: 6174 655f 6461 7461 7365 742e 7369 6465  ate_dataset.side
-00000b80: 5f65 6666 6563 7420 3d20 5b7b 2269 6422  _effect = [{"id"
-00000b90: 3a20 317d 2c20 7b22 6964 223a 2032 7d2c  : 1}, {"id": 2},
-00000ba0: 207b 2269 6422 3a20 337d 5d0a 0a20 2020   {"id": 3}]..   
-00000bb0: 2073 796e 635f 6461 7461 7365 7473 280a   sync_datasets(.
-00000bc0: 2020 2020 2020 2020 636c 6965 6e74 3d63          client=c
-00000bd0: 6c69 656e 742c 0a20 2020 2020 2020 206d  lient,.        m
-00000be0: 6f64 656c 733d 6d6f 6465 6c73 2c0a 2020  odels=models,.  
-00000bf0: 2020 2020 2020 6d65 7472 6963 733d 5b5d        metrics=[]
-00000c00: 2c0a 2020 2020 2020 2020 6461 7461 6261  ,.        databa
-00000c10: 7365 3d7b 2269 6422 3a20 317d 2c0a 2020  se={"id": 1},.  
-00000c20: 2020 2020 2020 6469 7361 6c6c 6f77 5f65        disallow_e
-00000c30: 6469 7473 3d46 616c 7365 2c0a 2020 2020  dits=False,.    
-00000c40: 2020 2020 6578 7465 726e 616c 5f75 726c      external_url
-00000c50: 5f70 7265 6669 783d 2222 2c0a 2020 2020  _prefix="",.    
-00000c60: 290a 2020 2020 636c 6965 6e74 2e63 7265  ).    client.cre
-00000c70: 6174 655f 6461 7461 7365 742e 6173 7365  ate_dataset.asse
-00000c80: 7274 5f68 6173 5f63 616c 6c73 280a 2020  rt_has_calls(.  
-00000c90: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00000ca0: 2020 2020 6d6f 636b 2e63 616c 6c28 6461      mock.call(da
-00000cb0: 7461 6261 7365 3d31 2c20 7363 6865 6d61  tabase=1, schema
-00000cc0: 3d22 7075 626c 6963 222c 2074 6162 6c65  ="public", table
-00000cd0: 5f6e 616d 653d 226d 6573 7361 6765 735f  _name="messages_
-00000ce0: 6368 616e 6e65 6c73 2229 2c0a 2020 2020  channels"),.    
-00000cf0: 2020 2020 5d2c 0a20 2020 2029 0a20 2020      ],.    ).   
-00000d00: 2063 6c69 656e 742e 7570 6461 7465 5f64   client.update_d
-00000d10: 6174 6173 6574 2e61 7373 6572 745f 6861  ataset.assert_ha
-00000d20: 735f 6361 6c6c 7328 0a20 2020 2020 2020  s_calls(.       
-00000d30: 205b 0a20 2020 2020 2020 2020 2020 206d   [.            m
-00000d40: 6f63 6b2e 6361 6c6c 280a 2020 2020 2020  ock.call(.      
-00000d50: 2020 2020 2020 2020 2020 312c 0a20 2020            1,.   
-00000d60: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00000d70: 6372 6970 7469 6f6e 3d22 222c 0a20 2020  cription="",.   
-00000d80: 2020 2020 2020 2020 2020 2020 2065 7874               ext
-00000d90: 7261 3d6a 736f 6e2e 6475 6d70 7328 0a20  ra=json.dumps(. 
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00000dc0: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-00000dd0: 6971 7565 5f69 6422 3a20 226d 6f64 656c  ique_id": "model
-00000de0: 2e73 7570 6572 7365 745f 6578 616d 706c  .superset_exampl
-00000df0: 6573 2e6d 6573 7361 6765 735f 6368 616e  es.messages_chan
-00000e00: 6e65 6c73 222c 0a20 2020 2020 2020 2020  nels",.         
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000e20: 6465 7065 6e64 735f 6f6e 223a 2022 7265  depends_on": "re
-00000e30: 6628 276d 6573 7361 6765 735f 6368 616e  f('messages_chan
-00000e40: 6e65 6c73 2729 222c 0a20 2020 2020 2020  nels')",.       
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 2022 6365 7274 6966 6963 6174 696f 6e22   "certification"
-00000e70: 3a20 7b22 6465 7461 696c 7322 3a20 2254  : {"details": "T
-00000e80: 6869 7320 7461 626c 6520 6973 2070 726f  his table is pro
-00000e90: 6475 6365 6420 6279 2064 6274 227d 2c0a  duced by dbt"},.
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00000ec0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00000ed0: 2020 2020 2020 2020 2020 6973 5f6d 616e            is_man
-00000ee0: 6167 6564 5f65 7874 6572 6e61 6c6c 793d  aged_externally=
-00000ef0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00000f00: 2020 2020 2020 206d 6574 7269 6373 3d5b         metrics=[
-00000f10: 5d2c 0a20 2020 2020 2020 2020 2020 2029  ],.            )
-00000f20: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-00000f30: 2029 0a0a 0a64 6566 2074 6573 745f 7379   )...def test_sy
-00000f40: 6e63 5f64 6174 6173 6574 735f 6e65 775f  nc_datasets_new_
-00000f50: 6271 5f65 7272 6f72 286d 6f63 6b65 723a  bq_error(mocker:
-00000f60: 204d 6f63 6b65 7246 6978 7475 7265 2920   MockerFixture) 
-00000f70: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-00000f80: 0a20 2020 2054 6573 7420 6060 7379 6e63  .    Test ``sync
-00000f90: 5f64 6174 6173 6574 7360 6020 7768 656e  _datasets`` when
-00000fa0: 206f 6e65 206f 6620 7468 6520 736f 7572   one of the sour
-00000fb0: 6365 7320 6973 2069 6e20 6120 6469 6666  ces is in a diff
-00000fc0: 6572 656e 7420 4251 2070 726f 6a65 6374  erent BQ project
-00000fd0: 2e0a 0a20 2020 2057 6865 6e20 7468 6174  ...    When that
-00000fe0: 2068 6170 7065 6e73 2077 6520 6361 6e27   happens we can'
-00000ff0: 7420 6164 6420 7468 6520 6461 7461 7365  t add the datase
-00001000: 742c 2073 696e 6365 2053 7570 6572 7365  t, since Superse
-00001010: 7420 6361 6e27 7420 7265 6164 2074 6865  t can't read the
-00001020: 206d 6574 6164 6174 612e 0a20 2020 2022   metadata..    "
-00001030: 2222 0a20 2020 2063 6c69 656e 7420 3d20  "".    client = 
-00001040: 6d6f 636b 6572 2e4d 6167 6963 4d6f 636b  mocker.MagicMock
-00001050: 2829 0a20 2020 2063 6c69 656e 742e 6765  ().    client.ge
-00001060: 745f 6461 7461 7365 7473 2e72 6574 7572  t_datasets.retur
-00001070: 6e5f 7661 6c75 6520 3d20 5b5d 0a20 2020  n_value = [].   
-00001080: 2063 6c69 656e 742e 6372 6561 7465 5f64   client.create_d
-00001090: 6174 6173 6574 2e73 6964 655f 6566 6665  ataset.side_effe
-000010a0: 6374 203d 205b 0a20 2020 2020 2020 2045  ct = [.        E
-000010b0: 7863 6570 7469 6f6e 2822 5461 626c 6520  xception("Table 
-000010c0: 6973 2069 6e20 6120 6469 6666 6572 656e  is in a differen
-000010d0: 7420 7072 6f6a 6563 7422 292c 0a20 2020  t project"),.   
-000010e0: 205d 0a0a 2020 2020 7379 6e63 5f64 6174   ]..    sync_dat
-000010f0: 6173 6574 7328 0a20 2020 2020 2020 2063  asets(.        c
-00001100: 6c69 656e 743d 636c 6965 6e74 2c0a 2020  lient=client,.  
-00001110: 2020 2020 2020 6d6f 6465 6c73 3d6d 6f64        models=mod
-00001120: 656c 732c 0a20 2020 2020 2020 206d 6574  els,.        met
-00001130: 7269 6373 3d6d 6574 7269 6373 2c0a 2020  rics=metrics,.  
-00001140: 2020 2020 2020 6461 7461 6261 7365 3d7b        database={
-00001150: 2269 6422 3a20 317d 2c0a 2020 2020 2020  "id": 1},.      
-00001160: 2020 6469 7361 6c6c 6f77 5f65 6469 7473    disallow_edits
-00001170: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00001180: 6578 7465 726e 616c 5f75 726c 5f70 7265  external_url_pre
-00001190: 6669 783d 2222 2c0a 2020 2020 290a 2020  fix="",.    ).  
-000011a0: 2020 636c 6965 6e74 2e63 7265 6174 655f    client.create_
-000011b0: 6461 7461 7365 742e 6173 7365 7274 5f68  dataset.assert_h
-000011c0: 6173 5f63 616c 6c73 280a 2020 2020 2020  as_calls(.      
-000011d0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000011e0: 6d6f 636b 2e63 616c 6c28 6461 7461 6261  mock.call(databa
-000011f0: 7365 3d31 2c20 7363 6865 6d61 3d22 7075  se=1, schema="pu
-00001200: 626c 6963 222c 2074 6162 6c65 5f6e 616d  blic", table_nam
-00001210: 653d 226d 6573 7361 6765 735f 6368 616e  e="messages_chan
-00001220: 6e65 6c73 2229 2c0a 2020 2020 2020 2020  nels"),.        
-00001230: 5d2c 0a20 2020 2029 0a20 2020 2063 6c69  ],.    ).    cli
-00001240: 656e 742e 7570 6461 7465 5f64 6174 6173  ent.update_datas
-00001250: 6574 2e61 7373 6572 745f 6861 735f 6361  et.assert_has_ca
-00001260: 6c6c 7328 5b5d 290a 0a0a 6465 6620 7465  lls([])...def te
-00001270: 7374 5f73 796e 635f 6461 7461 7365 7473  st_sync_datasets
-00001280: 5f65 7869 7374 696e 6728 6d6f 636b 6572  _existing(mocker
-00001290: 3a20 4d6f 636b 6572 4669 7874 7572 6529  : MockerFixture)
-000012a0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-000012b0: 220a 2020 2020 5465 7374 2060 6073 796e  ".    Test ``syn
-000012c0: 635f 6461 7461 7365 7473 6060 2077 6865  c_datasets`` whe
-000012d0: 6e20 6461 7461 7365 7473 2061 6c72 6561  n datasets alrea
-000012e0: 6479 2065 7869 7374 2e0a 2020 2020 2222  dy exist..    ""
-000012f0: 220a 2020 2020 636c 6965 6e74 203d 206d  ".    client = m
-00001300: 6f63 6b65 722e 4d61 6769 634d 6f63 6b28  ocker.MagicMock(
-00001310: 290a 2020 2020 636c 6965 6e74 2e67 6574  ).    client.get
-00001320: 5f64 6174 6173 6574 732e 7369 6465 5f65  _datasets.side_e
-00001330: 6666 6563 7420 3d20 5b5b 7b22 6964 223a  ffect = [[{"id":
-00001340: 2031 7d5d 2c20 5b7b 2269 6422 3a20 327d   1}], [{"id": 2}
-00001350: 5d2c 205b 7b22 6964 223a 2033 7d5d 5d0a  ], [{"id": 3}]].
-00001360: 0a20 2020 2073 796e 635f 6461 7461 7365  .    sync_datase
-00001370: 7473 280a 2020 2020 2020 2020 636c 6965  ts(.        clie
-00001380: 6e74 3d63 6c69 656e 742c 0a20 2020 2020  nt=client,.     
-00001390: 2020 206d 6f64 656c 733d 6d6f 6465 6c73     models=models
-000013a0: 2c0a 2020 2020 2020 2020 6d65 7472 6963  ,.        metric
-000013b0: 733d 6d65 7472 6963 732c 0a20 2020 2020  s=metrics,.     
-000013c0: 2020 2064 6174 6162 6173 653d 7b22 6964     database={"id
-000013d0: 223a 2031 7d2c 0a20 2020 2020 2020 2064  ": 1},.        d
-000013e0: 6973 616c 6c6f 775f 6564 6974 733d 4661  isallow_edits=Fa
-000013f0: 6c73 652c 0a20 2020 2020 2020 2065 7874  lse,.        ext
-00001400: 6572 6e61 6c5f 7572 6c5f 7072 6566 6978  ernal_url_prefix
-00001410: 3d22 222c 0a20 2020 2029 0a20 2020 2063  ="",.    ).    c
-00001420: 6c69 656e 742e 6372 6561 7465 5f64 6174  lient.create_dat
-00001430: 6173 6574 2e61 7373 6572 745f 6e6f 745f  aset.assert_not_
-00001440: 6361 6c6c 6564 2829 0a20 2020 2063 6c69  called().    cli
-00001450: 656e 742e 7570 6461 7465 5f64 6174 6173  ent.update_datas
-00001460: 6574 2e61 7373 6572 745f 6861 735f 6361  et.assert_has_ca
-00001470: 6c6c 7328 0a20 2020 2020 2020 205b 0a20  lls(.        [. 
-00001480: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
-00001490: 6361 6c6c 280a 2020 2020 2020 2020 2020  call(.          
-000014a0: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
-000014b0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-000014c0: 7469 6f6e 3d22 222c 0a20 2020 2020 2020  tion="",.       
-000014d0: 2020 2020 2020 2020 2065 7874 7261 3d6a           extra=j
-000014e0: 736f 6e2e 6475 6d70 7328 0a20 2020 2020  son.dumps(.     
-000014f0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001510: 2020 2020 2020 2020 2022 756e 6971 7565           "unique
-00001520: 5f69 6422 3a20 226d 6f64 656c 2e73 7570  _id": "model.sup
-00001530: 6572 7365 745f 6578 616d 706c 6573 2e6d  erset_examples.m
-00001540: 6573 7361 6765 735f 6368 616e 6e65 6c73  essages_channels
-00001550: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001560: 2020 2020 2020 2020 2020 2022 6465 7065             "depe
-00001570: 6e64 735f 6f6e 223a 2022 7265 6628 276d  nds_on": "ref('m
-00001580: 6573 7361 6765 735f 6368 616e 6e65 6c73  essages_channels
-00001590: 2729 222c 0a20 2020 2020 2020 2020 2020  ')",.           
-000015a0: 2020 2020 2020 2020 2020 2020 2022 6365               "ce
-000015b0: 7274 6966 6963 6174 696f 6e22 3a20 7b22  rtification": {"
-000015c0: 6465 7461 696c 7322 3a20 2254 6869 7320  details": "This 
-000015d0: 7461 626c 6520 6973 2070 726f 6475 6365  table is produce
-000015e0: 6420 6279 2064 6274 227d 2c0a 2020 2020  d by dbt"},.    
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001610: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00001620: 2020 2020 2020 6973 5f6d 616e 6167 6564        is_managed
-00001630: 5f65 7874 6572 6e61 6c6c 793d 4661 6c73  _externally=Fals
-00001640: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001650: 2020 206d 6574 7269 6373 3d5b 5d2c 0a20     metrics=[],. 
-00001660: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00001670: 2020 2020 2020 2020 2020 6d6f 636b 2e63            mock.c
-00001680: 616c 6c28 0a20 2020 2020 2020 2020 2020  all(.           
-00001690: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
-000016a0: 2020 2020 2020 2020 6d65 7472 6963 733d          metrics=
-000016b0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-000016c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2265 7870 7265 7373 696f 6e22 3a20 2243  "expression": "C
-000016f0: 4f55 4e54 282a 2922 2c0a 2020 2020 2020  OUNT(*)",.      
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 226d 6574 7269 635f 6e61 6d65 223a    "metric_name":
-00001720: 2022 636e 7422 2c0a 2020 2020 2020 2020   "cnt",.        
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 226d 6574 7269 635f 7479 7065 223a 2022  "metric_type": "
-00001750: 636f 756e 7422 2c0a 2020 2020 2020 2020  count",.        
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2276 6572 626f 7365 5f6e 616d 6522 3a20  "verbose_name": 
-00001780: 2263 6e74 222c 0a20 2020 2020 2020 2020  "cnt",.         
-00001790: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000017a0: 6465 7363 7269 7074 696f 6e22 3a20 2222  description": ""
-000017b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000017c0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000017d0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-000017e0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000017f0: 2020 205d 2c0a 2020 2020 290a 0a0a 6465     ],.    )...de
-00001800: 6620 7465 7374 5f73 796e 635f 6461 7461  f test_sync_data
-00001810: 7365 7473 5f6d 756c 7469 706c 655f 6578  sets_multiple_ex
-00001820: 6973 7469 6e67 286d 6f63 6b65 723a 204d  isting(mocker: M
-00001830: 6f63 6b65 7246 6978 7475 7265 2920 2d3e  ockerFixture) ->
-00001840: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
-00001850: 2020 2054 6573 7420 6060 7379 6e63 5f64     Test ``sync_d
-00001860: 6174 6173 6574 7360 6020 7768 656e 206d  atasets`` when m
-00001870: 756c 7469 706c 6520 6461 7461 7365 7473  ultiple datasets
-00001880: 2061 7265 2066 6f75 6e64 2074 6f20 6578   are found to ex
-00001890: 6973 742e 0a20 2020 2022 2222 0a20 2020  ist..    """.   
-000018a0: 2063 6c69 656e 7420 3d20 6d6f 636b 6572   client = mocker
-000018b0: 2e4d 6167 6963 4d6f 636b 2829 0a20 2020  .MagicMock().   
-000018c0: 2063 6c69 656e 742e 6765 745f 6461 7461   client.get_data
-000018d0: 7365 7473 2e72 6574 7572 6e5f 7661 6c75  sets.return_valu
-000018e0: 6520 3d20 5b7b 2269 6422 3a20 317d 2c20  e = [{"id": 1}, 
-000018f0: 7b22 6964 223a 2032 7d5d 0a0a 2020 2020  {"id": 2}]..    
-00001900: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
-00001910: 6573 2845 7863 6570 7469 6f6e 2920 6173  es(Exception) as
-00001920: 2065 7863 696e 666f 3a0a 2020 2020 2020   excinfo:.      
-00001930: 2020 7379 6e63 5f64 6174 6173 6574 7328    sync_datasets(
-00001940: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00001950: 656e 743d 636c 6965 6e74 2c0a 2020 2020  ent=client,.    
-00001960: 2020 2020 2020 2020 6d6f 6465 6c73 3d6d          models=m
-00001970: 6f64 656c 732c 0a20 2020 2020 2020 2020  odels,.         
-00001980: 2020 206d 6574 7269 6373 3d6d 6574 7269     metrics=metri
-00001990: 6373 2c0a 2020 2020 2020 2020 2020 2020  cs,.            
-000019a0: 6461 7461 6261 7365 3d7b 2269 6422 3a20  database={"id": 
-000019b0: 317d 2c0a 2020 2020 2020 2020 2020 2020  1},.            
-000019c0: 6469 7361 6c6c 6f77 5f65 6469 7473 3d46  disallow_edits=F
-000019d0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000019e0: 2020 6578 7465 726e 616c 5f75 726c 5f70    external_url_p
-000019f0: 7265 6669 783d 2222 2c0a 2020 2020 2020  refix="",.      
-00001a00: 2020 290a 2020 2020 6173 7365 7274 2073    ).    assert s
-00001a10: 7472 2865 7863 696e 666f 2e76 616c 7565  tr(excinfo.value
-00001a20: 2920 3d3d 2022 4d6f 7265 2074 6861 6e20  ) == "More than 
-00001a30: 6f6e 6520 6461 7461 7365 7420 666f 756e  one dataset foun
-00001a40: 6422 0a0a 0a64 6566 2074 6573 745f 7379  d"...def test_sy
-00001a50: 6e63 5f64 6174 6173 6574 735f 6578 7465  nc_datasets_exte
-00001a60: 726e 616c 5f75 726c 286d 6f63 6b65 723a  rnal_url(mocker:
-00001a70: 204d 6f63 6b65 7246 6978 7475 7265 2920   MockerFixture) 
-00001a80: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-00001a90: 0a20 2020 2054 6573 7420 6060 7379 6e63  .    Test ``sync
-00001aa0: 5f64 6174 6173 6574 7360 6020 7768 656e  _datasets`` when
-00001ab0: 2070 6173 7369 6e67 2065 7874 6572 6e61   passing externa
-00001ac0: 6c20 5552 4c20 7072 6566 6978 2e0a 2020  l URL prefix..  
-00001ad0: 2020 2222 220a 2020 2020 636c 6965 6e74    """.    client
-00001ae0: 203d 206d 6f63 6b65 722e 4d61 6769 634d   = mocker.MagicM
-00001af0: 6f63 6b28 290a 2020 2020 636c 6965 6e74  ock().    client
-00001b00: 2e67 6574 5f64 6174 6173 6574 732e 7369  .get_datasets.si
-00001b10: 6465 5f65 6666 6563 7420 3d20 5b5b 7b22  de_effect = [[{"
-00001b20: 6964 223a 2031 7d5d 2c20 5b7b 2269 6422  id": 1}], [{"id"
-00001b30: 3a20 327d 5d2c 205b 7b22 6964 223a 2033  : 2}], [{"id": 3
-00001b40: 7d5d 5d0a 0a20 2020 2073 796e 635f 6461  }]]..    sync_da
-00001b50: 7461 7365 7473 280a 2020 2020 2020 2020  tasets(.        
-00001b60: 636c 6965 6e74 3d63 6c69 656e 742c 0a20  client=client,. 
-00001b70: 2020 2020 2020 206d 6f64 656c 733d 6d6f         models=mo
-00001b80: 6465 6c73 2c0a 2020 2020 2020 2020 6d65  dels,.        me
-00001b90: 7472 6963 733d 6d65 7472 6963 732c 0a20  trics=metrics,. 
-00001ba0: 2020 2020 2020 2064 6174 6162 6173 653d         database=
-00001bb0: 7b22 6964 223a 2031 7d2c 0a20 2020 2020  {"id": 1},.     
-00001bc0: 2020 2064 6973 616c 6c6f 775f 6564 6974     disallow_edit
-00001bd0: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-00001be0: 2065 7874 6572 6e61 6c5f 7572 6c5f 7072   external_url_pr
-00001bf0: 6566 6978 3d22 6874 7470 733a 2f2f 6462  efix="https://db
-00001c00: 742e 6578 616d 706c 652e 6f72 672f 222c  t.example.org/",
-00001c10: 0a20 2020 2029 0a20 2020 2063 6c69 656e  .    ).    clien
-00001c20: 742e 6372 6561 7465 5f64 6174 6173 6574  t.create_dataset
-00001c30: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-00001c40: 6564 2829 0a20 2020 2063 6c69 656e 742e  ed().    client.
-00001c50: 7570 6461 7465 5f64 6174 6173 6574 2e61  update_dataset.a
-00001c60: 7373 6572 745f 6861 735f 6361 6c6c 7328  ssert_has_calls(
-00001c70: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
-00001c80: 2020 2020 2020 206d 6f63 6b2e 6361 6c6c         mock.call
-00001c90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00001ca0: 2020 312c 0a20 2020 2020 2020 2020 2020    1,.           
-00001cb0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00001cc0: 3d22 222c 0a20 2020 2020 2020 2020 2020  ="",.           
-00001cd0: 2020 2020 2065 7874 7261 3d6a 736f 6e2e       extra=json.
-00001ce0: 6475 6d70 7328 0a20 2020 2020 2020 2020  dumps(.         
-00001cf0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2020 2022 756e 6971 7565 5f69 6422       "unique_id"
-00001d20: 3a20 226d 6f64 656c 2e73 7570 6572 7365  : "model.superse
-00001d30: 745f 6578 616d 706c 6573 2e6d 6573 7361  t_examples.messa
-00001d40: 6765 735f 6368 616e 6e65 6c73 222c 0a20  ges_channels",. 
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 2020 2022 6465 7065 6e64 735f         "depends_
-00001d70: 6f6e 223a 2022 7265 6628 276d 6573 7361  on": "ref('messa
-00001d80: 6765 735f 6368 616e 6e65 6c73 2729 222c  ges_channels')",
-00001d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001da0: 2020 2020 2020 2020 2022 6365 7274 6966           "certif
-00001db0: 6963 6174 696f 6e22 3a20 7b22 6465 7461  ication": {"deta
-00001dc0: 696c 7322 3a20 2254 6869 7320 7461 626c  ils": "This tabl
-00001dd0: 6520 6973 2070 726f 6475 6365 6420 6279  e is produced by
-00001de0: 2064 6274 227d 2c0a 2020 2020 2020 2020   dbt"},.        
-00001df0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00001e10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001e20: 2020 6973 5f6d 616e 6167 6564 5f65 7874    is_managed_ext
-00001e30: 6572 6e61 6c6c 793d 4661 6c73 652c 0a20  ernally=False,. 
-00001e40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00001e50: 6574 7269 6373 3d5b 5d2c 0a20 2020 2020  etrics=[],.     
-00001e60: 2020 2020 2020 2020 2020 2065 7874 6572             exter
-00001e70: 6e61 6c5f 7572 6c3d 280a 2020 2020 2020  nal_url=(.      
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2268                "h
-00001e90: 7474 7073 3a2f 2f64 6274 2e65 7861 6d70  ttps://dbt.examp
-00001ea0: 6c65 2e6f 7267 2f23 2122 0a20 2020 2020  le.org/#!".     
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001ec0: 2f6d 6f64 656c 2f6d 6f64 656c 2e73 7570  /model/model.sup
-00001ed0: 6572 7365 745f 6578 616d 706c 6573 2e6d  erset_examples.m
-00001ee0: 6573 7361 6765 735f 6368 616e 6e65 6c73  essages_channels
-00001ef0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00001f00: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00001f10: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00001f20: 6d6f 636b 2e63 616c 6c28 0a20 2020 2020  mock.call(.     
-00001f30: 2020 2020 2020 2020 2020 2031 2c0a 2020             1,.  
-00001f40: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00001f50: 7472 6963 733d 5b0a 2020 2020 2020 2020  trics=[.        
-00001f60: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 2020 2265 7870 7265 7373 696f        "expressio
-00001f90: 6e22 3a20 2243 4f55 4e54 282a 2922 2c0a  n": "COUNT(*)",.
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fb0: 2020 2020 2020 2020 226d 6574 7269 635f          "metric_
-00001fc0: 6e61 6d65 223a 2022 636e 7422 2c0a 2020  name": "cnt",.  
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 2020 2020 2020 226d 6574 7269 635f 7479        "metric_ty
-00001ff0: 7065 223a 2022 636f 756e 7422 2c0a 2020  pe": "count",.  
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2020 2020 2276 6572 626f 7365 5f6e        "verbose_n
-00002020: 616d 6522 3a20 2263 6e74 222c 0a20 2020  ame": "cnt",.   
-00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002040: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00002050: 6e22 3a20 2222 2c0a 2020 2020 2020 2020  n": "",.        
-00002060: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00002070: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00002080: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
-00002090: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-000020a0: 290a                                     ).
+00000000: 7b0a 2020 226d 6574 7269 6373 223a 207b  {.  "metrics": {
+00000010: 0a20 2020 2022 6d65 7472 6963 2e73 7570  .    "metric.sup
+00000020: 6572 7365 745f 6578 616d 706c 6573 2e63  erset_examples.c
+00000030: 6e74 223a 207b 0a20 2020 2020 2022 6671  nt": {.      "fq
+00000040: 6e22 3a20 5b0a 2020 2020 2020 2020 2273  n": [.        "s
+00000050: 7570 6572 7365 745f 6578 616d 706c 6573  uperset_examples
+00000060: 222c 0a20 2020 2020 2020 2022 736c 6163  ",.        "slac
+00000070: 6b22 2c0a 2020 2020 2020 2020 2263 6e74  k",.        "cnt
+00000080: 220a 2020 2020 2020 5d2c 0a20 2020 2020  ".      ],.     
+00000090: 2022 756e 6971 7565 5f69 6422 3a20 226d   "unique_id": "m
+000000a0: 6574 7269 632e 7375 7065 7273 6574 5f65  etric.superset_e
+000000b0: 7861 6d70 6c65 732e 636e 7422 2c0a 2020  xamples.cnt",.  
+000000c0: 2020 2020 2270 6163 6b61 6765 5f6e 616d      "package_nam
+000000d0: 6522 3a20 2273 7570 6572 7365 745f 6578  e": "superset_ex
+000000e0: 616d 706c 6573 222c 0a20 2020 2020 2022  amples",.      "
+000000f0: 726f 6f74 5f70 6174 6822 3a20 222f 5573  root_path": "/Us
+00000100: 6572 732f 6265 746f 2f50 726f 6a65 6374  ers/beto/Project
+00000110: 732f 6462 742d 6578 616d 706c 6573 2f73  s/dbt-examples/s
+00000120: 7570 6572 7365 745f 6578 616d 706c 6573  uperset_examples
+00000130: 222c 0a20 2020 2020 2022 7061 7468 223a  ",.      "path":
+00000140: 2022 736c 6163 6b2f 7363 6865 6d61 2e79   "slack/schema.y
+00000150: 6d6c 222c 0a20 2020 2020 2022 6f72 6967  ml",.      "orig
+00000160: 696e 616c 5f66 696c 655f 7061 7468 223a  inal_file_path":
+00000170: 2022 6d6f 6465 6c73 2f73 6c61 636b 2f73   "models/slack/s
+00000180: 6368 656d 612e 796d 6c22 2c0a 2020 2020  chema.yml",.    
+00000190: 2020 226d 6f64 656c 223a 2022 7265 6628    "model": "ref(
+000001a0: 276d 6573 7361 6765 735f 6368 616e 6e65  'messages_channe
+000001b0: 6c73 2729 222c 0a20 2020 2020 2022 6e61  ls')",.      "na
+000001c0: 6d65 223a 2022 636e 7422 2c0a 2020 2020  me": "cnt",.    
+000001d0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+000001e0: 2022 222c 0a20 2020 2020 2022 6c61 6265   "",.      "labe
+000001f0: 6c22 3a20 2222 2c0a 2020 2020 2020 2274  l": "",.      "t
+00000200: 7970 6522 3a20 2263 6f75 6e74 222c 0a20  ype": "count",. 
+00000210: 2020 2020 2022 7371 6c22 3a20 222a 222c       "sql": "*",
+00000220: 0a20 2020 2020 2022 7469 6d65 7374 616d  .      "timestam
+00000230: 7022 3a20 6e75 6c6c 2c0a 2020 2020 2020  p": null,.      
+00000240: 2266 696c 7465 7273 223a 205b 5d2c 0a20  "filters": [],. 
+00000250: 2020 2020 2022 7469 6d65 5f67 7261 696e       "time_grain
+00000260: 7322 3a20 5b5d 2c0a 2020 2020 2020 2264  s": [],.      "d
+00000270: 696d 656e 7369 6f6e 7322 3a20 5b5d 2c0a  imensions": [],.
+00000280: 2020 2020 2020 2272 6573 6f75 7263 655f        "resource_
+00000290: 7479 7065 223a 2022 6d65 7472 6963 222c  type": "metric",
+000002a0: 0a20 2020 2020 2022 6d65 7461 223a 207b  .      "meta": {
+000002b0: 7d2c 0a20 2020 2020 2022 7461 6773 223a  },.      "tags":
+000002c0: 205b 5d2c 0a20 2020 2020 2022 736f 7572   [],.      "sour
+000002d0: 6365 7322 3a20 5b5d 2c0a 2020 2020 2020  ces": [],.      
+000002e0: 2264 6570 656e 6473 5f6f 6e22 3a20 7b0a  "depends_on": {.
+000002f0: 2020 2020 2020 2020 226d 6163 726f 7322          "macros"
+00000300: 3a20 5b5d 2c0a 2020 2020 2020 2020 226e  : [],.        "n
+00000310: 6f64 6573 223a 205b 0a20 2020 2020 2020  odes": [.       
+00000320: 2020 2022 6d6f 6465 6c2e 7375 7065 7273     "model.supers
+00000330: 6574 5f65 7861 6d70 6c65 732e 6d65 7373  et_examples.mess
+00000340: 6167 6573 5f63 6861 6e6e 656c 7322 0a20  ages_channels". 
+00000350: 2020 2020 2020 205d 0a20 2020 2020 207d         ].      }
+00000360: 2c0a 2020 2020 2020 2272 6566 7322 3a20  ,.      "refs": 
+00000370: 5b0a 2020 2020 2020 2020 5b0a 2020 2020  [.        [.    
+00000380: 2020 2020 2020 226d 6573 7361 6765 735f        "messages_
+00000390: 6368 616e 6e65 6c73 220a 2020 2020 2020  channels".      
+000003a0: 2020 5d0a 2020 2020 2020 5d2c 0a20 2020    ].      ],.   
+000003b0: 2020 2022 6372 6561 7465 645f 6174 223a     "created_at":
+000003c0: 2031 3634 3236 3330 3938 362e 3139 3432   1642630986.1942
+000003d0: 3835 320a 2020 2020 7d0a 2020 7d2c 0a20  852.    }.  },. 
+000003e0: 2022 736f 7572 6365 7322 3a20 7b0a 2020   "sources": {.  
+000003f0: 2020 2273 6f75 7263 652e 7375 7065 7273    "source.supers
+00000400: 6574 5f65 7861 6d70 6c65 732e 7075 626c  et_examples.publ
+00000410: 6963 2e6d 6573 7361 6765 7322 3a20 7b0a  ic.messages": {.
+00000420: 2020 2020 2020 2266 716e 223a 205b 0a20        "fqn": [. 
+00000430: 2020 2020 2020 2022 7375 7065 7273 6574         "superset
+00000440: 5f65 7861 6d70 6c65 7322 2c0a 2020 2020  _examples",.    
+00000450: 2020 2020 2273 6c61 636b 222c 0a20 2020      "slack",.   
+00000460: 2020 2020 2022 7075 626c 6963 222c 0a20       "public",. 
+00000470: 2020 2020 2020 2022 6d65 7373 6167 6573         "messages
+00000480: 220a 2020 2020 2020 5d2c 0a20 2020 2020  ".      ],.     
+00000490: 2022 6461 7461 6261 7365 223a 2022 6578   "database": "ex
+000004a0: 616d 706c 6573 5f64 6576 222c 0a20 2020  amples_dev",.   
+000004b0: 2020 2022 7363 6865 6d61 223a 2022 7075     "schema": "pu
+000004c0: 626c 6963 222c 0a20 2020 2020 2022 756e  blic",.      "un
+000004d0: 6971 7565 5f69 6422 3a20 2273 6f75 7263  ique_id": "sourc
+000004e0: 652e 7375 7065 7273 6574 5f65 7861 6d70  e.superset_examp
+000004f0: 6c65 732e 7075 626c 6963 2e6d 6573 7361  les.public.messa
+00000500: 6765 7322 2c0a 2020 2020 2020 2270 6163  ges",.      "pac
+00000510: 6b61 6765 5f6e 616d 6522 3a20 2273 7570  kage_name": "sup
+00000520: 6572 7365 745f 6578 616d 706c 6573 222c  erset_examples",
+00000530: 0a20 2020 2020 2022 726f 6f74 5f70 6174  .      "root_pat
+00000540: 6822 3a20 222f 5573 6572 732f 6265 746f  h": "/Users/beto
+00000550: 2f50 726f 6a65 6374 732f 6462 742d 6578  /Projects/dbt-ex
+00000560: 616d 706c 6573 2f73 7570 6572 7365 745f  amples/superset_
+00000570: 6578 616d 706c 6573 222c 0a20 2020 2020  examples",.     
+00000580: 2022 7061 7468 223a 2022 6d6f 6465 6c73   "path": "models
+00000590: 2f73 6c61 636b 2f73 6368 656d 612e 796d  /slack/schema.ym
+000005a0: 6c22 2c0a 2020 2020 2020 226f 7269 6769  l",.      "origi
+000005b0: 6e61 6c5f 6669 6c65 5f70 6174 6822 3a20  nal_file_path": 
+000005c0: 226d 6f64 656c 732f 736c 6163 6b2f 7363  "models/slack/sc
+000005d0: 6865 6d61 2e79 6d6c 222c 0a20 2020 2020  hema.yml",.     
+000005e0: 2022 6e61 6d65 223a 2022 6d65 7373 6167   "name": "messag
+000005f0: 6573 222c 0a20 2020 2020 2022 736f 7572  es",.      "sour
+00000600: 6365 5f6e 616d 6522 3a20 2270 7562 6c69  ce_name": "publi
+00000610: 6322 2c0a 2020 2020 2020 2273 6f75 7263  c",.      "sourc
+00000620: 655f 6465 7363 7269 7074 696f 6e22 3a20  e_description": 
+00000630: 2222 2c0a 2020 2020 2020 226c 6f61 6465  "",.      "loade
+00000640: 7222 3a20 2222 2c0a 2020 2020 2020 2269  r": "",.      "i
+00000650: 6465 6e74 6966 6965 7222 3a20 226d 6573  dentifier": "mes
+00000660: 7361 6765 7322 2c0a 2020 2020 2020 2272  sages",.      "r
+00000670: 6573 6f75 7263 655f 7479 7065 223a 2022  esource_type": "
+00000680: 736f 7572 6365 222c 0a20 2020 2020 2022  source",.      "
+00000690: 7175 6f74 696e 6722 3a20 7b0a 2020 2020  quoting": {.    
+000006a0: 2020 2020 2264 6174 6162 6173 6522 3a20      "database": 
+000006b0: 6e75 6c6c 2c0a 2020 2020 2020 2020 2273  null,.        "s
+000006c0: 6368 656d 6122 3a20 6e75 6c6c 2c0a 2020  chema": null,.  
+000006d0: 2020 2020 2020 2269 6465 6e74 6966 6965        "identifie
+000006e0: 7222 3a20 6e75 6c6c 2c0a 2020 2020 2020  r": null,.      
+000006f0: 2020 2263 6f6c 756d 6e22 3a20 6e75 6c6c    "column": null
+00000700: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
+00000710: 226c 6f61 6465 645f 6174 5f66 6965 6c64  "loaded_at_field
+00000720: 223a 206e 756c 6c2c 0a20 2020 2020 2022  ": null,.      "
+00000730: 6672 6573 686e 6573 7322 3a20 7b0a 2020  freshness": {.  
+00000740: 2020 2020 2020 2277 6172 6e5f 6166 7465        "warn_afte
+00000750: 7222 3a20 7b0a 2020 2020 2020 2020 2020  r": {.          
+00000760: 2263 6f75 6e74 223a 206e 756c 6c2c 0a20  "count": null,. 
+00000770: 2020 2020 2020 2020 2022 7065 7269 6f64           "period
+00000780: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
+00000790: 7d2c 0a20 2020 2020 2020 2022 6572 726f  },.        "erro
+000007a0: 725f 6166 7465 7222 3a20 7b0a 2020 2020  r_after": {.    
+000007b0: 2020 2020 2020 2263 6f75 6e74 223a 206e        "count": n
+000007c0: 756c 6c2c 0a20 2020 2020 2020 2020 2022  ull,.          "
+000007d0: 7065 7269 6f64 223a 206e 756c 6c0a 2020  period": null.  
+000007e0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000007f0: 2022 6669 6c74 6572 223a 206e 756c 6c0a   "filter": null.
+00000800: 2020 2020 2020 7d2c 0a20 2020 2020 2022        },.      "
+00000810: 6578 7465 726e 616c 223a 206e 756c 6c2c  external": null,
+00000820: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
+00000830: 696f 6e22 3a20 224d 6573 7361 6765 7320  ion": "Messages 
+00000840: 696e 2074 6865 2053 6c61 636b 2063 6861  in the Slack cha
+00000850: 6e6e 656c 222c 0a20 2020 2020 2022 636f  nnel",.      "co
+00000860: 6c75 6d6e 7322 3a20 7b7d 2c0a 2020 2020  lumns": {},.    
+00000870: 2020 226d 6574 6122 3a20 7b7d 2c0a 2020    "meta": {},.  
+00000880: 2020 2020 2273 6f75 7263 655f 6d65 7461      "source_meta
+00000890: 223a 207b 7d2c 0a20 2020 2020 2022 7461  ": {},.      "ta
+000008a0: 6773 223a 205b 5d2c 0a20 2020 2020 2022  gs": [],.      "
+000008b0: 636f 6e66 6967 223a 207b 0a20 2020 2020  config": {.     
+000008c0: 2020 2022 656e 6162 6c65 6422 3a20 7472     "enabled": tr
+000008d0: 7565 0a20 2020 2020 207d 2c0a 2020 2020  ue.      },.    
+000008e0: 2020 2270 6174 6368 5f70 6174 6822 3a20    "patch_path": 
+000008f0: 6e75 6c6c 2c0a 2020 2020 2020 2275 6e72  null,.      "unr
+00000900: 656e 6465 7265 645f 636f 6e66 6967 223a  endered_config":
+00000910: 207b 7d2c 0a20 2020 2020 2022 7265 6c61   {},.      "rela
+00000920: 7469 6f6e 5f6e 616d 6522 3a20 225c 2265  tion_name": "\"e
+00000930: 7861 6d70 6c65 735f 6465 765c 222e 5c22  xamples_dev\".\"
+00000940: 7075 626c 6963 5c22 2e5c 226d 6573 7361  public\".\"messa
+00000950: 6765 735c 2222 2c0a 2020 2020 2020 2263  ges\"",.      "c
+00000960: 7265 6174 6564 5f61 7422 3a20 3136 3432  reated_at": 1642
+00000970: 3632 3839 3333 2e30 3433 3231 3839 0a20  628933.0432189. 
+00000980: 2020 207d 2c0a 2020 2020 2273 6f75 7263     },.    "sourc
+00000990: 652e 7375 7065 7273 6574 5f65 7861 6d70  e.superset_examp
+000009a0: 6c65 732e 7075 626c 6963 2e63 6861 6e6e  les.public.chann
+000009b0: 656c 7322 3a20 7b0a 2020 2020 2020 2266  els": {.      "f
+000009c0: 716e 223a 205b 0a20 2020 2020 2020 2022  qn": [.        "
+000009d0: 7375 7065 7273 6574 5f65 7861 6d70 6c65  superset_example
+000009e0: 7322 2c0a 2020 2020 2020 2020 2273 6c61  s",.        "sla
+000009f0: 636b 222c 0a20 2020 2020 2020 2022 7075  ck",.        "pu
+00000a00: 626c 6963 222c 0a20 2020 2020 2020 2022  blic",.        "
+00000a10: 6368 616e 6e65 6c73 220a 2020 2020 2020  channels".      
+00000a20: 5d2c 0a20 2020 2020 2022 6461 7461 6261  ],.      "databa
+00000a30: 7365 223a 2022 6578 616d 706c 6573 5f64  se": "examples_d
+00000a40: 6576 222c 0a20 2020 2020 2022 7363 6865  ev",.      "sche
+00000a50: 6d61 223a 2022 7075 626c 6963 222c 0a20  ma": "public",. 
+00000a60: 2020 2020 2022 756e 6971 7565 5f69 6422       "unique_id"
+00000a70: 3a20 2273 6f75 7263 652e 7375 7065 7273  : "source.supers
+00000a80: 6574 5f65 7861 6d70 6c65 732e 7075 626c  et_examples.publ
+00000a90: 6963 2e63 6861 6e6e 656c 7322 2c0a 2020  ic.channels",.  
+00000aa0: 2020 2020 2270 6163 6b61 6765 5f6e 616d      "package_nam
+00000ab0: 6522 3a20 2273 7570 6572 7365 745f 6578  e": "superset_ex
+00000ac0: 616d 706c 6573 222c 0a20 2020 2020 2022  amples",.      "
+00000ad0: 726f 6f74 5f70 6174 6822 3a20 222f 5573  root_path": "/Us
+00000ae0: 6572 732f 6265 746f 2f50 726f 6a65 6374  ers/beto/Project
+00000af0: 732f 6462 742d 6578 616d 706c 6573 2f73  s/dbt-examples/s
+00000b00: 7570 6572 7365 745f 6578 616d 706c 6573  uperset_examples
+00000b10: 222c 0a20 2020 2020 2022 7061 7468 223a  ",.      "path":
+00000b20: 2022 6d6f 6465 6c73 2f73 6c61 636b 2f73   "models/slack/s
+00000b30: 6368 656d 612e 796d 6c22 2c0a 2020 2020  chema.yml",.    
+00000b40: 2020 226f 7269 6769 6e61 6c5f 6669 6c65    "original_file
+00000b50: 5f70 6174 6822 3a20 226d 6f64 656c 732f  _path": "models/
+00000b60: 736c 6163 6b2f 7363 6865 6d61 2e79 6d6c  slack/schema.yml
+00000b70: 222c 0a20 2020 2020 2022 6e61 6d65 223a  ",.      "name":
+00000b80: 2022 6368 616e 6e65 6c73 222c 0a20 2020   "channels",.   
+00000b90: 2020 2022 736f 7572 6365 5f6e 616d 6522     "source_name"
+00000ba0: 3a20 2270 7562 6c69 6322 2c0a 2020 2020  : "public",.    
+00000bb0: 2020 2273 6f75 7263 655f 6465 7363 7269    "source_descri
+00000bc0: 7074 696f 6e22 3a20 2222 2c0a 2020 2020  ption": "",.    
+00000bd0: 2020 226c 6f61 6465 7222 3a20 2222 2c0a    "loader": "",.
+00000be0: 2020 2020 2020 2269 6465 6e74 6966 6965        "identifie
+00000bf0: 7222 3a20 2263 6861 6e6e 656c 7322 2c0a  r": "channels",.
+00000c00: 2020 2020 2020 2272 6573 6f75 7263 655f        "resource_
+00000c10: 7479 7065 223a 2022 736f 7572 6365 222c  type": "source",
+00000c20: 0a20 2020 2020 2022 7175 6f74 696e 6722  .      "quoting"
+00000c30: 3a20 7b0a 2020 2020 2020 2020 2264 6174  : {.        "dat
+00000c40: 6162 6173 6522 3a20 6e75 6c6c 2c0a 2020  abase": null,.  
+00000c50: 2020 2020 2020 2273 6368 656d 6122 3a20        "schema": 
+00000c60: 6e75 6c6c 2c0a 2020 2020 2020 2020 2269  null,.        "i
+00000c70: 6465 6e74 6966 6965 7222 3a20 6e75 6c6c  dentifier": null
+00000c80: 2c0a 2020 2020 2020 2020 2263 6f6c 756d  ,.        "colum
+00000c90: 6e22 3a20 6e75 6c6c 0a20 2020 2020 207d  n": null.      }
+00000ca0: 2c0a 2020 2020 2020 226c 6f61 6465 645f  ,.      "loaded_
+00000cb0: 6174 5f66 6965 6c64 223a 206e 756c 6c2c  at_field": null,
+00000cc0: 0a20 2020 2020 2022 6672 6573 686e 6573  .      "freshnes
+00000cd0: 7322 3a20 7b0a 2020 2020 2020 2020 2277  s": {.        "w
+00000ce0: 6172 6e5f 6166 7465 7222 3a20 7b0a 2020  arn_after": {.  
+00000cf0: 2020 2020 2020 2020 2263 6f75 6e74 223a          "count":
+00000d00: 206e 756c 6c2c 0a20 2020 2020 2020 2020   null,.         
+00000d10: 2022 7065 7269 6f64 223a 206e 756c 6c0a   "period": null.
+00000d20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000d30: 2020 2022 6572 726f 725f 6166 7465 7222     "error_after"
+00000d40: 3a20 7b0a 2020 2020 2020 2020 2020 2263  : {.          "c
+00000d50: 6f75 6e74 223a 206e 756c 6c2c 0a20 2020  ount": null,.   
+00000d60: 2020 2020 2020 2022 7065 7269 6f64 223a         "period":
+00000d70: 206e 756c 6c0a 2020 2020 2020 2020 7d2c   null.        },
+00000d80: 0a20 2020 2020 2020 2022 6669 6c74 6572  .        "filter
+00000d90: 223a 206e 756c 6c0a 2020 2020 2020 7d2c  ": null.      },
+00000da0: 0a20 2020 2020 2022 6578 7465 726e 616c  .      "external
+00000db0: 223a 206e 756c 6c2c 0a20 2020 2020 2022  ": null,.      "
+00000dc0: 6465 7363 7269 7074 696f 6e22 3a20 2249  description": "I
+00000dd0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+00000de0: 2053 6c61 636b 2063 6861 6e6e 656c 7322   Slack channels"
+00000df0: 2c0a 2020 2020 2020 2263 6f6c 756d 6e73  ,.      "columns
+00000e00: 223a 207b 7d2c 0a20 2020 2020 2022 6d65  ": {},.      "me
+00000e10: 7461 223a 207b 7d2c 0a20 2020 2020 2022  ta": {},.      "
+00000e20: 736f 7572 6365 5f6d 6574 6122 3a20 7b7d  source_meta": {}
+00000e30: 2c0a 2020 2020 2020 2274 6167 7322 3a20  ,.      "tags": 
+00000e40: 5b5d 2c0a 2020 2020 2020 2263 6f6e 6669  [],.      "confi
+00000e50: 6722 3a20 7b0a 2020 2020 2020 2020 2265  g": {.        "e
+00000e60: 6e61 626c 6564 223a 2074 7275 650a 2020  nabled": true.  
+00000e70: 2020 2020 7d2c 0a20 2020 2020 2022 7061      },.      "pa
+00000e80: 7463 685f 7061 7468 223a 206e 756c 6c2c  tch_path": null,
+00000e90: 0a20 2020 2020 2022 756e 7265 6e64 6572  .      "unrender
+00000ea0: 6564 5f63 6f6e 6669 6722 3a20 7b7d 2c0a  ed_config": {},.
+00000eb0: 2020 2020 2020 2272 656c 6174 696f 6e5f        "relation_
+00000ec0: 6e61 6d65 223a 2022 5c22 6578 616d 706c  name": "\"exampl
+00000ed0: 6573 5f64 6576 5c22 2e5c 2270 7562 6c69  es_dev\".\"publi
+00000ee0: 635c 222e 5c22 6368 616e 6e65 6c73 5c22  c\".\"channels\"
+00000ef0: 222c 0a20 2020 2020 2022 6372 6561 7465  ",.      "create
+00000f00: 645f 6174 223a 2031 3634 3236 3238 3933  d_at": 164262893
+00000f10: 332e 3034 3333 3838 0a20 2020 207d 0a20  3.043388.    }. 
+00000f20: 207d 2c0a 2020 226e 6f64 6573 223a 207b   },.  "nodes": {
+00000f30: 0a20 2020 2022 6d6f 6465 6c2e 7375 7065  .    "model.supe
+00000f40: 7273 6574 5f65 7861 6d70 6c65 732e 6d65  rset_examples.me
+00000f50: 7373 6167 6573 5f63 6861 6e6e 656c 7322  ssages_channels"
+00000f60: 3a20 7b0a 2020 2020 2020 2272 6177 5f73  : {.      "raw_s
+00000f70: 716c 223a 2022 5345 4c45 4354 206d 6573  ql": "SELECT mes
+00000f80: 7361 6765 732e 7473 2c20 6368 616e 6e65  sages.ts, channe
+00000f90: 6c73 2e6e 616d 652c 206d 6573 7361 6765  ls.name, message
+00000fa0: 732e 7465 7874 2046 524f 4d20 7b7b 2073  s.text FROM {{ s
+00000fb0: 6f75 7263 6520 2827 7075 626c 6963 272c  ource ('public',
+00000fc0: 2027 6d65 7373 6167 6573 2729 207d 7d20   'messages') }} 
+00000fd0: 6d65 7373 6167 6573 204a 4f49 4e20 7b7b  messages JOIN {{
+00000fe0: 2073 6f75 7263 6520 2827 7075 626c 6963   source ('public
+00000ff0: 272c 2027 6368 616e 6e65 6c73 2729 207d  ', 'channels') }
+00001000: 7d20 6368 616e 6e65 6c73 204f 4e20 6d65  } channels ON me
+00001010: 7373 6167 6573 2e63 6861 6e6e 656c 5f69  ssages.channel_i
+00001020: 6420 3d20 6368 616e 6e65 6c73 2e69 6422  d = channels.id"
+00001030: 2c0a 2020 2020 2020 2263 6f6d 7069 6c65  ,.      "compile
+00001040: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
+00001050: 2272 6573 6f75 7263 655f 7479 7065 223a  "resource_type":
+00001060: 2022 6d6f 6465 6c22 2c0a 2020 2020 2020   "model",.      
+00001070: 2264 6570 656e 6473 5f6f 6e22 3a20 7b0a  "depends_on": {.
+00001080: 2020 2020 2020 2020 226d 6163 726f 7322          "macros"
+00001090: 3a20 5b5d 2c0a 2020 2020 2020 2020 226e  : [],.        "n
+000010a0: 6f64 6573 223a 205b 0a20 2020 2020 2020  odes": [.       
+000010b0: 2020 2022 736f 7572 6365 2e73 7570 6572     "source.super
+000010c0: 7365 745f 6578 616d 706c 6573 2e70 7562  set_examples.pub
+000010d0: 6c69 632e 6368 616e 6e65 6c73 222c 0a20  lic.channels",. 
+000010e0: 2020 2020 2020 2020 2022 736f 7572 6365           "source
+000010f0: 2e73 7570 6572 7365 745f 6578 616d 706c  .superset_exampl
+00001100: 6573 2e70 7562 6c69 632e 6d65 7373 6167  es.public.messag
+00001110: 6573 220a 2020 2020 2020 2020 5d0a 2020  es".        ].  
+00001120: 2020 2020 7d2c 0a20 2020 2020 2022 636f      },.      "co
+00001130: 6e66 6967 223a 207b 0a20 2020 2020 2020  nfig": {.       
+00001140: 2022 656e 6162 6c65 6422 3a20 7472 7565   "enabled": true
+00001150: 2c0a 2020 2020 2020 2020 2261 6c69 6173  ,.        "alias
+00001160: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
+00001170: 2022 7363 6865 6d61 223a 206e 756c 6c2c   "schema": null,
+00001180: 0a20 2020 2020 2020 2022 6461 7461 6261  .        "databa
+00001190: 7365 223a 206e 756c 6c2c 0a20 2020 2020  se": null,.     
+000011a0: 2020 2022 7461 6773 223a 205b 5d2c 0a20     "tags": [],. 
+000011b0: 2020 2020 2020 2022 6d65 7461 223a 207b         "meta": {
+000011c0: 7d2c 0a20 2020 2020 2020 2022 6d61 7465  },.        "mate
+000011d0: 7269 616c 697a 6564 223a 2022 7669 6577  rialized": "view
+000011e0: 222c 0a20 2020 2020 2020 2022 7065 7273  ",.        "pers
+000011f0: 6973 745f 646f 6373 223a 207b 7d2c 0a20  ist_docs": {},. 
+00001200: 2020 2020 2020 2022 7175 6f74 696e 6722         "quoting"
+00001210: 3a20 7b7d 2c0a 2020 2020 2020 2020 2263  : {},.        "c
+00001220: 6f6c 756d 6e5f 7479 7065 7322 3a20 7b7d  olumn_types": {}
+00001230: 2c0a 2020 2020 2020 2020 2266 756c 6c5f  ,.        "full_
+00001240: 7265 6672 6573 6822 3a20 6e75 6c6c 2c0a  refresh": null,.
+00001250: 2020 2020 2020 2020 226f 6e5f 7363 6865          "on_sche
+00001260: 6d61 5f63 6861 6e67 6522 3a20 2269 676e  ma_change": "ign
+00001270: 6f72 6522 2c0a 2020 2020 2020 2020 2270  ore",.        "p
+00001280: 6f73 742d 686f 6f6b 223a 205b 5d2c 0a20  ost-hook": [],. 
+00001290: 2020 2020 2020 2022 7072 652d 686f 6f6b         "pre-hook
+000012a0: 223a 205b 5d0a 2020 2020 2020 7d2c 0a20  ": [].      },. 
+000012b0: 2020 2020 2022 6461 7461 6261 7365 223a       "database":
+000012c0: 2022 6578 616d 706c 6573 5f64 6576 222c   "examples_dev",
+000012d0: 0a20 2020 2020 2022 7363 6865 6d61 223a  .      "schema":
+000012e0: 2022 7075 626c 6963 222c 0a20 2020 2020   "public",.     
+000012f0: 2022 6671 6e22 3a20 5b0a 2020 2020 2020   "fqn": [.      
+00001300: 2020 2273 7570 6572 7365 745f 6578 616d    "superset_exam
+00001310: 706c 6573 222c 0a20 2020 2020 2020 2022  ples",.        "
+00001320: 736c 6163 6b22 2c0a 2020 2020 2020 2020  slack",.        
+00001330: 226d 6573 7361 6765 735f 6368 616e 6e65  "messages_channe
+00001340: 6c73 220a 2020 2020 2020 5d2c 0a20 2020  ls".      ],.   
+00001350: 2020 2022 756e 6971 7565 5f69 6422 3a20     "unique_id": 
+00001360: 226d 6f64 656c 2e73 7570 6572 7365 745f  "model.superset_
+00001370: 6578 616d 706c 6573 2e6d 6573 7361 6765  examples.message
+00001380: 735f 6368 616e 6e65 6c73 222c 0a20 2020  s_channels",.   
+00001390: 2020 2022 7061 636b 6167 655f 6e61 6d65     "package_name
+000013a0: 223a 2022 7375 7065 7273 6574 5f65 7861  ": "superset_exa
+000013b0: 6d70 6c65 7322 2c0a 2020 2020 2020 2272  mples",.      "r
+000013c0: 6f6f 745f 7061 7468 223a 2022 2f55 7365  oot_path": "/Use
+000013d0: 7273 2f62 6574 6f2f 5072 6f6a 6563 7473  rs/beto/Projects
+000013e0: 2f64 6274 2d65 7861 6d70 6c65 732f 7375  /dbt-examples/su
+000013f0: 7065 7273 6574 5f65 7861 6d70 6c65 7322  perset_examples"
+00001400: 2c0a 2020 2020 2020 2270 6174 6822 3a20  ,.      "path": 
+00001410: 2273 6c61 636b 2f6d 6573 7361 6765 735f  "slack/messages_
+00001420: 6368 616e 6e65 6c73 2e73 716c 222c 0a20  channels.sql",. 
+00001430: 2020 2020 2022 6f72 6967 696e 616c 5f66       "original_f
+00001440: 696c 655f 7061 7468 223a 2022 6d6f 6465  ile_path": "mode
+00001450: 6c73 2f73 6c61 636b 2f6d 6573 7361 6765  ls/slack/message
+00001460: 735f 6368 616e 6e65 6c73 2e73 716c 222c  s_channels.sql",
+00001470: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
+00001480: 6d65 7373 6167 6573 5f63 6861 6e6e 656c  messages_channel
+00001490: 7322 2c0a 2020 2020 2020 2261 6c69 6173  s",.      "alias
+000014a0: 223a 2022 6d65 7373 6167 6573 5f63 6861  ": "messages_cha
+000014b0: 6e6e 656c 7322 2c0a 2020 2020 2020 2263  nnels",.      "c
+000014c0: 6865 636b 7375 6d22 3a20 7b0a 2020 2020  hecksum": {.    
+000014d0: 2020 2020 226e 616d 6522 3a20 2273 6861      "name": "sha
+000014e0: 3235 3622 2c0a 2020 2020 2020 2020 2263  256",.        "c
+000014f0: 6865 636b 7375 6d22 3a20 2262 3463 6532  hecksum": "b4ce2
+00001500: 3332 6232 3832 3830 6461 6135 3232 6233  32b28280daa522b3
+00001510: 3765 3132 6333 3662 3637 3931 3165 3261  7e12c36b67911e2a
+00001520: 3938 3435 3662 3861 3362 3939 3434 3030  98456b8a3b994400
+00001530: 3735 6563 3535 3634 3630 3922 0a20 2020  75ec5564609".   
+00001540: 2020 207d 2c0a 2020 2020 2020 2274 6167     },.      "tag
+00001550: 7322 3a20 5b5d 2c0a 2020 2020 2020 2272  s": [],.      "r
+00001560: 6566 7322 3a20 5b5d 2c0a 2020 2020 2020  efs": [],.      
+00001570: 2273 6f75 7263 6573 223a 205b 0a20 2020  "sources": [.   
+00001580: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00001590: 2022 7075 626c 6963 222c 0a20 2020 2020   "public",.     
+000015a0: 2020 2020 2022 6368 616e 6e65 6c73 220a       "channels".
+000015b0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+000015c0: 2020 205b 0a20 2020 2020 2020 2020 2022     [.          "
+000015d0: 7075 626c 6963 222c 0a20 2020 2020 2020  public",.       
+000015e0: 2020 2022 6d65 7373 6167 6573 220a 2020     "messages".  
+000015f0: 2020 2020 2020 5d0a 2020 2020 2020 5d2c        ].      ],
+00001600: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
+00001610: 696f 6e22 3a20 2222 2c0a 2020 2020 2020  ion": "",.      
+00001620: 2263 6f6c 756d 6e73 223a 207b 7d2c 0a20  "columns": {},. 
+00001630: 2020 2020 2022 6d65 7461 223a 207b 7d2c       "meta": {},
+00001640: 0a20 2020 2020 2022 646f 6373 223a 207b  .      "docs": {
+00001650: 0a20 2020 2020 2020 2022 7368 6f77 223a  .        "show":
+00001660: 2074 7275 650a 2020 2020 2020 7d2c 0a20   true.      },. 
+00001670: 2020 2020 2022 7061 7463 685f 7061 7468       "patch_path
+00001680: 223a 206e 756c 6c2c 0a20 2020 2020 2022  ": null,.      "
+00001690: 636f 6d70 696c 6564 5f70 6174 6822 3a20  compiled_path": 
+000016a0: 2274 6172 6765 742f 636f 6d70 696c 6564  "target/compiled
+000016b0: 2f73 7570 6572 7365 745f 6578 616d 706c  /superset_exampl
+000016c0: 6573 2f6d 6f64 656c 732f 736c 6163 6b2f  es/models/slack/
+000016d0: 6d65 7373 6167 6573 5f63 6861 6e6e 656c  messages_channel
+000016e0: 732e 7371 6c22 2c0a 2020 2020 2020 2262  s.sql",.      "b
+000016f0: 7569 6c64 5f70 6174 6822 3a20 6e75 6c6c  uild_path": null
+00001700: 2c0a 2020 2020 2020 2264 6566 6572 7265  ,.      "deferre
+00001710: 6422 3a20 6661 6c73 652c 0a20 2020 2020  d": false,.     
+00001720: 2022 756e 7265 6e64 6572 6564 5f63 6f6e   "unrendered_con
+00001730: 6669 6722 3a20 7b0a 2020 2020 2020 2020  fig": {.        
+00001740: 226d 6174 6572 6961 6c69 7a65 6422 3a20  "materialized": 
+00001750: 2276 6965 7722 0a20 2020 2020 207d 2c0a  "view".      },.
+00001760: 2020 2020 2020 2263 7265 6174 6564 5f61        "created_a
+00001770: 7422 3a20 3136 3432 3632 3839 3333 2e30  t": 1642628933.0
+00001780: 3034 3435 322c 0a20 2020 2020 2022 636f  04452,.      "co
+00001790: 6d70 696c 6564 5f73 716c 223a 2022 5345  mpiled_sql": "SE
+000017a0: 4c45 4354 206d 6573 7361 6765 732e 7473  LECT messages.ts
+000017b0: 2c20 6368 616e 6e65 6c73 2e6e 616d 652c  , channels.name,
+000017c0: 206d 6573 7361 6765 732e 7465 7874 2046   messages.text F
+000017d0: 524f 4d20 5c22 6578 616d 706c 6573 5f64  ROM \"examples_d
+000017e0: 6576 5c22 2e5c 2270 7562 6c69 635c 222e  ev\".\"public\".
+000017f0: 5c22 6d65 7373 6167 6573 5c22 206d 6573  \"messages\" mes
+00001800: 7361 6765 7320 4a4f 494e 205c 2265 7861  sages JOIN \"exa
+00001810: 6d70 6c65 735f 6465 765c 222e 5c22 7075  mples_dev\".\"pu
+00001820: 626c 6963 5c22 2e5c 2263 6861 6e6e 656c  blic\".\"channel
+00001830: 735c 2220 6368 616e 6e65 6c73 204f 4e20  s\" channels ON 
+00001840: 6d65 7373 6167 6573 2e63 6861 6e6e 656c  messages.channel
+00001850: 5f69 6420 3d20 6368 616e 6e65 6c73 2e69  _id = channels.i
+00001860: 6422 2c0a 2020 2020 2020 2265 7874 7261  d",.      "extra
+00001870: 5f63 7465 735f 696e 6a65 6374 6564 223a  _ctes_injected":
+00001880: 2074 7275 652c 0a20 2020 2020 2022 6578   true,.      "ex
+00001890: 7472 615f 6374 6573 223a 205b 5d2c 0a20  tra_ctes": [],. 
+000018a0: 2020 2020 2022 7265 6c61 7469 6f6e 5f6e       "relation_n
+000018b0: 616d 6522 3a20 225c 2265 7861 6d70 6c65  ame": "\"example
+000018c0: 735f 6465 765c 222e 5c22 7075 626c 6963  s_dev\".\"public
+000018d0: 5c22 2e5c 226d 6573 7361 6765 735f 6368  \".\"messages_ch
+000018e0: 616e 6e65 6c73 5c22 220a 2020 2020 7d2c  annels\"".    },
+000018f0: 0a20 2020 2022 7465 7374 2e6a 6166 666c  .    "test.jaffl
+00001900: 655f 7368 6f70 2e75 6e69 7175 655f 7374  e_shop.unique_st
+00001910: 675f 6375 7374 6f6d 6572 735f 6375 7374  g_customers_cust
+00001920: 6f6d 6572 5f69 642e 6337 3631 3464 6161  omer_id.c7614daa
+00001930: 6461 223a 207b 0a20 2020 2020 2022 7261  da": {.      "ra
+00001940: 775f 7371 6c22 3a20 227b 7b20 7465 7374  w_sql": "{{ test
+00001950: 5f75 6e69 7175 6528 2a2a 5f64 6274 5f67  _unique(**_dbt_g
+00001960: 656e 6572 6963 5f74 6573 745f 6b77 6172  eneric_test_kwar
+00001970: 6773 2920 7d7d 222c 0a20 2020 2020 2022  gs) }}",.      "
+00001980: 7465 7374 5f6d 6574 6164 6174 6122 3a20  test_metadata": 
+00001990: 7b0a 2020 2020 2020 2020 226e 616d 6522  {.        "name"
+000019a0: 3a20 2275 6e69 7175 6522 2c0a 2020 2020  : "unique",.    
+000019b0: 2020 2020 226b 7761 7267 7322 3a20 7b0a      "kwargs": {.
+000019c0: 2020 2020 2020 2020 2020 2263 6f6c 756d            "colum
+000019d0: 6e5f 6e61 6d65 223a 2022 6375 7374 6f6d  n_name": "custom
+000019e0: 6572 5f69 6422 2c0a 2020 2020 2020 2020  er_id",.        
+000019f0: 2020 226d 6f64 656c 223a 2022 7b7b 2067    "model": "{{ g
+00001a00: 6574 5f77 6865 7265 5f73 7562 7175 6572  et_where_subquer
+00001a10: 7928 7265 6628 2773 7467 5f63 7573 746f  y(ref('stg_custo
+00001a20: 6d65 7273 2729 2920 7d7d 220a 2020 2020  mers')) }}".    
+00001a30: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00001a40: 6e61 6d65 7370 6163 6522 3a20 6e75 6c6c  namespace": null
+00001a50: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
+00001a60: 2263 6f6d 7069 6c65 6422 3a20 7472 7565  "compiled": true
+00001a70: 2c0a 2020 2020 2020 2272 6573 6f75 7263  ,.      "resourc
+00001a80: 655f 7479 7065 223a 2022 7465 7374 222c  e_type": "test",
+00001a90: 0a20 2020 2020 2022 6465 7065 6e64 735f  .      "depends_
+00001aa0: 6f6e 223a 207b 0a20 2020 2020 2020 2022  on": {.        "
+00001ab0: 6d61 6372 6f73 223a 205b 0a20 2020 2020  macros": [.     
+00001ac0: 2020 2020 2022 6d61 6372 6f2e 6462 742e       "macro.dbt.
+00001ad0: 7465 7374 5f75 6e69 7175 6522 2c0a 2020  test_unique",.  
+00001ae0: 2020 2020 2020 2020 226d 6163 726f 2e64          "macro.d
+00001af0: 6274 2e67 6574 5f77 6865 7265 5f73 7562  bt.get_where_sub
+00001b00: 7175 6572 7922 0a20 2020 2020 2020 205d  query".        ]
+00001b10: 2c0a 2020 2020 2020 2020 226e 6f64 6573  ,.        "nodes
+00001b20: 223a 205b 0a20 2020 2020 2020 2020 2022  ": [.          "
+00001b30: 6d6f 6465 6c2e 6a61 6666 6c65 5f73 686f  model.jaffle_sho
+00001b40: 702e 7374 675f 6375 7374 6f6d 6572 7322  p.stg_customers"
+00001b50: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00001b60: 207d 2c0a 2020 2020 2020 2263 6f6e 6669   },.      "confi
+00001b70: 6722 3a20 7b0a 2020 2020 2020 2020 2265  g": {.        "e
+00001b80: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
+00001b90: 2020 2020 2020 2022 616c 6961 7322 3a20         "alias": 
+00001ba0: 6e75 6c6c 2c0a 2020 2020 2020 2020 2273  null,.        "s
+00001bb0: 6368 656d 6122 3a20 2264 6274 5f74 6573  chema": "dbt_tes
+00001bc0: 745f 5f61 7564 6974 222c 0a20 2020 2020  t__audit",.     
+00001bd0: 2020 2022 6461 7461 6261 7365 223a 206e     "database": n
+00001be0: 756c 6c2c 0a20 2020 2020 2020 2022 7461  ull,.        "ta
+00001bf0: 6773 223a 205b 5d2c 0a20 2020 2020 2020  gs": [],.       
+00001c00: 2022 6d65 7461 223a 207b 7d2c 0a20 2020   "meta": {},.   
+00001c10: 2020 2020 2022 6d61 7465 7269 616c 697a       "materializ
+00001c20: 6564 223a 2022 7465 7374 222c 0a20 2020  ed": "test",.   
+00001c30: 2020 2020 2022 7365 7665 7269 7479 223a       "severity":
+00001c40: 2022 4552 524f 5222 2c0a 2020 2020 2020   "ERROR",.      
+00001c50: 2020 2273 746f 7265 5f66 6169 6c75 7265    "store_failure
+00001c60: 7322 3a20 6e75 6c6c 2c0a 2020 2020 2020  s": null,.      
+00001c70: 2020 2277 6865 7265 223a 206e 756c 6c2c    "where": null,
+00001c80: 0a20 2020 2020 2020 2022 6c69 6d69 7422  .        "limit"
+00001c90: 3a20 6e75 6c6c 2c0a 2020 2020 2020 2020  : null,.        
+00001ca0: 2266 6169 6c5f 6361 6c63 223a 2022 636f  "fail_calc": "co
+00001cb0: 756e 7428 2a29 222c 0a20 2020 2020 2020  unt(*)",.       
+00001cc0: 2022 7761 726e 5f69 6622 3a20 2221 3d20   "warn_if": "!= 
+00001cd0: 3022 2c0a 2020 2020 2020 2020 2265 7272  0",.        "err
+00001ce0: 6f72 5f69 6622 3a20 2221 3d20 3022 0a20  or_if": "!= 0". 
+00001cf0: 2020 2020 207d 2c0a 2020 2020 2020 2264       },.      "d
+00001d00: 6174 6162 6173 6522 3a20 2264 6274 2d74  atabase": "dbt-t
+00001d10: 7574 6f72 6961 6c2d 3334 3731 3030 222c  utorial-347100",
+00001d20: 0a20 2020 2020 2022 7363 6865 6d61 223a  .      "schema":
+00001d30: 2022 6462 745f 6265 746f 5f64 6274 5f74   "dbt_beto_dbt_t
+00001d40: 6573 745f 5f61 7564 6974 222c 0a20 2020  est__audit",.   
+00001d50: 2020 2022 6671 6e22 3a20 5b0a 2020 2020     "fqn": [.    
+00001d60: 2020 2020 226a 6166 666c 655f 7368 6f70      "jaffle_shop
+00001d70: 222c 0a20 2020 2020 2020 2022 756e 6971  ",.        "uniq
+00001d80: 7565 5f73 7467 5f63 7573 746f 6d65 7273  ue_stg_customers
+00001d90: 5f63 7573 746f 6d65 725f 6964 220a 2020  _customer_id".  
+00001da0: 2020 2020 5d2c 0a20 2020 2020 2022 756e      ],.      "un
+00001db0: 6971 7565 5f69 6422 3a20 2274 6573 742e  ique_id": "test.
+00001dc0: 6a61 6666 6c65 5f73 686f 702e 756e 6971  jaffle_shop.uniq
+00001dd0: 7565 5f73 7467 5f63 7573 746f 6d65 7273  ue_stg_customers
+00001de0: 5f63 7573 746f 6d65 725f 6964 2e63 3736  _customer_id.c76
+00001df0: 3134 6461 6164 6122 2c0a 2020 2020 2020  14daada",.      
+00001e00: 2270 6163 6b61 6765 5f6e 616d 6522 3a20  "package_name": 
+00001e10: 226a 6166 666c 655f 7368 6f70 222c 0a20  "jaffle_shop",. 
+00001e20: 2020 2020 2022 726f 6f74 5f70 6174 6822       "root_path"
+00001e30: 3a20 222e 222c 0a20 2020 2020 2022 7061  : ".",.      "pa
+00001e40: 7468 223a 2022 756e 6971 7565 5f73 7467  th": "unique_stg
+00001e50: 5f63 7573 746f 6d65 7273 5f63 7573 746f  _customers_custo
+00001e60: 6d65 725f 6964 2e73 716c 222c 0a20 2020  mer_id.sql",.   
+00001e70: 2020 2022 6f72 6967 696e 616c 5f66 696c     "original_fil
+00001e80: 655f 7061 7468 223a 2022 6d6f 6465 6c73  e_path": "models
+00001e90: 2f73 6368 656d 612e 796d 6c22 2c0a 2020  /schema.yml",.  
+00001ea0: 2020 2020 226e 616d 6522 3a20 2275 6e69      "name": "uni
+00001eb0: 7175 655f 7374 675f 6375 7374 6f6d 6572  que_stg_customer
+00001ec0: 735f 6375 7374 6f6d 6572 5f69 6422 2c0a  s_customer_id",.
+00001ed0: 2020 2020 2020 2261 6c69 6173 223a 2022        "alias": "
+00001ee0: 756e 6971 7565 5f73 7467 5f63 7573 746f  unique_stg_custo
+00001ef0: 6d65 7273 5f63 7573 746f 6d65 725f 6964  mers_customer_id
+00001f00: 222c 0a20 2020 2020 2022 6368 6563 6b73  ",.      "checks
+00001f10: 756d 223a 207b 0a20 2020 2020 2020 2022  um": {.        "
+00001f20: 6e61 6d65 223a 2022 6e6f 6e65 222c 0a20  name": "none",. 
+00001f30: 2020 2020 2020 2022 6368 6563 6b73 756d         "checksum
+00001f40: 223a 2022 220a 2020 2020 2020 7d2c 0a20  ": "".      },. 
+00001f50: 2020 2020 2022 7461 6773 223a 205b 5d2c       "tags": [],
+00001f60: 0a20 2020 2020 2022 7265 6673 223a 205b  .      "refs": [
+00001f70: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00001f80: 2020 2020 2022 7374 675f 6375 7374 6f6d       "stg_custom
+00001f90: 6572 7322 0a20 2020 2020 2020 205d 0a20  ers".        ]. 
+00001fa0: 2020 2020 205d 2c0a 2020 2020 2020 2273       ],.      "s
+00001fb0: 6f75 7263 6573 223a 205b 5d2c 0a20 2020  ources": [],.   
+00001fc0: 2020 2022 6d65 7472 6963 7322 3a20 5b5d     "metrics": []
+00001fd0: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
+00001fe0: 7469 6f6e 223a 2022 222c 0a20 2020 2020  tion": "",.     
+00001ff0: 2022 636f 6c75 6d6e 7322 3a20 7b7d 2c0a   "columns": {},.
+00002000: 2020 2020 2020 226d 6574 6122 3a20 7b7d        "meta": {}
+00002010: 2c0a 2020 2020 2020 2264 6f63 7322 3a20  ,.      "docs": 
+00002020: 7b0a 2020 2020 2020 2020 2273 686f 7722  {.        "show"
+00002030: 3a20 7472 7565 0a20 2020 2020 207d 2c0a  : true.      },.
+00002040: 2020 2020 2020 2270 6174 6368 5f70 6174        "patch_pat
+00002050: 6822 3a20 6e75 6c6c 2c0a 2020 2020 2020  h": null,.      
+00002060: 2263 6f6d 7069 6c65 645f 7061 7468 223a  "compiled_path":
+00002070: 2022 7461 7267 6574 2f63 6f6d 7069 6c65   "target/compile
+00002080: 642f 6a61 6666 6c65 5f73 686f 702f 6d6f  d/jaffle_shop/mo
+00002090: 6465 6c73 2f73 6368 656d 612e 796d 6c2f  dels/schema.yml/
+000020a0: 756e 6971 7565 5f73 7467 5f63 7573 746f  unique_stg_custo
+000020b0: 6d65 7273 5f63 7573 746f 6d65 725f 6964  mers_customer_id
+000020c0: 2e73 716c 222c 0a20 2020 2020 2022 6275  .sql",.      "bu
+000020d0: 696c 645f 7061 7468 223a 206e 756c 6c2c  ild_path": null,
+000020e0: 0a20 2020 2020 2022 6465 6665 7272 6564  .      "deferred
+000020f0: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+00002100: 2275 6e72 656e 6465 7265 645f 636f 6e66  "unrendered_conf
+00002110: 6967 223a 207b 7d2c 0a20 2020 2020 2022  ig": {},.      "
+00002120: 6372 6561 7465 645f 6174 223a 2031 3635  created_at": 165
+00002130: 3732 3935 3639 382e 3239 3533 3836 382c  7295698.2953868,
+00002140: 0a20 2020 2020 2022 636f 6d70 696c 6564  .      "compiled
+00002150: 5f73 716c 223a 2022 5c5c 6e20 2020 205c  _sql": "\\n    \
+00002160: 5c6e 2020 2020 5c5c 6e5c 5c6e 7769 7468  \n    \\n\\nwith
+00002170: 2064 6274 5f74 6573 745f 5f74 6172 6765   dbt_test__targe
+00002180: 7420 6173 2028 5c5c 6e20 205c 5c6e 2020  t as (\\n  \\n  
+00002190: 7365 6c65 6374 2063 7573 746f 6d65 725f  select customer_
+000021a0: 6964 2061 7320 756e 6971 7565 5f66 6965  id as unique_fie
+000021b0: 6c64 5c5c 6e20 2066 726f 6d20 6064 6274  ld\\n  from `dbt
+000021c0: 2d74 7574 6f72 6961 6c2d 3334 3731 3030  -tutorial-347100
+000021d0: 602e 6064 6274 5f62 6574 6f60 2e60 7374  `.`dbt_beto`.`st
+000021e0: 675f 6375 7374 6f6d 6572 7360 5c5c 6e20  g_customers`\\n 
+000021f0: 2077 6865 7265 2063 7573 746f 6d65 725f   where customer_
+00002200: 6964 2069 7320 6e6f 7420 6e75 6c6c 5c5c  id is not null\\
+00002210: 6e20 205c 5c6e 295c 5c6e 5c5c 6e73 656c  n  \\n)\\n\\nsel
+00002220: 6563 745c 5c6e 2020 2020 756e 6971 7565  ect\\n    unique
+00002230: 5f66 6965 6c64 2c5c 5c6e 2020 2020 636f  _field,\\n    co
+00002240: 756e 7428 2a29 2061 7320 6e5f 7265 636f  unt(*) as n_reco
+00002250: 7264 735c 5c6e 5c5c 6e66 726f 6d20 6462  rds\\n\\nfrom db
+00002260: 745f 7465 7374 5f5f 7461 7267 6574 5c5c  t_test__target\\
+00002270: 6e67 726f 7570 2062 7920 756e 6971 7565  ngroup by unique
+00002280: 5f66 6965 6c64 5c5c 6e68 6176 696e 6720  _field\\nhaving 
+00002290: 636f 756e 7428 2a29 203e 2031 5c5c 6e5c  count(*) > 1\\n\
+000022a0: 5c6e 5c5c 6e22 2c0a 2020 2020 2020 2265  \n\\n",.      "e
+000022b0: 7874 7261 5f63 7465 735f 696e 6a65 6374  xtra_ctes_inject
+000022c0: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+000022d0: 2022 6578 7472 615f 6374 6573 223a 205b   "extra_ctes": [
+000022e0: 5d2c 0a20 2020 2020 2022 7265 6c61 7469  ],.      "relati
+000022f0: 6f6e 5f6e 616d 6522 3a20 6e75 6c6c 2c0a  on_name": null,.
+00002300: 2020 2020 2020 2263 6f6c 756d 6e5f 6e61        "column_na
+00002310: 6d65 223a 2022 6375 7374 6f6d 6572 5f69  me": "customer_i
+00002320: 6422 2c0a 2020 2020 2020 2266 696c 655f  d",.      "file_
+00002330: 6b65 795f 6e61 6d65 223a 2022 6d6f 6465  key_name": "mode
+00002340: 6c73 2e73 7467 5f63 7573 746f 6d65 7273  ls.stg_customers
+00002350: 220a 2020 2020 7d0a 2020 7d2c 0a20 2022  ".    }.  },.  "
+00002360: 6368 696c 645f 6d61 7022 3a20 7b0a 2020  child_map": {.  
+00002370: 2020 226d 6f64 656c 2e73 7570 6572 7365    "model.superse
+00002380: 745f 6578 616d 706c 6573 2e6d 6573 7361  t_examples.messa
+00002390: 6765 735f 6368 616e 6e65 6c73 223a 205b  ges_channels": [
+000023a0: 0a20 2020 2020 2022 6d65 7472 6963 2e73  .      "metric.s
+000023b0: 7570 6572 7365 745f 6578 616d 706c 6573  uperset_examples
+000023c0: 2e63 6e74 220a 2020 2020 5d2c 0a20 2020  .cnt".    ],.   
+000023d0: 2022 736f 7572 6365 2e73 7570 6572 7365   "source.superse
+000023e0: 745f 6578 616d 706c 6573 2e70 7562 6c69  t_examples.publi
+000023f0: 632e 6d65 7373 6167 6573 223a 205b 0a20  c.messages": [. 
+00002400: 2020 2020 2022 6d6f 6465 6c2e 7375 7065       "model.supe
+00002410: 7273 6574 5f65 7861 6d70 6c65 732e 6d65  rset_examples.me
+00002420: 7373 6167 6573 5f63 6861 6e6e 656c 7322  ssages_channels"
+00002430: 0a20 2020 205d 2c0a 2020 2020 2273 6f75  .    ],.    "sou
+00002440: 7263 652e 7375 7065 7273 6574 5f65 7861  rce.superset_exa
+00002450: 6d70 6c65 732e 7075 626c 6963 2e63 6861  mples.public.cha
+00002460: 6e6e 656c 7322 3a20 5b0a 2020 2020 2020  nnels": [.      
+00002470: 226d 6f64 656c 2e73 7570 6572 7365 745f  "model.superset_
+00002480: 6578 616d 706c 6573 2e6d 6573 7361 6765  examples.message
+00002490: 735f 6368 616e 6e65 6c73 220a 2020 2020  s_channels".    
+000024a0: 5d2c 0a20 2020 2022 6d65 7472 6963 2e73  ],.    "metric.s
+000024b0: 7570 6572 7365 745f 6578 616d 706c 6573  uperset_examples
+000024c0: 2e63 6e74 223a 205b 5d0a 2020 7d0a 7d0a  .cnt": [].  }.}.
```

### Comparing `preset-cli-0.1.1/tests/cli/superset/sync/dbt/exposures_test.py` & `preset-cli-0.2.0/tests/cli/superset/sync/dbt/exposures_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import yaml
 from pyfakefs.fake_filesystem import FakeFilesystem
 from pytest_mock import MockerFixture
 from yarl import URL
 
 from preset_cli.cli.superset.sync.dbt.exposures import (
+    ModelKey,
     get_chart_depends_on,
     get_dashboard_depends_on,
     sync_exposures,
 )
 
 dashboard_response: Dict[str, Any] = {
     "result": {
@@ -495,101 +496,101 @@
 
 
 def test_get_dashboard_depends_on(mocker: MockerFixture) -> None:
     """
     Test ``get_dashboard_depends_on``.
     """
     client = mocker.MagicMock()
-    client.get_dataset.return_value = dataset_response
-    session = client.auth.get_session()
+    client.get_dataset.return_value = dataset_response["result"]
+    session = client.auth.session
     session.get().json.return_value = datasets_response
 
-    depends_on = get_dashboard_depends_on(client, dashboard_response["result"])
+    depends_on = get_dashboard_depends_on(client, dashboard_response["result"], {})
     assert depends_on == ["ref('messages_channels')"]
 
 
 def test_get_dashboard_depends_on_no_extra(mocker: MockerFixture) -> None:
     """
     Test ``get_dashboard_depends_on`` without an extra payload.
     """
     client = mocker.MagicMock()
     modified_dataset_response = copy.deepcopy(dataset_response)
     modified_dataset_response["result"]["extra"] = None  # type: ignore
-    client.get_dataset.return_value = modified_dataset_response
-    session = client.auth.get_session()
+    client.get_dataset.return_value = modified_dataset_response["result"]
+    session = client.auth.session
     session.get().json.return_value = datasets_response
 
-    depends_on = get_dashboard_depends_on(client, dashboard_response["result"])
+    depends_on = get_dashboard_depends_on(client, dashboard_response["result"], {})
     assert not depends_on
 
 
 def test_get_dashboard_depends_on_invalid_extra(mocker: MockerFixture) -> None:
     """
     Test ``get_dashboard_depends_on`` when the extra payload is not JSON.
     """
     client = mocker.MagicMock()
     modified_dataset_response = copy.deepcopy(dataset_response)
     modified_dataset_response["result"]["extra"] = "{[("  # type: ignore
-    client.get_dataset.return_value = modified_dataset_response
-    session = client.auth.get_session()
+    client.get_dataset.return_value = modified_dataset_response["result"]
+    session = client.auth.session
     session.get().json.return_value = datasets_response
 
-    depends_on = get_dashboard_depends_on(client, dashboard_response["result"])
+    depends_on = get_dashboard_depends_on(client, dashboard_response["result"], {})
     assert not depends_on
 
 
 def test_get_chart_depends_on(mocker: MockerFixture) -> None:
     """
     Test ``get_chart_depends_on``.
     """
     client = mocker.MagicMock()
-    client.get_dataset.return_value = dataset_response
+    client.get_dataset.return_value = dataset_response["result"]
 
-    depends_on = get_chart_depends_on(client, chart_response["result"])
+    depends_on = get_chart_depends_on(client, chart_response["result"], {})
     assert depends_on == ["ref('messages_channels')"]
 
 
 def test_get_chart_depends_on_no_extra(mocker: MockerFixture) -> None:
     """
     Test ``get_chart_depends_on`` without an extra payload.
     """
     client = mocker.MagicMock()
     modified_dataset_response = copy.deepcopy(dataset_response)
     modified_dataset_response["result"]["extra"] = None  # type: ignore
-    client.get_dataset.return_value = modified_dataset_response
+    client.get_dataset.return_value = modified_dataset_response["result"]
 
-    depends_on = get_chart_depends_on(client, chart_response["result"])
+    depends_on = get_chart_depends_on(client, chart_response["result"], {})
     assert not depends_on
 
 
 def test_sync_exposures(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test ``sync_exposures``.
     """
     root = Path("/path/to/root")
     fs.create_dir(root / "models")
     exposures = root / "models/exposures.yml"
 
     client = mocker.MagicMock()
     client.baseurl = URL("https://superset.example.org/")
-    client.get_chart.return_value = chart_response
-    client.get_dashboard.return_value = dashboard_response
-    session = client.auth.get_session()
+    client.get_chart.return_value = chart_response["result"]
+    client.get_dashboard.return_value = dashboard_response["result"]
+    session = client.auth.session
     session.get().json.return_value = related_objects_response
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.exposures.get_dashboard_depends_on",
         return_value=["ref('messages_channels')"],
     )
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.exposures.get_chart_depends_on",
         return_value=["ref('messages_channels')"],
     )
 
     datasets = [dataset_response["result"]]
-    sync_exposures(client, exposures, datasets)
+    sync_exposures(client, exposures, datasets, {})
 
     with open(exposures, encoding="utf-8") as input_:
         contents = yaml.load(input_, Loader=yaml.SafeLoader)
     assert contents == {
         "version": 2,
         "exposures": [
             {
@@ -618,30 +619,71 @@
 
 
 def test_sync_exposures_no_charts_no_dashboards(
     mocker: MockerFixture,
     fs: FakeFilesystem,
 ) -> None:
     """
-    Test ``sync_exposures`` when no dashboads use the datasets.
+    Test ``sync_exposures`` when no dashboards use the datasets.
     """
     root = Path("/path/to/root")
     fs.create_dir(root / "models")
     exposures = root / "models/exposures.yml"
 
     client = mocker.MagicMock()
     client.baseurl = URL("https://superset.example.org/")
-    session = client.auth.get_session()
+    session = client.auth.session
     no_related_objects_response = copy.deepcopy(related_objects_response)
     no_related_objects_response["charts"]["result"] = []
     no_related_objects_response["dashboards"]["result"] = []
     session.get().json.return_value = no_related_objects_response
 
     datasets = [dataset_response["result"]]
-    sync_exposures(client, exposures, datasets)
+    sync_exposures(client, exposures, datasets, {})
 
     with open(exposures, encoding="utf-8") as input_:
         contents = yaml.load(input_, Loader=yaml.SafeLoader)
     assert contents == {
         "version": 2,
         "exposures": [],
     }
+
+
+def test_get_chart_depends_on_from_dataset(mocker: MockerFixture) -> None:
+    """
+    Test ``sync_exposures`` when datasets don't have model metadata.
+
+    This is the case when users created the datasets manually, pointing them to dbt
+    models, but still want to sync exposures back to dbt.
+    """
+    client = mocker.MagicMock()
+    modified_dataset_response = copy.deepcopy(dataset_response)
+    modified_dataset_response["result"]["extra"] = None  # type: ignore
+    client.get_dataset.return_value = modified_dataset_response["result"]
+
+    key = ModelKey("public", "messages_channels")
+    depends_on = get_chart_depends_on(
+        client,
+        chart_response["result"],
+        {key: "ref(messages_channels)"},
+    )
+    assert depends_on == ["ref(messages_channels)"]
+
+
+def test_get_dashboard_depends_on_from_dataset(mocker: MockerFixture) -> None:
+    """
+    Test ``get_dashboard_depends_on`` when dataset don't have model metadata.
+    """
+    client = mocker.MagicMock()
+    modified_dataset_response = copy.deepcopy(dataset_response)
+    modified_dataset_response["result"]["extra"] = None  # type: ignore
+    client.get_dataset.return_value = modified_dataset_response["result"]
+    session = client.auth.session
+    session.get().json.return_value = datasets_response
+
+    key = ModelKey("public", "messages_channels")
+    depends_on = get_dashboard_depends_on(
+        client,
+        dashboard_response["result"],
+        {key: "ref(messages_channels)"},
+    )
+    assert depends_on == ["ref(messages_channels)"]
```

### Comparing `preset-cli-0.1.1/tests/lib_test.py` & `preset-cli-0.2.0/tests/lib_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import logging
 
 import pytest
 from pytest_mock import MockerFixture
 
 from preset_cli.exceptions import ErrorLevel, SupersetError
-from preset_cli.lib import remove_root, setup_logging, validate_response
+from preset_cli.lib import dict_merge, remove_root, setup_logging, validate_response
 
 
 def test_remove_root() -> None:
     """
     Test ``remove_root``.
     """
     assert remove_root("bundle/database/examples.yaml") == "database/examples.yaml"
@@ -90,7 +90,17 @@
     assert excinfo.value.errors == [
         {
             "message": "An error occurred",
             "error_type": "UNKNOWN_ERROR",
             "level": ErrorLevel.ERROR,
         },
     ]
+
+
+def test_dict_merge() -> None:
+    """
+    Test ``dict_merge``.
+    """
+    base = {"a": {"b": 42, "c": 43}, "d": 1, "e": 3}
+    overrides = {"a": {"c": 44}, "d": 2, "f": 3}
+    dict_merge(base, overrides)
+    assert base == {"a": {"b": 42, "c": 44}, "d": 2, "e": 3, "f": 3}
```

### Comparing `preset-cli-0.1.1/tox.ini` & `preset-cli-0.2.0/tox.ini`

 * *Files identical despite different names*

